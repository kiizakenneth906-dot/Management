Kampala Solid Waste Collection and Citizen Engagement Portal
============================================================
Contact: 0755530904 | www.solidwaste@gmail.com

HOW TO RUN
1. Unzip the folder.
2. Double-click index.html to open it in a browser (no server needed).

FILES
index.html    page structure
css/style.css styling (light and dark mode)
js/app.js     portal logic: roles, reporting, tickets, dashboard, AI board

ROLES (selector at top): Citizen, Collector, Administrator

NOTES
- Tickets are saved in the browser's localStorage (per device). For real use,
  connect a backend database (e.g. Node/Express + PostgreSQL or Django + MySQL).
- The AI briefing and chat use the claude.ai runtime (claude.use("sample")) and
  work only on the claude.ai published page. Outside it, they show a fallback
  message. To enable AI on your own server, replace the calls in js/app.js
  (functions ask() and brief()) with requests to your backend that calls an AI API.
- The collection schedule in js/app.js (SCHED) is sample data; replace with real days.
