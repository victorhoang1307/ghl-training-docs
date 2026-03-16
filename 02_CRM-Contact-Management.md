# Module 2: CRM & Contact Management

🎯 **Objective:** Master contact management, segmentation with Tags & Smart Lists, and leverage 360° contact records for smarter selling.

---

## 2.1 CRM Overview

The CRM is the **central hub** of GHL — every email, SMS, call, form submission, page visit, and deal ties back to a contact record.

### Why GHL's CRM Stands Out
- ✅ **Unlimited contacts** on every plan
- ✅ **360° Contact Records** — full interaction history
- ✅ **Duplicate Detection** — auto-flags duplicates
- ✅ **Smart Lists** — dynamic, filter-based segmentation
- ✅ **Multi-channel tracking** — SMS, email, calls, chat, social

---

## 2.2 Managing Contacts

### 2.2.1 Adding New Contacts

| Method | How-to | Best for |
|--------|--------|----------|
| **Manual** | Contacts → "+ Add Contact" → fill details → Save | One-off entries |
| **CSV Import** | Contacts → Import → upload CSV → map columns | Migrating from another CRM |
| **Auto-capture** | Forms & funnels create contacts automatically | Ongoing lead gen |
| **Integrations** | Facebook Lead Ads, Google Ads, Zapier, etc. | Ad-driven campaigns |

> 💡 **Tip:** Always assign a **Tag** and **Source** when adding contacts — this pays off massively in reporting and automation later.

---

### 2.2.2 The 360° Contact Record

Every contact has a complete profile with these tabs:

| Tab | What it shows |
|-----|--------------|
| **Details** | Name, email, phone, company, custom fields |
| **Conversations** | Full SMS, email, and chat history |
| **Opportunities** | Linked deals and pipeline stages |
| **Appointments** | Booked meetings |
| **Tasks** | To-dos assigned to this contact |
| **Notes** | Internal team notes |
| **Activity** | Pages visited, emails opened, links clicked |
| **Payments** | Transaction and invoice history |

---

### 2.2.3 Custom Fields

Custom Fields let you store business-specific data that GHL doesn't include by default.

**To create:** Settings → Custom Fields → "+ Add Field"

| Field Type | Example Use |
|------------|------------|
| **Text** | Customer ID, Tax number |
| **Number** | Budget, Employee count |
| **Date** | Contract expiry, Birthday |
| **Dropdown** | Industry, Region |
| **Checkbox** | NDA signed, Opted-in |
| **Text Area** | Detailed notes |
| **File Upload** | Proposals, contracts |

> ⚠️ **Note:** Plan your Custom Fields carefully upfront. Changing them later may break existing workflows and reports.

---

## 2.3 Tags — Labeling & Segmentation

Tags are **labels** you attach to contacts for segmentation and to trigger automations.

### Recommended Naming Convention

Use a consistent `category_detail` pattern:

```
source_facebook-ads
source_google-ads
source_referral
source_website-form

interest_product-a
interest_product-b

status_new-lead
status_contacted
status_qualified
status_customer

campaign_spring-2026
campaign_blackfriday

segment_vip
segment_enterprise
segment_sme
```

### How Tags Get Applied
- **Manually** — Click into a contact → add tags
- **Via Workflows** — Auto-tag based on lead source or behavior
- **Via Forms** — Auto-tag when a specific form is submitted
- **Via Triggers** — Tag when an email is opened, a link is clicked, etc.

---

## 2.4 Smart Lists — Dynamic Segmentation

Smart Lists are **filter-based contact lists** that update automatically as contacts match (or stop matching) your criteria.

### Creating a Smart List
1. Go to **Contacts** → **Smart Lists** tab
2. Click **"+ Add Smart List"**
3. Name it and set **Filters**

### High-value Smart List Examples

| Smart List | Filter Logic | Purpose |
|------------|-------------|---------|
| **Hot Leads** | Tag = `status_qualified` AND Last Activity < 7 days | Priority follow-up |
| **Cold Leads** | Last Activity > 30 days AND Tag ≠ `status_customer` | Re-engagement campaign |
| **VIP Customers** | Tag = `segment_vip` AND Total Spent > $1,000 | White-glove service |
| **Birthdays This Month** | Birthday = current month | Birthday promo campaign |
| **Facebook Leads** | Source = "Facebook" AND Tag = `status_new-lead` | Evaluate FB Ads ROI |

> 💡 **Tip:** Smart Lists can feed directly into **Workflows** — e.g., auto-send a weekly nurture email to all "Cold Leads."

---

## 2.5 Lead Source Tracking

GHL captures the **origin** of every lead so you can measure channel ROI.

### Setup
1. Add **UTM parameters** to your ad and campaign links
2. GHL auto-captures UTMs when a lead arrives through a funnel or form
3. Review source data in **Reporting**

### UTM Example

```
https://yourfunnel.com/landing-page
  ?utm_source=facebook
  &utm_medium=cpc
  &utm_campaign=spring-2026
  &utm_content=video-ad-v1
```

---

## 2.6 Bulk Actions

Perform operations on many contacts at once:

- ✅ **Bulk Add/Remove Tags**
- ✅ **Bulk Email / SMS**
- ✅ **Bulk Add to Workflow**
- ✅ **Bulk Add to Pipeline**
- ✅ **Bulk Delete**
- ✅ **Export to CSV**

---

## 📝 Module 2 Exercises

1. **Create 5 Custom Fields** relevant to your business
2. **Design a Tag taxonomy** with at least 4 categories (source, interest, status, segment)
3. **Import 10 contacts** from a CSV and assign appropriate tags
4. **Build 3 Smart Lists:**
   - Hot leads (activity within last 7 days)
   - Leads by industry
   - Leads not yet contacted
5. **Compare** a blank contact record vs. a fully enriched one — notice the difference in usability

---

> ⏭️ **Next:** [Module 3 — Sales Pipelines & Opportunity Management](03_Sales-Pipelines.md)
