# Security Hack Lab

![Project Structure](/images/img-1.webp)

Welcome to the **Security Hack Lab**! This project aims to create a controlled environment for practicing and demonstrating penetration testing techniques using Docker. This lab includes various vulnerable web applications, allowing you to simulate real-world hacking scenarios safely and ethically.

## Table of Contents

- [Project Overview](#project-overview)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The **Security Hack Lab** is designed for cybersecurity enthusiasts, professionals, and learners who wish to enhance their skills in penetration testing and security analysis. The lab includes:

- A vulnerable web application for testing web vulnerabilities.
- An Nginx server configured with known vulnerabilities.
- A MySQL database to simulate real-world interactions.
- An SSH server for practicing secure shell access and privilege escalation techniques.

## Prerequisites

Before you begin, ensure you have the following installed:

- Docker: [Install Docker](https://docs.docker.com/get-docker/)
- Docker Compose: [Install Docker Compose](https://docs.docker.com/compose/install/)
- (Optional) Docker Buildx: For multi-architecture builds [Docker Buildx](https://docs.docker.com/buildx/working-with-buildx/)

## Getting Started

To set up your security hack lab, follow these steps:

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/security-hack-lab.git
   cd security-hack-lab
   ```

2. **Build and run the Docker containers**:

   ```bash
   docker-compose up -d
   ```

3. **Access the applications**:
   - Vulnerable Web App: [http://localhost:8080](http://localhost:8080)
   - SSH Server: Use your terminal or SSH client to connect to the SSH server.

## Project Structure

```
security-hack-lab/
│
├── docker-compose.yml      # Docker Compose configuration file
├── Dockerfile               # Base Dockerfile for the vulnerable web app
├── nginx/                  # Directory containing Nginx configuration
│   └── nginx.conf          # Nginx configuration file
├── vulnerable-app/         # Directory for the vulnerable web app code
│   └── app.py              # Main application file
└── README.md               # This README file
```

## Usage

1. After running `docker-compose up -d`, the lab environment will be up and running.
2. Access the vulnerable web application via your web browser at [http://localhost:8080](http://localhost:8080).
3. Use the provided SSH credentials to connect to the SSH server.

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Special thanks to the open-source community for providing the resources used in this project.
- Resources from [LinuxServer.io](https://www.linuxserver.io/) were instrumental in setting up the multi-platform environment.

---

Feel free to explore, learn, and most importantly, practice safely!
