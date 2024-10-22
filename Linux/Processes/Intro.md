In Linux, the kernel manages processes efficiently. Although the CPU can execute only one process at a time, it maintains a queue of processes, allocating time slices for each to perform its tasks. This scheduling allows multiple processes to run concurrently, creating the illusion of simultaneous execution. Each process is given a specific time to execute, ensuring effective CPU utilization while managing system resources.

- The `ps` command in Linux is used to display information about currently running processes. It provides various details, including:
    - **PID (Process ID)**: A unique identifier for each process.
    - **TTY (Terminal Type)**: The terminal associated with the process.
    - **TIME**: The total CPU time used by the process.
    - **CMD**: The command that started the process.
        
        To view all processes, you can use `ps aux` for a detailed listing. This command helps in monitoring and managing system processes effectively. Or `ps -ef` to see all processes.
        
    
- The `pgrep` command in Linux is used to search for processes based on their names and other attributes. It returns the Process IDs (PIDs) of the processes that match the specified criteria, making it useful for managing and interacting with processes. For example, `pgrep firefox` will return the PIDs of all running instances of the Firefox browser. You can also use options to refine your search, such as matching against the user or specifying regular expressions.
    - Here’s a breakdown of the `pgrep` command examples you mentioned:
        1. **`pgrep ls`**: This command returns the PIDs of all processes with the name "ls".
        2. **`pgrep -l ls`**: This includes the process names along with their PIDs for any processes named "ls".
        3. **`pgrep -u liam`**: This returns the PIDs of all processes owned by the user "liam".
        4. **`pgrep -i`**: This option allows case-insensitive matching for process names.
        5. To use `pgrep` with a regex that matches exactly the `bash` process, the shortened command is:
            
            ```bash
            pgrep '^bash$'
            
            ```
            
            This will return the process IDs (PIDs) of all processes named exactly `bash`, without the process names. If you need the names as well, you can add the `-l` flag:
            
            ```bash
            pgrep -l '^bash$'
            
            ```
            
    
- To continuously monitor processes in Linux, you can use the `watch` command in combination with a command like `ps` or `top`. Here are two examples:
    1. **Using `watch` with `ps`**:
        
        ```bash
        watch -n 2 'ps aux'
        ```
        
        This command updates the process list every 2 seconds.
        
    2. **Using `watch` with `top`**:
        
        ```bash
        watch -n 2 top
        ```
        
        This command refreshes the `top` output every 2 seconds.
        
    
    These commands help you keep track of system processes in real time.