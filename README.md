Here’s a draft of the README file for your GitHub repository:

---

# Blogging Site

This repository consists of a full-stack blogging platform with three main components: **frontend**, **common**, and **backend**. Each folder contains separate modules and functionalities that contribute to the overall project.

## Table of Contents

- [Frontend](#frontend)
- [Common](#common)
- [Backend](#backend)
- [Setup Instructions](#setup-instructions)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

---

## Frontend

The frontend is built using **React** and **Vite**, along with **Tailwind CSS** for styling and **Radix UI** for component primitives. It provides the user interface for the blogging site, handling the client-side rendering and user interactions.

### Features
- **Vite** for fast development and build tooling.
- **Tailwind CSS** for styling with utilities.
- **React Router** for routing and navigation.
- **Axios** for HTTP requests.
- Various UI components from **Radix UI** and **Bootstrap**.

### Available Scripts
```bash
npm run dev       # Runs the development server
npm run build     # Builds the project for production
npm run lint      # Lints the code
npm run preview   # Previews the production build
```

### Dependencies
- React 18.3
- Tailwind CSS
- Radix UI components (Dialog, Dropdown, etc.)
- Axios
- React Icons
- React Router DOM
- Jodit React (for WYSIWYG editing)

---

## Common

This folder contains an **npm package** called `@100xdevs/common-app`, which provides shared utilities across the project. It uses **Zod** for schema validation.

### Key Features
- Custom reusable logic shared between the frontend and backend.
- **Zod** for type-safe schema validation.

### Package.json Overview
```json
{
  "name": "@100xdevs/common-app",
  "version": "1.0.0",
  "dependencies": {
    "zod": "^3.23.8"
  }
}
```

---

## Backend

The backend is a serverless API powered by **Hono** (a lightweight web framework for Cloudflare Workers) and **Prisma** (for database interactions). The backend handles user authentication, blog management, and integrates the common npm package for shared logic.

### Features
- **Hono** for routing and middleware.
- **Prisma** for database management with the help of **Prisma Client** and **Prisma Accelerate**.
- **JWT** for secure authentication.
- **Wrangler** for Cloudflare Workers deployment.

### Available Scripts
```bash
npm run dev       # Starts the backend in development mode
npm run deploy    # Deploys the backend using Wrangler to Cloudflare Workers
```

### Dependencies
- Hono 4.5.8
- Prisma 5.18.0
- Zod 3.23.8
- JWT for authentication

---

## Setup Instructions

### Prerequisites
- Node.js (v16+)
- npm or Yarn
- Cloudflare Wrangler for deploying the backend

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ParthDevInnovator/Blogging-site.git
   cd Blogging-site
   ```

2. Install dependencies for each folder:

   - **Frontend**:
     ```bash
     cd frontend
     npm install
     ```

   - **Common**:
     ```bash
     cd common
     npm install
     ```

   - **Backend**:
     ```bash
     cd backend
     npm install
     ```

3. Set up environment variables if needed (e.g., for database connection or JWT secret).

4. Run the development servers:
   ```bash
   cd frontend && npm run dev    # Run frontend
   cd backend && npm run dev     # Run backend
   ```

---

## Technologies Used

- **Frontend**: React, Vite, Tailwind CSS, Radix UI
- **Backend**: Hono, Prisma, Cloudflare Workers
- **Common**: Zod for schema validation
- **Deployment**: Wrangler (for backend deployment)

---

## Contributing

Feel free to contribute by creating issues or submitting pull requests. Please follow the code of conduct.

---

## License

This project is licensed under the MIT License.

---

This README provides an overview of the project structure, dependencies, and usage instructions. Let me know if you'd like to modify or expand any section!
