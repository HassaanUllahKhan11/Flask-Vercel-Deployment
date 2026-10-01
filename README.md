# Flask-Vercel-Deployment

A lightweight **Python Flask web application deployed on Vercel**, demonstrating how a Flask backend can be configured and hosted using Vercel's Python runtime and deployment configuration.



---

## 📌 Overview

This project demonstrates a minimal Flask application configured for deployment on **Vercel**.

The application provides a simple web endpoint that responds with:

```text
Hello, Flask on Vercel!
```

Although intentionally small, the project demonstrates the complete workflow of:

```text
Python → Flask → Vercel Configuration → Cloud Deployment
```

The repository is primarily focused on **backend deployment, server configuration, and cloud hosting** rather than frontend development.

---

## 🏗️ Architecture

```text
                    User
                      │
                      ▼
              ┌───────────────┐
              │    Vercel     │
              │   Deployment  │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │ Python Runtime│
              │   + Flask     │
              └───────┬───────┘
                      │
                      ▼
                 Flask App
                      │
                      ▼
             GET /
                      │
                      ▼
       "Hello, Flask on Vercel!"
```

Vercel is configured to use its Python runtime for the Flask application through `vercel.json`.

---

## 🛠️ Technologies

* **Python**
* **Flask**
* **Gunicorn**
* **Vercel**
* **GitHub**

---

## 📂 Project Structure

```text
Flask-Vercel-Deployment/
│
├── .github/
│   └── workflows/
│
├── .gitignore
├── app.py
├── requirements.txt
└── vercel.json
```

---

## 🔑 Application

The Flask application is initialized using:

```python
from flask import Flask

app = Flask(__name__)
```

A root endpoint is then defined:

```python
@app.route('/')
def home():
    return "Hello, Flask on Vercel!"
```

The application can also be started locally using Flask's development server.

---

## ⚙️ Dependencies

The project uses a minimal dependency set:

```text
Flask
Gunicorn
```

These dependencies are specified in `requirements.txt`.

---

## ☁️ Vercel Deployment

The project includes a `vercel.json` configuration file that defines the Python runtime and routing used for deployment.

The deployment workflow allows the Flask application to run as a Python-based serverless deployment on Vercel.

### Deployment Flow

```text
1. Push project to GitHub
          ↓
2. Connect repository to Vercel
          ↓
3. Vercel reads deployment configuration
          ↓
4. Python runtime is configured
          ↓
5. Flask application is deployed
          ↓
6. Application becomes publicly accessible
```

---

## 💻 Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/HassaanUllahKhan11/Flask-Vercel-Deployment.git
cd Flask-Vercel-Deployment
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the environment

**Windows:**

```bash
venv\Scripts\activate
```

**Linux/macOS:**

```bash
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the application

```bash
python app.py
```

The application will be available locally at:

```text
http://127.0.0.1:5000
```

---

## 🌐 Deployment

The application is deployed using **Vercel**.

For Flask applications, Vercel can use its Python runtime to serve the Flask application as a serverless deployment. This approach is also demonstrated by other Flask/Vercel deployment examples.

### Production Deployment

**Live URL:**

https://flask-vercel-ruddy.vercel.app/

---

## 🎯 What This Project Demonstrates

This project demonstrates practical experience with:

* Building a Python web application using Flask
* Creating HTTP routes and backend logic
* Managing Python dependencies
* Configuring a cloud deployment
* Deploying Python applications to Vercel
* Working with serverless Python runtimes
* Connecting GitHub-based development with cloud deployment

---

## 🔮 Potential Extensions

The current project intentionally keeps the application minimal. It could be extended into:

* REST API development
* Database-backed Flask applications
* Authentication and authorization
* ML model inference APIs
* AI/LLM-powered APIs
* File upload and processing services
* Frontend + Flask backend applications
* Production monitoring and logging

---

## 👨‍💻 Author

**Hassaan Ullah Khan**

Data Science | AI/ML | Python | Backend Development

**GitHub:**
https://github.com/HassaanUllahKhan11

---

## 📜 Project Purpose

A compact deployment-focused project demonstrating the integration of **Flask, Python, GitHub, and Vercel** for hosting a backend web application.
