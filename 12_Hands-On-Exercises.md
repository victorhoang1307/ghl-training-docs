# Module 12: Hands-On Exercises & Real-World Scenarios

🎯 **Objective:** Apply everything you've learned in realistic scenarios. Complete these exercises to demonstrate proficiency with GHL.

---

## 12.1 How to Use This Module

Each scenario simulates a **real business situation**. Work through them step-by-step in your GHL sub-account. Where applicable, exercises build on each other.

**Difficulty Levels:**
- 🟢 **Beginner** — Single feature, straightforward setup
- 🟡 **Intermediate** — Combines 2-3 features
- 🔴 **Advanced** — End-to-end multi-feature implementation

---

## 12.2 Scenario 1: Launch a Lead Generation Campaign 🟡

### Background
You run a digital marketing agency. You want to generate leads for a "Free Marketing Audit" offer using Facebook Ads driving traffic to a GHL funnel.

### Tasks

| # | Task | Module Reference |
|---|------|-----------------|
| 1 | **Create a 2-step funnel:** Opt-in page + Thank You page | Module 5 |
| 2 | **Design the opt-in page** with: headline, 3 benefits, testimonial, and a form (Name, Email, Phone, Company, "Monthly Ad Spend" dropdown) | Module 5 |
| 3 | **Create Custom Fields** for "Company" and "Monthly Ad Spend" | Module 2 |
| 4 | **Build a Welcome Workflow:** | Module 4 |
|   | • Trigger: Form submitted | |
|   | • Email 1 (immediately): Deliver audit checklist PDF | |
|   | • SMS (1 hour later): "Got your request! We'll be in touch shortly" | |
|   | • Email 2 (Day 2): Case study | |
|   | • Email 3 (Day 5): CTA to book a strategy call | |
| 5 | **Create a "New Business" Pipeline** with stages: New Lead → Contacted → Audit Scheduled → Audit Delivered → Proposal Sent → Won → Lost | Module 3 |
| 6 | **Connect the workflow** to auto-create an Opportunity in the pipeline | Module 3 |
| 7 | **Set up UTM tracking** on the funnel URL for Facebook Ads | Module 2 |

### Verification Checklist
- ☐ Funnel loads and looks good on mobile
- ☐ Form submission creates a contact with correct tags and custom fields
- ☐ Welcome email arrives within 60 seconds
- ☐ Opportunity appears in pipeline
- ☐ SMS is received

---

## 12.3 Scenario 2: Sales Team Pipeline Management 🟡

### Background
You have 3 sales reps. Leads are coming in from multiple channels. You need to assign leads fairly and ensure timely follow-up.

### Tasks

| # | Task | Module Reference |
|---|------|-----------------|
| 1 | **Set up a Round Robin calendar** with 3 team members | Module 7 |
| 2 | **Create a lead assignment workflow:** | Module 9 |
|   | • Trigger: Contact created | |
|   | • If/Else: Lead source | |
|   | • Facebook → assign to Rep A | |
|   | • Google → assign to Rep B | |
|   | • Referral → assign to Rep C | |
|   | • Each branch: Create opportunity + internal notification | |
| 3 | **Build a stale-deal alert workflow:** | Module 9 |
|   | • Trigger: Opportunity in "Contacted" for > 3 days | |
|   | • Action: SMS reminder to assigned rep | |
|   | • If still stale after 7 days: Email manager | |
| 4 | **Create Smart Lists:** | Module 2 |
|   | • "My Active Deals" (per rep) | |
|   | • "Stale Deals" (no activity > 5 days) | |
|   | • "Won This Month" | |
| 5 | **Build a sales dashboard** with: Pipeline value, Deals by rep, Win rate, Appointments today | Module 11 |

### Verification Checklist
- ☐ New leads get assigned to the correct rep based on source
- ☐ Opportunity is auto-created in the right pipeline
- ☐ Rep receives notification within minutes
- ☐ Stale deal SMS fires after 3 days
- ☐ Dashboard shows accurate data

---

## 12.4 Scenario 3: Client Onboarding Automation 🔴

### Background
A new client signs up and pays. You need to onboard them: welcome them, collect information, schedule a kickoff call, and request a review after 30 days.

### Tasks

| # | Task | Module Reference |
|---|------|-----------------|
| 1 | **Create an "Onboarding" Pipeline:** Signed → Welcome Sent → Info Collected → Kickoff Scheduled → Kickoff Done → Onboarded | Module 3 |
| 2 | **Build the Onboarding Workflow:** | Module 4, 9 |
|   | Step 1: Invoice Paid → Move to "Welcome Sent" + send welcome email | |
|   | Step 2 (Day 1): Email with onboarding form (collect brand assets, credentials, goals) | |
|   | Step 3: When form submitted → Move to "Info Collected" + tag: "onboarding_info_received" | |
|   | Step 4 (Day 2): SMS + Email: "Let's schedule your kickoff call" + Calendar booking link | |
|   | Step 5: When appointment booked → Move to "Kickoff Scheduled" | |
|   | Step 6: After kickoff meeting → Move to "Kickoff Done" | |
|   | Step 7 (Day 7): Check-in email: "How's everything going?" | |
|   | Step 8 (Day 30): Review request workflow (Module 8 pattern) | |
| 3 | **Set a Goal:** if the client replies at any point → exit automated sequence, notify account manager | Module 9 |
| 4 | **Create a "Client Onboarding" calendar** for kickoff calls | Module 7 |

