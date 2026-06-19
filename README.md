# Docker-Git Integration Project

An automated CI/CD pipeline that builds a Python application Docker image and pushes it to Docker Hub using GitHub Actions whenever code changes are pushed to the repository.

## 🚀 Overview

This project demonstrates how to connect a GitHub repository to Docker Hub for continuous integration. By utilizing GitHub Actions, the entire process of building the container image and releasing it to a central registry is completely automated.

```text
[Local Machine] ──(git push)──> [GitHub Repository]
                                        │
                            (Triggers GitHub Actions)
                                        │
                                        ▼
                           [Ubuntu Cloud Runner]
                            ├── Pulls code
                            ├── Authenticates via PAT
                            └── Builds & Pushes Image ──> [Docker Hub] <br/>

🛠️ Tech Stack
Language: Python

Containerization: Docker

CI/CD Automation: GitHub Actions

Container Registry: Docker Hub
