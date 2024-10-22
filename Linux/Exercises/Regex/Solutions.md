
### 1. Find Processes Starting with "bash" (Easy)
```bash
pgrep '^bash'
```
This command searches for all processes that begin with the name "bash".

### 2. Find Processes Ending with "d" (Easy)
```bash
pgrep 'd$'
```
This command finds all processes whose names end with the letter "d".

### 3. Find Processes Starting with "s" and Ending with "d" (Medium)
```bash
pgrep '^s.*d$'
```
This command locates all processes that start with the letter "s" and end with the letter "d".

### 4. Find Processes Whose Name is Exactly "bash" (Medium)
```bash
pgrep '^bash$'
```
This command identifies processes whose names are exactly "bash", with no additional characters before or after.

### Running the Commands
To execute these commands, open a terminal and run each line individually. Here’s how you can do it:

1. Open a terminal.
2. Type or paste each command and press `Enter` to execute.
3. Observe the output to see the processes that match the specified criteria.

