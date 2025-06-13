# Svelte Satoria

A comprehensive SvelteKit-based industrial monitoring and configuration application with real-time capabilities for device management and alarm systems.

![Satoria Logo](src/assets/logo2.png)

## Overview

Svelte Satoria is a modern web application built for configuring and monitoring industrial devices, with a focus on temperature and pressure alarms. It features a responsive UI, real-time notifications, and comprehensive configuration options.

## Features

- **Modular Configuration**: Customize temperature and pressure alarm thresholds
- **Real-time Monitoring**: Live device status and alert notifications
- **User Authentication**: Secure access control with account management
- **Responsive UI**: Adapts to different screen sizes and devices
- **Database Integration**: Persistent storage with Postgres and Drizzle ORM
- **Docker Support**: Containerized development environment

## Technology Stack

### Core Framework
- **SvelteKit**: ^2.16.0
- **Svelte**: ^5.0.0 (Using the new Runes API)
- **TypeScript**: ^5.0.0
- **Vite**: ^6.2.6

### UI Components
- **TailwindCSS**: ^4.0.0
- **Shadcn UI**: Custom Svelte implementation
- **Lucide Icons**: ^0.514.0
- **Bits UI**: ^2.5.0
- **ECharts**: ^5.6.0 (For data visualization)
- **Svelte Sonner**: ^1.0.3 (Toast notifications)

### Backend and Data
- **Drizzle ORM**: ^0.40.0
- **Postgres**: ^3.4.5
- **Redis**: For caching and real-time features
- **Zod**: ^3.25.13 (Schema validation)
- **Superforms**: ^2.25.0 (Form handling)

### Development Tools
- **ESLint**: ^9.18.0
- **Prettier**: ^3.4.2
- **Docker/Docker Compose**: For development environment

## Getting Started

### Prerequisites
- Node.js (v18+)
- Docker and Docker Compose
- PostgreSQL
- Redis

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/svelte-satoria.git
   cd svelte-satoria
   ```

2. Install dependencies:
   ```sh
   npm install
   # or
   bun install
   ```

3. Start the database:
   ```sh
   npm run db:start
   ```

4. Run database migrations:
   ```sh
   npm run db:migrate
   ```

5. Start the development server:
   ```sh
   npm run dev
   ```

6. Access the application at `http://localhost:5173`

## Project Structure

```
svelte-satoria/
├── src/                   # Source code
│   ├── assets/            # Static assets
│   ├── components/        # UI components
│   │   ├── app-sidebar.svelte
│   │   ├── app-topbar.svelte
│   │   ├── account-app/   # Account management components
│   │   ├── configuration/ # Configuration components
│   │   └── ...
│   ├── lib/               # Utilities and shared logic
│   │   ├── server/        # Server-side utilities
│   │   ├── sidebar/       # Sidebar configuration
│   │   └── utils/         # Helper functions
│   ├── routes/            # SvelteKit routes
│   │   ├── (app)/         # Main application routes
│   │   ├── (login)/       # Authentication routes
│   │   └── (print)/       # Printable views
│   ├── shadcn/            # Shadcn UI components
│   └── app.css            # Global styles
├── drizzle/               # Database migrations
├── redis/                 # Redis configuration
├── static/                # Static files
├── drizzle.config.ts      # Drizzle ORM configuration
├── svelte.config.js       # SvelteKit configuration
├── tailwind.config.js     # TailwindCSS configuration
├── docker-compose.yml     # Docker services configuration
└── package.json           # Dependencies and scripts
```

## Database Management

The application uses Drizzle ORM with PostgreSQL. Manage your database with these commands:

```sh
# Start the database
npm run db:start

# Apply schema changes
npm run db:push

# Generate and run migrations
npm run db:migrate

# Open Drizzle Studio to manage data
npm run db:studio
```

## Configuration Options

### Temperature and Pressure Alarms

The application allows setting up thresholds for temperature and pressure values:

- **Low Threshold**: Triggers an alarm when values fall below this point
- **High Threshold**: Triggers an alarm when values exceed this point
- **Custom Messages**: Configurable notification messages with dynamic value placeholders

## Deployment

### Production Build

```sh
npm run build
```

The application uses the SvelteKit Node adapter and can be deployed to any Node.js hosting environment.

### Docker Deployment

A production Dockerfile is available for containerized deployment.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- [SvelteKit](https://kit.svelte.dev/)
- [Shadcn UI](https://ui.shadcn.com/)
- [TailwindCSS](https://tailwindcss.com/)
- [Drizzle ORM](https://orm.drizzle.team/)

## Release Information

This repository contains only the compiled version of the monitoring system. It is updated automatically via GitHub Actions.

Last updated: Fri Jun 13 08:55:30 UTC 2025
