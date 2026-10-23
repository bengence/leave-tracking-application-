# 🍃 LeaveTracker Pro

**LeaveTracker Pro** is a lightweight, fully automated leave management web application designed specifically for small businesses and teams of up to 20 people. 

Built with a clean, zero-build-step frontend (Vanilla JS + Tailwind CSS) and a powerful serverless backend (Supabase), it eliminates the friction of tracking employee time off, sick days, and hourly leave. 

### ✨ Key Features

* **Automated Accruals:** Uses PostgreSQL `pg_cron` to automatically credit users 1.25 days of annual leave on the 1st of every month.
* **Smart Day Calculations:** Automatically excludes weekends and custom public holidays from leave request durations.
* **Granular Time-Off:** Supports standard daily leave (Annual, Sick, Family) as well as hourly "Time Off" requests (2 hours, 4 hours, or half-days).
* **Role-Based Workflows:** 
  * **Users** can view dynamic dashboards, submit requests, and see team events.
  * **Managers** get a dedicated approval pipeline and "Out of Office" team visibility.
  * **Developers (Admins)** have access to balance adjustment tools, event scheduling, and system overrides.
* **Database-Level Safeguards:** Strict Row Level Security (RLS) policies and trigger-based 20-user capacity limits ensure data security and compliance.
* **Modern UI/UX:** A striking, responsive Black & Yellow theme with dynamic widgets (Birthdays, Who's Away Today, and Manager OOO alerts).

### 🛠️ Tech Stack

* **Frontend:** HTML5, Vanilla JavaScript, Tailwind CSS (via CDN), FontAwesome
* **Backend / Database:** Supabase (PostgreSQL)
* **Auth:** Supabase Authentication
* **Automation:** Supabase `pg_cron` & Database Triggers
