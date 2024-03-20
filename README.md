# Birddit - A Reddit Clone

Built with the Next.js App Router, TypeScript, Tailwind, Zod, NextAuth

## Features

- Infinite scrolling for dynamically loading posts using React-Query
- Authentication using Google OAuth
- Custom feed for authenticated users based on their subscriptions
- Advanced caching using [Upstash Redis](https://upstash.com/?utm_source=Josh2) for the most popular posts
- Optimistic updates for a great user experience for post and comment voting using React-Query
- Modern data fetching using React-Query
- A beautiful and highly functional post editor
- Image uploads & link previews using [UploadThing](https://uploadthing.com/)
- Full comment functionality with nested replies
- Prisma ORM for a type-safe database layer
- Zod for type-safe validation

## Getting started

### Prerequisites

- Node.js 18.17 or later
- pnpm (optional, but recommended) or another package manager
- A database compatible with Prisma (PostgreSQL, MySQL, SQLite, SQL Server, or a cloud database)
- An Upstash Redis instance for caching
- A Google OAuth client ID and secret
- An UploadThing app ID and secret

### Installation

#### Step 1: Git Clone

In your terminal, run the following command.

```bash
git clone git@github.com:dragos-cojocaru/birddit.git
```

#### Step 2: Place yourself at the root of the project

```bash
cd birddit
```

#### Step 3: Setup environment variables

Birddit requires you to set some environment variables. Locally, you should set them through a `.env` file.

To do so, make a copy of the `.env.example` file and rename it to `.env`:

```bash
cp .env.example .env
```

Then, open the `.env` file and fill in the required values for the database, Google OAuth, UploadThing, and Upstash Redis.

### Step 4: Install dependencies

```bash
pnpm install
```

### Step 5: Run the development server

```bash
pnpm dev
```

Birddit should now be running on [http://localhost:3000](http://localhost:3000).

## Acknowledgements

- [breadit](https://github.com/joschan21/breadit) by [Joscha Neske](https://github.com/joschan21) for many of the ideas and inspiration for this project
