## Introduction

In this lecture, we will understand how Git manages our source code through different stages.

When a developer creates or modifies code, the changes first exist in the **Working Area**. We then use Git commands to move the changes to the **Staging Area** and finally save them in the **Local Repository**.

After committing the changes, we can push the code to the **GitHub Repository**.

The basic Git workflow is:

Class Notes:
<img width="3830" height="4000" alt="Gitclass2" src="https://github.com/user-attachments/assets/a0ea4753-9b98-4eed-bd22-056ba143b4c7" />


```text
Working Area
      ↓
Staging Area
      ↓
Local Repository
      ↓
GitHub Repository
```

In this lecture, we will understand:

- Working Area
- Staging Area
- Local Repository
- How `git add` works
- How `git commit` works
- How `git push` works
- How `git status` helps us
- How `git log` shows commit history

---

# Git Workflow

When we work with Git, our code moves through different stages.

```text
Working Area
     ↓
Staging Area
     ↓
Local Repository
     ↓
GitHub Repository
```

---

## 1. Working Area

The **Working Area** is where we create or modify our files.

Example:

```text
logoutservices
├── logout
├── logoutschema
├── 1
├── 2
└── 3
```

When we create or modify a file, Git detects the change.

To check the current status:

```bash
git status
```

---

## 2. Staging Area

The **Staging Area** is also called the **Index Area**.

We use `git add` to move files from the Working Area to the Staging Area.

### Add a specific file

```bash
git add filename
```

Example:

```bash
git add logout
```

### Add multiple files

```bash
git add 1 2 3
```

### Add all files

```bash
git add .
```

or

```bash
git add -A
```

Check the status again:

```bash
git status
```

---

## 3. Local Repository

The **Local Repository** contains the committed changes on our local machine.

We use `git commit` to save the staged changes into the Local Repository.

```bash
git commit -m "message"
```

Example:

```bash
git commit -m "I have developed code for logout"
```

Another example:

```bash
git commit -m "Bug fixes done for logout"
```

A commit message should describe the change that was made.

---

## 4. Push Code to GitHub

After committing the changes, we can send the code to the GitHub Repository.

```bash
git push
```

The complete flow is:

```text
Working Area
     ↓
  git add
     ↓
Staging Area
     ↓
 git commit
     ↓
Local Repository
     ↓
  git push
     ↓
GitHub Repository
```

---

## 5. Git Status

`git status` is used to check the current state of our files.

```bash
git status
```

It helps us understand whether files are:

- Modified
- Untracked
- Staged
- Ready for commit

---

## 6. Git Log

After creating commits, we can view the commit history using:

```bash
git log
```

It shows information about previous commits.

Example:

```text
commit abc123
Author: Rushi

    I have developed code for logout
```

---

## 7. Git Configuration

Before creating commits, configure your Git username and email.

### Configure username

```bash
git config --global user.name "Your Name"
```

### Configure email

```bash
git config --global user.email "yourmail@example.com"
```

Check the configuration:

```bash
git config --global user.name
git config --global user.email
```

---

# Complete Git Flow

### Step 1: Create or modify files

```text
Working Area
```

### Step 2: Add files

```bash
git add .
```

```text
Working Area → Staging Area
```

### Step 3: Commit changes

```bash
git commit -m "Added logout functionality"
```

```text
Staging Area → Local Repository
```

### Step 4: Push to GitHub

```bash
git push
```

```text
Local Repository → GitHub Repository
```

### Step 5: Check commit history

```bash
git log
```

---

## Real-Time Example

Suppose we are developing a **Logout Service**.

```text
Developer creates/changes code
            ↓
       Working Area
            ↓
        git add .
            ↓
       Staging Area
            ↓
git commit -m "Added logout service"
            ↓
      Local Repository
            ↓
         git push
            ↓
      GitHub Repository
```

---

## Important Commands

```bash
git status
```

Check the current status of files.

```bash
git add .
```

Add changes to the Staging Area.

```bash
git commit -m "message"
```

Save staged changes in the Local Repository.

```bash
git push
```

Push committed changes to GitHub.

```bash
git log
```

View commit history.

---

## Key Point

> Git moves our code through the Working Area, Staging Area, and Local Repository. After committing the changes, we can push the code to the GitHub Repository.

---

## Author

**Rushi**  
**Lead DevOps Engineer & Cloud Trainer**
