# PRAVAAH INTEGRATION GUIDELINES

## Project Structure

Modules:

* usermgmt
* participants
* faculty
* courses
* hostel
* commonmodules
* dashboard

---

## Team Ownership

User Management Team

Owns:

* Authentication
* Registration
* Roles
* Permissions
* Audit Logs
* Profiles

Participant Team

Owns:

* Students
* Admissions
* Attendance
* Results

Faculty Team

Owns:

* Trainers
* Skills
* Certifications
* Availability

Course Team

Owns:

* Programs
* Courses
* Modules
* Materials
* Batches
* Sessions
* Assessments
* Certificates

Hostel Team

Owns:

* Hostels
* Rooms
* Allocations
* Visitors
* Maintenance

Common Modules Team

Owns:

* Notifications
* Documents
* Communication
* Calendar
* Scheduling

Dashboard Team

Owns:

* Reports
* Analytics
* Charts
* KPIs

---

## Standard Module Structure


PRAVAAH/
│
├── manage.py
├── requirements.txt
├── README.md
├── UI_STYLE_GUIDE.md
├── INTEGRATION_GUIDELINES.md
├── .gitignore
│
├── pravaah/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── usermgmt/
├── participants/
├── faculty/
├── courses/
├── hostel/
├── commonmodules/
├── dashboard/
│
├── templates/
│   ├── base.html
│   └── components/
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
└── media/

Every team must create the same internal structure:

module/
│
├── models.py
├── views.py
├── urls.py
├── forms.py
├── admin.py
├── services.py
│
├── templates/
│   └── module_name/
│
├── static/
│   └── module_name/
│
└── migrations/


## Naming Standards

App Names

Correct:

participants
faculty
courses
hostel

Wrong:

ParticipantManagement
FacultyModule
CourseSystem

---

Models

Use PascalCase

Examples:

Student
Trainer
Course
Hostel

---

Variables

Use snake_case

Examples:

student_name
course_fee
trainer_email

---

URL Naming

Use:

participants:list
participants:add
participants:edit
participants:delete

faculty:list
courses:list

---

## Database Rules

Follow the official PRAVAAH schema.

Use meaningful table names.

Examples:

students
student_guardians

trainers
trainer_skills

courses
modules
materials

hostels
rooms
room_allocations

notifications
documents
audit_logs

---

## Git Branch Rules

Main Branches:

main
develop

Feature Branches:

feature/usermgmt
feature/participants
feature/faculty
feature/courses
feature/hostel
feature/commonmodules
feature/dashboard

---

## Pull Request Rules

Before creating a Pull Request:

✓ Code runs successfully

✓ Migrations included

✓ UI follows style guide

✓ No unnecessary files added

✓ No merge conflicts

✓ No hardcoded credentials

---

## Restricted Files

Only Integration Team may modify:

pravaah/settings.py

pravaah/urls.py

templates/base.html

requirements.txt

static/css/pravaah.css

---

## Security Rules

Never commit:

.env

database passwords

API keys

secret keys

---

## Final Integration Rule

Every team must work only inside its assigned module.

Changes outside assigned modules will be rejected during integration review.
