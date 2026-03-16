# Module 7: Calendars & Appointment Booking

🎯 **Objective:** Set up calendars, configure booking pages, and automate the entire appointment lifecycle — from booking to follow-up.

---

## 7.1 Why Calendar Management Matters for Sales

Every missed booking or forgotten appointment costs revenue. GHL's Calendar system:
- ✅ Lets prospects **self-book** without back-and-forth emails
- ✅ **Syncs** with Google Calendar and Outlook
- ✅ Sends **automated reminders** to reduce no-shows
- ✅ Integrates with **Workflows** for follow-up automation
- ✅ Supports **team calendars** with round-robin assignment

---

## 7.2 Calendar Types in GHL

| Type | Description | Best for |
|------|------------|----------|
| **Personal Calendar** | Linked to one team member | 1-on-1 consultations |
| **Round Robin** | Distributes bookings across team members | Sales team scheduling |
| **Class Booking** | Multiple attendees book the same time slot | Webinars, group sessions |
| **Service Calendar** | Resource-based booking | Room reservations, equipment |

---

## 7.3 Setting Up a Calendar

### Step 1: Create the Calendar
1. Go to **Calendars** → **"+ Add Calendar"**
2. Select calendar type
3. Configure:
   - **Calendar Name** — e.g., "Free Strategy Session"
   - **Description** — what the meeting is about
   - **Duration** — 15 min, 30 min, 60 min
   - **Location** — in-person address, Zoom link, or phone call

### Step 2: Set Availability

| Setting | Description |
|---------|------------|
| **Working Hours** | Days and times you accept bookings (e.g., Mon–Fri, 9 AM – 5 PM) |
| **Buffer Time** | Gap between meetings (e.g., 15 min before/after) |
| **Min Scheduling Notice** | Earliest someone can book (e.g., 24 hours ahead) |
| **Max Booking Window** | How far in advance they can book (e.g., 30 days) |
| **Slot Interval** | Spacing of available slots (e.g., every 30 min) |

### Step 3: Customize the Booking Page

The booking page is what prospects see when they schedule:
- Add your **logo** and **brand colors**
- Write a **compelling description** of the meeting value
- Choose which **form fields** to collect (name, email, phone, custom questions)
- Add **pre-meeting instructions**

### Step 4: Sync External Calendars
- Connect **Google Calendar** or **Outlook** to avoid double-booking
- GHL checks your external calendar for conflicts in real-time

---

## 7.4 Embedding & Sharing Calendars

| Method | How |
|--------|-----|
| **Direct Link** | Share the booking URL via email, SMS, or social media |
| **Embed on Website** | Use the embed code in your website or funnel page |
| **Funnel Step** | Add a Calendar element directly to a funnel page |
| **QR Code** | Generate a QR code linking to the booking page |

---

## 7.5 Automating the Appointment Lifecycle

### Workflow: Complete Appointment Automation

```
BEFORE BOOKING:
[Lead clicks booking link] → Booking page opens

AT BOOKING:
Trigger: Appointment Booked
    │
    ▼
[Immediately]
    ✅ Email: Booking confirmation + meeting details
    ✅ SMS: "Confirmed! See you on {{appointment.date}} at {{appointment.time}}"
    ✅ Internal: Notify assigned team member
    ✅ CRM: Create/update Opportunity → "Discovery Call" stage

REMINDERS:
    ▼
[24 hours before]
    📱 SMS: "Reminder: Your meeting is tomorrow at {{time}}"
    │
    ▼
[1 hour before]
    📱 SMS: "Starting in 1 hour! Here's your meeting link: [URL]"

AFTER MEETING:
Trigger: Appointment Completed
    │
    ▼
[1 hour after]
    📧 Email: "Thanks for meeting! Here's a summary + next steps"
    ✅ CRM: Move Opportunity → "Proposal Sent" stage
    ✅ Task: "Send proposal within 24 hours"

NO-SHOW HANDLING:
Trigger: Appointment Status = No-Show
    │
    ▼
[Immediately]
    📱 SMS: "We missed you today! Want to reschedule?"
    │
    ▼
[Wait 1 day]
    📧 Email: Reschedule link + alternative time suggestions
    │
    ▼
[Wait 3 days - no response]
    📱 SMS: Final attempt to reconnect
```

---

## 7.6 Round Robin Setup for Sales Teams

### How It Works
1. Create a Round Robin calendar
2. Add team members
3. Set **distribution method:**
   - **Equal distribution** — distributes evenly
   - **Availability-based** — books whoever is free first
   - **Priority-based** — tries first team member first, then fallback

### Optimization Tips
- Set individual **availability** for each team member
- Use **lead assignment rules** based on region, deal size, or product interest
- Track **booking rates per team member** in Reporting

---

## 7.7 Payment Collection at Booking

GHL allows you to **charge at the time of booking** — great for paid consultations or services:
1. Connect **Stripe** or **PayPal** in Settings
2. In Calendar settings, enable **Require Payment**
3. Set the price and currency
4. Prospects pay when they book — reducing no-shows

---


> ⏭️ **Next:** [Module 8 — Reputation Management](08_Reputation-Management.md)

