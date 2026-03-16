# Module 15: Memberships, Courses & Communities

🎯 **Objective:** Build and sell online courses, create membership sites, and foster branded communities — all within GHL, replacing tools like Kajabi, Teachable, or Skool.

---

## 15.1 Overview — Three Powerful Features

| Feature | What It Does | Replaces |
|---------|-------------|---------|
| **Courses** | Create and sell online courses with video lessons, quizzes, and certificates | Kajabi, Teachable, Thinkific |
| **Memberships** | Gate content behind paid or free membership tiers | MemberPress, Patreon |
| **Communities** | Build private, branded discussion forums and groups | Skool, Circle, Facebook Groups |

> 💡 **Key Advantage:** Everything is natively integrated with GHL's CRM, workflows, payments, and email — so you can automate enrollment, drip content, and follow up without third-party tools.

---

## 15.2 Courses — Building Your Online Course

### 15.2.1 Course Builder Overview

GHL's Course Builder is a **full LMS (Learning Management System)** with:
- ✅ Unlimited video hosting
- ✅ Unlimited students
- ✅ Drag-and-drop content builder
- ✅ Quizzes with scoring
- ✅ Auto-generated completion certificates
- ✅ Progress tracking
- ✅ Drip scheduling (release lessons over time)
- ✅ White-label branding

### 15.2.2 Creating a Course

1. Go to **Memberships** → **Courses** → **"+ New Course"**
2. Set up course details:
   - **Title** — e.g., "Facebook Ads Mastery"
   - **Description** — what students will learn
   - **Thumbnail** — course cover image
   - **Instructor** — name and photo
   - **Category** — for organizing multiple courses

3. **Add Modules (Sections)**
   - Each module is a chapter of your course
   - Example structure:

```
📚 Facebook Ads Mastery
│
├── Module 1: Getting Started
│   ├── Lesson 1.1: Setting Up Your Ad Account (Video)
│   ├── Lesson 1.2: Understanding the Ads Manager (Video)
│   └── Quiz 1: Account Setup Basics
│
├── Module 2: Audience Targeting
│   ├── Lesson 2.1: Custom Audiences (Video)
│   ├── Lesson 2.2: Lookalike Audiences (Video)
│   ├── Lesson 2.3: Interest-Based Targeting (Video + PDF)
│   └── Quiz 2: Targeting Strategies
│
├── Module 3: Ad Creative
│   ├── Lesson 3.1: Writing Ad Copy (Video)
│   ├── Lesson 3.2: Designing Visuals (Video)
│   └── Assignment: Create Your First Ad
│
├── Module 4: Optimization & Scaling
│   ├── Lesson 4.1: Reading Ad Reports (Video)
│   ├── Lesson 4.2: Scaling Winners (Video)
│   └── Final Quiz
│
└── 🎓 Certificate of Completion
```

4. **Add Lesson Content**
   - Upload **videos** (unlimited hosting, no external platform needed)
   - Add **text content** with the rich text editor
   - Attach **downloadable files** (PDFs, templates, checklists)
   - Embed **images** and **external links**

### 15.2.3 Quizzes & Assessments

| Feature | Description |
|---------|------------|
| **Multiple Choice** | Single or multiple correct answers |
| **True/False** | Simple binary questions |
| **Pass/Fail Scoring** | Set minimum score to unlock next module |
| **Retake Policy** | Allow unlimited or limited retakes |
| **Auto-grading** | Instant results for students |

### 15.2.4 Certificates

Auto-generate **completion certificates** when a student finishes the course:
- Customizable design (your logo, colors, layout)
- Student name auto-populated
- Date of completion
- Unique certificate ID
- Can be downloaded as PDF

### 15.2.5 Drip Content

Release lessons over time instead of all at once:

| Drip Method | Example |
|-------------|---------|
| **By Days After Enrollment** | Module 1 on Day 1, Module 2 on Day 7, Module 3 on Day 14 |
| **By Specific Date** | Module 2 unlocks on March 15 for everyone |
| **By Completion** | Module 2 unlocks only after Module 1 quiz is passed |

---

## 15.3 Memberships — Gated Content

### 15.3.1 Membership Tiers

Create multiple access levels:

| Tier | Access | Price |
|------|--------|:-----:|
| **Free** | Intro course, community access | $0 |
| **Basic** | All courses, community, monthly Q&A | $29/mo |
| **Premium** | Everything + 1-on-1 coaching, exclusive events | $99/mo |
| **VIP** | Lifetime access + priority support | $499 one-time |

### 15.3.2 Setting Up a Membership

1. Go to **Memberships** → **Offers** → **"+ New Offer"**
2. Configure:
   - **Name** — e.g., "Premium Membership"
   - **Pricing** — Free, one-time, or recurring (monthly/annual)
   - **Payment** — Connect Stripe or PayPal
   - **Access** — Select which courses/products are included
   - **Trial Period** — Optional free trial (e.g., 7 or 14 days)

