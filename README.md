# PT. Satoria Aneka Pharma Monitoring System

## Overview

This project is a modern web application for monitoring systems at PT. Satoria Aneka Pharma. It is built using SvelteKit 2, Svelte 5, and Tailwind CSS, with a focus on providing a responsive, accessible, and user-friendly interface for monitoring various aspects of pharmaceutical production.

## Tech Stack

- **Frontend Framework:** Svelte 5.0.0 with SvelteKit 2.16.0
- **Build Tool:** Vite 6.2.6
- **Styling:** Tailwind CSS 4.0.0
- **Language:** TypeScript 5.0.0
- **Deployment:** Node.js (via @sveltejs/adapter-node)

## Key Features

- Modern UI components via shadcn/ui and bits-ui
- Responsive design that works across all device sizes
- Dark/light mode theming
- Authentication via JWT
- Form handling with validation (via sveltekit-superforms and zod)
- Custom OKLCH color system for improved color accessibility

## Project Structure

The application follows the SvelteKit conventional structure:

- `/src/routes` - Application routes and pages
- `/src/lib` - Shared components, utilities, and types
- `/src/shadcn/components` - UI components built with Tailwind CSS
- `/src/assets` - Static assets like images and fonts
- `/static` - Files served directly by the server

## Installation

```bash
# Clone the repository (requires permission)
git clone [repository-url]

# Navigate to project directory
cd svelte-satoria

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Dependencies and Plugins

### Core Dependencies

| Package                | Version | Purpose                              |
| ---------------------- | ------- | ------------------------------------ |
| svelte                 | 5.0.0   | Core UI framework                    |
| @sveltejs/kit          | 2.16.0  | Full-stack framework built on Svelte |
| @sveltejs/adapter-node | 5.2.12  | Adapter for Node.js deployment       |
| typescript             | 5.0.0   | Type safety and developer tooling    |

### UI and Styling

| Package            | Version | Purpose                                    |
| ------------------ | ------- | ------------------------------------------ |
| tailwindcss        | 4.0.0   | Utility-first CSS framework                |
| @tailwindcss/forms | 0.5.9   | Form styling for Tailwind                  |
| @tailwindcss/vite  | 4.0.0   | Tailwind integration for Vite              |
| bits-ui            | 1.5.3   | Accessible UI primitives                   |
| clsx               | 2.1.1   | Utility for constructing className strings |
| tailwind-merge     | 3.3.0   | Merges Tailwind CSS classes                |
| tailwind-variants  | 0.2.1   | Creates variants of Tailwind styles        |
| tw-animate-css     | 1.3.0   | Animation utilities for Tailwind CSS       |
| @lucide/svelte     | 0.482.0 | Icon library for Svelte                    |

### Development Tools

| Package                     | Version | Purpose                                |
| --------------------------- | ------- | -------------------------------------- |
| vite                        | 6.2.6   | Fast development server and build tool |
| eslint                      | 9.18.0  | Code linting                           |
| prettier                    | 3.4.2   | Code formatting                        |
| svelte-check                | 4.0.0   | Static analysis for Svelte components  |
| @eslint/js                  | 9.18.0  | ESLint JavaScript configuration        |
| @eslint/compat              | 1.2.5   | Compatibility helpers for ESLint       |
| eslint-config-prettier      | 10.0.1  | Integrates Prettier with ESLint        |
| eslint-plugin-svelte        | 3.0.0   | ESLint rules for Svelte                |
| prettier-plugin-svelte      | 3.3.3   | Prettier support for Svelte            |
| prettier-plugin-tailwindcss | 0.6.11  | Auto-sorts Tailwind classes            |
| typescript-eslint           | 8.20.0  | TypeScript support for ESLint          |

### Utility Libraries

| Package              | Version | Purpose                                      |
| -------------------- | ------- | -------------------------------------------- |
| @oslojs/jwt          | 0.3.0   | JWT handling for authentication              |
| zod                  | 3.25.13 | TypeScript-first schema validation           |
| sveltekit-superforms | 2.25.0  | Form handling for SvelteKit                  |
| globals              | 16.0.0  | Global variables for JavaScript environments |

### IDE Support

| Package                      | Version | Purpose                      |
| ---------------------------- | ------- | ---------------------------- |
| @tailwindcss/language-server | 0.14.17 | IDE support for Tailwind CSS |
| svelte-language-server       | 0.17.14 | Language server for Svelte   |
| typescript-svelte-plugin     | 0.3.47  | TypeScript plugin for Svelte |

## Theming

The application uses a custom theme system built with OKLCH color space for improved perceptual uniformity. The theme supports both light and dark modes with the following key design tokens:

- **Colors:** Primary, secondary, muted, accent, and destructive colors
- **UI Elements:** Background, foreground, card, popover, border, and input styles
- **Sidebar:** Custom styling for the application sidebar
- **Radius:** Consistent border radius throughout the application

## Layout System

The application uses a responsive layout system with:

- A main application layout with sidebar navigation
- A separate authentication layout for login/registration pages
- Responsive design that adapts to different screen sizes

## Scripts

| Command           | Description               |
| ----------------- | ------------------------- |
| `npm run dev`     | Start development server  |
| `npm run build`   | Build for production      |
| `npm run preview` | Preview production build  |
| `npm run check`   | Run type checking         |
| `npm run format`  | Format code with Prettier |
| `npm run lint`    | Lint code with ESLint     |

## Contributing

This is a proprietary project for PT. Satoria Aneka Pharma. All contributions must be approved by the repository owner. Please refer to the LICENSE.md file for usage restrictions.

## License

This project is licensed under a proprietary license. See the [LICENSE.md](./LICENSE.md) file for details.

## Contact

For any inquiries regarding this project, please contact PT. Satoria Aneka Pharma.
This documentation provides a comprehensive overview of your project, including the tech stack, dependencies, project structure, and usage instructions. It's organized in a clear and professional manner that will help both new developers understand the project and serve as a reference for existing team members.

The document covers all the plugins and libraries used in your project as shown in the package.json file, along with explanations of their purpose. It also includes information about the theming system as shown in your app.css file and the layout structure based on your +layout.svelte files.

You can save this as `README.md` in the root of your repository to provide immediate documentation for anyone accessing the project.

## Release Information

This repository contains only the compiled version of the monitoring system. It is updated automatically via GitHub Actions.

Last updated: Sat May 24 04:01:13 UTC 2025
