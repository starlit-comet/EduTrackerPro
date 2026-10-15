# 🎓 EduTrack Pro — Teacher's Classroom & Exam Companion

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/Vanilla_JS-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Mobile Friendly](https://img.shields.io/badge/Mobile-First_Responsive-1e40af?style=for-the-badge)

**EduTrack Pro** is a lightweight, mobile-first web application designed for school teachers to streamline daily classroom management and eliminate human calculation errors during exam paper correction. 

Built as a zero-dependency, offline-capable single-page application, it handles daily topic scheduling, interactive roll-call attendance, notebook correction tracking, and **pattern-aware exam totaling** with built-in duplicate answer protection.

---

## ✨ Key Features

### 1. 📅 Daily Topic Scheduler & Teaching History
* **Lesson Planning:** Schedule daily topics by class, subject/unit, and period.
* **Live Status Toggling:** Track whether a topic is **Planned**, **Completed (Taught)**, or **Carried Over** to the next day with a single tap.
* **Classroom Reflections:** Record homework assigned or teaching notes for every session.
* **Search & Filter:** View historical logs across classes and filter by status or keyword.

### 2. 🙋‍♂️ Dual-Mode Attendance & Notebook Correction Tracker
* **📱 Interactive Roll Call Card Mode (Mobile-Optimized):**
  * View **1 or 2 student cards at a time** so the teacher can call out names one by one.
  * Large, touch-friendly buttons to mark **Class Attendance** (*Present*, *Absent*, *Late*) and **Notebook Correction Status** (*Corrected*, *Submitted - Pending*, *Incomplete*, *Not Submitted*).
  * Quick-tap remark chips (e.g., *Neat work*, *Incomplete Qs*, *Forgot notebook*), **Previous / Next** navigation buttons, keyboard/swipe support, and an optional **Auto-Next on Attendance Tap** toggle.
* **📋 Full Class Sheet Mode:**
  * Traditional spreadsheet-style table view for rapid bulk editing and one-click *"Mark All Present & Corrected"*.
* **Cumulative Stats:** Automatically calculates each student's attendance rate and notebook submission history.

### 3. 📝 Question Paper Pattern Builder & Correction Tracker
* **Custom Exam Blueprints:** Define sections, question number ranges (e.g., `Q1–Q5`), marks per question, and section choice rules (e.g., *"Attempt any 3 out of 5"*).
* **Paper Correction Progress:** Track how many answer scripts were collected, how many have been graded, and how many are still pending correction.

### 4. 🛡️ Smart Anti-Mistake Exam Totaling Tool
Designed to match how teachers grade physical answer booklets page by page:
* **Chronological Booklet Entry:** Enter the `Question Number` and `Marks Awarded` in the exact order the student wrote them in their answer sheet.
* **Duplicate Question Detection:** If a student writes the answer to the same question twice on different pages, the app immediately triggers a **Duplicate Answer Alert**, prevents double-counting, and lets the teacher choose to:
  * *Keep the Higher Mark*
  * *Keep the First Entry Only*
  * *Overwrite with the New Mark*
* **Automatic "Best-N" Choice Enforcement:** If a section requires 3 answers out of 5 and a student attempts all 5, the engine automatically counts the **top 3 highest-scoring answers** and flags the lowest ones as *Ignored (Extra Choice — 0M)*.
* **Max-Mark Validation:** Prevents accidentally awarding more marks than a question carries according to the section pattern.
* **Audit Log:** Maintains a timestamped log of every mark entry, duplicate block, and ignored optional question.

### 5. 📊 Student Detailed Score Sheet History
* **Individual Student Profiles:** View every student's historical performance across all exams alongside their attendance and notebook check metrics.
* **Question-by-Question Breakdown:** Visual grid showing awarded marks, ignored optional questions, and unattempted questions for every exam.
* **Export & Print:** Export class marklists to **CSV** (Excel-compatible) or print individual student report cards directly from the browser.

---

## 🚀 Getting Started

Because **EduTrack Pro** is built with vanilla HTML, CSS (Tailwind CDN), and JavaScript, no build step or backend server is required.

### Option 1: Direct Browser Launch
1. Clone this repository:
   ```bash
   git clone [https://github.com/your-username/edutrack-pro.git](https://github.com/your-username/edutrack-pro.git)