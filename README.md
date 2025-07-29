# Posts Forum

A simple full-stack web application where users can create and view posts in a forum-style format. Built with Next.js, React 19, and SQLite.

## Tech Stack

- **Next.js 15**
- **React 19**
- **SQLite (via better-sqlite3)**
- **Cloudinary** (for storing images)
- **CSS Modules**

## Features

- View a list of posts on the homepage
- Create new posts with optional image upload
- Images are stored on Cloudinary
- All data is stored and queried from a local SQLite database
- Server-side rendering and routing via Next.js App Router

## Environment Variables

To use the app with Cloudinary, create a `.env.local` file in the root of your project with the following variables:

```
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18+ recommended)
- SQLite3 (installed on your system)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/plinadev/posts-forum.git
   cd posts-forum
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Add your `.env.local` file with the required Cloudinary credentials

4. Run the development server:

   ```bash
   npm run dev
   ```

5. Visit [http://localhost:3000](http://localhost:3000) to use the app

## Project Structure

```
/posts-forum
├── app/              # Next.js routes and pages (home, post details, new post form)
├── lib/              # SQLite query functions and Cloudinary integration
├── public/           # Static files
├── styles/           # CSS Modules for styling
├── database/         # SQLite database file
├── .env.local        # Environment variables for Cloudinary
├── package.json
└── README.md
```
