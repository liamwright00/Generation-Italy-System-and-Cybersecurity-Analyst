

### Script 1: "Creating a File and Setting Permissions"

```bash
#!/bin/bash

# Create a directory called 'progetto' in the home directory
mkdir -p ~/progetto

# Create a file named 'bozza.txt' and add content to it
echo "This is a draft of the project." > ~/progetto/bozza.txt

# Change the permissions of the file so that only the user can read and write it
chmod 600 ~/progetto/bozza.txt

# Change the umask so that new files have permissions rw-r--r--
umask 0022

# Verify the permissions
ls -l ~/progetto/bozza.txt
```

### Script 2: "Project Backup"

```bash
#!/bin/bash

# Create a directory called 'lavoro' in the home directory
mkdir -p ~/lavoro

# Create two files named 'file1.txt' and 'file2.txt' with some text
echo "This is the content of file 1." > ~/lavoro/file1.txt
echo "This is the content of file 2." > ~/lavoro/file2.txt

# Set the umask so that new files have permissions rw-------
umask 0077

# Create a backup directory
mkdir -p ~/lavoro/backup

# Copy the files to the backup directory, ignoring errors
cp ~/lavoro/file1.txt ~/lavoro/backup/ 2>/dev/null
cp ~/lavoro/file2.txt ~/lavoro/backup/ 2>/dev/null

# Log the backup operation with the date and time
echo "$(date): Backup completed." >> ~/lavoro/backup/log.txt
```

### Script 3: "Secure Moving and Cleanup"

```bash
#!/bin/bash

# Create a directory called 'documenti' in the home directory
mkdir -p ~/documenti

# Create three text files in 'documenti'
echo "This is the report." > ~/documenti/relazione.txt
echo "These are the calculations." > ~/documenti/calcoli.txt
echo "These are my notes." > ~/documenti/appunti.txt

# Move 'calcoli.txt' to a new directory called 'archivio'
mkdir -p ~/archivio
mv ~/documenti/calcoli.txt ~/archivio/

# Verify that 'calcoli.txt' has been moved
if [ ! -f ~/documenti/calcoli.txt ]; then
    echo "$(date): calcoli.txt has been moved to archivio." >> ~/archivio/spostamenti.log
fi

# Remove 'appunti.txt' and verify deletion
rm ~/documenti/appunti.txt
if [ ! -f ~/documenti/appunti.txt ]; then
    echo "$(date): appunti.txt has been deleted." >> ~/archivio/spostamenti.log
fi

# Change permissions for files in 'archivio'
chmod 640 ~/archivio/calcoli.txt
chmod 600 ~/archivio/spostamenti.log
```

### Instructions to Run the Scripts

1. **Save Each Script**: Create three separate `.sh` files for each script (e.g., `script1.sh`, `script2.sh`, `script3.sh`).

2. **Make the Scripts Executable**: Run the following command in your terminal for each script:
   ```bash
   chmod +x script1.sh
   chmod +x script2.sh
   chmod +x script3.sh
   ```

3. **Run the Scripts**: Execute each script with:
   ```bash
   ./script1.sh
   ./script2.sh
   ./script3.sh
   ```

### Explanation of the Scripts
- **Script 1** creates a directory and a draft file, sets permissions so only the user can read and write, and verifies permissions.
- **Script 2** creates a working directory and files, sets umask for permissions, creates a backup, and logs the backup operation.
- **Script 3** creates a documents directory, files, moves one file to an archive, logs operations, removes another file, and sets permissions.
