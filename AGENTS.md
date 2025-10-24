# Agent Development Guidelines for SafaArban Translator

This document provides guidelines for AI agents working on the SafaArban Translator project. By adhering to these guidelines, we can ensure a consistent and high-quality codebase.

## General Principles

- **Modularity:** Keep components and modules small and focused on a single responsibility.
- **Clarity:** Write clean, readable, and well-documented code.
- **Consistency:** Follow the established coding style and project structure.
- **Testing:** Write unit and integration tests for all new features and bug fixes.

## Frontend Development

- **Component Structure:** Components should be organized by feature or page in the `src/components` and `src/pages` directories.
- **State Management:** For simple state, use React's built-in hooks. For complex state, we will introduce a state management library like Zustand or Redux Toolkit.
- **Styling:** Use TailwindCSS for all styling. Avoid custom CSS files unless absolutely necessary.
- **API Communication:** Use the `fetch` API or a library like `axios` for all communication with the backend. Services should be defined in the `src/services` directory.

## Backend Development

- **Modular Architecture:** The backend is organized into modules by feature (e.g., `auth`, `users`, `projects`). Each module should contain its own controllers, services, and routes.
- **Error Handling:** Implement a consistent error handling mechanism. Use HTTP status codes to indicate the outcome of an API request.
- **Database Interaction:** Use a query builder or ORM to interact with the PostgreSQL database. All database-related code should be kept in a separate layer (e.g., a `data-access` or `repository` layer).
- **Validation:** Validate all incoming data from the client. Use a library like `zod` or `joi` to define validation schemas.

## Pre-commit Checks

Before submitting any code, please run the following checks:

1.  **Linting:** Run `npm run lint` in both the `frontend` and `backend` directories.
2.  **Testing:** Run `npm run test` in both the `frontend` and `backend` directories.
3.  **Build:** Ensure that both the `frontend` and `backend` applications build successfully (`npm run build`).
