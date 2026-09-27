#  03. DevOps

##  What is DevOps?

DevOps is a combination of **Development (Dev)** and **Operations (Ops)**.

In simple words:

> **DevOps is a way of working where Development and Operations teams work together to build, test, deploy, and maintain applications faster and more reliably.**

---

## 🤔 Why Do We Need DevOps?

In the traditional approach, Development and Operations teams often worked separately.

The Developer's responsibility was mainly to:

- Develop the application
- Write the code
- Fix application issues

The Operations team's responsibility was mainly to:

- Manage servers
- Deploy applications
- Maintain infrastructure
- Monitor applications

Because the teams worked separately, there could be delays and communication gaps.

DevOps helps bring these activities together using **collaboration and automation**.

---

# 🔄 DevOps Process

A simple DevOps flow is:

```text
Plan
  ↓
Code
  ↓
Build
  ↓
Test
  ↓
Release
  ↓
Deploy
  ↓
Operate
  ↓
Monitor
  ↓
Feedback
  ↺
````

The process is continuous.

---

# 🛠️ Important DevOps Practices

### 1. Collaboration

Development and Operations teams work together.

### 2. Automation

We automate repetitive activities such as:

* Build
* Testing
* Deployment
* Infrastructure creation
* Configuration

### 3. Continuous Integration

Developers frequently integrate their code into a shared repository.

### 4. Continuous Delivery

The application is continuously prepared for release.

### 5. Continuous Deployment

Changes can be automatically deployed to the required environment when the pipeline is configured for it.

### 6. Infrastructure as Code

Infrastructure can be created and managed using code.

Example:

**Terraform**

### 7. Monitoring

Applications and infrastructure are continuously monitored.

Example:

**Prometheus + Grafana**

---

# 🛠️ Common DevOps Tools

| Activity                 | Tools                   |
| ------------------------ | ----------------------- |
| Source Code              | Git, GitHub             |
| Build                    | Maven                   |
| CI/CD                    | Jenkins, GitHub Actions |
| Code Quality             | SonarQube               |
| Artifact Management      | Nexus                   |
| Containers               | Docker                  |
| Container Orchestration  | Kubernetes              |
| Cloud                    | AWS                     |
| Infrastructure as Code   | Terraform               |
| Configuration Management | Ansible                 |
| Monitoring               | Prometheus, Grafana     |
| Logging                  | ELK                     |

---

# 🏦 Real-Time Example – Banking Application

Let's consider our **SecureBank application**.

A developer writes the application code.

The DevOps process can be:

```text
Developer
    ↓
Git / GitHub
    ↓
Maven
    ↓
Jenkins
    ↓
SonarQube
    ↓
Nexus
    ↓
Docker
    ↓
Terraform + AWS
    ↓
Kubernetes / AWS EKS
    ↓
Prometheus + Grafana
```

Each tool performs a specific activity in the application delivery process.

---

# 🎯 Benefits of DevOps

* Faster software delivery
* More automation
* Better collaboration
* Faster feedback
* More reliable deployments
* Continuous testing
* Better monitoring
* Easier infrastructure management
* Faster issue identification

---

# 💡 Simple Example

Imagine a developer makes a change to the banking application.

Without automation:

```text
Developer
   ↓
Build manually
   ↓
Test manually
   ↓
Create deployment package
   ↓
Deploy manually
```

With DevOps:

```text
Developer
   ↓
Git Push
   ↓
CI/CD Pipeline
   ↓
Build
   ↓
Test
   ↓
Code Quality
   ↓
Security Checks
   ↓
Docker Image
   ↓
Deployment
   ↓
Monitoring
```

This is one of the main reasons organizations use DevOps practices.

---

# 📌 Key Point

> **DevOps is not just a tool. It is a combination of people, processes, practices, and tools that helps organizations deliver software faster, reliably, and continuously.**

---

## 👉 Next Topic

**04 - DevSecOps**

We will understand how security is integrated into the DevOps process.
