# Contributing to Web3Auth

Thank you for your interest in contributing to Web3Auth! This document outlines the setup process and guidelines for contributing to this monorepo project.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- [Node.js](https://nodejs.org/) version 20.16 or later
- [Yarn](https://yarnpkg.com/) package manager
- [Git](https://git-scm.com/)

We recommend using [nvm](https://github.com/nvm-sh/nvm) (Node Version Manager) to manage your Node.js versions.

## Setting Up the Development Environment

1. Fork the repository and clone your fork:

   ```
   git clone https://github.com/YOUR_USERNAME/Web3Auth.git
   cd Web3Auth
   ```

2. Install Node.js 20.16 using nvm:

   ```
   nvm install 20.16
   nvm use 20.16
   ```

3. Install sub packages dependencies using Yarn:

   ```
   npx lerna exec -- yarn install
   ```

   This will install all necessary packages, including Lerna and cross-env.

## Development Workflow

This project uses Lerna to manage the monorepo structure. Here are some common commands:

- Build all packages:
  ```
  yarn build
  ```

- Run tests:
  ```
  yarn test
  ```

- Lint the code:
  ```
  yarn lint
  ```

## Making Changes

1. Create a new branch for your feature or bugfix:
   ```
   git checkout -b feature/your-feature-name
   ```

2. Make your changes and commit them with a clear, descriptive commit message.

3. Push your changes to your fork:
   ```
   git push origin feature/your-feature-name
   ```

4. Open a pull request against the main repository.

## Additional Notes

- Use npm for managing dependencies in individual packages.
- Use npx lerna for monorepo-wide operations.
- When making changes, consider the impact on other packages within the monorepo.
- Make sure to run tests and linting before submitting a pull request.
- Keep your pull requests focused on a single feature or bugfix.
- When submitting a pull request, clearly describe which package(s) are affected.


Thank you for contributing to Web3Auth!