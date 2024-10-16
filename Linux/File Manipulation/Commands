

### `ls`

Use the `ls` command to list files and directories.  
**Example**: 
```bash
ls -h
```
This option displays file sizes in a human-readable format.

#### `ls -l` Output Summary Table

| **Column**                  | **Description**                                                                                   |
|-----------------------------|---------------------------------------------------------------------------------------------------|
| **File Type & Permissions** | Indicates the file type (e.g., `d` for directory or `-` for a file) and permissions (e.g., `rwxr-xr-x`). |
| **Number of Links**         | Shows the number of hard links to the file or directory.                                         |
| **Owner**                   | Displays the username of the file or directory owner.                                            |
| **Group**                   | Shows the group name associated with the file or directory.                                      |
| **File Size**               | Indicates the size of the file in bytes or a human-readable format.                             |
| **Modification Date**       | Displays the last modified date and time (e.g., `Oct 21 12:04`).                                |
| **File/Directory Name**     | The name of the file or directory.                                                               |

### Example Breakdown

For an entry like:
```
drwxr-xr-x 2 user group 4096 Oct 21 12:04 directory_name
```
- **d**: Directory
- **rwxr-xr-x**: Owner has full permissions; group can read and execute; others can read.
- **2**: Two links to this directory.
- **user**: Owner of the directory.
- **group**: Group associated with the directory.
- **4096**: Size of the directory in bytes.
- **Oct 21 12:04**: Last modified on October 21 at 12:04.
- **directory_name**: Name of the directory.

This table provides a quick reference for understanding the output of the `ls -l` command.

---

### `mkdir`

Creates a new directory.

**Example**:
```bash
mkdir -p progetto/cartella1
```
The command above creates the directory `cartella1` inside the parent directory `progetto`, creating both if they don’t exist. The `-p` option prevents errors if the parent directory already exists.

---

### `rmdir`

Deletes empty directories.

**Example**:
```bash
rmdir directory_name
```
This command deletes the specified empty directory. 

To delete directories with content, use:
```bash
rm -r directory_name
```

---

### `mv`

Moves or renames files or directories.

**Usage**:
- **Move File**: Takes two arguments: the file to move and the destination.
    ```bash
    mv source_file destination_directory/
    ```
- **Rename File**:
    ```bash
    mv old_filename new_filename
    ```

---

### `touch`

Creates a new file or updates the timestamp of an existing file.

**Example**:
```bash
touch newfile.txt
```
This command creates an empty file named `newfile.txt` or updates the timestamp if it already exists.

---

### `cp`

Copies files or directories. Takes two arguments: the source and the destination.

**Example**:
```bash
cp source_file destination_directory/
```
This command copies `source_file` to `destination_directory`.

---
