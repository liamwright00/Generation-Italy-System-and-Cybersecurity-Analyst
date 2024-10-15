## Linux File and Directory Management Exercises

### Exercise 1: Creating Directories and Files, Listing Contents, and Using `cat`

**Objective:** Create directories and files, and list the contents.

1. **Create a directory named `progetto`:**

   mkdir progetto


2. **Create two files inside the `progetto` directory:**

   touch progetto/file1.txt progetto/file2.txt


3. **List the files in the `progetto` directory and redirect the output to a file:**

   ls progetto > progetto/file_list.txt


4. **Display the content of one of the files:**

   cat progetto/file1.txt


---

### Exercise 2: Copying, Moving, and Using `mv` and `cp`

**Objective:** Copy and move files.

1. **Copy `file1.txt` to the home directory and rename it:**

   cp progetto/file1.txt ~/file1_copia.txt


2. **Move `file2.txt` from the `progetto` directory to the home directory:**

   mv progetto/file2.txt ~/


3. **List the contents of the home directory and redirect both standard output and error output to a file:**

   ls ~> ~/directory_list.txt 2>&1


---

### Exercise 3: Removing Files and Directories, Using `rm` and `rmdir`

**Objective:** Remove files and directories.

1. **Remove the file `file1_copia.txt`:**

   rm ~/file1_copia.txt


2. **Remove the `progetto` directory:**

   rmdir progetto


3. **Check that the directory has been removed:**

   ls | grep progetto || echo "Directory 'progetto' has been removed."


---

This repository provides practical exercises to familiarize users with basic file and directory management commands in Linux. Each section includes clear steps for creating, copying, moving, listing, and deleting files and directories.
