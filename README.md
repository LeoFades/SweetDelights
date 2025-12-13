## SweetDelights Bakery Website

Sweet Delights is a small family-run bakery looking to establish a stronger online presence and streamline how customers place orders. The client wants a website that showcases their baked goods in an attractive way and makes it easier for people to browse what they offer. They also mentioned that they have many different items throughout the year and would like a simple way to show seasonal or limited-time products.

The bakery’s current ordering process happens mostly through social media messages and walk-ins, which they find difficult to manage as order volume grows. They want a system that gathers all orders into one place and makes it easier for staff to handle them. The client hinted that different employees may need access to different parts of the system, but they aren’t entirely sure how that should work yet. They also expressed interest in letting customers customize certain products, such as cakes, though the exact customization options were not fully defined.

Sweet Delights would like customers to have a smooth experience when ordering. They aren’t certain whether customers should create accounts or simply checkout as guests, but they want the process to be convenient and mobile-friendly. They also expressed interest in allowing customers to receive updates about their orders, though they didn’t specify whether this should be through email, SMS, or something else.

Although the client did not provide specifics regarding payments, delivery options, or inventory control, they mentioned concerns about items selling out or not being available on certain days. They also asked whether the system could help prevent customers from ordering more items than the bakery can produce. The bakery occasionally runs promotions and seasonal discounts and would like an easy way to manage these.

Finally, Sweet Delights wants the website to reflect their warm, homey brand identity and to include basic business information such as their story, contact details, opening hours, and physical location. They are also active on social media and would like the website to connect with their existing social platforms. Beyond these requests, the client emphasized that they rely on your expertise to propose features, improvements, and a structure that can support future growth.

Listed out Requirements : https://docs.google.com/document/d/1l5RtDMOsVQj3gBPeIgkRW94fWE9JMLFzZgj9ltMY8uc/edit?usp=sharing


# Instructions for setting up the system 

## PREREQUISITES

- PHP 8.0 or higher

- Composer installed

- Node.js and npm installed

- Database server (MariaDB)

## INSTALLATION STEPS
### Install Laravel
Run the following command to install Laravel in your specified filepath:
```
composer global require laravel/installer
```

### Run Database Migrations
Create the necessary database tables:
```
php artisan migrate
```

If you need to refresh your database and run seeders (**DO NOT RUN IN PRODUCTION**):
```
php artisan migrate:fresh --seed
```

### Generate Encryption Key
Run the following command to generate an encryption key for bcrypt in env:
```
php artisan key:generate
```

### Install JavaScript Dependencies
Install frontend dependencies:
```
composer install
npm install
```

### Build Frontend Assets
Compile your CSS and JavaScript assets:
```
npm run build
```

 Or for continuous building during development:
```
npm run dev
```

### Start the Development Server
Launch the application:
```
php artisan serve
```
Your application should now be running at http://localhost:8000.

## ADDITIONAL NOTES

Configure your database connection in the .env file before running migrations
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

For production, change the env file from development to production
```
APP_ENV=production
```   


### <u>Developer's Note</u>
This is a practice because we have nothing better to do and we hate ourselves. Also this practice is given by ai since i asked it to become our client.
We also try to use no ai to help with coding, going back to the old documentation stackoverflow era, err see how far we can go la.

@LeoFades what libraries are we using and wtf are we doing here
