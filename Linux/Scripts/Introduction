

# Bash Automation Script Guide

This guide provides step-by-step instructions on how to create a basic automation script in Linux using Bash.

## Steps to Create and Run the Bash Script

### 1. Create the Script File

Use a text editor like `nano` to create a new script file. In this example, we will name the file `script.sh`.

```bash
nano script.sh
```

### 2. Add the Shebang (`#!/bin/bash`)

At the top of your script file, include the **shebang** line. This tells the system that the script should be executed with the Bash interpreter.

```bash
#!/bin/bash
```

### 3. Add Commands to Automate Tasks

Below the shebang, you can write commands to perform the tasks you want to automate. For example, the following script creates a directory, creates a file within that directory, sets permissions, and prints a confirmation message.

```bash
#!/bin/bash

# Example script for automating simple tasks

# Create a directory (if it doesn't exist)
mkdir -p /path/to/directory

# Create a file in the newly created directory
touch /path/to/directory/file.txt

# Set read and write permissions for the file
chmod 644 /path/to/directory/file.txt

# Display a message confirming the operation
echo "File created and permissions set!"
```

### 4. Save and Exit

Once you've added your commands, save and exit the file. If you're using `nano`, you can do this by:

- Pressing `CTRL + O` to write the changes.
- Pressing `CTRL + X` to exit the editor.

### 5. Make the Script Executable

To make the script executable, use the `chmod` command:

```bash
chmod +x script.sh
```

### 6. Verify the File's Permissions

To verify that the script has the appropriate permissions, use the `ls -l` command:

```bash
ls -l script.sh
```

The output should show the script with executable (`x`) permissions, like this:

```bash
-rwxr-xr-x 1 user user  date script.sh
```

### 7. Run the Script

Now you can execute the script by running:

```bash
./script.sh
```

### Example Script Summary

1. Create a script file using a text editor like `nano`.
2. Add the shebang line (`#!/bin/bash`).
3. Add your commands to automate tasks.
4. Make the script executable using `chmod +x`.
5. Run the script with `./script.sh`.



