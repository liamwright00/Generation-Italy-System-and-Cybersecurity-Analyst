In Linux, process priority is managed using the **nice** value, which ranges from -20 (highest priority) to 19 (lowest priority). A lower nice value indicates a higher priority for CPU time, while a higher nice value allows other processes to get more CPU time.

You can view a process's priority with the `ps` command, modify it using the `nice` command when starting a process, or change an existing process's priority using the `renice` command.

For example:

- Start a process with a higher priority:
    
    ```bash
    nice -n -5 your_command
    ```
    
- Change an existing process's priority:
    
    ```bash
    renice 10 -p [PID]
    ```