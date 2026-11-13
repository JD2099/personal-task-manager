# TaskMate – Personal Task Manager

## Project Title & Description

TaskMate is a web application designed to help students and individuals organize, manage, and track their daily activities. Users can create personal tasks, assign categories, update task information, and monitor their progress through a centralized dashboard.

The initial release focuses on essential task management features, including user authentication, task creation and management, task categorization, status tracking, and a dashboard displaying task statistics.

## Purpose & Target Audience

- **Audience:** Students and individuals who need a simple tool to organize their daily responsibilities.
- **Purpose:** Help users improve productivity by providing a centralized platform to create, organize, and track personal tasks.

## User Stories

1. As a new user, I want to create an account so that I can access my personal task manager.
2. As a registered user, I want to log in so that I can securely access my tasks.
3. As a user, I want to create tasks with a title, description, and category so that I can organize my activities.
4. As a user, I want to view all my tasks so that I can keep track of my responsibilities.
5. As a user, I want to edit or delete my tasks so that I can keep my task list updated.
6. As a user, I want to change a task's status between Pending and Completed so that I can track my progress.
7. As a user, I want to organize tasks into categories such as School, Work, and Personal so that I can separate my activities.
8. As a user, I want to view a dashboard with total, pending, and completed tasks so that I can monitor my productivity.
9. As a user, I want to manage my profile so that I can update my personal account information.

## Acceptance Criteria

### Story 1: Create an account
- Given a new user, when they submit valid registration information, then the system creates their account.
- Given an email address that is already registered, when the user attempts to sign up, then the system displays an appropriate error message.
- Given missing or invalid information, when the form is submitted, then the system displays validation messages.

### Story 2: Log in
- Given a registered user, when they enter valid credentials, then the system authenticates them and redirects them to the dashboard.
- Given invalid credentials, when the user attempts to log in, then the system displays an error message.

### Story 3: Create a task
- Given an authenticated user, when they submit a task with a title and category, then the system saves the task.
- Given missing required information, when the user submits the form, then the system prevents task creation and displays validation messages.
- Given a successfully created task, then it appears in the user's task list.

### Story 4: View tasks
- Given an authenticated user, when they open the tasks page, then the system displays their personal tasks.
- Given a user with no tasks, when they open the tasks page, then the system displays an appropriate empty-state message.
- Users must only be able to view their own tasks.

### Story 5: Edit or delete a task
- Given an existing task, when the user updates its information, then the system saves the changes.
- Given an existing task, when the user confirms deletion, then the system removes the task.
- Users cannot edit or delete tasks belonging to other users.

### Story 6: Update task status
- Given a pending task, when the user marks it as completed, then its status changes to Completed.
- Given a completed task, when the user marks it as pending, then its status changes to Pending.
- The dashboard statistics must reflect the updated status.

### Story 7: Organize tasks by category
- Given an authenticated user, when they create or edit a task, then they can assign it to a category such as School, Work, or Personal.
- Given multiple tasks, when the user views their task list, then each task displays its assigned category.

### Story 8: View dashboard statistics
- Given an authenticated user, when they open the dashboard, then the system displays the total number of tasks.
- The dashboard displays the number of pending and completed tasks.
- The statistics are updated when tasks are created, deleted, or their status changes.

### Story 9: Manage user profile
- Given an authenticated user, when they open their profile, then the system displays their account information.
- Given valid updated information, when the user saves their changes, then the system updates their profile.

## Technical Requirements

- **Framework:** Next.js with App Router.
- **Language:** TypeScript.
- **Styling:** Tailwind CSS.
- **Database:** PostgreSQL.
- **ORM:** Prisma.
- **Authentication:** NextAuth/Auth.js or Clerk.
- **Architecture:** Component-based architecture with reusable UI components.
- **Security:** Users must only access and modify their own tasks.
- **Validation:** Validate user input on both the client and server sides.
- **Performance:** Use server components by default and client components when interactivity is required.

## Core API Endpoints

- POST /api/auth/register
- POST /api/auth/login
- GET /api/tasks
- GET /api/tasks/:id
- POST /api/tasks
- PUT /api/tasks/:id
- DELETE /api/tasks/:id
- PATCH /api/tasks/:id/status
- GET /api/dashboard
- GET /api/profile
- PUT /api/profile

## Implementation Priority

- **P0 – Essential Features:**
  - User registration and login.
  - Create, view, edit, and delete tasks.
  - Update task status.
  - Organize tasks by category.
  - Dashboard with task statistics.

- **P1 – Important Features:**
  - User profile management.
  - Task filtering by category and status.
  - Improved form validation and error handling.

- **P2 – Future Improvements:**
  - Task due dates and reminders.
  - Task search functionality.
  - Task priority levels.
  - Calendar integration.
