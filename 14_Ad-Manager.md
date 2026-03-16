# Module 14: Ad Manager — Facebook & Google Ads

🎯 **Objective:** Run, manage, and measure Facebook (Meta) and Google Ads directly from GHL, with leads syncing instantly into your CRM and pipelines.

---

## 14.1 Why Manage Ads Inside GHL?

| Traditional Approach | GHL Ad Manager |
|---------------------|---------------|
| Create ads in Facebook/Google dashboards | Create and manage from one dashboard |
| Export leads manually or via Zapier | Leads sync instantly into CRM |
| Track ROI across 3+ tools | End-to-end attribution in one place |
| No post-click automation | Auto-trigger SMS, email, pipeline on form submit |
| Separate billing for ad management tools | Included in GHL |

> 💡 **Key Advantage:** GHL closes the loop between **ad spend → lead capture → CRM → pipeline → revenue**. You can finally see exactly which ad generated which deal.

---

## 14.2 Connecting Ad Accounts

### Facebook (Meta) Ads
1. Go to **Settings** → **Integrations** → **Facebook**
2. Log in with your Facebook account
3. Select the **Ad Account(s)** and **Page(s)** to connect
4. Grant necessary permissions (manage ads, access lead forms)

### Google Ads
1. Go to **Settings** → **Integrations** → **Google**
2. Click **"Connect Google Ads"**
3. Log in with your Google account
4. Select the **Ad Account(s)** to connect

> ⚠️ **Note:** You need admin or advertiser access to the ad accounts you want to connect.

---

## 14.3 Facebook Ads in GHL

### 14.3.1 Creating Facebook Ads

1. Go to **Marketing** → **Ad Manager**
2. Click **"+ Create Ad"** → select **Facebook/Instagram**
3. Configure:

| Setting | Description |
|---------|------------|
| **Campaign Objective** | Lead Generation, Traffic, Conversions, Awareness |
| **Audience** | Demographics, interests, behaviors, custom audiences |
| **Placement** | Facebook Feed, Instagram Feed, Stories, Reels, Messenger |
| **Budget** | Daily or lifetime budget |
| **Schedule** | Start/end dates |
| **Ad Creative** | Image/video, headline, description, CTA button |
| **Lead Form** | Use Facebook Lead Form or redirect to GHL funnel |

### 14.3.2 Facebook Lead Form Integration

When a prospect fills out a **Facebook Lead Form**:
1. Lead data syncs **instantly** to GHL CRM
2. Contact is created with tags and source tracking
3. **Workflow triggers automatically:**

```
Trigger: Facebook Lead Form Submitted
    │
    ▼
[Within seconds]
    ✅ Create Contact in CRM (Name, Email, Phone)
    ✅ Tag: "source_facebook-ads" + "campaign_[name]"
    ✅ Create Opportunity in Pipeline → "New Lead"
    ✅ SMS to lead: "Thanks for your interest! A team member will call you shortly"
    ✅ Notify Sales Rep: "🔥 New Facebook Lead: [Name] — [Phone]"
    │
    ▼
[5 minutes later]
    📞 Auto-dial: Connect sales rep to lead
```

> 💡 **Speed-to-Lead:** Responding within 5 minutes increases conversion by **400%**. GHL's instant sync + auto-notification makes this possible.

### 14.3.3 Custom Audiences from GHL

Leverage your CRM data for smarter ad targeting:

| Audience Type | Source | Use Case |
|--------------|--------|----------|
| **Retargeting** | Website/funnel visitors | Re-engage people who didn't convert |
| **Lookalike** | Your best customers (Smart List) | Find similar prospects |
| **Email Match** | CRM contact list upload | Target existing contacts on Facebook |
| **Engagement** | People who interacted with your content | Warm audience campaigns |
| **Exclusion** | Current customers | Avoid wasting spend on existing clients |

---

## 14.4 Google Ads in GHL

### 14.4.1 Creating Google Ads

1. Go to **Marketing** → **Ad Manager**
2. Click **"+ Create Ad"** → select **Google**
3. Configure:

| Setting | Description |
|---------|------------|
| **Campaign Type** | Search, Display, Performance Max, YouTube |
| **Keywords** | Target keywords + negative keywords |
| **Ad Copy** | Headlines (up to 15), descriptions (up to 4) |
| **Landing Page** | GHL funnel page or external URL |
| **Budget** | Daily budget |
| **Bidding** | Manual CPC, Maximize Conversions, Target CPA |
| **Extensions** | Sitelinks, callout, call, location |

### 14.4.2 Google Ads Conversion Tracking

GHL syncs conversion data with your Google Ads account:

1. **Install GHL tracking pixel** on your funnels and website
2. GHL reports back to Google which clicks became:
   - Form submissions
   - Appointment bookings
   - Pipeline stage changes
   - Payments
