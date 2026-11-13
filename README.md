# TaskMate – Personal Task Manager

## About the Project

TaskMate is a web application designed to help students and individuals organize, manage, and track their daily activities.

The platform provides a simple and centralized way to create personal tasks, organize them into categories, update their status, and monitor productivity through a dashboard.

TaskMate aims to improve productivity by helping users keep track of their responsibilities and stay organized.

## Main Features

- **User Authentication:** Create an account and securely log in.
- **Dashboard:** View a summary of total, pending, and completed tasks.
- **Task Management:** Create, view, edit, and delete personal tasks.
- **Task Status:** Mark tasks as Pending or Completed.
- **Task Categories:** Organize tasks into School, Work, and Personal categories.
- **User Profile:** View and manage personal account information.
- **Task Filtering:** Filter tasks by category and status.

## Target Audience

TaskMate is designed for:
- Students who need to organize academic activities and assignments.
- Individuals who want to manage their daily responsibilities.
- Anyone looking for a simple and centralized task management tool.

## Technologies Used

The project is planned to use the following technologies:

- **Framework:** Next.js (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **Database:** PostgreSQL
- **ORM:** Prisma
- **Authentication:** Auth.js (NextAuth) or Clerk (final selection pending)

## Project Structure

The application will follow a component-based architecture using Next.js App Router.

```text
TaskMate/
├── app/
│   ├── dashboard/
│   ├── tasks/
│   ├── profile/
│   ├── login/
│   └── register/
├── components/
│   ├── ui/
│   ├── dashboard/
│   └── tasks/
├── lib/
├── prisma/
├── public/
├── specification.md
├── package.json
└── README.md
```

## Getting Started

### Prerequisites

Before running the project, make sure you have installed:

- Node.js
- npm
- PostgreSQL
- Git

### Installation

1. Clone the repository:

```bash
git clone <repository-url>
```

2. Navigate to the project directory:

```bash
cd TaskMate
```

3. Install dependencies:

```bash
npm install
```

4. Configure your environment variables in a `.env` file:

```env
DATABASE_URL="your_postgresql_connection_string"
```

5. Generate the Prisma client:

```bash
npx prisma generate
```

6. Run database migrations:

```bash
npx prisma migrate dev
```

7. Start the development server:

```bash
npm run dev
```

8. Open your browser and navigate to:

```text
http://localhost:3000
```

*Note: These instructions describe the planned development setup and will apply once the corresponding application structure and configuration have been implemented.*

## Project Documentation

For more information about the project requirements, user stories, acceptance criteria, technical requirements, and implementation priorities, see:

- [TaskMate Specification Document](./specification.md)

## Project Management

The development process is organized using GitHub Projects.

The team uses GitHub Issues to:
- Track development tasks.
- Assign responsibilities to team members.
- Define acceptance criteria.
- Monitor development progress.

## Future Improvements

Potential future features include:

- Task due dates and reminders.
- Task priority levels.
- Advanced task search.
- Calendar integration.

## Team Members

- [Team Member 1]
- [Team Member 2]
- [Team Member 3]

## Project Status

**Status:** In Development

TaskMate is currently in the planning and initial development stage.