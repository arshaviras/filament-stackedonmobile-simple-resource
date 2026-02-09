## Filament stackedOnMobile() Simple Resource Issue

This repository reproduces an issue where wrapped `TextColumn` text becomes
center-aligned when using `stackedOnMobile()` in a Simple (modal) resource.

### Steps
Clone the repository with `git clone`
Copy the `.env.example` file to `.env` and edit database credentials there
Run `composer install`
Run `php artisan key:generate`
Run `php artisan migrate --seed` (it has some seeded data for your testing)
Create Filament user with `php artisan make:filament-user` command
That's it: launch the URL /admin and log in with credentials
Open Item resource

### Expected
Text remains left-aligned.

### Actual
Text is center-aligned.
