# Module 6: Email & SMS Marketing

🎯 **Objective:** Create, send, and automate email and SMS campaigns that engage leads and drive conversions.

---

## 6.1 Why Email & SMS Together?

| Channel | Open Rate | Response Speed | Best for |
|---------|:---------:|:--------------:|----------|
| **Email** | 20–30% | Hours to days | Detailed content, nurture, newsletters |
| **SMS** | 90–98% | Minutes | Urgent messages, reminders, short offers |

> 💡 **Tip:** Use them together — email for content-rich messages, SMS for time-sensitive nudges. GHL lets you orchestrate both in a single workflow.

---

## 6.2 Email Marketing in GHL

### 6.2.1 Email Builder

GHL provides a **drag-and-drop email builder** with:
- Pre-designed templates (categorized by industry)
- Custom HTML support
- Mobile-responsive preview
- Dynamic content with merge fields

### 6.2.2 Types of Emails

| Type | Description | When to use |
|------|------------|-------------|
| **Broadcast** | One-time send to a list or Smart List | Announcements, promotions |
| **Workflow Email** | Triggered by an event (auto-sent) | Welcome series, follow-ups |
| **Template** | Reusable design saved for later | Standardize branding |

### 6.2.3 Writing Effective Emails

**Subject Line Best Practices:**
- Keep under 50 characters
- Create curiosity or urgency
- Personalize: "{{contact.first_name}}, here's your exclusive offer"
- Avoid spam words: FREE!!!, CLICK HERE, ACT NOW

**Email Structure:**

```
┌─────────────────────────────────┐
│  HEADER (Logo + brand color)    │
├─────────────────────────────────┤
│  OPENING LINE                   │
│  "Hi {{first_name}},"           │
│  Hook them in the first line    │
├─────────────────────────────────┤
│  BODY                           │
│  • One main idea per email      │
│  • Short paragraphs (2-3 lines) │
│  • Use bullet points            │
│  • Include relevant image       │
├─────────────────────────────────┤
│  CTA (Call-to-Action)           │
│  One clear button or link       │
│  e.g., "Book Your Free Call"    │
├─────────────────────────────────┤
│  SIGNATURE                      │
│  Name, title, company, photo    │
├─────────────────────────────────┤
│  FOOTER                         │
│  Unsubscribe link (required)    │
│  Company address                │
└─────────────────────────────────┘
```

### 6.2.4 Sending a Broadcast Email

1. Go to **Marketing** → **Emails** → **"+ Create Email"**
2. Choose a template or start from scratch
3. Design the email content
4. Select recipients:
   - All contacts
   - A specific **Smart List**
   - Contacts with specific **Tags**
5. Set **send time** (immediate or scheduled)
6. **Preview & Test** — send a test email to yourself first
7. Click **Send** or **Schedule**

### 6.2.5 Email Metrics to Track

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

### 6.3.3 SMS Best Practices

✅ **Do:**
- Keep messages under 160 characters (1 SMS segment)
- Include your business name (recipients may not know the number)
- Personalize: "Hi [Name], ..."
- Include a clear CTA
- Respect time zones — send during business hours

❌ **Don't:**
- Send more than 2–3 SMS per week
- Use ALL CAPS
- Include unsolicited links without context
- Forget to include opt-out instructions: "Reply STOP to unsubscribe"

### 6.3.4 SMS Templates

Save time with pre-written templates:

**Appointment Reminder:**
> Hi {{contact.first_name}}, this is a reminder of your appointment with [Company] tomorrow at {{appointment.time}}. Reply YES to confirm or call us at [Phone].

**Follow-up After No Reply:**
> Hi {{contact.first_name}}, we tried reaching you regarding [service]. Still interested? Reply YES and we'll get back to you shortly.

**Post-Purchase Thank You:**
> Thanks for choosing [Company], {{contact.first_name}}! Your order is confirmed. Questions? Reply to this message.

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

## 6.5 Compliance & Deliverability

### Email Compliance
- ✅ Include an **unsubscribe link** in every email (legally required)
- ✅ Use a **verified sending domain** (SPF, DKIM, DMARC)
- ✅ Maintain list hygiene — remove bounced addresses
- ✅ Honor opt-out requests within 24 hours

### SMS Compliance
- ✅ Obtain **explicit opt-in** before sending
- ✅ Include **business identification** in messages
- ✅ Provide **opt-out instructions** (reply STOP)
- ✅ Comply with **TCPA** (USA), **CASL** (Canada), or local regulations

### Deliverability Tips
- Warm up new email domains gradually (start with 50/day, increase weekly)
- Avoid spam trigger words in subject lines
- Maintain a clean contact list — remove inactive addresses regularly
- Authenticate your domain (SPF + DKIM + DMARC)

---


> ⏭️ **Next:** [Module 7 — Calendars & Appointment Booking](07_Calendars-Booking.md)

