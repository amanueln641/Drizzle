# Drizzel

A TypeScript-based Node.js application using Drizzle ORM with PostgreSQL for user management.

## Features

- User management with CRUD operations
- PostgreSQL database with Drizzle ORM
- Docker Compose setup for easy database deployment
- TypeScript with strict type checking
- Database migrations support
- Drizzle Studio for database visualization

## Tech Stack

- **Runtime**: Node.js with TypeScript
- **ORM**: Drizzle ORM
- **Database**: PostgreSQL
- **Package Manager**: npm

## Prerequisites

- Node.js (v18 or higher)
- Docker and Docker Compose (for database)
- npm or pnpm

## Installation

1. Clone the repository:

```bash
git clone git@github.com:ParvejAliDev/Drizzle.git
cd Drizzel
```

2. Install dependencies:

```bash
npm install
# or
pnpm install
```

3. Set up environment variables:
Copy `.env.example` to `.env` and update the values if needed:

4. Start the PostgreSQL database using Docker Compose:

```bash
docker-compose up -d
```

5. Run database migrations:

```bash
npm run db:migrate
```

## Usage

### Development

Start the development server:

```bash
npm run dev
```

### Database Operations

Generate a new migration:

```bash
npm run db:generate <migration-name>
```

Run migrations:

```bash
npm run db:migrate
```

Open Drizzle Studio (database GUI):

```bash
npm run db:studio
```

### Code Formatting

Format code:

```bash
npm run format
```

Check code formatting:

```bash
npm run format:check
```

## Database Schema

### Users Table

- `id` (UUID, primary key)
- `name` (VARCHAR)
- `email` (VARCHAR, unique)
- `password` (VARCHAR)
- `createdAt` (TIMESTAMP)
- `updatedAt` (TIMESTAMP)

### Projects Table

- `id` (UUID, primary key)
- `name` (VARCHAR)
- `description` (VARCHAR, optional)
- `userId` (UUID, foreign key to users)
- `createdAt` (TIMESTAMP)
- `updatedAt` (TIMESTAMP)

> **Note**: The projects table schema exists in the database, but project CRUD operations are not yet implemented.

## Available Scripts

- `npm run dev` - Start development server with hot reload
- `npm run dev:with-studio` - Start dev server and Drizzle Studio (Windows only, uses `start` command)
- `npm run db:generate` - Generate a new database migration
- `npm run db:migrate` - Run database migrations
- `npm run db:studio` - Open Drizzle Studio
- `npm run format` - Format code with Prettier
- `npm run format:check` - Check code formatting

## Docker Database Setup

The project includes a Docker Compose configuration for PostgreSQL:

To start the database:

```bash
docker-compose up -d
```

To stop the database:

```bash
docker-compose down
```

## License

ISC

## Author

Parvej Ali
