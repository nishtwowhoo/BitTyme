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

#### Problem Context and Root Causes
For university students, academic burnout is rarely triggered by a single massive event, such as a final exam. Instead, it is the cumulative result of a silent, multi dimensional pile up of daily stressors. Students constantly juggle lectures, part time employment, group projects, student club commitments, and basic household errands. Because cognitive and physical stress accumulation is invisible, students struggle to gauge their active limits. They continuously accept new responsibilities, sacrifice sleep, and run on empty until sudden exhaustion hits.

#### The Target Stakeholders
Our primary users are highly active university students who balance complex, non academic responsibilities alongside their degree programs. This includes working student professionals, student organization leaders, and final year students managing intensive research projects.

#### Why Existing Market Solutions Fail
Industry standard tools like Google Calendar, Notion, and Todoist are fundamentally time centric or task centric. They treat a calendar hour of passive laundry exactly the same as a calendar hour of a high stakes examination. These applications operate under the assumption of infinite human capacity, encouraging users to pack schedules with back to back blocks. 

Furthermore, traditional productivity software relies on constant manual input, tedious self categorization, and active list management. This administrative overhead creates heavy cognitive friction, quickly causing tracking fatigue and forcing busy students to abandon the software entirely. They fail to account for real cognitive and emotional bandwidth limits, allowing users to overbook themselves continuously until burnout occurs.

---

### 🥁 Our Solution: BitTyme

BitTyme is an intelligent, voice first personal workload assistant and conversational wellness companion designed to protect students from academic burnout. 

Instead of forcing users to manage tedious calendars and stress inducing to do lists, BitTyme acts as a proactive helper. By combining background schedule intelligence with a supportive companion mascot, the application completely removes the administrative burden of staying organized. BitTyme shifts the focus from simple time tracking to active, conversational workload protection.

---

### ✨ Key Features

#### 1. Hands Free Voice Widget
Students can add, schedule, or update any task on their calendar simply by speaking to a home screen widget. The conversational artificial intelligence automatically parses the task details in the background, completely eliminating the need to open the app or type manual entries on the go.

#### 2. Active Schedule Rebalancing 
This is the core engine of BitTyme. When the system detects that your schedule is getting too packed, it actively intervenes. The app automatically scans your database, flags low priority responsibilities such as optional social commitments or non urgent errands, and suggests postponing them to a lighter week. This active postponement ensures your schedule dynamically adapts to your actual cognitive capacity, keeping your daily workload balanced.

#### 3. Interactive Mascot Companion
Rather than presenting a cold, clinical utility dashboard, BitTyme introduces an animated mascot to serve as the face of the platform. This companion makes the artificial intelligence integration feel warm, alive, and supportive, acting as a personal advocate for the student's mental and physical well being.

### 2. Ideation & Process

##### 2.1 Ideas We Considered

We explored several distinct concepts during our initial brainstorming sessions before choosing our final direction. Below is the exact matrix of the ideas we evaluated and the rationale behind our decisions.

| Idea | Why it was dropped / kept |
| :--- | :--- |
| **Active Schedule Rebalancing** | **Kept.** This core engine directly resolves the passivity of traditional calendars by actively protecting student bandwidth. Instead of merely tracking and reporting stress levels, the system dynamically analyzes active workload limits and automatically suggests postponing low priority tasks to lighter weeks. This feature was highly validated during mentor consultations as our primary market differentiator and our most impactful product innovation. |
| **Streak System** | **Dropped.** We considered introducing a TikTok style daily streak system to encourage consistent task updates and increase engagement. However, mentor feedback highlighted that daily streak requirements introduce unnecessary psychological pressure on already stressed students. Forcing a busy student to log in daily simply to preserve a virtual streak transforms a supportive wellness companion into an administrative burden, actively worsening the very academic burnout we are trying to prevent. |
| **five bucket system** | **Dropped.** Requiring busy students to manually log and self rate every single task across multiple categories creates heavy cognitive friction and tracking fatigue. This administrative burden risks causing user burnout, turning a wellness tool into an exhausting daily chore rather than a helpful assistant. |

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
| 8 September 2026 | Danial Koh Yu Hang | The mentor raised critical concerns regarding cognitive friction and tracking fatigue. Requiring students to manually log and self rate every daily task across five categories creates heavy administrative overhead. This manual effort risks causing user burnout, turning a wellness tool into an active chore rather than a relief. | We completely eliminated the manual five bucket tracking system. To reduce cognitive friction, we integrated conversational artificial intelligence that allows users to add tasks simply by speaking through a home screen widget, without even opening the app. We also introduced an interactive companion mascot as the face of the application. Now, when users open BitTyme, they are immediately welcomed and assisted, shifting the app experience from tedious data entry to passive, friendly support. |

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
