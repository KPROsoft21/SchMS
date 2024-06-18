# School Management System

<img width="1498" alt="ss" src="https://github.com/KPROsoft21/SchMS/assets/99348571/8d3467e9-477a-481c-9a79-f7bdbd4b8d29">

Current features
----------------
* Dashboard: School demographics and analytics. Restricted to only admins
* News And Events: All users can access this page
* Admin manages students(Add, Update, Delete)
* Admin manages lecturers(Add, Update, Delete)
* Students can Add and Drop courses
* Lecturers submit students' scores: _Attendance, Mid exam, Final exam, assignment_
* The system calculates students' _Total, average, point, and grades automatically_
* Grade comment for each student with a **pass**, **fail**, or **pass with a warning**
* Assessment result page for students
* Grade result page for students
* Session/year and semester management
* Assessments and grades will be grouped by semester
* Upload video and documentation for each course
* PDF generator for students' registration slip and grade result
* Page access restriction
* Storing of quiz results under each user
* Question order randomization
* Previous quiz scores can be viewed on the category page
* Correct answers can be shown after each question or all at once at the end
* Logged-in users can return to an incomplete quiz to finish it and non-logged-in users can complete a quiz if their session persists
* The quiz can be limited to one attempt per user
* Questions can be given a category
* Success rate for each category can be monitored on a progress page
* Explanation for each question result can be given
* Pass marks can be set
* Multiple choice question type
* True/False question type
* Essay question type
* Custom message displayed for those that pass or fail a quiz
* Custom permission (view_sittings) added, allowing users with that permission to view quiz results from users
* A marking page which lists completed quizzes, can be filtered by quiz or user, and is used to mark essay questions

# Requirements:

> The following programs are required to run the project

- [Python3.9+](https://www.python.org/downloads/)
- [PostgreSQL database](https://www.postgresql.org/download/)

# Installation

- Clone the repo with

```bash
git clone https://github.com/KPROsoft21/SchMS.git
```

- Create and activate a python virtual environment

```bash
pip install -r requirements.txt
```

- Create `.env` file inside the root directory and include the following variables

```bash
DB_NAME=[YOUR_DB_NAME]
DB_USER=[DB_ADMIN_NAME]
DB_PASSWORD=[DB_ADMIN_PASSWORD]
DB_HOST=localhost
DB_PORT=[YOUR_POSTGRES_PORT default is 5432]
USER_EMAIL=[YOUR_EMAIL]
USER_PASSWORD=[EMAIL_PASSWORD]
DEBUG=True
SECRET_KEY=[YOUR_SECRET_KEY]
```

```bash
python manage.py migrate
```

```bash
python manage.py runserver
```

Lastly, go to http://127.0.0.1:8000
