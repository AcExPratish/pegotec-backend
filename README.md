Prerequisites
PHP: Ensure PHP (>= 7.4) is installed on your machine.
Composer: A dependency manager for PHP. Install it from getcomposer.org.
Database: MySQL. Ensure it is installed and accessible.


1. Clone the Repository
Start by cloning the Laravel project repository from your version control system (e.g., GitHub).

git clone https://github.com/AcExPratish/pegotec-backend.git
cd pegotec-backend

2. Install PHP Dependencies
Run Composer to install PHP dependencies defined in composer.json.
composer install

3. Set Up Environment Configuration

3.1. Copy .env.example to .env
The .env file contains environment-specific configurations for your Laravel application. Copy the example file provided.

cp .env.example .env

3.2. Configure .env File
Edit the .env file to configure your environment settings such as database credentials and application key.

APP_NAME=Laravel
APP_ENV=local
APP_KEY=base64:YOUR_APP_KEY
APP_DEBUG=true
APP_URL=http://localhost

LOG_CHANNEL=stack

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_database_username
DB_PASSWORD=your_database_password

4. Migrate the Database
Run migrations to create the necessary tables in your database. Ensure your database is correctly set up and configured in the .env file.

php artisan migrate

5. Start the Development Server
Start the Laravel development server to run your application locally.

php artisan serve