3. Google optimizes targeting based on **actual conversions**, not just clicks

```
Google Ad Click
    │
    ▼
GHL Funnel / Landing Page
    │
    ▼
Form Submission → CRM Contact Created
    │
    ▼
Appointment Booked → Conversion sent back to Google
    │
    ▼
Deal Won → Revenue attributed to specific keyword/ad
```

### 14.4.3 Keyword-to-Revenue Tracking

With GHL, you can trace the full path:

```
Keyword: "marketing agency near me"
    → Ad: "Top-Rated Marketing Agency"
        → Click → Landing Page
            → Form Submit → Contact: John Smith
                → Pipeline: Discovery Call
                    → Proposal Sent
                        → Won: $5,000/month
```

This lets you calculate **ROI per keyword** — something most businesses can't do.

---

## 14.5 Ad Reporting & Analytics

### Facebook Ads Reports

| Metric | Where to Find | What It Tells You |
|--------|--------------|------------------|
| **Impressions** | Ad Manager | How many times your ad was shown |
| **Reach** | Ad Manager | Unique people who saw your ad |
| **CPC (Cost Per Click)** | Ad Manager | How much each click costs |
| **CTR (Click-Through Rate)** | Ad Manager | % of viewers who clicked |
| **CPL (Cost Per Lead)** | Ad Manager + Pipeline | How much each lead costs |
| **CPA (Cost Per Acquisition)** | Pipeline + Payments | How much each customer costs |
| **ROAS (Return on Ad Spend)** | Pipeline + Revenue | Revenue generated per $1 spent |

### Google Ads Reports

| Metric | Description |
|--------|------------|
| **Clicks & Impressions** | Traffic volume |
| **CPC & CTR** | Click efficiency |
| **Quality Score** | Google's rating of ad relevance (1–10) |
| **Conversion Rate** | % of clicks that convert |
| **Cost Per Conversion** | Ad spend ÷ conversions |
| **Search Impression Share** | % of eligible impressions captured |

### Cross-Channel ROI Dashboard

```
┌─────────────────────────────────────────────────────┐
│                   AD PERFORMANCE                     │
│                                                      │
│  Facebook Ads          Google Ads                    │
│  ┌────────────────┐    ┌────────────────┐           │
│  │ Spend: $2,000  │    │ Spend: $1,500  │           │
│  │ Leads: 45      │    │ Leads: 30      │           │
│  │ CPL: $44       │    │ CPL: $50       │           │
│  │ Deals Won: 8   │    │ Deals Won: 5   │           │
│  │ Revenue: $24K  │    │ Revenue: $15K  │           │
│  │ ROAS: 12x      │    │ ROAS: 10x      │           │
│  └────────────────┘    └────────────────┘           │
│                                                      │
│  Total Spend: $3,500   Total Revenue: $39,000       │
│  Overall ROAS: 11.1x ✅                              │
└─────────────────────────────────────────────────────┘
```

---

## 14.6 Ad + Workflow Automation Patterns

### Pattern 1: Instant Lead Response (Facebook)

```
Facebook Lead Form Submitted
    │
    ▼
[0 sec]  CRM: Create contact + tag
[0 sec]  SMS to lead: "Thanks! We'll call you in 5 min"
[0 sec]  Notify sales rep (SMS + internal notification)
[5 min]  If no call made → Create Task: "URGENT: Call [Name]"
[1 hr]   Email: Welcome + company intro
[1 day]  If no appointment → SMS: "Ready to schedule a call?"
```

### Pattern 2: Google Ads Landing Page Retargeting

```
Visitor lands on pricing page (from Google Ad) but doesn't convert
    │
    ▼
[1 hr]   Email: "Still comparing options? Here's why clients choose us"
[1 day]  SMS: "Any questions about pricing? Reply and we'll help"
[3 days] Add to Facebook Custom Audience → Retargeting ad
[7 days] Email: "Limited time: 15% off for first-time clients"
```

---

## 14.7 Client Reporting for Agencies

If you manage ads for clients:

1. Go to **Reporting** → **Ad Reports**
2. Select client sub-account
3. Choose date range and metrics
4. **Export as PDF** — branded with your agency logo
5. **Schedule auto-reports** — send weekly/monthly via email

---

## 📝 Module 14 Exercises

1. **Connect** your Facebook and/or Google Ads accounts to GHL
2. **Create a Facebook Lead Ad** with a lead form that syncs to GHL CRM
3. **Build a speed-to-lead workflow** that triggers within seconds of a lead form submission
4. **Set up conversion tracking** on a GHL funnel for Google Ads
5. **Generate an ad performance report** and calculate ROAS for one campaign
6. **Create a Custom Audience** from your GHL CRM data for retargeting

---

> ⏭️ **Next:** [Module 15 — Memberships, Courses & Communities](15_Memberships-Courses.md)
