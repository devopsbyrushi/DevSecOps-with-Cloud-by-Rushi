In this lecture, we will learn how to check the **commit history** of a Git repository using `git log`.

Git logs are useful when we want to know:

- Who made the changes
- When the changes were made
- What commits were created
- How many commits were created
- Commit history within a specific time period

We can also filter Git logs based on an **author** and **date range**.

---

# 1. Basic Git Log

To view the complete commit history:

```bash
git log
```

This displays information such as:

- Commit ID
- Author
- Date
- Commit message

---

# 2. Git Log Based on Author

We can filter the commits based on the author.

```bash
git log --author=devopsbyrushi
```

This displays commits made by the specified author.

Example:

```bash
git log --author=devopsbyrushi
```

---

# 3. Git Log in One Line

To display the commit history in a simple one-line format:

```bash
git log --author=devopsbyrushi --oneline
```

Example:

```text
a12bc34 Added logout service
b45de67 Fixed logout issue
c78fg90 Updated logout schema
```

This makes it easier to quickly understand the commit history.

---

# 4. Git Log Based on Date

We can also filter commits based on a date.

### Since a Particular Date

Syntax:

```bash
git log --since=YYYY-MM-DD
```

Example:

```bash
git log --since=2022-01-01
```

This displays commits created from the specified date onwards.

---

### Until a Particular Date

Syntax:

```bash
git log --until=YYYY-MM-DD
```

Example:

```bash
git log --until=2024-01-01
```

This displays commits created before the specified date.

---

# 5. Git Log Based on Author and Date

We can combine author and date filters.

Example:

```bash
git log --since=2022-01-01 --author=devopsbyrushi -10
```

This displays the latest 10 commits from the specified author since January 1, 2022.

---

# 6. Git Log Between Two Dates

We can use both `--since` and `--until` to check commits within a specific time period.

Example:

```bash
git log --since=2024-01-01 --until=2026-10-08 --author=devopsbyrushi -10
```

This displays up to the latest 10 commits made by `devopsbyrushi` between:

```text
2024-01-01
     ↓
2026-10-08
```

---

# 7. Real-Time Example

Suppose a repository was created in **2022** and we want to check the commits made by a particular developer.

We can start with:

```bash
git log --author=devopsbyrushi
```

Then make the output simpler:

```bash
git log --author=devopsbyrushi --oneline
```

Then filter based on dates:

```bash
git log --since=2022-01-01 --author=devopsbyrushi -10
```

Or check a specific period:

```bash
git log --since=2024-01-01 --until=2026-10-08 --author=devopsbyrushi -10
```

---

# 8. Important Git Log Commands

### View all commits

```bash
git log
```

### View commits by author

```bash
git log --author=devopsbyrushi
```

### View commits by author in one line

```bash
git log --author=devopsbyrushi --oneline
```

### View commits since a date

```bash
git log --since=2022-01-01
```

### View commits until a date

```bash
git log --until=2024-01-01
```

### View latest 10 commits since a date

```bash
git log --since=2022-01-01 --author=devopsbyrushi -10
```

### View latest 10 commits between two dates

```bash
git log --since=2024-01-01 --until=2026-10-08 --author=devopsbyrushi -10
```

---

## Date Format

Git uses the following date format in these examples:

```text
YYYY-MM-DD
```

Example:

```text
2026-10-08
```

Where:

```text
YYYY = Year
MM   = Month
DD   = Day
```



## Key Point

> `git log` is used to view Git commit history, and we can filter the history based on author, date, and number of commits.

---

## Author

**Rushi**  
**Lead DevOps Engineer & Cloud Trainer**
```
