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
For university students, academic burnout is rarely triggered by a single massive event, such as a final exam. Instead, it is the cumulative result of a silent, multi-dimensional pile up of daily stressors. Students constantly juggle lectures, part-time employment, group projects, student club commitments, and basic household errands. Because cognitive and physical stress accumulation is invisible, students struggle to gauge their active limits. They continuously accept new responsibilities, sacrifice sleep, and run on empty until sudden exhaustion hits.

#### The Target Stakeholders
Our primary users are highly active university students who balance complex, non-academic responsibilities alongside their degree programs. This includes working student-professionals, student organization leaders, and final-year students managing intensive research projects.

#### Why Existing Market Solutions Fail
Industry standard tools like **Google Calendar, Notion, and Todoist** are fundamentally time-centric or task-centric. They treat a calendar hour of passive laundry exactly the same as a calendar hour of a high stakes examination. These applications operate under the assumption of infinite human capacity, encouraging users to pack schedules with back-to-back blocks. They fail to account for real cognitive and emotional bandwidth limits, allowing users to overbook themselves continuously until burnout occurs.

---

### 🥁 Our Solution: BitTyme

**BitTyme** is a holistic personal workload manager and active capacity shield designed to prevent student burnout. Inspired by musical tempos and computer bits, BitTyme transitions student productivity from managing static time blocks to actively preserving human energy. 

The application maps out a student's live energy levels across five distinct resource buckets:
1. **Mental**: Cognitive exhaustion from study or exam preparation.
2. **Physical**: Physical fatigue from workouts, chores, or shifts.
3. **Social**: The battery required for networking, team meetings, and events.
4. **Errands**: General daily logistics and life administration.
5. **Time**: Actual hourly availability.

By tracking active capacity rather than just calendar hours, BitTyme helps students adjust their daily tempo and establish a sustainable lifestyle rhythm.

---

### ✨ Key Features

#### 1. The Tempo Dashboard
Instead of presenting a traditional static calendar, this interface visualizes student bandwidth across the five core resource buckets. Designed as a set of fluid, audio-player style gauges, the dashboard provides a clear sanity check of personal capacity. When any resource gauge enters critical thresholds, the interface changes states to warn the user before severe burnout occurs.

#### 2. The Tempo Balancer
When any energy gauge passes eighty five percent capacity, the rebalancing engine intervenes. The system scans the database to isolate low-priority items, such as optional social engagements or non-urgent chores. It then generates a single-tap option to defer those specific tasks to lighter weeks, lowering active stress and protecting user bandwidth.

#### 3. Beat Breaks
To safeguard mental health, the system automates mandatory recovery blocks when the user enters high burnout risk zones. During these protected downtime windows, the application prevents the user from scheduling new academic or vocational tasks. The system then guides the student toward tailored recovery suggestions, such as matching a low physical fatigue score with a recommendation for an outdoor walk.

### 2. Ideation & Process

##### 2.1 Ideas We Considered

We explored several distinct concepts during our initial brainstorming sessions before choosing our final direction. Below is the exact matrix of the ideas we evaluated and the rationale behind our decisions.

| Idea | Why it was dropped / kept |
| :--- | :--- |
| **BitTyme (Five Bucket Capacity System)** | **Kept.** This solution directly addresses the root causes of student burnout. By shifting the focus from time blocks to multi category cognitive energy capacity, we can actively prevent silent stress accumulation. |
| **Gamified Academic Quest System** | **Dropped.** Awarding virtual experience points for completing tasks creates an unhealthy incentive loop. It encourages already stressed students to take on more work to gain virtual rewards, which actively worsens burnout. |
| **AI Notification & Email Responder** | **Dropped.** This is a highly reactive tool. While it helps resolve minor daily chores, it completely fails to address the core problem of lifestyle over commitment and physical exhaustion. |

##### 2.2 Ideation Boards

We mapped out our ideation process using visual diagrams to understand the relationship between student stress triggers and our application features.

![Student Burnout Problem Tree](images/problem-tree.png)  
*Figure 1: Our Problem Tree illustrates how invisible stress accumulation and the habit of constantly saying yes lead directly to student burnout.*

![BitTyme User Journey Flow](images/user-flow.png)  
*Figure 2: Our User Journey Flow tracks how a newly scheduled task is calculated by the energy algorithm, triggering the rebalancing engine if load limits are exceeded.*

##### 2.3 Mentor Consultation

We consulted with hackathon mentors during the prototype week to pressure test our concept and refine our user experience.

