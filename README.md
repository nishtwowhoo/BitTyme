# 🥁 BitTyme by The Bit-tles
**Problem Statement:** Beating the Burnout (Stress & Workload Manager)  
**Video Presentation:** [Insert Unlisted YouTube Link Here] (Strictly under 5 minutes!)  
**Presentation Slides:** [Insert Public Google Slides or Canva Link Here]  

---

## 📋 Team Members ("The Bit-tles")
* **Danish Firdaus** - Product Lead
* **[Member 2 Name]** - UI/UX Designer
* **[Member 3 Name]** - Tech Lead & Architect
* **[Member 4 Name]** - Pitch Lead & Storyteller

---

## 1. Project Overview

### 🎯 The Problem
University students are increasingly overwhelmed by competing commitments [1]. However, they rarely burn out from one massive task. Instead, it is the silent, multi-dimensional accumulation of academic deadlines, part-time jobs, social obligations, and everyday errands that drains them [1]. 

Existing solutions like **Google Calendar, Notion, and Todoist** fall short because they are strictly **time-centric or task-centric** [2]. They treat 1 hour of low-effort laundry exactly the same as 1 hour of high-stakes exam preparation. They lack an understanding of cognitive and physical limits, allowing students to overbook their mental energy [3].

### 🥁 Our Solution: BitTyme
**BitTyme** is a holistic workload manager and active capacity shield for students [3]. Inspired by musical tempos and computer bits, BitTyme shifts the focus from managing "time" to managing **human energy**. The application models a student's personal bandwidth as a balanced rhythm that shifts dynamically based on daily load across 5 core categories: **Mental, Physical, Social, Errands, and Time** [3].

#### ✨ Key Features:
1. **5-Bucket "Tempo Dashboard"**: Visualizing overall energy across Mental, Physical, Social, Time, and Errands as an active dashboard gauge [3]. 
2. **Smart "Tempo Balancer" (Auto-Deferral)**: When any capacity bucket exceeds 85% load, BitTyme flags low-priority items (e.g., non-urgent chores or optional events) and suggests auto-deferring them to lighter weeks [3].
3. **Smart "Beat Breaks" (Active Recovery Locks)**: Protects a student's mental well-being by actively blocking mandatory "Recovery Time" (e.g., sleep, outdoor walking) and preventing new task additions during locked recovery zones [3].

---

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
* **Hosting/Deployment**: **Expo Go** (for instant mobile previewing) & **Vercel** (for landing page / web dashboard) [9].

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
