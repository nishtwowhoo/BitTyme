# 🥁 BitTyme by The Bit-tles
**Problem Statement:** Beating the Burnout (Stress & Workload Manager)  
**Video Presentation:** [Insert Unlisted YouTube Link Here]  
**Presentation Slides:** [Insert Public Google Slides or Canva Link Here]  

---

## 📋 Team Members ("The Bit-tles")
* **Danish Firdaus** - Product Lead
* **Muhaimin** - UI/UX Designer
* **Haqemy** - Tech Lead & Architect
* **Ben Mudassir** - Pitch Lead & Storyteller

---

## 1. Project Overview

### 🎯 The Problem

#### Problem Context & Root Causes
For university students, academic burnout is rarely triggered by a single massive event, such as a final exam. Instead, it is the cumulative result of a silent, multi-dimensional pile up of daily stressors [3]. Students constantly juggle lectures, part-time employment, group projects, student club commitments, and basic household errands [3]. Because cognitive and physical stress accumulation is invisible, students struggle to gauge their active limits. They continuously accept new responsibilities, sacrifice sleep, and run on empty until sudden exhaustion hits [3].

#### The Target Stakeholders
Our primary users are highly active university students who balance complex, non-academic responsibilities alongside their degree programs [3]. This includes working student-professionals, student organization leaders, and final-year students managing intensive research projects.

#### Why Existing Market Solutions Fail
Industry standard tools like **Google Calendar, Notion, and Todoist** are fundamentally time-centric or task-centric. They treat a calendar hour of passive laundry exactly the same as a calendar hour of a high stakes examination. These applications operate under the assumption of infinite human capacity, encouraging users to pack schedules with back-to-back blocks. They fail to account for real cognitive and emotional bandwidth limits, allowing users to overbook themselves continuously until burnout occurs.

---

### 🥁 Our Solution: BitTyme

**BitTyme** is a holistic personal workload manager and active capacity shield designed to prevent student burnout [4]. Inspired by musical tempos and computer bits, BitTyme transitions student productivity from managing static time blocks to actively preserving human energy. 

The application maps out a student's live energy levels across five distinct resource buckets [3, 4]:
1. **Mental**: Cognitive exhaustion from study or exam preparation.
2. **Physical**: Physical fatigue from workouts, chores, or shifts.
3. **Social**: The battery required for networking, team meetings, and events.
4. **Errands**: General daily logistics and life administration.
5. **Time**: Actual hourly availability.

By tracking active capacity rather than just calendar hours, BitTyme helps students adjust their daily tempo and establish a sustainable lifestyle rhythm.

---

### ✨ Key Features

#### 1. The Tempo Dashboard
Instead of presenting a traditional static calendar, this interface visualizes student bandwidth across the five core resource buckets. Designed as a set of fluid, audio-player style gauges, the dashboard provides a clear sanity check of personal capacity. When any resource gauge enters critical thresholds, the interface changes states to warn the user before severe burnout occurs [4].

#### 2. The Tempo Balancer
When any energy gauge passes eighty five percent capacity, the rebalancing engine intervenes [4]. The system scans the database to isolate low-priority items, such as optional social engagements or non-urgent chores [4]. It then generates a single-tap option to defer those specific tasks to lighter weeks, lowering active stress and protecting user bandwidth [4].

#### 3. Beat Breaks
To safeguard mental health, the system automates mandatory recovery blocks when the user enters high burnout risk zones [4]. During these protected downtime windows, the application prevents the user from scheduling new academic or vocational tasks. The system then guides the student toward tailored recovery suggestions, such as matching a low physical fatigue score with a recommendation for an outdoor walk [4].

## 2. Ideation & Process

### 2.1 Ideas We Considered
We evaluated multiple concepts before aligning on our final direction [4]. To prove our iteration process, we documented why we selected or dropped each path [5]:

| Idea | Status | Why It Was Kept or Dropped |
| :--- | :--- | :--- |
| **A: BitTyme (5-Bucket Load Manager)** | **CHOSEN** | Focuses on active workload capacity across Mental, Physical, Social, Time, and Errands, forcing rest via recovery nudges [3]. Addresses the core issue of silent energy depletion [1]. |
| **B: Gamified Student Quest & XP System** | *Dropped* | We realized that awarding XP and levels for task completion creates an unhealthy incentive structure. It encourages students to work *more* when they should be resting, actively worsening burnout. |
| **C: AI Email & Notification Auto-Responder** | *Dropped* | While it reduces a minor daily chore, it is highly reactive and fails to address the root causes of student over-commitment and stress [1]. |

