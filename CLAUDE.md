# Laravel Project

This is a Laravel 12 application with Inertia.js and React.

## Commands

- `php artisan test` - Run tests
- `php artisan serve` - Start dev server
- `./vendor/bin/pint` - Format PHP code
- `npm run dev` - Build frontend with hot reload
- `npm run build` - Build frontend for production

## Architecture

- **Controllers** in `app/Http/Controllers/` handle requests and return Inertia responses
- **Models** in `app/Models/` are Eloquent models with relationships
- **React components** in `resources/js/Pages/` are rendered by Inertia
- **Routes** in `routes/web.php` for web routes, `routes/api.php` for API

## Conventions

- Use form requests for validation (`php artisan make:request`)
- Use resources for API responses (`php artisan make:resource`)
- Follow PSR-12 coding style (enforced by Pint)
- Use TypeScript for all React components
- Prefer server-side rendering via Inertia over client-side API calls

## Database

- PostgreSQL via Laravel Sail
- Migrations in `database/migrations/`
- Run `php artisan migrate` to apply migrations
- Run `php artisan migrate:fresh --seed` to reset with seeders
