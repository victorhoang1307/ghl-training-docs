# Module 6: Email & SMS Marketing

🎯 **Objective:** Create, send, and automate email and SMS campaigns that engage leads and drive conversions.

---

## 6.1 Why Email & SMS Together?

| Channel | Open Rate | Response Speed | Best for |
|---------|:---------:|:--------------:|----------|
| **Email** | 20–30% | Hours to days | Detailed content, nurture, newsletters |
| **SMS** | 90–98% | Minutes | Urgent messages, reminders, short offers |

---

## 6.2 Email Marketing in GHL

### 6.2.1 Email Builder

GHL provides a **drag-and-drop email builder** with:
- Pre-designed templates (categorized by industry)
- Custom HTML support
- Mobile-responsive preview
- Dynamic content with merge fields

### 6.2.2 Types of Emails in GHL

| Type | Description | When to use |
|------|------------|-------------|
| **Email Campaign** | One-time send to a list or Smart List (under **Marketing → Email Marketing → Campaigns**) | Newsletters, announcements, promotions |
| **Workflow Campaign** | Triggered automatically within a Workflow | Welcome series, drip sequences, follow-ups |
| **Bulk Action Campaign** | Quick send to selected contacts via Bulk Actions | One-off messages to a hand-picked group |
| **1-to-1 Email** | Manual send from the **Conversations** tab | Personal replies, individual follow-ups |

### 6.2.3 Sending Emails — All Four Methods

#### A. Email Campaign (one-time send)

1. Go to **Marketing** → **Email Marketing** → **Campaigns**
2. Make sure you're on the **Email Campaigns** tab (selected by default)
3. Click **"+ New"** → choose a template or start from scratch
4. Design the email content using the drag-and-drop builder
5. Click **Send or Schedule** and configure:
   - **Sender Name** and **Sender Email**
   - **Subject Line**
   - **Recipients** (Smart List, Tags, or Lists)
   - **Additional Settings** (Link Tracking, UTM Tracking, Tags)
6. Choose delivery: **Send Now** (immediate) or **Schedule** (future date/time)
7. **Preview & Test** — send a test email to yourself first
8. Click **Send** or **Schedule**

#### B. Workflow Campaign (automated trigger)

1. Go to **Automation** → **Workflows**
2. Create or open a workflow
3. Set a **Trigger** (e.g., Form Submitted, Tag Added, Appointment Booked)
4. Add an **Email** action step in the workflow
5. Choose an existing email template or build one inline
6. Configure timing with **Wait** steps between emails for drip sequences
7. **Publish** the workflow — emails will send automatically when the trigger fires

#### C. Bulk Action Campaign (quick ad-hoc send)

1. Go to **Contacts** or open a **Smart List**
2. Select the contacts you want to email (use checkboxes)
3. Click **Bulk Actions** → **Send Email**
4. Choose an email template or compose a message
5. Send immediately or enable **Drip Mode** to stagger delivery and improve deliverability

#### D. 1-to-1 Email (personal send)

1. Open **Conversations** in the sidebar
2. Select or search for a contact
3. Choose the **Email** channel
4. Compose your message (you can use templates)
5. Click **Send**

### 6.2.4 Email Metrics

| Metric | Target | What it tells you |
|--------|:------:|------------------|
| **Open Rate** | > 25% | Is your subject line compelling? |
| **Click Rate** | > 3% | Is your content engaging? |
| **Bounce Rate** | < 2% | Is your list clean? |
| **Unsubscribe Rate** | < 0.5% | Are you over-sending? |
| **Reply Rate** | > 1% | Are leads engaging? |

---

## 6.3 SMS Marketing in GHL

### 6.3.1 SMS Setup Requirements

Before sending SMS:
1. Register a **phone number** in GHL (local or toll-free)
2. Set up **A2P 10DLC registration** (USA) or comply with local SMS regulations
3. Configure **opt-in compliance** — contacts must consent to receive SMS

> ⚠️ **Note:** SMS costs are **usage-based** (not included in GHL subscription). Rates vary by country and carrier.

### 6.3.2 Types of SMS

| Type | Description | Example |
|------|------------|---------|
| **1-to-1** | Manual conversation from Conversations tab | Personal follow-up |
| **Broadcast** | Bulk send to a list | Flash sale announcement |
| **Workflow SMS** | Automatically triggered | Appointment reminders |
| **Two-way** | Real-time back-and-forth conversation | Customer support, qualification |

---

## 6.4 Combining Email & SMS in Workflows

### Multi-Channel Nurture Sequence

```
Trigger: New Lead (Form Submitted)
    │
    ▼
[Immediately]
    Email: "Welcome! Here's your free guide"
    │
    ▼
[Wait 1 hour]
    SMS: "Hi {{first_name}}, did you get the guide? Let us know if you have questions!"
    │
    ▼
[Wait 2 days]
    Email: "3 ways [product] can help your business"
    │
    ▼
[Wait 3 days]
    │
    ├── [If email opened]
    │       Email: Case study + book a call CTA
    │
    └── [If email NOT opened]
            SMS: "{{first_name}}, we shared some tips you might find useful. Check your inbox!"
    │
    ▼
[Wait 4 days]
    Email: "Special offer — 20% off, ends Friday"
    SMS: "Don't miss our limited-time offer! Check your email for details 🎉"
```

---

> 📖 **Best Practices:** For email/SMS writing tips, templates, compliance, and deliverability guidelines, see [Best Practices — Email & SMS](Best-Practices-Email-SMS.md)

> ⏭️ **Next:** [Module 7 — Calendars & Appointment Booking](07_Calendars-Booking.md)

