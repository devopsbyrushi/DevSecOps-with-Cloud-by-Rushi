# 🔐 04. DevSecOps

## 📚 What is DevSecOps?

DevSecOps stands for:

**Development + Security + Operations**

In simple words:

> **DevSecOps means integrating security into the DevOps process from the beginning instead of checking security only at the end.**

The main goal is to build and deliver applications with **security, quality, and automation**.

---

# 🤔 Why Do We Need DevSecOps?

In a traditional software delivery process, security may be checked after the application is developed.

For example:

```text
Development
     ↓
Build
     ↓
Testing
     ↓
Deployment
     ↓
Security Check
````

If security issues are identified at the end, fixing them can require additional effort and rework.

DevSecOps brings security into the development and delivery lifecycle.

---

# 🔄 DevOps vs DevSecOps

### DevOps

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
```

### DevSecOps

```text
Plan
 ↓
Code
 ↓
Security
 ↓
Build
 ↓
Security
 ↓
Test
 ↓
Security
 ↓
Release
 ↓
Deploy
 ↓
Operate
 ↓
Monitor
```

The important difference is:

> **Security becomes part of the complete software delivery lifecycle.**

---

# 🛡️ DevSecOps Security Areas

According to our program, we will cover the following security areas:

### 1. SAST

**Static Application Security Testing**

SAST is used to identify security issues in application source code.

Example:

* SonarQube

---

### 2. DAST

**Dynamic Application Security Testing**

DAST is used to test an application while it is running.

---

### 3. SCA

**Software Composition Analysis**

SCA helps identify security risks in application dependencies and open-source components.

---

### 4. Container Security

Container images should be scanned for vulnerabilities before they are deployed.

Example:

* Trivy

---

### 5. Infrastructure as Code Security

Infrastructure code should also be checked for security issues.

Example:

* Checkov

---

### 6. Secret Detection

Sensitive information such as:

* Passwords
* API Keys
* Access Tokens
* Secrets

should not be stored directly in source code.

Example:

* Gitleaks

---

# 🛠️ DevSecOps Tools

| Security Area           | Tool      |
| ----------------------- | --------- |
| Code Analysis           | SonarQube |
| Container Security      | Trivy     |
| Infrastructure Security | Checkov   |
| Secret Detection        | Gitleaks  |
| Secrets Management      | Vault     |

---

# 🔄 DevSecOps CI/CD Pipeline

A simple DevSecOps pipeline can look like this:

```text
Developer
    ↓
Git / GitHub
    ↓
Maven Build
    ↓
SonarQube
    ↓
Security Scanning
    ↓
Nexus
    ↓
Docker Build
    ↓
Trivy Scan
    ↓
Terraform / Checkov
    ↓
Deployment
    ↓
Kubernetes / AWS
    ↓
Monitoring
```

---

# 🏦 DevSecOps in Our Banking Application

Let's take our **SecureBank application** as an example.

We will integrate security into different stages of the application delivery process.

### Source Code

Developer pushes application code to GitHub.

↓

### Build

Maven builds the application.

↓

### Code Quality

SonarQube performs code analysis.

↓

### Security Scanning

Security checks are performed on the application and its dependencies.

↓

### Docker

A Docker image is created for the application.

↓

### Container Security

Trivy scans the Docker image for vulnerabilities.

↓

### Infrastructure Security

Checkov can scan Terraform infrastructure code.

↓

### Deployment

The application is deployed to Kubernetes / AWS.

↓

### Monitoring

Prometheus and Grafana are used for monitoring and observability.

---

# 🎯 Benefits of DevSecOps

* Security is considered from the beginning.
* Security checks can be automated.
* Vulnerabilities can be identified earlier.
* Security becomes part of the CI/CD pipeline.
* Development, Security and Operations teams work together.
* Reduces manual security activities.
* Helps improve the overall software delivery process.

---

# 👥 Security is a Shared Responsibility

In DevSecOps:

```text
Development
      +
Security
      +
Operations
      ↓
Secure Software Delivery
```

Security is not only the responsibility of the Security team.

Everyone involved in the software delivery lifecycle should consider security.

---

# 💡 Simple Real-Time Example

Suppose a developer accidentally pushes an API key into GitHub.

With DevSecOps:

```text
Developer
    ↓
Git Push
    ↓
Gitleaks
    ↓
Secret Detected
    ↓
Pipeline Stops
```

The issue can be identified before the application continues through the delivery pipeline.

---

# 🔑 DevOps vs DevSecOps

| DevOps                       | DevSecOps                           |
| ---------------------------- | ----------------------------------- |
| Development + Operations     | Development + Security + Operations |
| Focuses on software delivery | Focuses on secure software delivery |
| Automation                   | Automation + Security Automation    |
| CI/CD                        | Secure CI/CD                        |
| Monitoring                   | Monitoring + Security               |

---

# 📌 Key Point

> **DevOps helps us build, test and deliver applications efficiently. DevSecOps adds security into this process so that security is considered throughout the software development and delivery lifecycle.**

