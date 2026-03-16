# Module 9: Advanced Workflows & Automation

🎯 **Objective:** Master advanced workflow techniques — conditional logic, multi-branch sequences, webhooks, and workflow architecture best practices.

---

## 9.1 Beyond Basic Workflows

Module 4 covered the basics. This module dives into **advanced patterns** that unlock the full power of GHL automation.

---

## 9.2 If/Else Branching

If/Else lets you create **conditional paths** — different contacts take different routes through the workflow.

### Example: Lead Qualification Router

```
Trigger: Form Submitted ("Request a Quote")
    │
    ▼
If/Else: Budget Custom Field
    │
    ├── [Budget > $10,000]
    │       ▼
    │   Tag: "segment_enterprise"
    │   Assign to: Senior Sales Rep
    │   Create Opportunity: "Enterprise" pipeline
    │   SMS to Sales: "🔥 High-value lead incoming!"
    │
    ├── [Budget $2,000 – $10,000]
    │       ▼
    │   Tag: "segment_sme"
    │   Assign to: Sales Team (Round Robin)
    │   Create Opportunity: "SME" pipeline
    │   Email: "Thanks for your interest — a rep will call you today"
    │
    └── [Budget < $2,000]
            ▼
        Tag: "segment_small"
        Email: "Here are our self-service options and pricing page"
        Add to Nurture Workflow (long-term)
```

### Conditions Available in If/Else

| Condition Type | Examples |
|---------------|----------|
| **Contact Field** | Name, email, phone, custom fields |
| **Tag** | Has / doesn't have a specific tag |
| **Pipeline Stage** | Current stage of an opportunity |
| **Engagement** | Opened email, clicked link, replied |
| **Source** | UTM source, medium, campaign |
| **Date/Time** | Day of week, time of day, custom date |
| **Payment** | Has paid, total spent, invoice status |

---

## 9.3 Wait Steps & Timing Strategies

### Types of Wait Steps

| Wait Type | Description | Example |
|-----------|------------|---------|
| **Wait (Duration)** | Pause for X minutes/hours/days | Wait 2 days before next email |
| **Wait Until** | Pause until a specific date/time | Wait until next Monday 9 AM |
| **Wait for Event** | Pause until a condition is met | Wait until email is opened (max 3 days) |

### Timing Best Practices

```
Monday–Friday, 9 AM–11 AM    → Best for B2B emails
Tuesday–Thursday, 10 AM      → Best for SMS
Avoid: Weekends, late nights  → Lower engagement, higher unsubscribe
```

> 💡 **Tip:** Use the **"Smart Send"** time feature to optimize delivery based on each contact's timezone.

---

## 9.4 Goals — Smart Workflow Exits

A **Goal** is a checkpoint. When a contact reaches it, they **exit the current workflow** — preventing unnecessary messages.

### Example: Stop Nurture When They Book

```
Trigger: Tag "status_new-lead" added
    │
    ▼
Email 1: Welcome + value prop
    │
    ▼
[GOAL: Appointment Booked] ←── If booked at any point, EXIT here
    │
    ▼
[Wait 3 days]
Email 2: Case study
    │
    ▼
[Wait 3 days]
Email 3: Limited offer
    │
    ▼
[Wait 5 days]
Email 4: Final CTA
```

Without Goals, a contact who books after Email 1 would still receive Emails 2–4. Goals prevent this.

---

## 9.5 Webhooks & External Integrations

Webhooks let workflows **communicate with external systems** — send data out, or receive data in.

### Outbound Webhook (GHL → External)

Use case: When a deal is won, send data to your accounting software.

```
Trigger: Opportunity Stage = "Won"
    │
    ▼
Action: Webhook (POST)
    URL: https://your-accounting-app.com/api/invoices
    Body:
    {
      "customer_name": "{{contact.full_name}}",
      "email": "{{contact.email}}",
      "deal_value": "{{opportunity.monetary_value}}",
      "deal_name": "{{opportunity.name}}"
    }
```

### Inbound Webhook (External → GHL)

Use case: When your e-commerce platform has a new order, trigger a GHL workflow.

