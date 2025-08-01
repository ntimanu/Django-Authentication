# Django Authentication App

A simple Django application that implements user authentication features using custom forms. The app supports user registration, login, logout, and protected pages accessible only to logged-in users.

## 🚀 Features

- User registration with username and password
- User login and logout
- CSRF protection on all POST forms
- Redirects to intended pages using `next` parameter
- Protected views using `@login_required` and `LoginRequiredMixin`
- Form validation and error messages
- Simple HTML templates with Django templating language

## 🛠 Tech Stack

- Python 3.13
- Django 5.2.4
- HTML/CSS (no frontend framework used)

## 📁 Project Structure

authProject/
├── authApp/
│ ├── migrations/
│ ├── templates/
│ │ └── accounts/
│ │ ├── login.html
│ │ ├── register.html
│ │ └── home.html
│ ├── forms.py
│ ├── views.py
│ ├── urls.py
│ └── ...
├── authProject/
│ ├── settings.py
│ ├── urls.py
│ └── ...
├── manage.py
└── README.md


## 🧪 How to Run Locally

### 1. Clone the repository

git clone https://github.com/your-username/django-auth-app.git
cd django-auth-app

### 2. Create and activate a virtual environment

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

## 3. Install dependencies
bash

Copy

To modify
pip install -r requirements.txt
## 4. Run migrations
bash

Copy

To modify
python manage.py migrate
## 5. Start the development server
bash

Copy

To modify
python manage.py runserver
Visit http://127.0.0.1:8000/accounts/login/to log in or http://127.0.0.1:8000/accounts/register/to register.

🧾 Example Credentials (for testing)
You can create a superuser:

bash

Copy

To modify
python manage.py createsuperuser
🔐 Security Notes
All forms are protected with CSRF tokens.

Passwords are securely hashed using Django's built-in user model.

📌 TODOs
Add email field and verify

Improve UI with Bootstrap or Tailwind

Add password reset functionality

Use Django's UserCreationForminstead of custom form (optional)

🙌 Acknowledgements
Built with ❤️ using Django.
