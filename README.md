# DevOps Intern Final Assessment

**Name:** Harsh Pralhad Hatade
**Date:** 04-06-2026

## Project Description

This project demonstrates fundamental DevOps concepts including Git & GitHub, Linux Shell Scripting, Docker, GitHub Actions (CI/CD), Nomad job deployment, and Grafana Loki documentation.

---

## Project Structure

```text
harsh-devops-final-assessment
│
├── README.md
├── hello.py
├── Dockerfile
│
├── scripts/
│   └── sysinfo.sh
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
├── nomad/
│   └── hello.nomad
│
└── monitoring/
    └── loki_setup.txt
```

---

## Step 1: Git & GitHub

Repository initialized using Git and pushed to GitHub.

Sample Python file:

```python
print("Hello, DevOps!")
```

Run:

```bash
python hello.py
```

Expected Output:

```text
Hello, DevOps!
```

---

## Step 2: Linux Shell Script

File:

```text
scripts/sysinfo.sh
```

This script displays:

* Current User
* Current Date
* Disk Usage

Run:

```bash
chmod +x scripts/sysinfo.sh
./scripts/sysinfo.sh
```

---

## Step 3: Docker

Dockerfile containerizes the Python application.

Build Image:

```bash
docker build -t hello-devops .
```

Run Container:

```bash
docker run hello-devops
```

Expected Output:

```text
Hello, DevOps!
```

---

## Step 4: CI/CD with GitHub Actions

Workflow File:

```text
.github/workflows/ci.yml
```

The workflow automatically runs:

```bash
python hello.py
```

on every push to the repository.

---

## Step 5: Nomad Deployment

Nomad Job File:

```text
nomad/hello.nomad
```

Run:

```bash
nomad job run nomad/hello.nomad
```

The job deploys the Docker container using Nomad.

---

## Step 6: Monitoring with Grafana Loki

Documentation File:

```text
monitoring/loki_setup.txt
```

Example Commands:

```bash
docker run -d -p 3100:3100 grafana/loki:3.0.0
```

Check Status:

```text
http://localhost:3100/ready
```

View Logs:

```bash
docker logs <container_id>
```

---

## Technologies Used

* Git
* GitHub
* Linux
* Bash Scripting
* Docker
* GitHub Actions
* Nomad
* Grafana Loki

---

## Assessment Completion

All required files, configurations, and documentation have been included as requested in the DevOps Intern Final Assessment.
