# Learning DevOps

A hands-on sandbox repository for learning and practicing core DevOps concepts, including CI/CD pipelines, GitHub Actions workflows, and automated testing on a simple Node.js application.

## About

This repo is used to experiment with building and testing CI/CD pipelines using GitHub Actions. It contains a minimal Node.js app that serves as the target for pipeline automation, covering steps like installing dependencies, running tests, and triggering builds on every push.

## Project Structure

```
learning-devops/
├── .github/
│   └── workflows/       # GitHub Actions CI/CD pipeline definitions
├── index.js              # Application entry point
├── package.json           # Project metadata and dependencies
├── test.js               # Test suite for the application
└── README.md
```

## Tech Stack

- Node.js - application runtime
- GitHub Actions - CI/CD automation
- npm - package management

## CI/CD Pipeline

Every push to this repository triggers a GitHub Actions workflow (see `.github/workflows/`) that:

1. Checks out the code
2. Installs dependencies via `npm install`
3. Runs the test suite (`test.js`)
4. Reports build/test status

## Getting Started

Clone the repository:

```bash
git clone https://github.com/AryanHulawale/learning-devops.git
cd learning-devops
```

Install dependencies:

```bash
npm install
```

Run the app:

```bash
node index.js
```

Run tests:

```bash
npm test
```

## Purpose

This repository is part of an ongoing personal learning journey into DevOps practices, covering CI/CD pipeline design, automation, and workflow orchestration using GitHub Actions.

## License

This project is for personal learning purposes.
