# Best Practices: Email & SMS Marketing

> 📖 **Reference companion** to [Module 6 — Email & SMS Marketing](06_Email-SMS-Marketing.md)

---

## 1. Writing Effective Emails

### Subject Line Best Practices

| ✅ Do | ❌ Don't |
|-------|---------| 
| Keep under 50 characters | Write novels in the subject |
| Create curiosity or urgency | Use ALL CAPS |
| Personalize: "{{first_name}}, quick question" | Use spam words: FREE!!! CLICK NOW! |
| A/B test 2 versions | Use the same subject every time |

### Recommended Email Structure

```
┌──────────────────────────────┐
│ HEADER: Logo + brand colors  │
├──────────────────────────────┤
│ Hi {{first_name}},           │
│                              │
│ [One compelling opening line │
│  that hooks them]            │
│                              │
│ [2-3 short paragraphs with  │
│  the main value/message]     │
│                              │
│ [Optional: bullet points]    │
│                              │
│ ┌────────────────────────┐   │
│ │   [ CTA BUTTON ]       │   │
│ │   "Book Your Call"      │   │
│ └────────────────────────┘   │
│                              │
│ Best regards,                │
│ [Name + Signature]           │
├──────────────────────────────┤
│ FOOTER: Unsubscribe | Address│
└──────────────────────────────┘
```

---

## 2. Email Operations Checklist

```
BEFORE SENDING:
☐ Subject line is compelling and under 50 chars
☐ Personalization fields are correct (test with preview)
☐ CTA button works and links to correct page
☐ Unsubscribe link is present (legally required)
☐ Mobile preview looks good
☐ Test email sent to yourself

AFTER SENDING:
☐ Check delivery rate within 1 hour
☐ Monitor open rate after 24 hours
☐ Review click rate after 48 hours
☐ Respond to any replies in Conversations
```

---

## 3. SMS Best Practices

| ✅ Do | ❌ Don't |
|-------|---------|
| Keep under 160 characters (1 SMS segment) | Send more than 2–3 SMS per week |
| Include your business name | Use ALL CAPS |
| Personalize: "Hi {{first_name}}" | Send late at night or early morning |
| Include a clear CTA | Forget opt-out: "Reply STOP to unsubscribe" |
| Send during business hours | Send links without context |

---

## 4. SMS Templates

**Appointment Reminder:**
> Hi {{contact.first_name}}, this is a reminder of your appointment with [Company] tomorrow at {{appointment.time}}. Reply YES to confirm or call us at [Phone].

**Follow-up After No Reply:**
> Hi {{contact.first_name}}, we tried reaching you regarding [service]. Still interested? Reply YES and we'll get back to you shortly.

**Post-Purchase Thank You:**
> Thanks for choosing [Company], {{contact.first_name}}! Your order is confirmed. Questions? Reply to this message.

**Post-Service Thank You:**
> Thanks for choosing [Company], {{contact.first_name}}! We hope you loved the experience. Reply with any feedback — we'd love to hear from you.

**Review Request:**
> Hi {{contact.first_name}}, it was great working with you! Would you mind leaving us a quick review? [Google Review Link] Thank you! ⭐

---

## 5. Compliance & Deliverability

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
