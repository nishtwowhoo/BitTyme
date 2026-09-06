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

## 2. Ideation & Process

### 2.1 Idea Evaluation & Evolution Matrix
To secure maximum value from our initial brainstorming, we explored multiple divergent solutions before consolidating our product scope. Below is the documentation of our design evolution, detailing the concepts we analyzed and our explicit engineering rationale for selecting or discarding each direction.

| Brainstormed Concept | Status | Evaluation & Selection Rationale |
| :--- | :--- | :--- |
| **A: BitTyme (Five Bucket Capacity System)** | **CHOSEN** | Focuses on active workload capacity across Mental, Physical, Social, Time, and Errands. Addresses the root cause of silent energy depletion by actively rebalancing schedules and enforcing mandatory recovery downtime. |
| **B: Gamified Academic Quest System** | *Discarded* | We analyzed a model that awarded experience points and level upgrades for task completion. However, user research indicated this creates an unhealthy incentive loop. It encourages already stressed students to take on more work to gain virtual rewards, actively compounding academic burnout. |
| **C: AI Email & Notification Auto Responder** | *Discarded* | This reactive approach only resolves minor clerical chores. It fails to address the cognitive overload of schedule over commitment, treating the symptoms of burnout rather than the lifestyle cause. |

### 2.2 System Mapping & Design Boards
To transition from theory to visual execution, our team constructed a multi layered design board mapping user distress to product utility.

#### 1. The Student Burnout Problem Tree
Our problem mapping identified that student exhaustion is not caused by singular academic events. It is driven by three core systemic failures:
* **The Visibility Deficit:** Students cannot quantify their active cognitive and physical energy expenditure.
* **The Default Acceptance Trap:** Calendars show free time as blank slots, prompting students to say yes to more commitments without evaluating active bandwidth.
* **The Low Priority Accumulation:** Minor errands and housekeeping logistics pile up, slowly draining the remaining mental energy needed for core academic performance.

#### 2. The BitTyme User Journey Flow
Our design flow charts how a task transitions from system input to active capacity balancing:

[User inputs academic assignment] ──> [Algorithm calculates Mental & Time load weight] │ ┌──────────────────────────────┴──────────────────────────────┐ ▼ (Load under 85%)                                            ▼ (Load exceeds 85%) [Task scheduled on calendar]                                 [Tempo Balancer system triggers] │                                                             │ ▼                                                             ▼ [Normal dashboard display]                              [Suggests auto deferrals for low priority tasks] │ ▼ [Locks in mandatory Beat Break rest block]

### 2.3 Mentor Consultation & Feedback Integration
*This framework documents our collaborative iteration with industry mentors during the prototype sprint.*

| Date of Session | Mentor Name & Role | Critical Feedback Provided | Engineering Actions & Design Changes |
| :--- | :--- | :--- | :--- |
| [Date] | [Insert Mentor Name, e.g., Senior Mobile Engineer] | "The active recovery suggestions might feel like just another set of tasks or annoying notification pop ups that students will immediately swipe away without reading." | We restructured our design to implement Hard Locks for critical burnout zones. When mental capacity exceeds ninety percent, the system physically prevents the scheduling of new academic tasks and auto reserves calendar space for rest. |

---

## 3. Design & Prototype
👉 **[Click Here to Access the High Fidelity Interactive Figma Prototype]**  
*(Note: Link must be public and verified for grading access in external browsers)*

### 📱 Product Interface Architecture
Our user experience strategy is centered on high accessibility, high contrast dark mode elements, and responsive touch controls designed to keep students engaged.

#### 1. Screen 1: The Tempo Dashboard
* **User Experience Objective:** Instant cognitive clarity of active energy reserves.
* **Design Execution:** Features five dynamic audio style capacity gauges representing Mental, Physical, Social, Time, and Errands. When overall capacity remains below seventy five percent, the interface displays a soothing deep green and blue styling. As thresholds cross eighty five percent, the gauges shift to high contrast amber and red, providing an immediate visual warning of incoming burnout.

