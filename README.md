# Laravel Template

Full-stack PHP application with Laravel 12, Inertia.js, and React.

## Stack

- **PHP 8.3** with Laravel 12
- **Inertia.js** for server-driven SPA
- **React 19** with TypeScript
- **Tailwind CSS** for styling
- **PostgreSQL** database
- **Laravel Sail** for Docker development

## Getting Started

```bash
# Install dependencies
composer install
npm install

# Copy environment file
cp .env.example .env

# Generate application key
php artisan key:generate

# Start development server (with Sail)
./vendor/bin/sail up -d

# Run migrations
./vendor/bin/sail artisan migrate

# Build frontend assets
npm run dev
```

## Development

```bash
# Run tests
php artisan test

# Run linting
./vendor/bin/pint

# Build for production
npm run build
```

## Project Structure

```
├── app/                 # Application code
│   ├── Http/           # Controllers, middleware
│   └── Models/         # Eloquent models
├── resources/
│   └── js/             # React components
├── routes/             # Route definitions
├── database/           # Migrations, seeders
└── tests/              # Test suite
```