### 15.3.3 Payment Integration

| Integration | Supports |
|-------------|---------|
| **Stripe** | Credit/debit cards, recurring billing, 135+ currencies |
| **PayPal** | PayPal balance, cards, bank transfers |

### 15.3.4 Access Control & Automation

Use **workflows** to manage membership access:

```
Trigger: Payment Received (Stripe) for "Premium Membership"
    │
    ▼
✅ Grant access to: Course A, Course B, Community
✅ Tag: "membership_premium"
✅ Email: Welcome + login credentials
✅ Create Opportunity in "Membership" pipeline
    │
    ▼
[If payment fails / subscription canceled]
    ❌ Revoke course access
    📧 Email: "Your access has been paused — update payment info"
    ✅ Tag: "membership_churned"
    ✅ Start re-engagement workflow
```

---

## 15.4 Communities — Building Your Branded Community

### 15.4.1 What Are GHL Communities?

GHL Communities are **private, branded online forums** where members can:
- Post and discuss topics
- Share files and resources
- Direct message each other
- Attend events
- Compete on leaderboards
- Access courses

Think of it as **Skool or Facebook Groups, but inside your platform**.

### 15.4.2 Setting Up a Community

1. Go to **Memberships** → **Communities** → **"+ New Community"**
2. Configure:
   - **Name** — e.g., "Marketing Pros Inner Circle"
   - **Description** — what the community is about
   - **Branding** — logo, colors, banner image
   - **Access** — Public, Free (requires signup), or Paid
   - **Channels** — create topic-based discussion channels

### 15.4.3 Community Features

| Feature | Description |
|---------|------------|
| **Discussion Posts** | Members create posts, others comment and react |
| **Channels** | Organized by topic (e.g., #introductions, #wins, #questions, #resources) |
| **Direct Messages** | Private 1-on-1 messaging between members |
| **Events** | Schedule live events, webinars, and Q&A sessions |
| **Leaderboards** | Gamification — rank members by engagement, course completion |
| **File Sharing** | Upload and share resources, templates, tools |
| **Announcements** | Pin important posts to the top |
| **Member Directory** | Browse and search community members |

### 15.4.4 Community Monetization

| Model | How It Works |
|-------|-------------|
| **Paid Community** | Monthly/annual fee to access the community |
| **Freemium** | Free tier + premium channels for paying members |
| **Course + Community Bundle** | Sell courses that include community access |
| **Coaching Add-on** | Free community + paid coaching tiers |

### 15.4.5 Community + Workflow Integration

```
Trigger: New Community Member Joins
    │
    ▼
✅ Email: Welcome + community guidelines + "Introduce yourself" prompt
✅ Tag: "community_member"
✅ DM in Community: "Welcome, {{first_name}}! 👋 Start by posting in #introductions"
    │
    ▼
[Day 3 — If no post yet]
    📧 Email: "We'd love to hear from you — here's how to get started"
    │
    ▼
[Day 7]
    📧 Email: Feature highlight — "Have you checked out these resources?"
```

---

## 15.5 Student & Member Management

### Managing Enrolled Users

| Action | How |
|--------|-----|
| **View enrolled students** | Memberships → Course → Students tab |
| **Track progress** | See completed lessons, quiz scores, % completion |
| **Grant/Revoke access** | Manually or via workflow triggers |
| **Send broadcasts** | Email/SMS all enrolled students at once |
| **Export data** | Download student list as CSV |

### Engagement Tracking

| Metric | What It Tells You |
|--------|------------------|
| **Enrollment Count** | Total active students/members |
| **Completion Rate** | % of students who finish the course |
| **Module Drop-off** | Where students stop engaging |
| **Quiz Pass Rate** | Lesson effectiveness |
| **Community Activity** | Posts, comments, logins per day/week |
| **Revenue per Member** | Average lifetime value |

---

## 15.6 Use Cases

### For Coaches & Consultants
- Sell online courses as a scalable revenue stream
- Create a paid community for ongoing coaching
- Use certificates to add credibility

### For Agencies
- Train clients on how to use their tools (GHL, social media, ads)
- Create onboarding courses for new clients
- Build a community where clients share wins and ask questions

### For SaaS & Product Companies
- Product training academy
- Customer onboarding courses
- Feature-update webinars with a community for feedback

---

## 📝 Module 15 Exercises

1. **Create a mini-course** with 3 modules and at least 1 quiz
2. **Set up a membership offer** with a monthly pricing plan connected to Stripe
3. **Configure a drip schedule** — release Module 2 one week after enrollment
4. **Create a community** with 3 channels (#introductions, #questions, #wins)
5. **Build a workflow** that grants course access when payment is received and revokes access when subscription is canceled
6. **Design a certificate** with your branding for course completion

---

> 📖 **Return to:** [Table of Contents](00_Table-of-Contents.md)