### Verification Checklist
- ☐ Full sequence fires after a test payment
- ☐ Pipeline stages update automatically
- ☐ Kickoff booking link works
- ☐ Review request goes out on Day 30
- ☐ Goal correctly stops automation when client replies

---

## 12.5 Scenario 4: Re-Engagement & Reputation Campaign 🟡

### Background
You have 500 contacts who haven't interacted in 60+ days. You also want to request reviews from your 50 existing customers.

### Tasks

| # | Task | Module Reference |
|---|------|-----------------|
| 1 | **Create Smart Lists:** | Module 2 |
|   | • "Inactive 60+ days" | |
|   | • "Active Customers" | |
| 2 | **Build a Re-Engagement Workflow:** | Module 4 |
|   | • Email: "We miss you! Here's what's new" | |
|   | • If opened → SMS: Special offer | |
|   | • If not opened (7 days) → SMS: "Still interested? Reply STOP to opt out" | |
|   | • If replied → Tag "re-engaged" + notify sales | |
| 3 | **Build a Review Request Workflow:** | Module 8 |
|   | • SMS: "How would you rate us? Reply 1-5" | |
|   | • 4-5 stars → Send Google review link | |
|   | • 1-3 stars → "Sorry to hear that" + private feedback form | |
| 4 | **Monitor results** via Reporting dashboard after 1 week | Module 11 |

---

## 12.6 Scenario 5: Full AI-Powered Sales System 🔴

### Background
You want to deploy AI to handle after-hours inquiries, qualify leads, and book appointments automatically.

### Tasks

| # | Task | Module Reference |
|---|------|-----------------|
| 1 | **Build a Knowledge Base** with 20 Q&A entries covering your products, pricing, process, and FAQs | Module 10 |
| 2 | **Configure Conversation AI** in Suggestive mode on SMS and webchat | Module 10 |
| 3 | **Connect a calendar** so the AI can book appointments | Module 7, 10 |
| 4 | **Create an AI qualification workflow:** | Module 10 |
|   | • New lead → AI asks 3 qualifying questions | |
|   | • If qualified → Book appointment + create opportunity | |
|   | • If not qualified → Add to newsletter + nurture | |
| 5 | **Test with 10 different message scenarios** and log AI accuracy | Module 10 |
| 6 | **Set up escalation rules:** | Module 10 |
|   | • Billing questions → transfer to human | |
|   | • Complaints → create urgent task for manager | |
| 7 | After 1 week in Suggestive mode, evaluate accuracy → decide whether to enable Auto-pilot | Module 10 |

---

## 12.7 Final Certification Checklist

Complete all items below to demonstrate GHL proficiency:

### CRM Mastery
- ☐ Created and organized Custom Fields
- ☐ Established a Tag naming convention
- ☐ Built 3+ useful Smart Lists
- ☐ Successfully imported contacts via CSV

### Sales Pipeline
- ☐ Built a pipeline with 5+ stages
- ☐ Created and managed 5+ Opportunities
- ☐ Connected pipeline to automation

### Marketing Automation
- ☐ Built a complete email nurture sequence (5+ emails)
- ☐ Created a multi-channel workflow (email + SMS)
- ☐ Implemented If/Else logic in a workflow
- ☐ Used Goals to stop unnecessary messages

### Funnels & Landing Pages
- ☐ Built a 2-step funnel (opt-in + thank you)
- ☐ Connected a form to a workflow
- ☐ Set up a custom domain

### Email & SMS
- ☐ Sent a broadcast email
- ☐ Created 3+ SMS templates
- ☐ Set up domain authentication

### Calendars
- ☐ Created a booking calendar
- ☐ Synced with Google/Outlook
- ☐ Built appointment reminder workflow

### Reputation
- ☐ Connected Google Business Profile
- ☐ Built a review request workflow
- ☐ Written response templates

### AI
- ☐ Created a Knowledge Base
- ☐ Configured Conversation AI on at least one channel
- ☐ Tested AI responses and documented accuracy

### Reporting
- ☐ Built a custom dashboard
- ☐ Identified top lead source from reports
- ☐ Calculated ROI for one channel

---

## 🎓 Congratulations!

If you've completed all the modules and exercises, you're now equipped to:

- **Run an entire Sales & Marketing operation** from a single platform
- **Automate** repetitive tasks to focus on what matters
- **Measure** everything to continuously improve
- **Scale** your business with AI-powered tools

### Recommended Next Steps
1. **Join the GHL community** — share tips and ask questions
2. **Explore Snapshots** — pre-built configurations for specific industries
3. **Stay updated** — GHL releases new features regularly
4. **Practice daily** — the best way to master GHL is by using it every day
5. **Teach someone else** — explaining concepts solidifies your own understanding

---

> 📖 **Return to:** [Table of Contents](00_Table-of-Contents.md)
