# Module 4: Marketing Automation & Workflows

🎯 **Objective:** Understand and apply GHL automation to nurture leads, increase conversion rates, and save time through automated sequences.

---

## 4.1 What is Marketing Automation?

Marketing Automation uses software to **automate repetitive marketing tasks** — sending emails, SMS, classifying leads, and following up — so your team can focus on high-value work.

| Benefit | Description |
|---------|------------|
| ⏰ **Time savings** | No more manually emailing or texting each lead |
| 🎯 **Personalization at scale** | Right message, right person, right time |
| 📈 **Higher conversion** | Automated follow-ups keep leads warm |
| 📊 **Accurate measurement** | Track performance at every step |
| 🔄 **Consistency** | Every lead gets the same quality experience |

---

## 4.2 Building Blocks of Automation

```
┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│   TRIGGERS   │────▶│   ACTIONS    │────▶│  CONDITIONS  │
│  (Start it)  │     │  (Do this)   │     │ (Decide)     │
└──────────────┘     └──────────────┘     └──────────────┘
       │                    │                     │
 • Form submitted    • Send Email          • If/Else logic
 • Tag added         • Send SMS            • Wait timer
 • Email opened      • Add Tag             • Goal reached
 • Link clicked      • Move Pipeline       • Split test
 • Appointment       • Create Task
 • Birthday          • Add to Workflow
 • Custom Date       • Internal Notify
```

---

## 4.3 Triggers — Events That Start a Workflow

| Trigger | Description | Use Case |
|---------|------------|----------|
| **Contact Created** | A new contact enters the CRM | Welcome sequence |
| **Form Submitted** | A prospect fills out a form | Lead-magnet delivery |
| **Tag Added** | A tag is applied to a contact | Segment-specific nurture |
| **Tag Removed** | A tag is removed | Stop a campaign |
| **Email Opened** | Contact opens an email | Follow up on interest |
| **Link Clicked** | Contact clicks a link in email/SMS | Interest tracking |
| **Appointment Booked** | Meeting is scheduled | Send reminders & prep |
| **Appointment No-Show** | Contact misses the meeting | Re-booking campaign |
| **Pipeline Stage Changed** | A deal moves stages | Send stage-appropriate content |
| **Customer Reply** | Contact replies to a message | Notify salesperson |
| **Birthday** | Contact's birthday | Birthday promo |
| **Custom Date** | Any custom date field | Contract renewal reminder |
| **Invoice Paid** | Payment received | Onboarding sequence |
| **Stale Opportunity** | Deal hasn't moved in X days | Auto follow-up |

---

## 4.4 Actions — What the Workflow Does

### Communication Actions
- 📧 **Send Email** — pre-designed template or custom
- 📱 **Send SMS** — text message
- 📞 **Voicemail Drop** — leave a voicemail without ringing
- 💬 **Send Chat Message** — via live chat widget

### CRM Actions
- 🏷️ **Add / Remove Tag**
- 📋 **Update Contact Field**
- 📊 **Create / Update Opportunity**
- 🔄 **Move Pipeline Stage**

### Internal Actions
- ✅ **Create Task** — assign to-dos to team members
- 🔔 **Internal Notification** — alert via email or in-app
- 👤 **Assign User** — set the owner of a contact
- 📝 **Add Note** — append a note to the contact record

### Logic Actions
- ⏱️ **Wait** — pause for a set duration
- 🔀 **If/Else** — branch based on conditions
- 🎯 **Goal** — when the goal is met, the contact exits the workflow
- 🔗 **Webhook** — send data to an external system

---

## 4.5 Common Marketing Workflows

### 4.5.1 Welcome Sequence (Lead Magnet Delivery)

```
Trigger: Form Submitted (Lead Magnet Download)
    │
    ▼
[Immediately] Email 1: Deliver the lead magnet + Welcome message
    │
    ▼
[Wait 1 day]
    │
    ▼
Email 2: Share a relevant case study
    │
    ▼
[Wait 2 days]
    │
    ▼
Email 3: Introduce your main product/service
    │
    ▼
[Wait 2 days]
    │
    ▼
Email 4: Social proof — testimonials & reviews
    │
    ▼
[Wait 3 days]
    │
    ▼
Email 5: CTA — Book a consultation / Purchase
    │
    ├── [If: Appointment Booked] → Exit workflow ✅
    └── [Else] → Continue nurture sequence…
```

### 4.5.2 Lead Nurture (Long-term)

```
Trigger: Tag "status_qualified" added
    │
    ▼
[Week 1] Email: Industry insights + helpful tips
    │
    ▼
[Week 2] SMS: "Hi [First Name], we published a new article just for you"
    │
    ▼
[Week 3] Email: Detailed case study
    │
    ▼
[Week 4] Email: Limited-time offer
    │
    ├── [If clicked] → Tag "interest_high" → Notify Sales
    └── [If not opened] → Resend with a new subject line
```

### 4.5.3 Re-Engagement (Cold Leads)

```
Trigger: No activity for > 60 days
    │
    ▼
Email: "We miss you! Here's what's new"
    │
    ├── [If opened]
    │      └── SMS: "Hi [Name], we have a special offer for you"
    │             │
    │             ├── [If replied] → Tag "re-engaged" → Add to nurture
    │             └── [No reply in 5 days] → Send final offer email
    │
    └── [Not opened in 7 days]
           └── SMS: "Still interested in [service]? Reply STOP to unsubscribe"
                  │
                  ├── [Reply = "STOP"] → Unsubscribe
                  └── [Any other reply] → Notify Sales
```

### 4.5.4 Appointment Reminders

```
Trigger: Appointment Booked
    │
    ▼
[Immediately] Email: Confirmation + details (date, time, location/link)
    │
    ▼
[24 hrs before] SMS: "Reminder: You have an appointment tomorrow at [Time]"
    │
    ▼
[1 hr before] SMS: "Your appointment starts in 1 hour. Reply YES to confirm"
    │
    ├── [Confirmed] → "Thanks! See you soon."
    └── [No response] → Flag as potential no-show
```

---

## 4.6 Best Practices

### ✅ Do
1. **Start simple** — launch 2–3 workflows first, then expand
2. **Test before going live** — run through with a test contact
3. **Personalize** — use merge fields like `{{contact.first_name}}`
4. **Set Goals** — when the contact converts, they exit the workflow
5. **Monitor metrics** — review open rates and click rates weekly

### ❌ Don't
1. **Over-send** — max 1 email/day and 3 SMS/week
2. **Create infinite loops** — every workflow needs an exit point
3. **Ignore unsubscribes** — always honor opt-out requests
4. **Over-complicate** — workflows with too many branches are hard to maintain

---


> ⏭️ **Next:** [Module 5 — Funnels & Landing Pages](05_Funnels-Landing-Pages.md)

