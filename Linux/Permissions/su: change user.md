
## `sudo su` Command in Linux

The `sudo su` command is used to switch the current user to the root user (superuser) while maintaining the user's environment. Below is a breakdown of its functionality and usage:

### What `sudo su` Does

- **`sudo`**: Stands for "superuser do." It allows a permitted user to execute a command as the superuser or another user, as specified by the security policy.
- **`su`**: Stands for "substitute user" or "switch user." When executed without any arguments, it defaults to switching to the root user.

### Usage Steps

1. **Open Terminal**: Launch your terminal application.
2. **Execute the Command**:
   ```bash
   sudo su
   ```
3. **Enter Your Password**: 
   After running the command, you will be prompted to enter your user password (not the root password). If your user account has permission to use `sudo`, you'll switch to the root user.

### Example

```bash
# Switch to root user
sudo su
```

### Important Notes

- **Root User Access**: When you successfully switch to the root user, you gain full administrative privileges, allowing any operation on the system. Use caution when running commands as root.
- **Exit Root Shell**: To return to your normal user shell, type `exit` or press `Ctrl + D`.

```bash
# Exit from root user
exit
```

### Differences from Other Commands

- **`sudo -i`**: Opens a new shell as the root user while initializing the root user's environment.
- **`su -`**: Similar to `sudo su`, but requires the root password and initializes the root environment.

### Conclusion

The `sudo su` command is a powerful tool for managing system administration tasks in Linux. It is particularly useful for users needing temporary elevated privileges to perform specific tasks or configurations. Always exercise caution when operating as the root user to avoid unintended system changes.

