# Simple CI Pipeline for Node.js Application

A beginner-friendly DevOps project demonstrating how to build a basic CI pipeline for a Node.js application using GitHub Actions.

## Project Overview

This project demonstrates:

- Node.js project setup
- Automated testing with Jest
- GitHub Actions CI pipeline
- Dependency installation in CI
- Clean runner environments
- Push, pull request, and manual workflow triggers

## What This Project Does

The project contains a simple Jest test and a GitHub Actions workflow that automatically:

1. Checks out the repository
2. Sets up Node.js
3. Installs project dependencies
4. Runs automated tests

If the tests pass, the pipeline succeeds.  
If the tests fail, the pipeline fails.

## CI Pipeline Flow

```text
Push / Pull Request / Manual Run
        ↓
GitHub Actions starts runner
        ↓
Checkout repository
        ↓
Setup Node.js
        ↓
Install dependencies
        ↓
Run tests
        ↓
Pass or fail
```

## Project Structure

```text
ci-demo/
├── .github/
│   └── workflows/
│       └── node-ci.yml
├── tests/
│   └── sum.test.js
├── package.json
├── package-lock.json
└── README.md
```

## How to Run Locally

Install dependencies:

```bash
npm install
```

Run tests:

```bash
npm test
```

## GitHub Actions Workflow

The CI workflow runs on:

- push
- pull request
- manual trigger

Workflow file:

```text
.github/workflows/node-ci.yml
```

## Skills Demonstrated

- GitHub Actions
- CI pipeline design
- Node.js environment setup
- Dependency installation
- Automated testing
- Clean CI runner usage
- Basic DevOps workflow understanding

## Future Improvements

Planned improvements:

- Add more test cases
- Add linting
- Add build step
- Add CI status badge
- Add artifact upload
- Add Docker support
- Deploy to a cloud platform
