

```bash
#!/bin/bash

# Prompt the user for a filename
echo "Inserisci il nome del file da creare"
read nome_file

# Try to create the file and redirect errors to /dev/null
touch $nome_file 2> /dev/null

# Check if the file was created successfully
if [ $? -eq 0 ]; then
    echo "Il file '$nome_file' è stato creato con successo."
else
    echo "Errore: Impossibile creare il file '$nome_file'."
fi
```

### Explanation:

1. **`touch $nome_file 2> /dev/null`**:
   - This command attempts to create the file. Any errors (e.g., insufficient permissions, invalid filename) are redirected to `/dev/null`, preventing them from being displayed.

2. **`if [ $? -eq 0 ]; then`**:
   - `$?` is a special variable that stores the exit status of the last command. If the `touch` command succeeds, `$?` will be `0`, and the script will print a success message.
   - If `$?` is not `0`, it indicates an error, and the script will print an error message.

---

### Benefits of This Approach:

- **Feedback to the User**: Now, the script informs the user if the file was created successfully or if an error occurred.
- **Error Handling**: This method helps the user understand when something goes wrong, improving the overall usability of the script.

