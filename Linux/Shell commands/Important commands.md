
# Command Overview

## Basic Syntax
```bash
command [options] [arguments]
```
This is the general syntax for executing commands in the terminal.

### 1. `uname`
Displays system information.

| **Short Option** | **Long Option** | **Prints**                |
|------------------|------------------|---------------------------|
| -a               | --all            | All information           |
| -s               | --kernel-name    | Kernel name               |
| -n               | --node-name      | Network node name         |
| -r               | --kernel-release  | Kernel release            |
| -v               | --kernel-version  | Kernel version            |
| -m               | --machine        | Machine hardware name     |
| -p               | --processor      | Processor type or unknown |
| -i               | --hardware-platform | Hardware platform or unknown |
| -o               | --operating-system | Operating system         |
|                  | --help           | Help information          |
|                  | --version        | Version information       |

### 2. `man`
Accesses the manual pages for commands.

**Commands:**
- `man -f name`: Matches a command name.
- `man -k keyword`: Matches a keyword.

**Navigation**: Use `H` or `Shift+h` for movement commands within the man page.

**Pagers**: Common pagers are `less` (most used) and `more`.

### 3. SYNOPSIS Section
Provides command usage guidelines, indicating optional features with square brackets.

**Example for `cal`:**
```bash
cal [-3hjy] [-A number] [-B number] [[month] year]
```

**Example for `date`:**
```bash
date [OPTION]... [+FORMAT]
date [-u|--utc|--universal] [MMDDhhmm[[CC]YY][.ss]]
```

### 4. Searching Man Pages
- Use `/` followed by the search term to locate keywords.
- Use `N` to find the next match and `Shift+N` for the previous one.

### 5. Man Page Sections
There are nine default sections:
1. Executable programs or shell commands
2. System calls
3. Library calls
4. Special files (in `/dev`)
5. File formats and conventions
6. Games
7. Miscellaneous (including macro packages)
8. System administration commands
9. Kernel routines

**Example for Configuration File:**
```bash
man 5 passwd
```
This command accesses the man page for `/etc/passwd`, covering file format and structure.

### 6. `ls`
Lists the contents of directories.

**Options:**
- Short: `-l` for long format, `-r` for reverse order.
- Long: `--all` for all files.

### 7. `exec`
Replaces the current shell with a command.

**Use**: Optimizes resource usage by not running an intermediate shell.  
**Example**: Redirects input/output in scripts.

### 8. `alias`
Creates shortcuts for commands.

**Example:**
```bash
alias c=clear
```
To make it permanent, add it to `.bashrc`.

### 9. `pwd`
Displays the current working directory.

### 10. `touch`
Creates an empty file or updates the timestamp of an existing file.

### 11. `cd`
Changes the current directory.

### 12. `cp`
Copies files and directories.

**Example:**
```bash
cp /etc/hosts myhosts
```

### 13. `rm`
Removes files or directories.

**Example**: `rm -r` deletes directories and their contents.

### 14. `rmdir`
Deletes empty directories.

---

