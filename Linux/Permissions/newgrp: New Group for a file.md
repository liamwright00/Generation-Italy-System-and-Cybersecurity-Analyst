
# Understanding File Ownership in Linux

When a file is created in Linux, it has an **owner** (the user who creates it) and a **group**. By default, the group ownership is set to the user's primary group. However, this behavior can be changed using the `newgrp` command, which temporarily switches the user’s active group for the current session.

## 1. File Creation

When you create a file (e.g., with `touch`), the ownership is set as follows:

- **Owner**: The user who creates the file.
- **Group**: The user’s current group (usually their primary group).

### Example:

```bash
# Create a file
touch file1.txt

# Check the file's ownership
ls -l file1.txt

# Sample output:
# -rw-r--r-- 1 user users 0 Oct 17 12:00 file1.txt
```

In this example, `user` is the owner and `users` is the group.

---

## 2. Changing the Group with `newgrp`

The `newgrp` command allows you to switch to a different group within your shell session. After switching, any files you create will belong to that group, while the **owner** remains unchanged.

### Example Workflow:

```bash
# Step 1: Check your current user ID and group
id
# Output might show the current group as 'users'

# Step 2: Create a new file, it will belong to your default group
touch file1.txt
ls -l file1.txt
# Output: -rw-r--r-- 1 user users ... file1.txt

# Step 3: Change the active group to 'developers' using newgrp
newgrp developers

# Step 4: Create another file
touch file2.txt
ls -l file2.txt
# Output: -rw-r--r-- 1 user developers ... file2.txt
```

---

### Explanation:

- **Before `newgrp`:** When `file1.txt` is created, it belongs to the user’s primary group, `users`.
- **After `newgrp developers`:** When `file2.txt` is created, it belongs to the new active group, `developers`, while the **owner** remains the same.

---

## 3. Viewing Available Groups

To view the groups that a user belongs to, use the `groups` command:

```bash
groups
# Output: users developers
```

This shows that the user is part of both the `users` and `developers` groups.

---


