# 💼 Job Application Tracker

A full-stack, database-driven web app that helps job seekers organize and track their job search in one place: applications, statuses, follow-ups, and analytics.

Built as the final project for **CIS 552 – Database Design** at UMass Dartmouth by **Stephanie Asinobi** and **Lavanya Murugesan**.

---

## ✨ Features

- **User accounts:** register and log in, with passwords securely hashed using bcrypt
- **Full CRUD:** add, view, edit, and delete job applications stored in MongoDB
- **Status tracking:** Applied → Interview Scheduled → Offer Received / Rejected / Withdrawn
- **Dashboard:** live counts for every status, plus recent applications
- **Follow-up reminders:** flags applications with no update in 14+ days
- **Browse Jobs:** save job listings you're interested in before applying
- **Search & filter:** by company, role, status, job type, and work mode
- **Analytics:** average response time, rejection rate by company, source performance (LinkedIn, Indeed, etc.), salary range analysis, and a weekly activity report
- **CSV export:** download your application data

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Language | Python 3 |
| Backend | Flask |
| Database | MongoDB (NoSQL) |
| Database Driver | PyMongo |
| Authentication | Flask-Bcrypt, Flask sessions |
| Frontend | HTML5, CSS3, Jinja2 templates |
| Tools | VS Code, MongoDB Compass |

**Why MongoDB?** Its flexible document model fits job application data well, since each application can have different fields, and its query and aggregation features power the search and analytics pages.

---

## 📸 Screenshots

![Screenshot](Screenshot%202026-10-22%20180924.png)
![Screenshot](Screenshot%202026-10-22%20181107.png)
![Screenshot](Screenshot%202026-10-22%20181116.png)
![Screenshot](Screenshot%202026-10-22%20181159.png)
![Screenshot](Screenshot%202026-10-22%20181341.png)
![Screenshot](Screenshot%202026-10-22%20182108.png)

---

## 🚀 How to Run Locally

**Requirements:** Python 3 and MongoDB installed and running on `localhost:27017`

```bash
# 1. Clone the repo
git clone https://github.com/stephanieokpi-purple/job-application-tracker.git
cd job-application-tracker

# 2. Install dependencies
pip install flask pymongo flask-bcrypt

# 3. Start the app
python app.py
```

Then open **http://127.0.0.1:5000** in your browser, register an account, and start tracking.

---

## 📁 Project Structure

```
job-application-tracker/
├── app.py            # Flask routes and MongoDB queries
├── static/
│   └── style.css     # Styling
└── templates/        # HTML pages (dashboard, applications, analytics, etc.)
```
