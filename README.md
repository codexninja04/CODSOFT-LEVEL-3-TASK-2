# ProjectHub - Project Management Tool

A full-featured project management application built with React, TypeScript, and Supabase (PostgreSQL). Track projects, manage tasks, set deadlines, and monitor progress with an intuitive interface.

## Features

- **User Authentication**: Secure email/password authentication with Supabase Auth
- **Project Management**: Create, edit, and delete projects with different status levels
- **Task Management**: Organize tasks with priorities, deadlines, and status tracking
- **Progress Tracking**: Visual progress charts and completion rates
- **Dashboard**: Overview of all projects and tasks with key statistics
- **Responsive Design**: Works seamlessly on desktop and mobile devices

## Tech Stack

- **Frontend**: React 18, TypeScript, Tailwind CSS
- **Backend**: Supabase (PostgreSQL + Auth)
- **Icons**: Lucide React
- **Build Tool**: Vite

## Setup Instructions

### 1. Install Dependencies

```bash
npm install
```

### 2. Configure Supabase

1. Create a Supabase account at [supabase.com](https://supabase.com)
2. Create a new project
3. Get your project URL and anon key from Project Settings > API
4. Create a `.env` file in the root directory:

```env
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

### 3. Database Setup

The database schema has been created with the following tables:

- **profiles**: User profile information
- **projects**: Project data with status tracking
- **tasks**: Task management with priorities and deadlines

All tables have Row Level Security (RLS) enabled for data protection.

### 4. Run the Application

```bash
npm run dev
```

The application will be available at `http://localhost:5173`

### 5. Build for Production

```bash
npm run build
```

## Usage

1. **Sign Up**: Create a new account with email and password
2. **Create Projects**: Add new projects with descriptions, dates, and status
3. **Add Tasks**: Create tasks within projects with priorities and deadlines
4. **Track Progress**: Monitor completion rates and project status in the dashboard
5. **Manage Workflow**: Move tasks between To Do, In Progress, and Completed

## Features Breakdown

### Dashboard
- Total project count
- Active projects tracking
- Task completion statistics
- Overall progress visualization

### Projects
- Create/edit/delete projects
- Status management (Planning, Active, Completed, On Hold)
- Deadline tracking
- Task completion overview per project

### Tasks
- Create/edit/delete tasks
- Priority levels (Low, Medium, High)
- Status tracking (To Do, In Progress, Completed)
- Deadline management
- Overdue task alerts
- Filter by status and project

## Security

- Row Level Security (RLS) policies ensure users can only access their own data
- Secure authentication with Supabase Auth
- Protected API routes

## Deployment

This application can be deployed to any static hosting provider:

- Vercel
- Netlify
- GitHub Pages
- 000webhost
- Heroku

Make sure to set the environment variables in your hosting provider's settings.
