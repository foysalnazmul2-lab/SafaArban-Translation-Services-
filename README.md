# SafaArban Translator

SafaArban Translator is a professional, human-in-the-loop translation web application designed for accuracy and efficiency. This platform allows users to upload various document formats, extract text while preserving the original layout, and perform manual, line-by-line translations in a user-friendly bilingual editor. The application supports right-to-left (RTL) languages and provides tools like translation memory and a glossary to ensure consistency and quality.

## Project Vision

Our goal is to build a production-ready web portal that streamlines the professional translation workflow. By focusing on human translation and providing robust tools, we aim to deliver a secure, scalable, and intuitive platform for language professionals. This project is built with a modular design to allow for future integration of self-hosted AI models, without relying on external AI APIs in its core version.

## Tech Stack

- **Frontend:** React, TypeScript, Vite, TailwindCSS
- **Backend:** Node.js, Express, TypeScript
- **Database:** PostgreSQL, Redis
- **Storage:** AWS S3 or Local File System
- **OCR:** Tesseract.js
- **PDF Tools:** pdf.js, pdf-lib, docx, pdfkit

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Docker (for PostgreSQL and Redis)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/safaarban-translator.git
    cd safaarban-translator
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Set up environment variables:**
    - Create a `.env` file in the `backend` directory.
    - Add the necessary environment variables (e.g., database credentials, JWT secret).

4.  **Run the development servers:**
    ```bash
    # In the root directory
    npm run dev
    ```
    This will start both the frontend and backend development servers.

## Project Structure

The project is organized as a monorepo with two main packages:

-   `frontend/`: The React application that provides the user interface.
-   `backend/`: The Node.js/Express application that handles the business logic and API.

Each package has its own `package.json` and scripts. The root `package.json` contains scripts for running both applications concurrently.