| Date | Mentor | Feedback Received | What Was Changed |
| :--- | :--- | :--- | :--- |
| 10 September 2026 | Varsha Selvakumar (Hackathon Mentor) | The recovery suggestions might feel like just another set of tasks or annoying pop up notifications that busy students will immediately swipe away without reading. | We added a Hard Lock feature for critical burnout zones. When mental capacity exceeds ninety percent, the system physically locks the task scheduling interface and auto reserves calendar blocks for rest. |

---

### 3. Design & Prototype

**UI Prototype: [ Public Link to Figma Prototype ]**  
*(Note: Please ensure your Figma link is set to public so reviewers can open it in an incognito window)*

We designed a clean, high contrast dark mode mobile interface to keep students engaged and minimize visual fatigue. Below are the three key screens illustrating our core user flow.

#### 1. The Tempo Dashboard
![Tempo Dashboard Screen](images/screen-dashboard.png)  
*Caption: The main dashboard visualizes active capacity across Mental, Physical, Social, Time, and Errands. The gauges glow green during healthy periods and shift to bright amber or red when thresholds are breached.*

#### 2. The Tempo Balancer
![Tempo Balancer Screen](images/screen-balancer.png)  
*Caption: When a capacity gauge exceeds eighty five percent, the Tempo Balancer card slides up, offering a simple single tap option to defer low priority chores to a lighter week.*

#### 3. Active Beat Breaks
![Beat Breaks Screen](images/screen-recovery.png)  
*Caption: In critical red zones, the screen locks with a soothing rest timer. The app prevents the user from scheduling new academic tasks, guiding them instead toward tailored recovery habits.*

---

### 4. What Makes It Different

BitTyme is not a calendar app. It is a protective energy shield. Below is our market differentiation showing why we stand out from existing tools.

* **Five Category Capacity Tracking:** Traditional apps like Google Calendar only track chronological hours. BitTyme tracks actual cognitive and physical limits across five distinct areas.
* **Active Rebalancing Engine:** Notion and Todoist let users pile up infinite lists of tasks. BitTyme actively intervenes to suggest auto deferrals, keeping schedules balanced.
* **Enforced Rest Windows:** Standard productivity tools push users to constantly do more work. BitTyme protects student wellness by locking in mandatory rest periods during high stress events.

---

### 5. Technical Architecture & Feasibility

#### Tech Stack

To ensure rapid development and reliable execution during the hackathon, we selected a lightweight and highly efficient developer stack.

* **Frontend: React Native with Expo**
  * *Why we chose it:* It allows us to write a single clean TypeScript codebase that compiles natively for iOS and Android. Expo Go enables our team to run live tests on actual mobile devices instantly.
  * *Expected constraints:* Expo Go has minor limitations when integrating custom native device modules, meaning we must restrict our features to standard web and mobile APIs.
* **Backend & Database: Supabase (PostgreSQL)**
  * *Why we chose it:* Supabase provides a powerful PostgreSQL database with built in user authentication and real time database listeners out of the box, saving us from building a heavy custom backend.
  * *Expected constraints:* The Supabase free tier has a strict limit on active database connections, so we must write clean, efficient database queries to avoid rate limits.
* **Hosting & Deployment: Vercel & Expo Application Services (EAS)**
  * *Why we chose it:* It offers seamless continuous deployment pipelines. Web assets are hosted on Vercel, while mobile builds are distributed smoothly through EAS.
  * *Expected constraints:* The EAS free tier can have long build queues during peak hackathon hours, so we will run local emulator testing before triggering cloud builds.

#### Build Plan & Scope

To deliver a working, fully deployable mobile build by the end of the competition, we have scoped our development timeline into a tight three week roadmap.

* **Week 1: Base Core & Authentication (September 21 to September 27)**
  * Set up user registration and login flows using Supabase Auth.
  * Initialize the PostgreSQL database schema and link the tables to our app.
  * Build the static frontend mobile home screen displaying our five capacity gauges.
* **Week 2: Capacity Logic & Balancer Middleware (September 28 to October 4)**
  * Write the client side algorithm that aggregates user tasks to calculate live energy percentages.
  * Develop the Tempo Balancer pop up card that queries the database for low priority tasks when load limits are crossed.
  * Build the interactive task input screen.
* **Week 3: Recovery Locks & Deployment (October 5 to October 11)**
  * Implement the Beat Break dashboard lockout screen and countdown timer.
  * Run thorough end to end bug testing on physical devices using Expo Go.
  * Deploy the final builds and generate a scannable QR code for the judges.
