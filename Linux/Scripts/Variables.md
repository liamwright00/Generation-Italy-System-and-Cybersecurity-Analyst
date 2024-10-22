

# Example of Variable Substitution in a Backup Script

```bash
#!/bin/bash

# Create a variable named DATA to store the current date
DATA=$(date +%Y-%m-%d)

# Create a directory for the backup, with the current date as part of its name
mkdir backup_$DATA

# Copy the file 'dati.txt' into the newly created backup directory
cp dati.txt backup_$DATA
```

### Explanation:

1. **`DATA=$(date +%Y-%m-%d)`**:
   - The `$(...)` syntax captures the output of a command and stores it in a variable. In this case, the `date` command is used to format the current date as `YYYY-MM-DD`, and this formatted date is stored in the `DATA` variable.
   - This makes it easy to create backups with a timestamp, ensuring that files and directories are uniquely named based on the date they are created.

2. **`mkdir backup_$DATA`**:
   - The `$DATA` variable is substituted with the value it holds (the current date), and this creates a directory with the name `backup_YYYY-MM-DD`. The underscore `_` separates "backup" from the date, making the directory name readable and organized.
   
3. **`cp dati.txt backup_$DATA`**:
   - This copies the file `dati.txt` into the newly created backup directory. The use of the `$DATA` variable ensures that each day's backup is stored in a different directory, preventing file overwrites and ensuring that a history of backups is maintained.

---

### Key Concepts of Variable Substitution

- **Dynamic Values**: With variable substitution, you can use dynamic values like dates or user inputs to manage files or directories in an automated and efficient manner.
  
- **Command Substitution**: The `$(command)` syntax runs the command inside the parentheses and assigns the output to a variable. This is commonly used with commands like `date`, `hostname`, `whoami`, etc.
  
- **Variables in Filenames**: By incorporating variables into filenames and directory names (e.g., `backup_$DATA`), you can create more flexible and automated scripts for tasks like backups, logging, or organizing files.

### Example Customization

You can modify the date format to include the time, for example:

```bash
DATA=$(date +%Y-%m-%d_%H-%M-%S)
```

This would include the hours, minutes, and seconds in the `DATA` variable, resulting in more precise timestamping.

### Best Practices

- **Error Handling**: If a command fails (e.g., `mkdir` or `cp`), the script might continue running unless handled explicitly. You can add error handling like:

    ```bash
    if [ $? -ne 0 ]; then
      echo "Error occurred. Exiting."
      exit 1
    fi
    ```

- **Automation**: Variable substitution is especially useful in automation tasks for system administration, data backup, and file management.

