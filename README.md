# Offesy

**AI-Powered Project Management SaaS**

Offesy is a modern project management platform built to help teams collaborate, organize work, and manage projects efficiently. It enables users to create workspaces, invite members, organize teams, manage projects, track issues, and collaborate in real time with AI-powered assistance.

---

# Features

### Authentication

* Secure authentication with Clerk
* Sign up and sign in
* Session management
* Protected routes

### Workspaces

* Create multiple workspaces
* Workspace owner becomes the Admin
* Invite members via email
* Manage workspace settings
* Role-based access (Admin & Member)

### Teams

* Create multiple teams inside a workspace
* Add workspace members to teams
* Manage team members
* Team-based collaboration

### Projects

* Create and manage projects
* Edit project details
* Organize project information
* Track project progress
* Dedicated comment section

### Issues

* Create issues inside projects
* Set priority and status
* Assign labels
* Update issue details
* Dedicated discussion thread

### Comments

* Real-time comments
* Threaded discussions
* Collaboration on projects
* Collaboration on issues

### Notifications

* Real-time notifications
* Activity updates
* Email notifications using Resend

### AI Assistant

* AI-powered project assistant
* Summarize projects and issues
* Generate insights
* Answer project-related questions
* Improve workflow using LLMs

---

# Tech Stack

## Frontend

* Next.js
* React
* TypeScript
* Tailwind CSS
* shadcn/ui

## Backend

* Next.js API Routes
* MongoDB
* Mongoose

## Authentication

* Clerk

## Real-Time Communication

* Pusher

## Email Service

* Resend

## AI

* LLM API Integration

## Deployment

* Vercel
* MongoDB Atlas

---

# Architecture

```
Users
   │
   ▼
Clerk Authentication
   │
   ▼
Workspace
   │
   ├── Members
   │
   ├── Teams
   │      │
   │      └── Projects
   │               │
   │               └── Issues
   │                        │
   │                        └── Comments
   │
   └── AI Assistant (LLM)

Next.js API Routes
        │
        ▼
MongoDB Atlas
```

---

# Folder Structure

```
app/
components/
hooks/
lib/
models/
actions/
api/
public/
types/
utils/
```

---

# Workflow

1. User signs in using Clerk.
2. User creates a Workspace.
3. The creator automatically becomes the Workspace Admin.
4. Admin invites members.
5. Admin creates Teams.
6. Members are added to Teams.
7. Teams create Projects.
8. Projects contain Issues.
9. Members collaborate through Comments.
10. AI Assistant provides intelligent suggestions and insights.
11. Pusher delivers real-time updates.
12. Resend sends email notifications.

---

# Database Models

* User
* Workspace
* WorkspaceMember
* Team
* TeamMember
* Project
* Issue
* Comment
* Notification
* Activity

---

# Future Roadmap

* AI issue generation
* AI sprint planning
* AI project summaries
* Calendar integration
* GitHub integration
* Slack integration
* File attachments
* Kanban board improvements
* Analytics dashboard
* Search with AI
* Role permissions
* Mobile application

---

# Project Status

🚧 **Currently under active development.** New features, AI capabilities, and workflow improvements are continuously being added to enhance collaboration and project management.

---

# License

This project is available for learning and portfolio purposes. Please do not copy or redistribute the source code without permission.
