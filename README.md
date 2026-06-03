# 🩺 GDM Health Prediction System

A Django-based healthcare web application for **Gestational Diabetes Mellitus (GDM) risk prediction**, patient monitoring, clinician management, appointments, education, and medical report generation.

This project was developed as a health-focused web platform that supports both **patients** and **clinicians** through dashboards, prediction tools, health tracking, and data visualization.

---

## 📌 Project Overview

The GDM Health Prediction System helps users assess the risk of Gestational Diabetes Mellitus using health-related inputs such as glucose levels, BMI, HbA1c, blood pressure, pregnancy history, and other clinical factors.

The system includes a patient portal, clinician dashboard, prediction history, data analysis pages, appointment booking, glucose/vitals tracking, educational resources, and PDF report generation.

---

## ✨ Features

* User registration and login
* Patient and clinician roles
* GDM risk prediction
* Patient dashboard
* Clinician dashboard
* Glucose tracking
* Vitals tracking
* Pregnancy timeline
* Appointment booking and payment pages
* Clinician patient roster
* Clinician calendar
* Clinical messaging system
* Educational article library
* Prediction history
* Export prediction records as CSV and Excel
* Generate PDF reports
* Dataset upload and download pages
* Exploratory Data Analysis visualizations
* Machine learning model comparison pages
* Contact and about pages
* Custom admin dashboard

---

## 🛠️ Tech Stack

* **Backend:** Django / Python
* **Frontend:** HTML, CSS, JavaScript
* **Database:** SQLite
* **Machine Learning/Data:** Pandas, NumPy, Scikit-learn
* **Visualization:** Matplotlib, Seaborn, Plotly
* **PDF Reports:** xhtml2pdf / ReportLab
* **Deployment Support:** Gunicorn, Procfile

---

## 📁 Project Structure

```bash
health/
├── capstone/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── gdm/
│   ├── management/
│   │   └── commands/
│   │       ├── seed_demo_data.py
│   │       ├── seed_education.py
│   │       ├── repair_db.py
│   │       └── clear_test_data.py
│   ├── migrations/
│   ├── templates/
│   │   └── gdm/
│   │       ├── welcome.html
│   │       ├── login.html
│   │       ├── register.html
│   │       ├── patient_dashboard.html
│   │       ├── clinician_dashboard.html
│   │       ├── glucose_tracker.html
│   │       ├── vitals_tracker.html
│   │       ├── pregnancy_timeline.html
│   │       ├── appointment_book.html
│   │       ├── education_library.html
│   │       ├── report.html
│   │       └── result.html
│   ├── admin.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
│
├── static/
│   ├── css/
│   ├── js/
│   ├── img/
│   ├── plots/
│   └── eda_plots/
│
├── Data/
│   ├── gdm_synthetic_data.csv
│   └── GDM_Variable_Descriptions.xlsx
│
├── code/
│   └── gdm_jupyter.ipynb
│
├── files/
│   ├── senior_project.pdf
│   ├── senior_project.docx
│   └── GDM.pptx
│
├── manage.py
├── requirements.txt
├── Procfile
├── db.sqlite3
└── README.md
```

---

## 🚀 Getting Started

Follow these steps to run the project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/health.git
cd health
```

### 2. Create a Virtual Environment

```bash
python -m venv env
```

Activate the environment:

For Windows:

```bash
env\Scripts\activate
```

For macOS/Linux:

```bash
source env/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Apply Database Migrations

```bash
python manage.py migrate
```

### 5. Seed Demo Data

Optional, but recommended:

```bash
python manage.py seed_demo_data
python manage.py seed_education
```

### 6. Run the Development Server

```bash
python manage.py runserver
```

Open your browser and visit:

```bash
http://127.0.0.1:8000/
```

---

## 🔐 Admin Panel

Create a superuser:

```bash
python manage.py createsuperuser
```

Then run the server and visit:

```bash
http://127.0.0.1:8000/admin/
```

---

## 🧑‍⚕️ Main User Roles

### Patient

Patients can:

* Register and log in
* View their health dashboard
* Submit GDM prediction data
* Track glucose readings
* Track vital signs
* View pregnancy timeline
* Book appointments
* Read educational articles
* Download reports

### Clinician

Clinicians can:

* View clinician dashboard
* Manage patient roster
* View patient details
* Check appointments
* View payments
* Send clinical messages
* Review dataset information
* Monitor patient alerts

---

## 🧪 Prediction Features

The system calculates GDM risk based on several health factors, including:

* Age
* BMI
* Glucose level
* Blood pressure
* Insulin level
* HbA1c
* OGTT fasting level
* OGTT 1-hour level
* OGTT 2-hour level
* Number of pregnancies
* Family history
* Previous GDM history
* PCOS status

The prediction result provides a risk score and risk level such as:

* Low Risk
* Medium Risk
* High Risk

---

## 📊 Data Analysis and Visualization

The project includes EDA and model visualization pages such as:

* BMI analysis
* HbA1c distribution
* Glucose distribution
* Risk distribution
* Correlation heatmap
* Model comparison
* Confusion matrices
* ROC curve
* Precision-recall curve
* Feature importance charts
* SHAP summary plots

---

## 📄 Reports and Exporting

Users can export or generate:

* PDF reports
* CSV files
* Excel files
* Prediction history records
* Dataset downloads

---



## 📦 Requirements

The main dependencies are listed in:

```bash
requirements.txt
```

Install them using:

```bash
pip install -r requirements.txt
```
---

## 🔮 Future Improvements

* Add stronger machine learning model integration
* Improve UI responsiveness
* Add email notifications
* Add appointment reminders
* Add real online payment integration
* Add password reset functionality
* Improve data privacy and security
* Add doctor-patient chat in real time
* Add charts inside patient dashboards
* Deploy the system online

---

## 👨‍🎓 Project Author

Developed by Razane Chabib
---

## 📄 License

This project is for educational and academic purposes.
