

### Script 1: "Creating a File and Setting Permissions"
**Task:**
- Create a directory called `progetto` in your home directory.
- Inside it, create a file named `bozza.txt` containing the sentence "This is a draft of the project."
- Change the permissions of the file so that only the user can read and modify it.
- Change the umask so that newly created files have permissions `rw-r--r--` for the user.
- Verify the permissions with `ls -l`.

### Script 2: "Project Backup"
**Task:**
- Create a directory called `lavoro` in your home directory.
- Inside, create two files named `file1.txt` and `file2.txt`, containing any text.
- Set the umask so that newly created files have permissions `rw-------`.
- Then, create a backup of these files in a new directory called `backup`.
- Add a log that records the backup operation (reporting the date and time) in a file called `log.txt` inside the backup folder.
- Ignore any errors due to lack of permissions during the copy.

### Script 3: "Secure Moving and Cleanup"
**Task:**
1. Create a directory called `documenti` in your home directory.
2. Inside `documenti`, create three text files: `relazione.txt`, `calcoli.txt`, and `appunti.txt`, with any text of your choice.
3. Move the file `calcoli.txt` to a new directory called `archivio`.
4. Verify that the file has been successfully moved. If the file no longer exists in `documenti`, log the move operation in a log file called `spostamenti.log` inside `archivio`, including the date and time.
5. Remove the file `appunti.txt` and verify that it has been deleted correctly. If so, log the operation in the log file.
6. Change the permissions of the files in `archivio` to make the file `calcoli.txt` readable and writable only by the user and readable by others, while `spostamenti.log` will be readable only by the user.

