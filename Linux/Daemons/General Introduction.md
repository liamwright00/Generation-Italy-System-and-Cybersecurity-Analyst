### **Daemons in Linux**

1. **Definition**:
    - Daemons are background processes that manage system services and perform tasks without direct user interaction. They are essential for ensuring that the system operates smoothly.
2. **Naming Convention**:
    - Daemons often start with a **K** or **S** in their runlevel scripts:
        - **K**: Indicates scripts for stopping services (Kill).
        - **S**: Indicates scripts for starting services (Start).
    - For example, a script named `K01service` would stop the service associated with it, and `S99service` would start it.
3. **Location of Daemons**:
    - Daemon scripts are usually found in the `/etc/rc.d/` directory, where different runlevels (levels of system operation) can manage the starting and stopping of services.
4. **Service Management with systemctl**:
    - Modern Linux systems use **systemd** as the init system to manage daemons and services. The `systemctl` command is used to control these services:
        - To view currently running services and their associated daemons, use:
            
            ```bash
            systemctl --type=service --state=running
            
            ```
            
        - This command provides a list of active services along with their statuses, helping you understand which daemons are currently operating on your machine.
5. **Service Configuration**:
    - The `chkconfig` command can display which services are stopped or started at specific runlevels. It helps in managing service startup behavior across different system states.

### **Examples of Common Commands**:

- **To start a service**:
    
    ```bash
    sudo systemctl start <service-name>
    
    ```
    
- **To stop a service**:
    
    ```bash
    sudo systemctl stop <service-name>
    
    ```
    
- **To enable a service to start at boot**:
    
    ```bash
    sudo systemctl enable <service-name>
    
    ```
    
- **To disable a service from starting at boot**:
    
    ```bash
    sudo systemctl disable <service-name>
    
    ```
    
