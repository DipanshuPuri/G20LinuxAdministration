# Lab Overview: Process Management and Software Management

In this lab, we will explore process management using commands like `ps`, `top`, and `kill`, and practice installing, updating, and removing software packages using the `apt-get` command.

### Objective:
1. Monitor and manage processes using `ps`, `top`, and `kill`.
2. Install, update, and remove software using `apt-get`.

---

### Input Commands:

1. **Monitor processes with `ps` and `top`**:  
   Use the `ps aux` command to list all processes with details, and `top` to view real-time system resource usage:

   ```bash
   ps aux
   top

2. **Manage processes with kill**
   Find the process ID (PID) from ps aux or top, and use the kill command to terminate it:

   ```bash
   kill <PID>

3. **Install, update, and remove software with apt-get**
   To install, update, or remove software, use the following commands:

   ```bash
   sudo apt-get install <package-name>
   sudo apt-get update
   sudo apt-get upgrade
   sudo apt-get remove <package-name>
   ```

---

### Expected Output:

1. After running ps aux:
A list of all processes running on the system with details like PID, user, and resource usage.

2. After running top:
A real-time display of CPU and memory usage, with an update every few seconds.

3. After running kill <PID>:
The specified process will be terminated, and you will return to the command prompt.

4. After running apt-get commands:
Depending on the operation (install, update, or remove), you will see a series of messages confirming the action, such as downloading and installing packages, or removing them.
