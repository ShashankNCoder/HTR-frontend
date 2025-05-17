# Hathor Wallet Frontend

A modern, responsive full-stack application for the Hathor network, built with React, TypeScript, and Express.

## Features

- Wallet management interface
- Token creation and management
- Rewards system
- User profile management
- Telegram Mini App integration
- Responsive design with mobile-first approach
- Real-time data updates
- Secure authentication

## Tech Stack

### Frontend
- React 18.3
- TypeScript 5.6
- Vite 5.4
- Tailwind CSS 3.4
- Radix UI Components
- Tanstack React Query 5.60
- Wouter 3.3 (for routing)
- Framer Motion 11.13 (for animations)
- Chart.js & Recharts (for data visualization)
- React Hook Form (for form handling)
- Zod (for validation)

### Backend
- Node.js
- Express 4.21
- Drizzle ORM
- NeonDB (PostgreSQL)

## Prerequisites

- Node.js (v20 or higher)
- npm package manager

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ShashankNCoder/hathorconnect.git
cd HTR-frontend
```

2. Install dependencies:
```bash
# Install all dependencies from package.json
npm install
```

## Development

To start the development server:

```bash
npm run dev
```

The application will be available at `http://localhost:3000`

## Docker Deployment

The project includes a multi-stage Dockerfile for optimized production deployment:

1. Build the Docker image:

```bash
docker build -t hathorconnect .
```

2. Run the container:

```bash
docker run -p 3000:3000 hathorconnect
```

## Netlify Deployment

The project can also be deployed to Netlify using the included `netlify.toml` configuration:

1. Push your code to GitHub
2. Connect your GitHub repository to Netlify
3. Netlify will automatically build and deploy your application

## Building for Production

To create a production build:

```bash
npm run build
```

The built files will be in the `dist` directory.

To start the production server:

```bash
npm start
```

## Project Structure

```
HTR-frontend/
├── client/                     # Frontend application
│   ├── src/
│   │   ├── assets/            # Static assets (images, fonts)
│   │   ├── components/        # Reusable UI components
│   │   ├── context/           # React context providers
│   │   ├── hooks/             # Custom React hooks
│   │   ├── lib/               # Utility functions and configurations
│   │   ├── pages/             # Page components
│   │   ├── types/             # TypeScript type definitions
│   │   ├── App.tsx            # Main application component
│   │   ├── main.tsx           # Application entry point
│   │   └── index.css          # Global styles
│   └── index.html             # HTML template
├── server/                     # Backend application
│   ├── services/              # Business logic and services
│   ├── index.ts               # Server entry point
│   ├── vite.ts                # Vite configuration for server
│   ├── storage.ts             # Storage related functionality
│   └── routes.ts              # API route definitions
├── shared/                    # Shared code between client and server
├── node_modules/              # Dependencies
├── package.json               # Project dependencies and scripts
├── package-lock.json          # Locked dependencies
├── tsconfig.json              # TypeScript configuration
├── vite.config.ts             # Vite configuration
├── tailwind.config.ts         # Tailwind CSS configuration
├── postcss.config.js          # PostCSS configuration
├── drizzle.config.ts          # Drizzle ORM configuration
├── components.json            # UI components configuration
├── ngrok.yml                  # Ngrok configuration for tunneling
├── netlify.toml               # Netlify deployment configuration
├── Dockerfile                 # Docker configuration for containerization
├── .dockerignore              # Files to exclude from Docker build
└── README.md                  # Project documentation
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run check` - Run TypeScript type checking
- `npm run db:push` - Push database schema changes using Drizzle Kit

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

