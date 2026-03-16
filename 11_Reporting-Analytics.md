# Module 11: Reporting & Analytics

🎯 **Objective:** Read, interpret, and act on GHL's reports to make data-driven decisions across sales and marketing.

---

## 11.1 Why Reporting Matters

> "You can't improve what you don't measure."

GHL centralizes all your sales and marketing data, giving you a single source of truth instead of logging into five different tools.

---

## 11.2 GHL Reporting Dashboard

Navigate to **Reporting** in the sidebar. The main dashboard provides an at-a-glance overview:

```
┌─────────────────────────────────────────────────────┐
│                  REPORTING DASHBOARD                 │
│                                                      │
│  ┌────────────┐  ┌────────────┐  ┌────────────────┐ │
│  │ Total Leads│  │  Pipeline  │  │    Revenue     │ │
│  │   This Mo. │  │   Value    │  │   This Month   │ │
│  │    142     │  │  $285,000  │  │   $42,500      │ │
│  └────────────┘  └────────────┘  └────────────────┘ │
│                                                      │
│  ┌────────────┐  ┌────────────┐  ┌────────────────┐ │
│  │Appointments│  │ Conversion │  │  Avg. Deal     │ │
│  │  Booked    │  │    Rate    │  │    Size        │ │
│  │    38      │  │   18.5%    │  │   $3,800       │ │
│  └────────────┘  └────────────┘  └────────────────┘ │
└─────────────────────────────────────────────────────┘
```

---

## 11.3 Report Categories

### 11.3.1 Pipeline & Opportunity Reports

| Report | What It Shows | Key Insight |
|--------|-------------|-------------|
| **Pipeline Overview** | Deals by stage, total value per stage | Where deals are stacking up |
| **Win/Loss Report** | Won vs. lost deals over time | Closing effectiveness |
| **Stage Conversion** | % of deals moving stage to stage | Where leads drop off |
| **Sales Cycle Report** | Average days from New to Won | How long deals take to close |
| **Revenue by Source** | Revenue broken down by lead source | Which channels drive the most revenue |
| **Rep Performance** | Deals, revenue, and activity per salesperson | Top performers & coaching needs |

### 11.3.2 Marketing Reports

| Report | What It Shows | Key Insight |
|--------|-------------|-------------|
| **Lead Source Report** | Where contacts came from (UTM tracking) | Which channels generate the most leads |
| **Email Campaign Stats** | Open rate, click rate, bounces, unsubscribes | Campaign engagement level |
| **SMS Campaign Stats** | Delivery rate, response rate, opt-outs | SMS effectiveness |
| **Funnel Stats** | Page views, opt-ins, conversion rate per step | Funnel performance |
| **Appointment Report** | Bookings, shows, no-shows | Scheduling effectiveness |

### 11.3.3 Communication Reports

| Report | What It Shows | Key Insight |
|--------|-------------|-------------|
| **Call Report** | Total calls, duration, answered vs. missed | Phone activity level |
| **Conversation Report** | Messages sent/received across channels | Communication volume |
| **Response Time** | Average time to first response | Speed-to-lead metric |

---

## 11.4 Key Metrics Every Role Should Track

### For Sales Managers

| Metric | Target | Action if off-target |
|--------|--------|---------------------|
| **Lead-to-Opportunity Rate** | > 30% | Improve qualification criteria |
| **Win Rate** | > 20% | Review proposals, improve pitch |
| **Average Deal Size** | Trending up | Focus on upsells and higher-value segments |
| **Sales Cycle Length** | Trending down | Streamline follow-up process |
| **Pipeline Coverage** | 3× revenue target | Generate more leads if under |
| **Response Time** | < 5 minutes | Set up auto-notifications & AI |

### For Marketing Managers

| Metric | Target | Action if off-target |
|--------|--------|---------------------|
| **Cost Per Lead (CPL)** | < industry avg | Optimize ad spend and targeting |
| **Email Open Rate** | > 25% | Test subject lines, clean list |
| **Email Click Rate** | > 3% | Improve CTAs and content |
| **Funnel Conversion Rate** | > 15% | A/B test headlines, forms, offers |
| **SMS Response Rate** | > 15% | Adjust messaging and timing |
| **Review Volume** | 5+ per month | Increase review request frequency |

### For Sales Reps

| Metric | Target | Action if off-target |
|--------|--------|---------------------|
| **Deals in Pipeline** | > 20 active | Prospect more aggressively |
| **Activities Per Day** | > 15 (calls + emails) | Increase outreach volume |
| **Appointments Set** | > 5 per week | Improve qualification scripts |
| **Follow-up Compliance** | 100% | Use task reminders |
| **Stage Aging** | < 7 days per stage | Speed up next actions |

---

## 11.5 Building Custom Dashboards

GHL allows you to create **custom dashboard widgets** for personalized views:

### Steps
1. Go to **Dashboard**
2. Click **"+ Add Widget"**
3. Choose widget type:
   - Opportunity stats
   - Manual actions
   - Pipeline value
   - Funnel performance
   - Calendar overview
4. Configure filters (date range, pipeline, team member)
5. Arrange widgets by dragging

### Recommended Dashboards

**Sales Manager Dashboard:**
```
┌─────────────────────┬─────────────────────┐
│ Pipeline Overview   │ Rep Leaderboard     │
│ (by stage + value)  │ (deals won, revenue)│
├─────────────────────┼─────────────────────┤
│ Appointments Today  │ Win Rate Trend      │
│ (upcoming meetings) │ (30-day chart)      │
├─────────────────────┼─────────────────────┤
│ Stale Deals Alert   │ Revenue This Month  │
│ (deals > 7 days     │ vs. Target          │
│  with no activity)  │                     │
└─────────────────────┴─────────────────────┘
```

**Marketing Dashboard:**
```
┌─────────────────────┬─────────────────────┐
│ Leads This Week     │ Lead Source          │
│ (total + trend)     │ Breakdown (pie)      │
├─────────────────────┼─────────────────────┤
│ Email Campaign      │ Funnel Performance   │
│ Performance         │ (conversion rates)   │
├─────────────────────┼─────────────────────┤
│ Review Score        │ SMS Response Rate    │
│ (avg rating + #)    │ (last 30 days)       │
└─────────────────────┴─────────────────────┘
```

---

## 11.6 Attribution & ROI Tracking

### How to Track Marketing ROI

1. **Tag every campaign** with UTM parameters
2. **Track lead source** at the contact level
3. **Follow leads through the pipeline** to closed deals
4. **Calculate ROI per channel:**

```
Channel ROI = (Revenue from Channel - Cost of Channel) / Cost of Channel × 100

Example:
  Facebook Ads spend:     $2,000
  Leads generated:        40
  Deals closed:           6
  Revenue from deals:     $18,000
  
  ROI = ($18,000 - $2,000) / $2,000 × 100 = 800% ✅
```

### Attribution Models in GHL
- **First Touch** — credit goes to the first interaction (where the lead came from)
- **Last Touch** — credit goes to the last interaction before conversion
- **Linear** — credit is split equally across all touchpoints

---

## 11.7 Reporting Best Practices

1. **Review reports weekly** — set a recurring calendar reminder
2. **Compare periods** — this month vs. last month, or vs. same month last year
3. **Share with the team** — transparency drives performance
4. **Act on insights** — a report is useless if nobody changes behavior
5. **Clean your data** — bad data = bad reports. Keep contacts, tags, and pipelines tidy

---


> ⏭️ **Next:** [Module 13 — Social Media Management](13_Social-Media-Management.md)

