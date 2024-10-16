- `find`: search commands and their directory
    - `find /etc -name hostname`: To find the `hostname` file in the `/etc` directory
    - The `find` command generates a lot of output related to files that it cannot access due to inadequate permissions. To suppress this type of output, redirect it to `/dev/null`, as shown in the example below. To find the `hostname` file in the `/etc` directory and also redirect the error stream, execute the following command:
        
        ```bash
        find /etc -name hostname 2>/dev/null
        ```
        
    - The `find` command has options to find files per their timestamps. To find all files in the `/etc` directory which were modified less than 2 days ago, execute the following command:
        
        ```bash
        find /etc -mtime -2 2>/dev/null
        ```
        
    - To find all files which were modified less than 30 minutes ago in the `/etc` directory, execute the following command:
        
        ```bash
        find /etc -mmin -30 2>/dev/null
        ```
        
    - To find files which are larger than 8MB in size, execute the following command:
        
        ```bash
        find / -size +8M 2>/dev/null
        ```
        
    - To find all empty files in your home directory, execute the following commands:
        
        ```bash
        touch sample
        find ~/ -empty 2>/dev/null
        ```
        
    - To display a count of all of the files in the `/etc` directory structure that end in `.conf`, execute the following command:
        
        ```
        find /etc -name "*.conf" 2>/dev/null | wc -l
        ```
        
    - To find all files starting with `hosts` in the `/etc` directory structure and display detailed information about the files, use the following command:
        
        ```
        find /etc -name "hosts*" -ls 2>/dev/null
        ```
        
    - To limit the depth that the find command searches, use the `-maxdepth` option:
        
        ```
        find /etc -name "*.conf" -maxdepth 1 2>/dev/null | wc -l
        ```
        
    - To find all files that are directory files in your home directory, execute the following commands:
        
        ```
        *mkdir dir1 dir2 dir3*
        find ~/ -type d 2>/dev/null
        ```
        
- The `-exec` option is used to execute a specific command using the results of `find` as the input. To find all files in your home directory that end in `.conf` and delete them with the `rm` command, execute the following commands:
    
    ```bash
    cp /etc/*.conf .
    ls
    find ~ -name "*.conf" –exec rm {} \;
    ls
    ```
    
- The `-ok` option is used to execute a specific command using the results of the `find` command as the input after confirming with the user. To find all files that end with the word `.conf` and then delete them interactively, execute the following commands:
    
    ```
    cp /etc/*.conf .
    ls
    find ~ -name "*.conf" –ok rm {} \;
    ```
    
    When prompted, type **y** to delete each directory interactively:
    
    ```
    < rm ... /home/sysadmin/debconf.conf > ?y
    ```
