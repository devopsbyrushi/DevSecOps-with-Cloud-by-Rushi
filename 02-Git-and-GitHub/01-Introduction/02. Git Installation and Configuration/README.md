## 1. Install Git on Windows

Git can be installed on Windows using the official Git website.

### Download Git

Official Git website:

https://git-scm.com/install/windows

Open the website and download the latest Git for Windows installer.

### Installation Steps

1. Open the downloaded installer.
2. Follow the installation wizard.
3. Keep the default options.
4. Complete the installation.
5. Open **Git Bash**.

---

## 2. Verify Git Installation

After installation, check the Git version:

```bash
git --version
```

Example:

```text
git version 2.x.x
```

If the version is displayed, Git is installed successfully.

---

## 3. Configure Git Username

Git needs to know who is making the changes.

Set your username:

```bash
git config --global user.name "Your Name"
```

Example:

```bash
git config --global user.name "Rushi"
```

---

## 4. Configure Git Email

Set your email address:

```bash
git config --global user.email "yourmail@example.com"
```

Example:

```bash
git config --global user.email "rushi@example.com"
```

---

## 5. Verify Username and Email

Check the configured username:

```bash
git config --global user.name
```

Check the configured email:

```bash
git config --global user.email
```

Check all Git configurations:

```bash
git config --list
```

---

## 6. Unset Git Username

To remove the configured username:

```bash
git config --global --unset user.name
```

Verify:

```bash
git config --global user.name
```

---

## 7. Unset Git Email

To remove the configured email:

```bash
git config --global --unset user.email
```

Verify:

```bash
git config --global user.email
```

---

## 8. Configure Again

You can configure the username and email again:

```bash
git config --global user.name "Your Name"

git config --global user.email "yourmail@example.com"
```

---

## Important Commands

```bash
git --version

git config --global user.name "Your Name"

git config --global user.email "yourmail@example.com"

git config --global user.name

git config --global user.email

git config --global --unset user.name

git config --global --unset user.email

git config --list
```

## Key Point

> Install Git → Verify Git → Configure Username and Email → Verify Configuration

---

## Author

**Rushi**  
**Lead DevOps Engineer & Cloud Trainer**
```

**Section:** `02-Git-and-GitHub`  
**Topic:** `02-Git-Installation-and-Configuration`
