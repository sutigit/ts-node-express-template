# ts-node-express Template

This repository is a template for setting up a Node.js server with TypeScript and Express, based on the [LogRocket article](https://blog.logrocket.com/how-to-set-up-node-typescript-express/). It provides a clean and efficient development environment to build scalable and type-safe backend applications.

## Features

### 1. **Project Structure**
- **Organized Codebase**: The entry point is `src/index.ts` for better code management and scalability.
- **Structured `package.json`**: Defines dependencies, scripts, and metadata for the project.

### 2. **Express Integration**
- **Express Framework**: Efficiently handles HTTP requests and routes.
- **Environment Variables**: Managed with `dotenv` via `.env` files for secure configuration.

### 3. **TypeScript Integration**
- **Type Safety**: TypeScript ensures robust and predictable code.
- **Type Definitions**: Includes `@types/express` and `@types/node` for seamless integration with TypeScript.
- **TypeScript Configuration**: Customizable options set in `tsconfig.json`.

### 4. **Development Tools**
- **`ts-node`**: Allows direct execution of TypeScript files without pre-compilation.
- **`nodemon`**: Monitors file changes and automatically restarts the server during development.

### 5. **Path Aliases**
- **`tsconfig-paths`**: Simplifies imports with custom path aliases defined in `tsconfig.json`.

### 6. **Build and Run Scripts**
- **Development Server**:
```bash
npm run dev
```
Starts the server with hot-reloading using `nodemon`.

- **Build**:
```bash
npm run build
```
Compiles TypeScript files and resolves path aliases.

- **Production start**:
```bash
npm run start
```
Runs the compiled JavaScript code in the `dist` directory.

## Setup instructions

### 1. **Clone repository**:
```bash
git clone https://github.com/sutigit/ts-node-express-template.git
cd ts-node-express-template
```

### 2. **Install dependencies**:
```bash
npm install
```

### 3. **Configure environment variables**:
- Create a .env file in the root directory.
- Add your environment-specific variables, such as:
```
PORT=3000 
```

### 4. **Run in development**:
```bash
npm run dev
```

### 5. **Build for production**:
```bash
npm run build
```

### 6. **Start the porduction server**:
```bash
npm run start
```

## Dependencies

### Runtime Dependencies
- **`dotenv`** — Loads environment variables from a `.env` file.
- **`express`** — Web framework for building APIs.
- **`tsconfig-paths`** — Resolves TypeScript path aliases in runtime.

### Development Dependencies
- **`@types/express`** — Type definitions for Express.
- **`@types/node`** — Type definitions for Node.js.
- **`concurrently`** — Runs multiple scripts concurrently.
- **`nodemon`** — Monitors file changes and restarts the server automatically.
- **`ts-node`** — Executes TypeScript directly without pre-compilation.
- **`tsc-alias`** — Resolves path aliases during the build process.
- **`typescript`** — A strongly typed programming language for JavaScript.


## File structure
```
ts-node-express/
│
├── src/
│   ├── index.ts       # Main entry point
│   └── ...            # Additional files and modules
│
├── dist/              # Compiled JavaScript (after build)
├── .env               # Environment variables
├── tsconfig.json      # TypeScript configuration
├── package.json       # Project metadata and scripts
└── README.md          # Documentation
```
