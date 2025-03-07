# Django Admin Boilerplate

🚀 A simple boilerplate for Django admin dashboards with theme settings, user management, and database model overview.

## Features
- 📊 Admin dashboard with dynamic database stats.
- 🎨 User-based theme selection.
- 🔄 Easy integration into existing Django projects.
- 📈 User analytics visualization.

---

## 📦 Installation

1. Install via pip (run this command from your Django project root):
   ```sh
   pip install django-admin-boilerplate
   ```

2. Add to `INSTALLED_APPS` in your Django project:
   ```python
   INSTALLED_APPS = [
       "django_admin_boilerplate",
       "django.contrib.admin",
       "django.contrib.auth",
       ...
   ]
   ```

3. 🔗 Add URLs to `urls.py`
   Modify your project's `urls.py` to include the admin dashboard:
   ```python
   from django.urls import path, include

   urlpatterns = [
       path("", include("django_admin_boilerplate.urls")),
   ]
   ```

---

## 🛠️ Usage

1. Run migrations:
   ```sh
   python manage.py migrate
   ```

2. Create a superuser if needed:
   ```sh
   python manage.py createsuperuser
   ```

3. Install the boilerplate (this moves `django_admin_boilerplate` to your Django root folder for customization):
   ```sh
   python manage.py install_boilerplate
   ```

4. Start the Django server:
   ```sh
   python manage.py runserver
   ```

5. Access the admin dashboard at:
   ```
   http://127.0.0.1:8000/admin-dashboard/
   ```

---

## 🎨 Customization
Once the boilerplate is installed, you are free to customize:
- `views.py` for custom admin logic.
- `templates/` for styling and UI updates.
- `static/` for custom CSS, JavaScript, or images.

---

## 📂 Expected File Structure

```
Your_Django_Project/
├── manage.py
├── sqldb/
├── djangoadminboilerplate/   # Installed boilerplate folder
│   ├── views.py
│   ├── templates/
│   ├── static/
│   ├── urls.py
│   ├── ...
```

---

## 📸 Screenshot (Project Root)
![Screenshot](./screenshot.png)  


---

## 🚀 TODO / Contribution Ideas

1. **Enhance UI:** Improve default admin panel styling and layout.
2. **Add User Roles:** Implement granular user role management for dashboard access.

---

## 📜 License
This project is licensed under the MIT License.

## 🤝 Contributing
Contributions are welcome! Feel free to submit a pull request or open an issue.

## 📧 Contact
For questions or support, reach out via [GitHub Issues](https://github.com/Aremu-damilare/django_admin_boilerplate).

[PYPI homepage](https://pypi.org/project/django-admin-boilerplate/)

