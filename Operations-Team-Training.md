# 📚 GoHighLevel (GHL) Training — Operations Team
## Comprehensive Hands-On Guide

---

> **Version:** 1.0 | **Updated:** March 2026  
> **Audience:** Operations Team — Account Managers, Campaign Operators, Client Success  
> **Format:** Detailed training on daily-use features + overview of supporting features

---

## 📋 Table of Contents

### Part 1: Detailed Training (Day-to-Day Operations)

| # | Topic | Depth |
|---|-------|:-----:|
| 1 | [Platform Overview & Navigation](#1-platform-overview--navigation) | 🟢 Overview |
| 2 | [CRM & Contact Management](#2-crm--contact-management) | 🔵 **Detailed** |
| 3 | [Sales Pipelines & Opportunities](#3-sales-pipelines--opportunities) | 🔵 **Detailed** |
| 4 | [Email Marketing](#4-email-marketing) | 🔵 **Detailed** |
| 5 | [SMS Campaigns](#5-sms-campaigns) | 🔵 **Detailed** |
| 6 | [Calendar & Appointment Booking](#6-calendar--appointment-booking) | 🔵 **Detailed** |
| 7 | [Reputation Management](#7-reputation-management) | 🔵 **Detailed** |
| 8 | [Social Media Planner](#8-social-media-planner) | 🔵 **Detailed** |
| 9 | [Ad Manager (Facebook & Google)](#9-ad-manager-facebook--google) | 🔵 **Detailed** |

### Part 2: Feature Overviews (Awareness Level)

| # | Topic | Depth |
|---|-------|:-----:|
| 10 | [Funnels & Landing Pages](#10-funnels--landing-pages-overview) | 🟢 Overview |
| 11 | [Workflows & Automation](#11-workflows--automation-overview) | 🟢 Overview |
| 12 | [AI Features](#12-ai-features-overview) | 🟢 Overview |
| 13 | [Memberships & Communities](#13-memberships--communities-overview) | 🟢 Overview |
| 14 | [Reporting & Analytics](#14-reporting--analytics-overview) | 🟢 Overview |

---

# PART 1: DETAILED TRAINING

---

# 1. Platform Overview & Navigation

GoHighLevel (GHL) is an **all-in-one Sales & Marketing platform** that replaces 10+ standalone tools with a single dashboard.

### Sidebar Navigation

| # | Menu Item | What You'll Use It For |
|---|-----------|----------------------|
| 1 | **Dashboard** | Quick KPI overview |
| 2 | **Conversations** | Reply to SMS, email, chat, DMs — all in one inbox |
| 3 | **Calendars** | Manage and monitor bookings |
| 4 | **Contacts** | CRM — your daily home base |
| 5 | **Opportunities** | Pipeline — track deals |
| 6 | **Payments** | View invoices and transactions |
| 7 | **Marketing** | Email campaigns, SMS blasts, Social Planner, Ads |
| 8 | **Automation** | Workflows (view/monitor, not build) |
| 9 | **Sites** | Funnels & websites (view/minor edits) |
| 10 | **Memberships** | Courses & communities (manage access) |
| 11 | **Reputation** | Reviews — request and respond |
| 12 | **Reporting** | Check campaign performance |

### Key Terms Quick Reference

| Term | Meaning |
|------|---------|
| **Contact** | A person (lead or customer) in your CRM |
| **Tag** | A label for segmentation (e.g., `source_facebook`, `status_vip`) |
| **Smart List** | A dynamic, auto-updating filtered contact list |
| **Opportunity** | A deal on your sales pipeline board |
| **Workflow** | An automated sequence of actions triggered by an event |
| **Funnel** | A multi-page lead-capture or sales sequence |

---

# 2. CRM & Contact Management

> 🔵 **Detailed Training** — This is your daily home base. Master it.

## 2.1 Accessing Contacts

Go to **Contacts** in the sidebar. You'll see:
- **All Contacts** list with search and filters
- **Smart Lists** tab for saved filtered views
- **Bulk Actions** bar for operating on multiple contacts

## 2.2 Adding Contacts

### Manual Entry
1. Click **"+ Add Contact"**
2. Fill in required fields:
   - **First Name** / **Last Name**
   - **Email** and/or **Phone**
   - **Tags** — always tag at creation (e.g., `source_manual`, `status_new-lead`)
   - **Source** — where the lead came from
3. Click **Save**

### CSV Import
1. Contacts → **Import Contacts**
2. Upload your CSV file
3. **Map columns** to GHL fields (First Name → First Name, Email → Email, etc.)
4. Set a default **Tag** for all imported contacts (e.g., `import_march-2026`)
5. Click Import

### Automatic Entry
Contacts are auto-created when someone:
- Fills out a **form** on a funnel or website
- Submits a **Facebook Lead Ad**
- Sends a message via **chat widget**, SMS, or social DM
- Books an **appointment**

## 2.3 The 360° Contact Record

Click any contact to open their full profile:

| Tab | What's Inside | Operations Use |
|-----|--------------|---------------|
| **Details** | Name, email, phone, company, custom fields | Update info, add tags |
| **Conversations** | Full SMS, email, chat, and call history | Review past communications |
| **Opportunities** | Linked deals in pipelines | Check deal status |
| **Appointments** | Booked meetings | Verify upcoming calls |
| **Tasks** | To-dos linked to this contact | Track follow-up items |
| **Notes** | Internal team notes | Add context for team |
| **Activity** | Pages visited, emails opened, links clicked | Gauge engagement level |
| **Payments** | Invoices and transaction history | Verify payment status |

## 2.4 Tags — Your Segmentation System

Tags let you label and group contacts. Use a consistent naming convention:

```
FORMAT: category_detail

EXAMPLES:
source_facebook-ads       status_new-lead
source_google-ads         status_contacted
source_referral           status_qualified
source_website            status_customer

interest_seo              segment_vip
interest_web-design       segment_enterprise
interest_social-media     segment_sme

campaign_spring-2026      action_booked-call
campaign_webinar-mar      action_downloaded-guide
```

### How to Add Tags
- **On a contact:** Open contact → Tags field → type and add
- **In bulk:** Select multiple contacts → Bulk Actions → Add Tag
- **Automatically:** Via workflows (form submitted → add tag)

### Daily Operations with Tags
- **Before calling a lead:** Check their tags to know their interest and source
- **After a call:** Update tags (e.g., remove `status_new-lead`, add `status_contacted`)
- **For campaigns:** Use tags to target specific segments

## 2.5 Smart Lists

Smart Lists are **saved filter views** that auto-update. Essential for daily operations.

### Must-Have Smart Lists for Operations

| Smart List Name | Filter Logic | Daily Use |
|----------------|-------------|-----------|
| **Today's Follow-ups** | Task Due = Today | Morning priority list |
| **New Leads (24h)** | Created < 24 hours ago | Speed-to-lead check |
| **Hot Leads** | Tag = `status_qualified` + Activity < 7 days | Priority outreach |
| **Uncontacted** | Tag = `status_new-lead` + Created > 24h ago | Catch missed leads |
| **VIP Clients** | Tag = `segment_vip` | White-glove attention |
| **Facebook Leads** | Source = Facebook | Channel performance |
| **Birthday This Week** | Birthday = this week | Personal touch campaigns |

### Creating a Smart List
1. Go to **Contacts** → **Smart Lists** tab
2. Click **"+ Add Smart List"**
3. Name it → set filters → **Save**
4. Pin your most-used lists for quick access

## 2.6 Custom Fields

Custom Fields store business-specific data. Common operations fields:

| Field | Type | Example |
|-------|------|---------|
| Company Size | Dropdown | 1-10, 11-50, 51-200, 200+ |
| Monthly Budget | Number | 5000 |
| Industry | Dropdown | E-commerce, Healthcare, Real Estate |
| Account Manager | Dropdown | Staff names |
| Contract End Date | Date | 2026-12-31 |
| NDA Signed | Checkbox | Yes/No |

## 2.7 Bulk Actions

Select multiple contacts (checkbox) to perform:
- ✅ **Add / Remove Tags** in bulk
- ✅ **Send bulk Email or SMS**
- ✅ **Add to a Workflow**
- ✅ **Add to a Pipeline**
- ✅ **Export to CSV**
- ✅ **Delete** (use with caution!)

> ⚠️ **Warning:** Bulk delete is permanent. Always export before deleting.

## 2.8 Daily CRM Routine (Recommended)

```
MORNING (9:00 AM):
☐ Review "New Leads (24h)" Smart List → ensure all are contacted
☐ Check "Today's Follow-ups" → complete pending tasks
☐ Review Unified Inbox → reply to all new messages

MIDDAY (12:00 PM):
☐ Update contact tags/notes after morning calls
☐ Move opportunities to correct pipeline stages
☐ Flag any stuck leads for manager review

END OF DAY (5:00 PM):
☐ Log all interactions (notes on contacts)
☐ Set tomorrow's tasks and follow-ups
☐ Review pipeline for stale deals
```

### 📝 CRM Exercises
1. Create 5 contacts manually, each with proper tags and source
2. Import 10 contacts from a CSV with column mapping
3. Build 3 Smart Lists from the table above
4. Practice the Daily CRM Routine for one full day

---

# 3. Sales Pipelines & Opportunities

> 🔵 **Detailed Training** — Track every deal from first contact to closed-won.

## 3.1 Understanding the Pipeline Board

Go to **Opportunities** → select your pipeline. You'll see a Kanban board:

```
  New Lead    Contacted    Qualified    Proposal    Won ✅    Lost ❌
 ┌────────┐  ┌────────┐  ┌────────┐  ┌────────┐  ┌──────┐  ┌──────┐
 │ Deal A │  │ Deal C │  │ Deal F │  │ Deal H │  │Deal J│  │Deal K│
 │ $2,500 │  │ $5,000 │  │ $3,000 │  │ $8,000 │  │$4,000│  │$1,500│
 │ Deal B │  │ Deal D │  │ Deal G │  │        │  │      │  │      │
 │ $1,000 │  │ Deal E │  │        │  │        │  │      │  │      │
 └────────┘  └────────┘  └────────┘  └────────┘  └──────┘  └──────┘
```

Each card shows: **Contact name**, **Deal value**, **Assigned to**, **Age of deal**

## 3.2 Creating an Opportunity

1. Click **"+ Add Opportunity"** (or it auto-creates from a workflow)
2. Fill in:
   - **Contact** — select from CRM
   - **Pipeline** — choose which pipeline
   - **Stage** — starting stage (usually "New Lead")
   - **Value ($)** — deal amount
   - **Name** — descriptive (e.g., "Acme Corp — SEO Package")
   - **Assigned To** — responsible team member
   - **Expected Close Date** — when you expect to close

## 3.3 Moving Deals Through Stages

| Method | When to Use |
|--------|------------|
| **Drag & drop** on the board | Quick daily updates |
| **Edit the opportunity** → change Stage | When adding notes at the same time |
| **Automatic (Workflow)** | When a trigger fires (e.g., appointment booked) |

### Stage Update Checklist

After moving a deal, always:
1. ✅ Add a **Note** explaining why it moved
2. ✅ Set a **Task** for the next action
3. ✅ Update the **deal value** if it changed
4. ✅ Update the **expected close date**

## 3.4 Opportunity Details

Click any opportunity card to see:
- 📝 **Notes** — log every call, email, meeting
- ✅ **Tasks** — set follow-ups with due dates
- 📅 **Appointments** — linked meetings
- 💬 **Conversation history** — all messages with this contact
- 💰 **Value & close date** — editable at any time

## 3.5 Pipeline Views

| View | When to Use |
|------|------------|
| **Board (Kanban)** | Daily management — visual, drag-and-drop |
| **List** | Sorting by value, date, or assignee |
| **Table** | Exporting or detailed filtering |

## 3.6 Pipeline Hygiene Rules

1. **Update daily** — move deals to their correct stage every morning
2. **Mark "Lost" promptly** — dead deals clutter the board and skew forecasts
3. **No deal without a next action** — every opportunity needs a task or appointment
4. **Accurate values** — this drives revenue forecast accuracy
5. **Notes on every move** — "Why did the deal advance/stall?"

## 3.7 Key Pipeline Metrics

| Metric | How to Read It |
|--------|---------------|
| **Total Pipeline Value** | Sum of all open deals |
| **Deals per stage** | Are deals clustering somewhere? → bottleneck |
| **Average deal age** | Growing? → deals are stalling |
| **Win rate** | Won ÷ (Won + Lost) — target > 20% |
| **Average deal size** | Trending up = good upselling |

### 📝 Pipeline Exercises
1. Create 5 opportunities with realistic contact links and values
2. Practice drag-and-drop through all stages
3. Add a note and set a follow-up task on each opportunity
4. Calculate your total and weighted pipeline values

---

# 4. Email Marketing

> 🔵 **Detailed Training** — Create, send, and measure email campaigns.

## 4.1 Types of Emails in GHL

| Type | Trigger | Use Case |
|------|---------|----------|
| **Broadcast** | Manually sent to a list | Announcements, promos, newsletters |
| **Workflow Email** | Auto-sent by a workflow trigger | Welcome series, follow-ups |
| **1-to-1** | Sent from Conversations tab | Personal replies |

## 4.2 Creating a Broadcast Email

1. Go to **Marketing** → **Emails** → **"+ Create Email Campaign"**
2. **Name** the campaign
3. **Design** the email:
   - Start from a **template** or blank
   - Use the **drag-and-drop builder**:
     - Header (logo, brand colors)
     - Text blocks (short paragraphs, 2-3 lines max)
     - Images / videos
     - Button (CTA)
     - Footer (unsubscribe link + company address)
4. **Personalize** with merge fields:
   - `{{contact.first_name}}` → "Hi Sarah"
   - `{{contact.company_name}}` → "at Acme Corp"
5. **Select recipients:**
   - A **Smart List** (recommended)
   - Contacts with a specific **Tag**
   - All contacts (use sparingly)
6. **Set send time:**
   - Immediately
   - Scheduled (specific date + time)
7. **Preview & Test** — send to yourself first!
8. Click **Send** or **Schedule**

## 4.3 Writing Effective Emails

### Subject Line Rules
| ✅ Do | ❌ Don't |
|-------|---------|
| Keep under 50 characters | Write novels in the subject |
| Create curiosity | Use ALL CAPS |
| Personalize: "{{first_name}}, quick question" | Use spam words: FREE!!! CLICK NOW! |
| A/B test 2 versions | Use the same subject every time |

### Email Structure

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
│  the main value/message]    │
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

## 4.4 Email Metrics — What to Monitor

| Metric | Good Benchmark | If Low → Action |
|--------|:--------------:|----------------|
| **Open Rate** | > 25% | Fix subject lines, clean list |
| **Click Rate** | > 3% | Improve CTA, content relevance |
| **Bounce Rate** | < 2% | Remove invalid emails |
| **Unsubscribe Rate** | < 0.5% | Reduce frequency, improve targeting |

## 4.5 Email Operations Checklist

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

### 📝 Email Exercises
1. Create a broadcast email using a template
2. Write 3 subject lines for the same email and pick the best
3. Send a test email to yourself — check desktop + mobile rendering
4. Send a broadcast to a Smart List of 10+ contacts
5. Check the campaign report 24 hours later

---

# 5. SMS Campaigns

> 🔵 **Detailed Training** — Send targeted SMS messages with 90%+ open rates.

## 5.1 Types of SMS

| Type | How It Works | Use Case |
|------|-------------|----------|
| **1-to-1** | Manual from Conversations tab | Personal follow-ups |
| **Broadcast** | Bulk send to a list/tag | Flash sales, announcements |
| **Workflow SMS** | Auto-sent by trigger | Appointment reminders |
| **Two-way** | Real-time conversation | Qualification, support |

## 5.2 Sending a 1-to-1 SMS

1. Open **Conversations** in the sidebar
2. Select a contact (or search)
3. Choose the **SMS** channel
4. Type your message → click **Send**

## 5.3 Sending a Broadcast SMS

1. Go to **Marketing** → **Bulk Actions** or use a workflow
2. Select recipients (Smart List or Tag)
3. Write the message:

### SMS Templates for Operations

**Appointment Reminder:**
> Hi {{contact.first_name}}, reminder: you have an appointment with [Company] tomorrow at {{appointment.time}}. Reply YES to confirm or call us at [Phone].

**Follow-up After No Reply:**
> Hi {{contact.first_name}}, we tried reaching you about [service]. Still interested? Reply YES and we'll get back to you shortly.

**Post-Service Thank You:**
> Thanks for choosing [Company], {{contact.first_name}}! We hope you loved the experience. Reply with any feedback — we'd love to hear from you.

**Review Request:**
> Hi {{contact.first_name}}, it was great working with you! Would you mind leaving us a quick review? [Google Review Link] Thank you! ⭐

## 5.4 SMS Best Practices

| ✅ Do | ❌ Don't |
|-------|---------|
| Keep under 160 characters | Send more than 3 SMS/week |
| Include your business name | Use ALL CAPS |
| Personalize: "Hi {{first_name}}" | Send late at night or early morning |
| Include a clear CTA | Forget opt-out: "Reply STOP to unsubscribe" |
| Send during business hours | Send links without context |

## 5.5 Compliance Essentials

- ✅ **Opt-in required** — contacts must consent before you send
- ✅ **Include business ID** — they need to know who's texting
- ✅ **Offer opt-out** — always include "Reply STOP to unsubscribe"
- ✅ **Respect opt-outs** — removing contacts who reply STOP is automatic in GHL

> ⚠️ **SMS costs money** — each segment (160 chars) has a per-message cost. Keep messages concise.

### 📝 SMS Exercises
1. Send a 1-to-1 SMS from the Conversations tab
2. Write 3 SMS templates (reminder, follow-up, review request)
3. Send a test broadcast to a small list (5 contacts)
4. Check delivery status and responses

---

# 6. Calendar & Appointment Booking

> 🔵 **Detailed Training** — Manage appointments end-to-end.

## 6.1 Calendar Types

| Type | Description | Use Case |
|------|------------|----------|
| **Personal** | One person's calendar | 1-on-1 consultations |
| **Round Robin** | Distributes across team | Balanced team scheduling |
| **Class Booking** | Multiple attendees, same slot | Webinars, group sessions |

## 6.2 Creating a Calendar

1. Go to **Calendars** → **"+ Add Calendar"**
2. Configure:

| Setting | What to Set |
|---------|------------|
| **Name** | "Free Strategy Session" |
| **Duration** | 15, 30, or 60 minutes |
| **Location** | Zoom link, phone, or address |
| **Working Hours** | Mon–Fri, 9 AM – 5 PM |
| **Buffer Time** | 15 min gap between meetings |
| **Min Notice** | 24 hours (how far ahead they must book) |
| **Max Window** | 30 days (how far ahead they can book) |

3. **Sync** external calendar (Google or Outlook) → prevents double-bookings
4. Customize the **booking page** (logo, colors, description, form fields)

## 6.3 Sharing the Calendar

| Method | How |
|--------|-----|
| **Direct link** | Copy booking URL → share via email, SMS, social |
| **Embed** | Paste embed code into a funnel or website page |
| **QR code** | Generate a QR code linking to the booking page |

## 6.4 Managing Appointments

In the **Calendars** section, you can:
- View by **day, week, or month**
- See **who is booked** and with which team member
- **Reschedule** — drag to a new time slot
- **Cancel** — click → cancel (sends notification)
- **Mark No-show** — if contact didn't appear
- View **appointment notes** added by the team

## 6.5 Appointment Lifecycle (Operations View)

```
1. BOOKING         → Contact books via link or you book manually
2. CONFIRMATION    → Auto-email/SMS: "You're confirmed for [Date/Time]"
3. REMINDER (24h)  → Auto-SMS: "Your meeting is tomorrow"
4. REMINDER (1h)   → Auto-SMS: "Starting in 1 hour!"
5. MEETING         → Conduct the meeting
6. POST-MEETING    → Update pipeline stage + add notes
7. NO-SHOW         → Auto-SMS: "We missed you — want to reschedule?"
```

> Steps 2–4 and 7 are automated via workflows. Your job is steps 1, 5, and 6.

## 6.6 Booking Manually for a Contact

1. Open the contact's record
2. Click **"Book Appointment"**
3. Select calendar and time slot
4. Confirm → auto-sends confirmation to contact

### 📝 Calendar Exercises
1. Create a "Free Consultation" calendar with 30-min slots
2. Sync your Google or Outlook calendar
3. Share the booking link and make a test booking
4. Practice rescheduling and canceling
5. Book an appointment from inside a contact's record

---

# 7. Reputation Management

> 🔵 **Detailed Training** — Get more 5-star reviews and handle negative feedback.

## 7.1 Why It Matters

- **93%** of consumers read reviews before buying
- Businesses with **4.5+ stars** get dramatically more leads
- **70%** of people will leave a review *if asked*

## 7.2 Setting Up

1. Go to **Reputation** in the sidebar
2. Connect **Google Business Profile**
3. Connect **Facebook Page** (optional)
4. Dashboard now shows: average rating, review count, recent reviews

## 7.3 The Smart Review Funnel

This is the most effective review strategy:

```
Service Completed
    │
    ▼
Send SMS: "How was your experience? Reply 1-5"
    │
    ├── Reply: 4 or 5 ⭐
    │     └── SMS: "So glad! Would you leave us a Google review?"
    │           └── [Direct link to Google review page]
    │
    └── Reply: 1–3 ⭐
          └── SMS: "We're sorry. What can we improve?"
                └── Routes to private feedback form
                └── Creates task for manager: "Call {{name}}"
```

> 💡 **Key Insight:** Happy customers go to public reviews. Unhappy customers go to private feedback. This protects your rating while still capturing complaints.

## 7.4 Responding to Reviews

### Response Templates

**5-Star Review:**
> Thank you so much, [Name]! We're thrilled you had a great experience. It was a pleasure working with you, and we look forward to helping you again soon! ⭐

**3-Star Review:**
> Thank you for your feedback, [Name]. We're glad you had a positive experience, and we'd love to know how we can earn that 5th star. Please reach out to us at [email/phone].

**1-2 Star Review:**
> We're sorry to hear about your experience, [Name]. This isn't the standard we aim for. Please contact us directly at [email/phone] so we can make things right.

### Response Rules
1. ✅ **Respond within 24 hours**
2. ✅ **Always be professional** — never argue publicly
3. ✅ **Use the reviewer's name**
4. ✅ **Take complaints offline** — offer to call/email
5. ✅ **Respond to every review** — including positive ones

## 7.5 Daily Reputation Routine

```
DAILY (takes 5 minutes):
☐ Check Reputation dashboard for new reviews
☐ Respond to any unresponded reviews
☐ Trigger review requests for completed services (if not automated)
```

### 📝 Reputation Exercises
1. Connect your Google Business Profile
2. Write response templates for 5-star, 3-star, and 1-star reviews
3. Send a test review request SMS to yourself
4. Review your current average rating and set a 90-day goal

---

# 8. Social Media Planner

> 🔵 **Detailed Training** — Schedule and manage social media content.

## 8.1 Supported Platforms

| Platform | Post Types |
|----------|-----------|
| **Facebook** (Pages & Groups) | Image, Video, Link, Text |
| **Instagram** (Business/Creator) | Posts, Stories, Reels |
| **LinkedIn** (Profiles & Pages) | Image, Video, Text |
| **X (Twitter)** | Text, Image, Video |
| **TikTok** | Video |
| **Google Business Profile** | Posts, Offers |
| **Threads** / **Bluesky** | Text, Image |

## 8.2 Connecting Accounts

1. Go to **Marketing** → **Social Planner**
2. Click **"Connect Account"**
3. Authorize each platform
4. Select which pages/profiles to manage

## 8.3 Creating & Scheduling Posts

1. Click **"Create Post"**
2. Select **platforms** (multi-select)
3. Write **caption** — use AI (✨ button) to help generate or refine
4. Attach **media** (image, video, GIF)
5. Add **hashtags**
6. Choose timing:
   - **Post Now**
   - **Schedule** for a specific date/time
   - **Add to Queue** (auto-posts based on queue schedule)
7. **Preview** each platform view
8. Click **Schedule** or **Publish**

## 8.4 Content Calendar View

The **Calendar View** shows all scheduled posts across platforms:
- **Drag & drop** to reschedule
- Color-coded by platform
- Click any slot to create a new post
- Filter by platform or status (draft, scheduled, published)

## 8.5 Content Categories & Queues

Set up recurring time slots for category-based posting:

| Category | Schedule | Content Type |
|----------|----------|-------------|
| Tips & Tricks | Monday 10 AM | Educational |
| Customer Story | Wednesday 2 PM | Social proof |
| Behind the Scenes | Friday 11 AM | Engagement |
| Promo / Offer | Saturday 9 AM | Sales-driven |

Posts assigned to a category auto-publish at the next available slot.

## 8.6 Bulk Content Upload

For planning weeks ahead:
1. Prepare a **CSV file** (date, time, caption, image URL, platform)
2. Social Planner → **Bulk Upload**
3. Map columns → import
4. Review on calendar

## 8.7 Comment Management

- View and **reply to comments** directly in GHL
- No need to open each platform separately
- Comments from Facebook, Instagram, and Google Business Profile

## 8.8 Social Media Analytics

Track per-post performance:

| Metric | What It Tells You |
|--------|------------------|
| **Reach** | How many unique people saw the post |
| **Impressions** | Total times the post was displayed |
| **Engagement** | Likes, comments, shares, saves |
| **Clicks** | Link clicks from the post |

### Weekly Review
- Identify **top-performing** content type and platform
- Double down on what works
- Adjust posting times based on engagement patterns

### 📝 Social Planner Exercises
1. Connect 2+ social media accounts
2. Create and schedule 5 posts for the upcoming week
3. Use AI to generate 3 captions
4. Set up 3 content category queues
5. Review analytics for the past 7 days

---

# 9. Ad Manager (Facebook & Google)

> 🔵 **Detailed Training** — Run, monitor, and measure paid ads from GHL.

## 9.1 Connecting Ad Accounts

### Facebook Ads
1. **Settings** → **Integrations** → **Facebook**
2. Log in → select Ad Account(s) and Page(s) → authorize

### Google Ads
1. **Settings** → **Integrations** → **Google**
2. Click "Connect Google Ads" → log in → select account(s)

## 9.2 Creating Facebook Ads

1. **Marketing** → **Ad Manager** → **"+ Create Ad"** → Facebook
2. Configure:
   - **Objective** — Lead Generation, Traffic, or Conversions
   - **Audience** — demographics, interests, custom audience, lookalike
   - **Placement** — Feed, Stories, Reels, Messenger
   - **Budget** — daily or lifetime
   - **Creative** — image/video, headline, description, CTA
   - **Lead Form** — Facebook form or redirect to GHL funnel

### What Happens When a Facebook Lead Comes In

```
Lead submits Facebook form
    │
    ▼ [Instant — within seconds]
    ✅ Contact created in CRM with tags + source
    ✅ Opportunity created in pipeline
    ✅ SMS to lead: "Thanks for reaching out!"
    ✅ Notification to sales rep: "New Facebook lead 🔥"
```

## 9.3 Creating Google Ads

1. **Marketing** → **Ad Manager** → **"+ Create Ad"** → Google
2. Configure:
   - **Campaign Type** — Search, Display, or Performance Max
   - **Keywords** — target + negative keywords
   - **Ad Copy** — headlines + descriptions
   - **Landing Page** — GHL funnel or external URL
   - **Budget** — daily
   - **Bidding** — maximize conversions or target CPA

## 9.4 Custom Audiences (Facebook)

Build audiences from your CRM data:

| Audience Type | Source | Use For |
|--------------|--------|---------|
| **Retargeting** | Funnel/site visitors | Re-engage non-converters |
| **Lookalike** | Your best customers | Find similar prospects |
| **Email Match** | CRM contact list | Target existing contacts on FB |
| **Exclusion** | Current customers | Avoid wasting spend |

## 9.5 Monitoring Ad Performance

### Key Metrics Dashboard

| Metric | Facebook | Google |
|--------|----------|--------|
| **Impressions** | ✅ | ✅ |
| **Clicks** | ✅ | ✅ |
| **CTR** | ✅ | ✅ |
| **CPC** | ✅ | ✅ |
| **Leads / Conversions** | ✅ | ✅ |
| **CPL (Cost Per Lead)** | ✅ | ✅ |
| **ROAS** | Pipeline + Revenue | Pipeline + Revenue |

### Daily Ad Operations Checklist

```
DAILY:
☐ Check ad spend vs. budget
☐ Review CPL — is it within target?
☐ Verify new leads synced to CRM
☐ Check for disapproved ads → fix and resubmit

WEEKLY:
☐ Compare this week vs. last week performance
☐ Pause underperforming ad sets (high CPC, low CTR)
☐ Test new ad creative or copy variations
☐ Update custom audiences with fresh CRM data
```

## 9.6 Generating Client Reports

1. **Reporting** → **Ad Reports**
2. Select date range and campaigns
3. Export as **PDF** (branded with your logo)
4. Schedule **auto-reports** weekly or monthly via email

### 📝 Ad Manager Exercises
1. Connect a Facebook and/or Google Ads account
2. Create a test Facebook Lead Ad campaign
3. Verify a test lead syncs to CRM with correct tags
4. Generate an ad performance report for the past 7 days
5. Create a custom audience from a CRM Smart List

---

# PART 2: FEATURE OVERVIEWS

> The following features are managed by specialists or leadership. As operations, you only need awareness-level understanding.

---

# 10. Funnels & Landing Pages (Overview)

**What they are:** Multi-step web pages designed to capture leads or drive sales.

**Your involvement:**
- Share funnel links with leads when needed
- Report broken pages or form issues to the team
- Know which funnels are active for which campaigns

**Key terms:** Funnel = multi-page sequence. Landing page = single focused page. Both have forms that auto-create contacts in CRM.

> 📖 Full training: See `05_Funnels-Landing-Pages.md`

---

# 11. Workflows & Automation (Overview)

**What they are:** Automated sequences — when X happens, do Y (then Z, then...).

**Your involvement:**
- You **trigger** workflows by adding tags or moving pipeline stages
- You **monitor** if a contact is stuck in a workflow
- You **don't build** workflows (that's admin/strategy)

**Common workflows you'll interact with:**
- Welcome email sequence → triggered when a new lead enters
- Appointment reminders → triggered when a booking is made
- Follow-up SMS → triggered when a deal stalls
- Review request → triggered after service completion

**How to check:** Open a contact → Activity tab → see which workflows are active

> 📖 Full training: See `04_Marketing-Automation.md` and `09_Advanced-Workflows.md`

---

# 12. AI Features (Overview)

**What they are:** AI-powered assistants that handle calls, chats, and content.

**Your involvement:**
- Monitor AI conversations for accuracy
- Escalate complex queries the AI can't handle
- Flag incorrect AI responses for Knowledge Base updates

**Key AI tools:**
| Tool | What It Does |
|------|-------------|
| **Voice AI** | Answers phone calls, qualifies leads, books appointments |
| **Conversation AI** | Responds to SMS, chat, social DMs automatically |
| **AI Content** | Helps write email copy, social captions, SMS templates |

> 📖 Full training: See `10_AI-Features.md`

---

# 13. Memberships & Communities (Overview)

**What they are:** Online courses (LMS) and private community forums built into GHL.

**Your involvement:**
- **Grant/revoke** course access for clients (via tags or manually)
- **Monitor** enrollment and completion rates
- **Moderate** community posts if assigned
- Escalate technical issues to admin

**Key concepts:** Course = video lessons + quizzes + certificates. Community = branded discussion forum.

> 📖 Full training: See `15_Memberships-Courses.md`

---

# 14. Reporting & Analytics (Overview)

**What they are:** Dashboards and reports covering pipeline, marketing, and ads performance.

**Your involvement:**
- Check your **personal performance** dashboard daily
- Review **campaign metrics** after sends (open rate, click rate)
- Pull **pipeline reports** for weekly team meetings
- Export data when requested by management

**Key reports:**
| Report | What It Shows |
|--------|-------------|
| Pipeline Overview | Deals by stage and value |
| Lead Source | Where leads are coming from |
| Campaign Stats | Email/SMS open and click rates |
| Ad Performance | CPL, ROAS, spend vs. budget |

> 📖 Full training: See `11_Reporting-Analytics.md`

---

# Quick Reference Card

## Daily Operations Checklist

```
🌅 MORNING
  ☐ Check Unified Inbox — respond to all new messages
  ☐ Review "New Leads (24h)" Smart List
  ☐ Complete "Today's Follow-ups" tasks
  ☐ Check pipeline board — any stale deals?
  ☐ Review Reputation dashboard — respond to new reviews

📊 MIDDAY
  ☐ Update CRM — add notes from morning calls
  ☐ Move pipeline opportunities to correct stages
  ☐ Check scheduled social posts — any drafts need attention?
  ☐ Monitor ad performance — CPL within target?

🌙 END OF DAY
  ☐ Log all interactions (notes on contacts)
  ☐ Set tomorrow's follow-up tasks
  ☐ Review email/SMS campaign metrics if any sent today
  ☐ Flag issues for manager in Slack/team channel
```

---

> 📖 **For the full detailed training on all features**, see the complete documentation set in the `GHL Training` folder.