### 2.2 Ideation Boards
*Note for the Team: Have Member 2 design your mindmap and user flows in Figma, export them as PNGs, add them to your repo's `/images` folder, and link them below!*

![Mindmap & Problem Tree](images/ideation-board.png)  
*Figure 1: Our team's mindmap linking core student burnout triggers (over-commitment, peer pressure, unstructured rest) to BitTyme's feature solutions [6].*

### 2.3 Mentor Consultation
*Note for the Team: During the mentorship sprint (Sep 7–13), consult a mentor, log their feedback, and complete this table to secure easy rubric points [5].*

| Date | Mentor Name | Feedback Received | What Was Changed / Action Taken |
| :--- | :--- | :--- | :--- |
| [Date] | [Mentor Name] | "E.g., The recovery nudge should not feel like another chore or pop-up notification the student just swipes away." | "We added a 'Forced Recovery Lock' in Figma that physically prevents task scheduling during protected downtime blocks." |

---

## 3. Design & Prototype
👉 **[Click Here to View Our High-Fidelity Interactive Figma Prototype]**  
*(Make sure this link is public and testable in an incognito window!)*

### 📱 Key Screen Walkthroughs
*Note for the Team: Export your key Figma screens as PNG images, place them in `/images`, and write descriptive captions below [7].*

#### 1. The Tempo Dashboard (Main Screen)
![Dashboard Screen](images/screen-dashboard.png)  
*Caption: The main view visualizes overall energy. When Mental or Time capacities exceed 85%, warning metrics appear, signaling instant burnout warnings [3].*

#### 2. The Tempo Balancer
![Load Balancer Screen](images/screen-balancer.png)  
*Caption: When the system detects high stress, the Tempo Balancer banner pops up, offering one-tap recommendations to reschedule non-urgent errands and tasks [3].*

#### 3. Active "Beat Breaks" & Protected Downtime
![Recovery Screen](images/screen-recovery.png)  
*Caption: A Beat Break Nudge blocks out calendar segments for mental rest [3]. The user is locked out from adding new tasks during these protected periods to protect wellness.*

---

## 4. What Makes It Different

| Feature | Google Calendar / Notion | Standard To-Do Apps | **BitTyme (Our App)** |
| :--- | :--- | :--- | :--- |
| **Metric Tracked** | ❌ Time slots only | ❌ Quantity of tasks | **✅ 5-Bucket Human Bandwidth** [3] |
| **Action on Overload** | ❌ Passive overbooking | ❌ Infinite, stressful lists | **✅ Active Deferral & Auto-Balancing** [3] |
| **Downtime Focus** | ❌ None (constant work) | ❌ Keeps pushing tasks | **✅ Smart Recovery Blocks & Locks** [3] |

---

## 5. Technical Architecture & Build Plan

### 💻 Chosen Tech Stack
* **Frontend**: **React Native (Expo)** — Allows rapid development of a cross-platform mobile application (iOS & Android) with clean native styling and fast emulators [8].
* **Backend & Database**: **Supabase** — Provides PostgreSQL databases, built-in Authentication, and real-time database listeners for immediate task updates [9].
* **Hosting/Deployment**: **Expo Go** (for instant mobile previewing) & 
[React Native / Expo App Frontend] │  ▲ (Real-time updates) ▼  │ [Supabase Auth & Database (PostgreSQL)] │ ▼ [Capacity Scoring Algorithm (Local Client Logic)]

### 📅 Building Phase Roadmap (3-Week Sprint)
To ensure we deliver a working, deployable build by the end of the hackathon, we have mapped out a realistic development plan [9]:

* **Week 1 (Sep 21 – Sep 27) — Base Core & Auth**:
  * Set up Supabase PostgreSQL tables (Tasks, Capacity Logs, Users).
  * Build user authentication and the basic mobile home screen dashboard.
* **Week 2 (Sep 28 – Oct 4) — Capacity Logic & Balancer**:
  * Code the client-side algorithm to calculate capacity across the 5 buckets.
  * Implement the interactive Tempo Balancer logic and pop-up suggestions.
* **Week 3 (Oct 5 – Oct 11) — Beat Breaks & Refinement**:
  * Build the mandatory Recovery Downtime lock-out feature.
  * Conduct rigorous bug testing and deploy the app live via Expo.
