# Blog Livewire Kit

A blog web application built on Laravel 12 with Livewire, Tailwind CSS, and Vite. This starter kit includes a public blog experience, user profiles, admin dashboard, role-based access control, post management, comments, feedback handling, and more.

## Features

- Public blog pages: home, about, contact, posts listing, post details, tags, and author pages
- User authentication: register, login, password reset, email verification, and secure account settings
- Livewire-powered UI for reactive page updates without full page reloads
- Admin dashboard with authenticated access and ACL middleware
- Post management: create, edit, publish, trash, restore, and filter posts
- Comment system with moderation and user activity tracking
- Tag management for posts, including admin CRUD
- Feedback collection and admin review
- User center for managing own posts, comments, activity, and profile settings
- Role and permission management with author request workflow
- Appearance settings and profile configuration for users and admins
- Support for likes/dislikes and tracking user actions

## Technologies

- PHP 8.2+
- Laravel 12
- Livewire Flux + Volt
- Tailwind CSS 4
- Vite
- Laravel Sail for Docker development
- Font Awesome for icons
- Laravel Debugbar for local debugging

## Installation

### Docker and Sail

1. Clone or download the repository
2. Go to the project directory and run `composer install`
3. Copy `.env.example` to `.env`: `cp .env.example .env`
4. Update database credentials and other environment settings in `.env`
5. Start Sail: `sail up -d`
6. Run database migrations and seeders: `sail artisan migrate --seed`
7. Generate application key: `sail artisan key:generate`
8. Create storage symlink: `sail artisan storage:link`
9. Install frontend dependencies: `sail npm install`
10. Start Vite: `sail npm run dev`
11. Open the app in your browser at `http://localhost:8080`

### Local development without Sail

1. Install PHP, Composer, Node.js, and npm on your machine
2. Run `composer install`
3. Run `npm install`
4. Copy `.env.example` to `.env` and configure database settings
5. Run `php artisan key:generate`
6. Run `php artisan migrate --seed`
7. Run `php artisan storage:link`
8. Start the app: `php artisan serve`
9. Start Vite: `npm run dev`

## Useful commands

- `sail artisan migrate`
- `sail artisan db:seed`
- `sail artisan test`
- `sail npm run dev`
- `composer test`
- `npm run build`

## License

[MIT license](https://opensource.org/licenses/MIT)
