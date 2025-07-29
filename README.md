# Little Lemon Restaurant

Little Lemon is a Django-based web application for managing a restaurant's menu, bookings, and online presence. It provides a user-friendly interface for customers to view menu items, book tables, and learn more about the restaurant.

## Features
- **Menu Management:** View detailed menu items with images and descriptions.
- **Booking System:** Customers can book tables online.
- **About & Info Pages:** Learn about the restaurant, chefs, and history.
- **Static Assets:** Includes images, CSS, and icons for a modern look.

## Project Structure
- `littlelemon/` - Django project configuration (settings, URLs, WSGI/ASGI).
- `restaurant/` - Main app for restaurant logic (models, views, forms, admin, URLs).
- `restaurant/static/` - Static files (CSS, images).
- `restaurant/templates/` - HTML templates for all pages.
- `restaurant/migrations/` - Database migrations.
- `db.sqlite3` - Default SQLite database.
- `manage.py` - Django management script.

## Configuration
- **Settings:** Edit `littlelemon/settings.py` for database, static files, and app configuration.
- **URLs:** Main routing in `littlelemon/urls.py` and app-specific routes in `restaurant/urls.py`.
- **Static Files:** Configure static and media paths in `settings.py` if needed.

## Getting Started
1. **Install dependencies:**
   - Python 3.8+
   - Django (see requirements.txt if available)
2. **Run migrations:**
   ```powershell
   python manage.py migrate
   ```
3. **Start the server:**
   ```powershell
   python manage.py runserver
   ```
4. **Access the site:**
   Open `http://127.0.0.1:8000/` in your browser.

## Customization
- **Menu Items:** Add/edit menu items in the Django admin or via models in `restaurant/models.py`.
- **Bookings:** Booking logic is handled in `restaurant/views.py` and `restaurant/forms.py`.
- **Templates:** Customize HTML in `restaurant/templates/`.
- **Static Files:** Add images/CSS in `restaurant/static/`.

## Admin Access
- Create a superuser to access the Django admin:
  ```powershell
  python manage.py createsuperuser
  ```

## Additional Notes
- For production, update `ALLOWED_HOSTS` and static/media settings in `settings.py`.
- Use environment variables for sensitive data.
- For more apps or features, add new Django apps and update settings/URLs accordingly.

## License
This project is for educational/demo purposes. Please update the license as needed.