#### 2. Screen 2: The Tempo Balancer Interface
* **User Experience Objective:** Frictionless stress mitigation.
* **Design Execution:** A warning card slides into view when a resource bucket is overloaded. The screen displays a curated list of low priority tasks, such as optional errands or club meetings. The user is presented with a prominent, single tap button to defer these specific items to lighter weeks, immediately recalculating and reducing the dashboard load meters.

#### 3. Screen 3: Beat Breaks & Protected Recovery Zones
* **User Experience Objective:** Uncompromising wellness protection.
* **Design Execution:** When critical capacity is reached, the screen transitions to a calm, minimalist overlay locking the calendar interface. Users cannot input new academic tasks during this period. The screen displays a clear countdown timer alongside active, personalized recovery activities designed to restore the depleted resource bucket.

---

## 4. What Makes It Different

Our product shifts the paradigm of productivity software by treating personal energy as a finite, multi dimensional resource. Below is our strategic market differentiation:

| Product Metric | Google Calendar / Notion | Standard To-Do Checklists | **BitTyme (Our Application)** |
| :--- | :--- | :--- | :--- |
| **Primary Unit of Measurement** | Tracks strict chronological time slots. | Tracks numerical quantity of tasks completed. | **Tracks multi dimensional human energy capacity.** |
| **System Behavior on Overload** | Passively allows overlapping bookings, facilitating over commitment. | Displays endless, stress inducing lists without assessing context. | **Intervenes dynamically to suggest task deferrals and rebalance schedules.** |
| **Core Product Philosophy** | Prioritizes constant, unyielding output and scheduling. | Focuses entirely on task completion without considering rest. | **Actively enforces mandatory recovery blocks to protect mental health.** |

---

## 5. Technical Architecture & Build Plan

### 💻 System Stack Selection
Our engineering architecture is selected to ensure high performance, rapid iteration, and reliable cross platform execution.

#### 1. Frontend Framework: React Native with Expo
* **Engineering Justification:** Allows our team to write a single, clean TypeScript codebase that compiles natively to both iOS and Android. Expo Go enables rapid, hot reloading testing on physical devices, satisfying the deployability requirements of the hackathon.

#### 2. Database & Backend: Supabase (PostgreSQL)
* **Engineering Justification:** Supabase provides a robust PostgreSQL database with instant REST APIs and built in user authentication. Its real time database listeners allow BitTyme to synchronize capacity logs instantly across devices without building a heavy custom backend infrastructure.

#### 3. Host & Deployment Pipeline: Vercel & Expo Application Services
* **Engineering Justification:** The landing page and web dashboards are deployed continuously via Vercel. Mobile builds are compiled and distributed through Expo Application Services, ensuring judges can interact with the live application on emulators or actual devices.

### 📊 PostgreSQL Database Schema
To prove our technical feasibility to the engineering judges, we have mapped out our core database tables:

```sql
-- Core User Profiles Table
CREATE TABLE profiles (
    id UUID REFERENCES auth.users PRIMARY KEY,
    username TEXT UNIQUE NOT NULL,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT TIMEZONE('utc'::text, NOW()) NOT NULL
);

-- Active Student Tasks Table
CREATE TABLE tasks (
    id UUID DEFAULT gen_random_uuid() PRIMARY KEY,
    user_id UUID REFERENCES profiles(id) ON DELETE CASCADE NOT NULL,
    title TEXT NOT NULL,
    description TEXT,
    due_date TIMESTAMP WITH TIME ZONE NOT NULL,
    priority INT DEFAULT 3, -- 1: High, 2: Medium, 3: Low
    is_completed BOOLEAN DEFAULT FALSE NOT NULL,
    -- Capacity load weights assigned by the user or system
    mental_weight INT DEFAULT 0,  -- Scale 0-10
    physical_weight INT DEFAULT 0, -- Scale 0-10
    social_weight INT DEFAULT 0,   -- Scale 0-10
    errands_weight INT DEFAULT 0,  -- Scale 0-10
    time_minutes INT DEFAULT 60 NOT NULL
);