1. Create a workflow with **Trigger: Inbound Webhook**
2. GHL generates a unique URL
3. Configure your external system to POST to that URL
4. The workflow processes the incoming data

### Common Integrations via Webhooks / Zapier

| Platform | Direction | Use Case |
|----------|-----------|----------|
| **Stripe** | → GHL | New payment → tag contact |
| **Shopify** | → GHL | New order → start onboarding |
| **Google Sheets** | ← GHL | Export lead data for reporting |
| **Slack** | ← GHL | Notify sales channel on new deal |
| **Calendly** | → GHL | External booking → create contact + opportunity |

---

## 9.6 Advanced Workflow Patterns

### Pattern 1: Drip Campaign with Smart Stops

```
Trigger: Downloaded whitepaper
    │
    ▼
[GOAL: Booked meeting OR Purchased]
    │
    ▼
Day 0:  Email → Deliver whitepaper
Day 2:  Email → Related blog post
Day 5:  SMS → "Did you find the whitepaper useful?"
Day 7:  Email → Product demo video
Day 10: Email → Customer testimonial
Day 14: Email → Special offer (expires in 48h)
Day 16: SMS → "Last chance! Offer expires tonight"
    │
    └── END (if goal not met → Tag "nurture_exhausted")
```

### Pattern 2: Lead Scoring Workflow

```
Trigger:  Contact Activity (runs continuously)

Points system:
+5  → Opened an email
+10 → Clicked a link
+15 → Visited pricing page
+20 → Filled out a form
+25 → Booked an appointment
-5  → Unsubscribed from topic
-10 → No activity for 30 days

If/Else: Total Score
    ├── [Score > 50]  → Tag "lead_hot" → Notify Sales → Priority follow-up
    ├── [Score 20-50] → Tag "lead_warm" → Continue nurture
    └── [Score < 20]  → Tag "lead_cold" → Slow-drip content
```

### Pattern 3: Multi-Channel Retargeting

```
Trigger: Visited pricing page but didn't convert (tracked via page visit)
    │
    ▼
[Wait 1 hour]
    Email: "We noticed you were checking our pricing…"
    │
    ▼
[Wait 1 day - If no response]
    SMS: "Any questions about our plans? Reply and we'll help!"
    │
    ▼
[Wait 2 days - If no response]
    Voicemail Drop: Personalized message about their interest
    │
    ▼
[Wait 3 days - If no response]
    Email: Limited-time discount or bonus offer
    │
    ▼
[Wait 5 days]
    → Add to long-term nurture (monthly newsletter)
```

---

## 9.7 Workflow Architecture Best Practices

### Naming Convention
Use a consistent naming system:

```
[Category] - [Purpose] - [Version]

Examples:
SALES - New Lead Assignment - v2
MARKETING - Welcome Sequence - v3
SUPPORT - Post-Purchase Onboarding - v1
REPUTATION - Review Request - v1
INTERNAL - Sales Notification - v1
```

### Organization Tips
1. **One purpose per workflow** — don't combine unrelated automations
2. **Use sub-workflows** — break complex sequences into modular pieces
3. **Document your workflows** — add notes explaining the logic
4. **Version control** — duplicate before major changes (keep v1 inactive as backup)
5. **Regular audits** — review all active workflows monthly; deactivate unused ones

### Testing Checklist
- ☐ Create a test contact with a unique email
- ☐ Trigger the workflow manually
- ☐ Verify each step fires correctly (check Conversations tab)
- ☐ Test every If/Else branch
- ☐ Confirm Goals work (contact exits properly)
- ☐ Check timing (are waits correct?)
- ☐ Review on mobile (email/SMS formatting)

---

## 📝 Module 9 Exercises

1. **Build a lead-qualification workflow** with If/Else branching (at least 3 branches)
2. **Create a drip campaign** with a Goal that stops the sequence on conversion
3. **Set up an outbound webhook** that sends data to a Google Sheet when a deal is won
4. **Design a lead-scoring system** on paper — define point values for 5+ actions
5. **Audit your existing workflows** — name them properly, add notes, deactivate unused ones

---

> ⏭️ **Next:** [Module 10 — AI Features & AI Employees](10_AI-Features.md)
