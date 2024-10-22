

## **Runlevels in Linux**

Runlevels are a traditional method of defining the state of a Unix-like operating system, indicating which services and processes should be running. Each runlevel corresponds to a specific operational mode for the system.

### **Base Runlevels (0 to 6)**

1. **Runlevel 0: Halt**
   - **Description:** Safely shuts down the system.
   - **Function:** Halts the machine.

2. **Runlevel 1: Single User Mode**
   - **Description:** Single-user mode, primarily for maintenance.
   - **Function:** Provides a minimal environment for administrative tasks. Only the root user has access, and most services are stopped.

3. **Runlevel 2: Multi-user without Networking**
   - **Description:** Allows multiple users to log in without starting networking services.
   - **Function:** Often used for local logins.

4. **Runlevel 3: Multi-user with Networking**
   - **Description:** Supports multiple users with network services.
   - **Function:** Common default runlevel for server environments.

5. **Runlevel 4: User-definable Mode**
   - **Description:** Not commonly used; can be configured for specific tasks.
   - **Function:** Reserved for custom configurations.

6. **Runlevel 5: Multi-user with GUI**
   - **Description:** Similar to runlevel 3, but with a graphical user interface.
   - **Function:** Starts a display manager for graphical login.

7. **Runlevel 6: Reboot**
   - **Description:** Safely restarts the system.
   - **Function:** Reboots the machine.

### **Managing Runlevels**

- **Changing Runlevels:**
   - You can change the current runlevel using the `init` or `telinit` command, followed by the desired runlevel number:
   ```bash
   sudo init 3  # Switch to runlevel 3
   ```

- **Viewing Current Runlevel:**
   - Use the `runlevel` command to see the current and previous runlevels:
   ```bash
   runlevel
   ```

### **Using the `who -r` Command**

The `who -r` command in Linux displays the current runlevel of the system along with additional information.

#### **Command:**
```bash
who -r
```

### **Output Explanation**

When you run `who -r`, you typically see output that includes:

1. **Runlevel:** Indicates the current runlevel of the system (e.g., 3, 5).
2. **Nrun:** Displays the number of the next runlevel if the system is in a transitional state.
3. **Time:** Shows when the current runlevel was set.
4. **User:** Indicates the user who executed the command that changed the runlevel (if applicable).
5. **State:** Shows the current state of the system, which could be "N" for normal operation, "S" for single-user mode, etc.

### **Example Output**
```
run-level 5  2024-10-17 12:00   previous run-level: 3
```

### **Conclusion**

The `who -r` command is useful for quickly checking the system's current operational state, especially in multi-user or server environments. If you have more questions about the command or related topics, feel free to ask!

