# PHP User Management System

A simple PHP-based User Management System with admin panel and MySQL database.

## Features

- User registration with name and email
- Admin panel with authentication
- CRUD operations for user management
- Form validation and security measures
- Clean and responsive UI

## Requirements

- PHP 8.0 or higher
- MySQL/MariaDB
- Node.js and npm (optional, for development server)

## Installation

1. Clone the repository:
```bash
git clone [your-repository-url]
cd [repository-name]
```

2. Import the database schema:
```bash
mysql -u root -p < database.sql
```

3. Configure the database connection:
Edit `config/db_config.php` and update the following constants:
```php
define('DB_SERVER', 'localhost');
define('DB_USERNAME', 'your_username');
define('DB_PASSWORD', 'your_password');
define('DB_NAME', 'user_management');
```

4. Start the development server:
```bash
php -S localhost:8000
```
Or using npm:
```bash
npm install
npm start
```

5. Access the application:
- Main page: http://localhost:8000
- Admin panel: http://localhost:8000/admin/login.php

## Admin Credentials

- Username: admin
- Password: admin123

## Security Features

- Password-protected admin panel
- SQL injection prevention using prepared statements
- XSS prevention using htmlspecialchars()
- Session management for admin authentication
- Input validation and sanitization

## License

ISC
