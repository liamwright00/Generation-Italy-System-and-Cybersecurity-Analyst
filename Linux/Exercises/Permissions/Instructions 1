

#### Step 1: Creating the directory structure
- Create a directory called `progetto` in the `/home/utente` directory.
- Inside the `progetto` directory, create two subdirectories named `src` and `backup`.

#### Step 2: Creating files and content
- Move into the `src` directory and create an empty file called `main.c`.
- Create another file called `README.txt` and write the phrase "Progetto di gestione file" inside it.

#### Step 3: Setting up variables
- Create an environment variable called `PROGETTO_PATH` and assign it the path to the `progetto` directory.
- Verify that the variable has been set correctly.

#### Step 4: Setting permissions
- Set the permissions of the `src` directory so that the owner has read, write, and execute permissions; the group and others have only read and execute permissions.
- Set the permissions of `main.c` and `README.txt` so that only the owner has read and write permissions, while the group and others have no permissions.

#### Step 5: Creating a backup
- Copy the `main.c` file from the `src` directory to the `backup` directory.
- Verify that the copy was made correctly.

#### Step 6: Moving and renaming files
- Move the `README.txt` file from the `src` directory to the `backup` directory and rename it to `INFO.txt`.

#### Step 7: Setting the umask value
- Set the `umask` value to `027`, so that newly created files have restrictive permissions (the owner has all permissions, the group has only read permission, and others have no permissions).
- Create a new file called `config.ini` in the `backup` directory and verify the permissions assigned automatically.

#### Step 8: Creating links
- Create a hard link to the `main.c` file (located in `src`) in the `backup` directory.
- Create a soft link called `link_main` that points to the `main.c` file in the `src` directory.

#### Step 9: Removing files and directories
- Remove the `config.ini` file from the `backup` directory.
- Delete the `src` directory and all of its contents, but only after removing the files inside.

#### Step 10: Final verification
- Check the structure of the directories and the final permissions of the files inside the `progetto` directory to ensure everything was executed correctly. 

