# School Management System

**Author:** Bhaskar Kafle
**Email:** [kaphlebhaskar012345@gmail.com](mailto:kaphlebhaskar012345@gmail.com)

A comprehensive **School Management System** built with **Django Admin** to efficiently manage students, fees, teachers, and other school-related records. This system leverages Django’s built-in administration interface to simplify day-to-day operations for educational institutions.

[Django Admin Documentation](https://www.google.com/search?client=opera&q=django+admin&sourceid=opera&ie=UTF-8&oe=UTF-8)

---

## Features

* Manage student records directly from the admin panel.
* Record and track fee submissions.
* Maintain teacher profiles and salary records.
* Link students to multiple courses.
* Search records using multiple fields.
* Export data in CSV format.
* Optimized queries for faster performance.
* Future enhancement: visual graphs comparing teacher salaries vs. student fees collected.

---

## Getting Started

### Prerequisites

* Python 3.x
* pip
* virtualenv (recommended)
* Docker & Docker Compose (optional for containerized deployment)

---

### Local Development

1. **Create and activate a virtual environment:**

```bash
virtualenv venv
source venv/bin/activate
```

2. **Clone the repository:**

```bash
git clone https://github.com/Vaskoor/school_management_system_django .
```

3. **Navigate to the project directory and install dependencies:**

```bash
cd school_management_system_django/schoolmanagemntsystem
pip install -r requirements.txt
```

4. **Apply database migrations and create a superuser:**

```bash
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
```

5. **Run the development server:**

```bash
python manage.py runserver
```

Visit `http://localhost:8000` to access the application.

> Optionally, you can use **Foreman** with **Gunicorn**:

```bash
foreman start
```

---

### Using Docker

1. **Build the Docker container:**

```bash
docker-compose build
```

2. **Create a superuser inside the container:**

```bash
docker-compose run web python manage.py createsuperuser
```

3. **Start the container:**

```bash
docker-compose up
```

The application will be available at `http://127.0.0.1:8000`.

---

## To-Do

* [x] Manage student records in admin
* [x] Submit and track fees
* [x] Show last submitted fee per student
* [x] Link students to courses
* [x] Search records by multiple fields
* [x] Optimize query performance
* [x] Manage teacher records and salaries
* [x] Export admin data in CSV format
* [ ] Visualize teacher salaries vs. student fees collected

---

## License

This project is licensed under [GLWTPL](LICENSE).

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind are welcome!
