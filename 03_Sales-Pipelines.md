# Module 3: Sales Pipelines & Opportunity Management

🎯 **Objective:** Build and operate effective Sales Pipelines, manage deals through stages, and forecast revenue accurately.

---

## 3.1 What is a Sales Pipeline?

A Sales Pipeline is a **visual board** that maps your sales process. Each column represents a stage; each card represents a deal (called an "Opportunity" in GHL).

```
  New Lead    Contacted    Qualified    Proposal    Negotiation    Won ✅
 ┌────────┐  ┌────────┐  ┌────────┐  ┌────────┐  ┌───────────┐  ┌──────┐
 │ Deal A │  │ Deal D │  │ Deal F │  │ Deal H │  │  Deal J   │  │Deal L│
 │ Deal B │  │ Deal E │  │ Deal G │  │        │  │           │  │      │
 │ Deal C │  │        │  │        │  │        │  │           │  │      │
 └────────┘  └────────┘  └────────┘  └────────┘  └───────────┘  └──────┘
                                                                    │
                                                              ┌─────┴─────┐
                                                              │  Lost ❌   │
                                                              └───────────┘
```

### Why Pipelines Matter
| Benefit | Description |
|---------|------------|
| 📊 **Visibility** | See every active deal at a glance |
| 🎯 **Prioritization** | Know which deals need attention right now |
| 📈 **Revenue Forecasting** | Sum deal values at each stage |
| 🔍 **Bottleneck Detection** | Spot stages where deals stall |
| 📉 **Conversion Metrics** | Measure stage-to-stage conversion rates |

---

## 3.2 Building a Pipeline

### Step 1: Navigate
Go to **Opportunities** → click **"+ Add Pipeline"** → name it.

### Step 2: Define Stages

**Example — Marketing Agency Pipeline:**

| # | Stage | Description | Win Probability |
|---|-------|-------------|:--------------:|
| 1 | New Lead | Just entered the system | 10% |
| 2 | Contacted | Initial outreach completed | 20% |
| 3 | Discovery Call | Needs-analysis call booked or done | 30% |
| 4 | Proposal Sent | Pricing/proposal delivered | 50% |
| 5 | Negotiation | Terms under discussion | 70% |
| 6 | Won ✅ | Deal closed successfully | 100% |
| 7 | Lost ❌ | Deal did not close | 0% |

**Example — Real Estate Pipeline:**

| # | Stage | Description |
|---|-------|------------|
| 1 | Inquiry | Prospect asked for info |
| 2 | Site Visit Scheduled | Viewing booked |
| 3 | Site Visited | Viewing completed |
| 4 | Interested | Actively considering |
| 5 | Deposit | Deposit received |
| 6 | Closed | Transaction finalized |

> 💡 **Tip:** Keep it simple — 5 to 7 stages max. Too many stages means salespeople will skip updates.

---

## 3.3 Managing Opportunities

### 3.3.1 Creating an Opportunity

**Manual:**
1. Open the pipeline → **"+ Add Opportunity"**
2. Fill in:
   - **Contact** — link to a CRM record
   - **Stage** — current pipeline stage
   - **Value ($)** — deal size
   - **Name** — descriptive deal name
   - **Assigned To** — responsible salesperson
   - **Expected Close Date**

**Automatic (via Workflow):**
- Lead submits a form → Opportunity auto-created at "New Lead"
- Lead books an appointment → Opportunity moved to "Discovery Call"

### 3.3.2 Moving Opportunities Between Stages

| Method | How |
|--------|-----|
| **Drag & Drop** | Drag the card from one column to another |
| **Edit Detail** | Open the opportunity → change Stage dropdown |
| **Workflow** | Auto-move when a trigger fires (e.g., email replied → "Contacted") |

### 3.3.3 Opportunity Card Details

Each card shows:
- 👤 Contact name & company
- 💰 Deal value
- 📅 Created date & expected close date
- 👨‍💼 Assigned salesperson
- 📝 Notes, tasks, and appointments
- 📞 Interaction history

---

## 3.4 Pipeline Views

| View | Description | Best for |
|------|------------|----------|
| **Board (Kanban)** | Visual columns, drag-and-drop | Daily management |
| **List** | Sortable/filterable list | Exporting reports |
| **Table** | Spreadsheet-style detail | Data analysis |

---

## 3.5 Pipeline Best Practices

### Golden Rules for the Sales Team

1. **Update the pipeline DAILY** — review every deal each morning
2. **Log every interaction** — add a Note after every call or email
3. **Always set a next action** — never leave a deal without a follow-up task
4. **Enter accurate deal values** — this drives your revenue forecast
5. **Keep the pipeline clean** — mark stale deals "Lost" promptly

### Using Multiple Pipelines

Create separate pipelines for different processes:

```
Pipeline 1: "New Business"       → New customer acquisition
Pipeline 2: "Upsell / Cross-sell" → Existing customer expansion
Pipeline 3: "Partnerships"       → Strategic partnerships
Pipeline 4: "Renewals"           → Contract renewals
```

---

## 3.6 Connecting Pipelines to Workflows

### Example 1: Auto-assign new leads

```
Trigger:  Contact created (Source = Facebook Ads)
    │
    ▼
Action 1: Create Opportunity in "New Business" → Stage "New Lead"
    │
    ▼
Action 2: Assign to salesperson (Round Robin)
    │
    ▼
Action 3: SMS to salesperson: "New lead: [Name] — [Phone]"
    │
    ▼
Action 4: Send welcome email to the lead
```

### Example 2: Stale-deal follow-up

```
Trigger:  Opportunity in "Proposal Sent" for > 3 days
    │
    ▼
Action 1: Email to lead: "Just checking in — any questions on the proposal?"
    │
    ▼
Action 2: Create Task for salesperson: "Follow up on [Deal Name]"
    │
    ▼
Action 3: If > 7 days still stale → send SMS reminder
```

---

## 3.7 Pipeline Reporting Metrics

| Metric | What It Tells You | Formula |
|--------|-------------------|---------|
| **Total Pipeline Value** | Sum of all active deals | Σ deal values |
| **Weighted Pipeline** | Probability-adjusted value | Σ (value × win %) |
| **Win Rate** | Closing effectiveness | Won ÷ (Won + Lost) |
| **Average Deal Size** | Typical deal value | Total Revenue ÷ Deals Won |
| **Sales Cycle Length** | Average time to close | Mean days from New → Won |
| **Stage Conversion** | Drop-off between stages | Deals exiting stage ÷ Deals entering |

---

## 📝 Module 3 Exercises

1. **Create a Pipeline** that matches your sales process (5–7 stages)
2. **Add 5 Opportunities** with realistic values and close dates
3. **Drag at least 2 deals** between stages
4. **Design a Workflow** that auto-creates an opportunity when a lead arrives
5. **Calculate** your Total Pipeline Value and Weighted Pipeline Value

### Practice Scenario
> You receive 10 new leads from Facebook Ads for a web design service.
> - Create contact records for all 10
> - Add them to your "New Business" pipeline
> - Move 3 to "Contacted," 2 to "Discovery Call," leave 5 at "New Lead"
> - Calculate total and weighted pipeline value

---

> ⏭️ **Next:** [Module 4 — Marketing Automation & Workflows](04_Marketing-Automation.md)
