##🐛 BugHive — Bug Tracking System

A Django-based web application that helps users submit their buggy code and get it fixed by professional developers. Users can choose their preferred developer, track bug status in real time, comment on reports, and give website feedback.



## 🚀 Features

* 🐛 Submit bug reports with code snippets
* 👨‍💻 Choose your own developer to fix the bug
* 🔧 Developers analyze and submit fixed code with explanation
* 💬 Comment on any bug report
* 📣 Give feedback about the website
* 🔐 Role-based access — User, Developer, Admin
* 🏷️ Priority & status badges — Critical, High, Medium, Low
* 🔍 Filter bugs by status, priority, and language
* ⚡ Fast and clean light-themed UI
* 

## 🛠️ Built With

* **Backend:** Django 4.2 (Python)
* **Frontend:** HTML, CSS (no framework)
* **Database:** SQLite
* **Auth:** Django AbstractUser (custom roles)


## 📁 Project Structure

bugtracker/
├── manage.py
├── requirements.txt
├── bugtracker/              # Project config
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── accounts/                # App 1 — User management
│   ├── models.py            ← CustomUser (role: user / developer / admin)
│   ├── views.py
│   ├── forms.py
│   ├── urls.py
│   └── admin.py
├── bugs/                    # App 2 — Bug tracking
│   ├── models.py            ← BugReport, Comment, Feedback
│   ├── views.py
│   ├── forms.py
│   ├── urls.py
│   └── admin.py
└── templates/
    ├── base.html
    ├── accounts/
    │   ├── login.html
    │   ├── register.html
    │   ├── profile.html
    │   └── developer_list.html
    └── bugs/
        ├── home.html
        ├── bug_list.html
        ├── bug_detail.html
        ├── bug_form.html
        ├── feedback_form.html
        └── feedback_list.html

## 📦 Getting Started

Follow these steps to run the project locally:

### 1. Clone the Repository

```bash
git clone https://github.com/FariaFiza/Bug_Tracking..git
cd bugtracker
