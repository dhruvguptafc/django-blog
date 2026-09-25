# Blog Management System

A full-stack blog management application built with **Django** and **PostgreSQL**. The application allows users to create, manage, search, and publish blog content with role-based access for **Managers and Editors**.

## Features

* 🔐 User registration and authentication
* 👥 Role-based access for Managers and Editors
* ✍️ Create, update, and delete blog posts
* 🗂️ Category management
* 🔎 Search blog posts
* 📢 Publish and manage blog content
* 🛡️ Protected views using Django authentication and permissions
* ⚙️ Django Admin for application management
* 📱 Responsive interface using Bootstrap

## User Roles

### Manager

Managers have higher-level content management permissions and can manage blog content and categories.

### Editor

Editors can manage blog posts according to their assigned permissions.

## Tech Stack

| Technology | Usage                  |
| ---------- | ---------------------- |
| Python     | Backend programming    |
| Django     | Web framework          |
| PostgreSQL | Database               |
| Bootstrap  | Frontend styling       |
| HTML/CSS   | User interface         |
| JavaScript | Frontend functionality |

## Application Flow

```text
User
 │
 ├── Register / Login
 │
 └── Blog
      │
      ├── Browse Posts
      ├── Search Posts
      └── View Post
             │
             └── Role-based Management
                    ├── Manager
                    └── Editor
```

## Project Structure

```text
blog/
├── blog/
│   ├── settings.py
│   ├── urls.py
│   └── ...
│
├── <app_name>/
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   ├── urls.py
│   └── ...
│
├── templates/
├── static/
├── manage.py
└── requirements.txt
```

## Getting Started

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd <project-folder>
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the database

Update the database configuration in `settings.py` or configure the required environment variables.

### 5. Run migrations

```bash
python manage.py migrate
```

### 6. Start the development server

```bash
python manage.py runserver
```

Open the application at:

```text
http://127.0.0.1:8000/
```





## Future Improvements

* Dedicated Manager dashboard
* Dedicated Editor dashboard
* Django REST Framework API
* React frontend
* Deployment with production configuration
