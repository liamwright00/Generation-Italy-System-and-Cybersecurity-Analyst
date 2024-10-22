In Linux, variables can be either **local** or **global** (environment) variables:

1. **Local variables**: These are only accessible within the shell or script in which they are defined. They are not passed to any child processes. For example:
    
    ```bash
    name="Liam"
    
    ```
    
2. **Global (environment) variables**: These are accessible system-wide, meaning they can be inherited by child processes and other shells. They are created using `export`:
    
    ```bash
    export name="Liam"
    
    ```
    

To remove a variable, you can use the `unset` command.