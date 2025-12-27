# Full-Stack Web Application

This repository contains a full-stack web application built with Node.js,
Express, and SQLite. It includes scripts and documentation for setting up,
configuring, and deploying the application on an AWS EC2 instance.

- [Development Guide](dev-node/README.md)
- [Deployment Guide (Docker)](deploy-docker/README.md)
- [Deployment Guide (Manual)](deploy-node/README.md)

## Quick Start

These are instructions to quickly get the application up and running using
Docker. To push Docker images to Docker Hub, please refer to the [Deployment Guide (Docker)](deploy-docker/README.md)
for detailed steps regarding Docker Hub authentication and image management.

To quickly get started with the application using Docker, follow these steps:
1. Clone the repository:
   ```bash
   git clone
    ```
2. Navigate to the project directory
3. Build and start the application with the `dev.sh` script:
   ```bash
    ./dev.sh build

### Validate Setup

Before deploying, you can validate each part independently:

```bash
# Docker Hub authentication
./dev.sh docker

# EC2 SSH connectivity and env check (writes ec2-ssh.sh)
./dev.sh ec2

# Or run both together
./dev.sh login
```

## Technology Stack

- Backend technology stack
    - Web Server: [nginx](https://www.nginx.com/) as a reverse proxy server
    - Backend Runtime: [Node.js](https://nodejs.org/)
    - Backend Framework: [Express](https://expressjs.com/)
    - Database: [SQLite](https://www.sqlite.org/index.html) for lightweight data storage
- Frontend technology stack
    - Templates: [EJS](https://ejs.co/) for server-side rendering
    - UX/UI: [Bootstrap](https://getbootstrap.com/) for responsive design
- Testing Frameworks
    - End-to-End Testing: [Playwright](https://playwright.dev/)
