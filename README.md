Countdown — Study Planner / Exam Countdown

A single-page, no-database study planner built with plain HTML, CSS, and JavaScript. All data is stored locally in the browser using localStorage — no backend, no server, no setup required.

Features
Subject & Syllabus Tracking Add subjects along with an exam date and a list of topics/chapters. Mark each topic as done or pending.
Progress Tracking Each subject shows a progress bar and completion percentage based on topics marked done.
Exam Countdown Live countdown (in days) to each subject's exam date, shown as ticket-style cards at the top of the page. Subjects with 3 or fewer days remaining are visually flagged as urgent.
Daily Study Target For every subject with pending topics, the app calculates:
  topics per day = ceil(pending topics / days remaining)

This keeps the daily workload realistic as the exam date approaches.

Today's Focus An auto-generated list of exactly which topics to study today, pulled from all subjects based on their calculated daily pace.
How to run

No installation or server needed.

Open index.html directly in any modern browser (double-click, or right-click → Open With → Browser).
Start adding subjects, exam dates, and topics.
All data is saved automatically to your browser's localStorage and will persist between visits on the same browser/device.

Note: Since this uses localStorage, data is device- and browser-specific. Clearing browser data/cache will erase saved subjects and topics. There is no login, sync, or cloud storage — this is intentional, matching the "no-database" project requirement.

Tech stack
HTML5
CSS3 (custom properties, no framework)
Vanilla JavaScript (ES6+)
Google Fonts (Fraunces, IBM Plex Mono, Inter) — loaded via CDN
Browser localStorage API for persistence
File structure
study-planner/
├── index.html   # Full app: markup, styles, and script in one file
└── README.md    # This file