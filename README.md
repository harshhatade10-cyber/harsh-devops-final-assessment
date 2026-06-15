# DevOps Foundations Project

## Project Description

This project was built to practice core DevOps concepts and tools used in modern software delivery pipelines. It demonstrates version control, Linux automation, containerization, CI/CD pipelines, workload orchestration, and log monitoring using industry-standard DevOps tools.

The project includes Git & GitHub for source code management, Bash scripting for automation, Docker for containerization, GitHub Actions for continuous integration, Nomad for workload deployment, and Grafana Loki for log management and monitoring.

---

## Project Structure

```text
devops-foundations-project
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

## Git & GitHub

The repository is managed using Git and hosted on GitHub to enable version control and collaboration.

### Sample Application

```python
print("Hello, DevOps!")
```

### Run Application

```bash
python hello.py
```

### Expected Output

```text
Hello, DevOps!
```

---

## Linux Shell Scripting

The project includes a Bash script that collects basic system information.

### File

```text
scripts/sysinfo.sh
```

### Features

- Displays current user
- Displays current date and time
- Displays disk usage information

### Run Script

```bash
chmod +x scripts/sysinfo.sh
./scripts/sysinfo.sh
```

---

## Docker Containerization

The Python application is containerized using Docker.

### Build Docker Image

```bash
docker build -t hello-devops .
```

### Run Container

```bash
docker run hello-devops
```

### Expected Output

```text
Hello, DevOps!
```

---

## CI/CD with GitHub Actions

A GitHub Actions workflow is configured to automate code validation.

### Workflow File

```text
.github/workflows/ci.yml
```

### Pipeline Activities

- Triggered on every push
- Executes the Python application
- Verifies successful execution

---

## Nomad Deployment

Nomad is used to deploy and manage the Docker workload.

### Job File

```text
nomad/hello.nomad
```

### Run Deployment

```bash
nomad job run nomad/hello.nomad
```

### Purpose

- Simple workload scheduling
- Container deployment management
- Basic orchestration practice

---

## Monitoring with Grafana Loki

Grafana Loki documentation and setup steps are included for log aggregation and monitoring.

### Documentation File

```text
monitoring/loki_setup.txt
```

### Start Loki

```bash
docker run -d -p 3100:3100 grafana/loki:3.0.0
```

### Health Check

```text
http://localhost:3100/ready
```

### View Container Logs

```bash
docker logs <container_id>
```

---

## Workflow

```text
Developer
    ↓
GitHub Repository
    ↓
GitHub Actions CI/CD
    ↓
Docker Image Build
    ↓
Nomad Deployment
    ↓
Grafana Loki Monitoring
```

---

## Skills Demonstrated

- Git and GitHub Version Control
- Linux Administration Fundamentals
- Bash Scripting and Automation
- Docker Containerization
- CI/CD Automation with GitHub Actions
- Nomad Workload Scheduling
- Log Management with Grafana Loki
- DevOps Workflow Understanding

---

## Technologies Used

| Category | Technology |
|-----------|------------|
| Version Control | Git, GitHub |
| Operating System | Linux |
| Scripting | Bash |
| Programming Language | Python |
| Containerization | Docker |
| CI/CD | GitHub Actions |
| Orchestration | Nomad |
| Monitoring | Grafana Loki |

---

## Future Enhancements

- Kubernetes Deployment
- Terraform Infrastructure Provisioning
- AWS Cloud Deployment
- Prometheus Monitoring Integration
- Automated Docker Image Publishing
- Multi-Environment CI/CD Pipelines

---

## Conclusion

This project serves as a practical implementation of foundational DevOps concepts and demonstrates hands-on experience with modern tools used for automation, deployment, orchestration, and monitoring in software delivery workflows.