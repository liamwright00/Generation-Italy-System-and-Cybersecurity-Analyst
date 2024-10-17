

# `ls -lh` and `id` Commands in Linux

## 1. `ls -lh` Command

The `ls -lh` command in Linux is used to list files and directories with detailed information in a **human-readable** format.

### Command Breakdown:

- **`-l`**: Displays files in long format, providing information such as permissions, number of links, owner, group, file size, and modification date.
- **`-h`**: Converts file sizes into a human-readable format (e.g., KB, MB, GB), instead of showing them in bytes.

### Usage Example:

```bash
ls -lh
```

### Sample Output:

```bash
-rw-r--r-- 1 liam users 4.0K Oct 17 2024 file1.txt
drwxr-xr-x 2 liam users 4.0K Oct 17 2024 my_directory
lrwxrwxrwx 1 liam users   12 Oct 17 2024 my_link -> /etc/file.txt
```

### Output Breakdown:

1. **File/Directory Type and Permissions**:  
   - `-rw-r--r--`: Regular file with read and write permissions for the owner, and read-only permissions for the group and others.
   - `drwxr-xr-x`: A directory where the owner has full control (read, write, execute), and others have read and execute permissions.
   - `lrwxrwxrwx`: A symbolic link where everyone has full permissions (this applies to the link itself, not its target).

2. **Number of Links**:  
   - `1`: Number of hard links to the file.

3. **Owner and Group**:  
   - `liam`: The owner of the file.
   - `users`: The group to which the owner belongs.

4. **File Size**:  
   - `4.0K`: The size of the file, in kilobytes (KB).

5. **Last Modified Date**:  
   - `Oct 17 2024`: The date and time the file was last modified.

6. **File Name**:  
   - `file1.txt`: The name of the file.

---

## 2. `id` Command

The `id` command in Linux displays information about the user’s identity, including the user ID (UID), group ID (GID), and group memberships.

### Command Usage:

```bash
id
```

### Sample Output:

```bash
uid=1000(liam) gid=1000(users) groups=1000(users),27(sudo),1001(developers)
```

### Output Breakdown:

1. **User ID (UID)**:  
   - `uid=1000(liam)`: The user ID is `1000`, and the username is **liam**.

2. **Group ID (GID)**:  
   - `gid=1000(users)`: The group ID is `1000`, and the primary group is **users**.

3. **Group Memberships**:  
   - `groups=1000(users),27(sudo),1001(developers)`: The user is part of additional groups like **sudo** (for administrative tasks) and **developers** (custom group).

