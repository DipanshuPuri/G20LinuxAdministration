# Lab Overview: Managing Processes and Software with `ps`, `top`, `kill`, and `apt-get` Commands

In this lab, we will practice managing processes and software on a Linux system using the `ps`, `top`, `kill`, and `apt-get` commands. The objective is to understand how to monitor, control, and manage processes, as well as how to install, update, and remove software packages using the `apt-get` command.

### Objective:
1. **Monitor processes** using the `ps` and `top` commands.
2. **Terminate processes** using the `kill` command.
3. **Install, update, and remove software** using the `apt-get` command.

---

### Input Commands:

To achieve the above objectives, we will use the following commands:

1. **Monitor processes**:
   
   - **List all running processes**:
     
     ```bash
     ps aux
     ```
   
   - **Display real-time system processes**:
     
     ```bash
     top
     ```

2. **Terminate processes**:
   
   - **Find the Process ID (PID) of a specific process** (e.g., `firefox`):
     
     ```bash
     pidof firefox
     ```
   
   - **Terminate a process using its PID**:
     
     ```bash
     kill <PID>
     ```
   
   - **Forcefully terminate a process**:
     
     ```bash
     kill -9 <PID>
     ```

3. **Install, update, and remove software**:
   
   - **Update the package list**:
     
     ```bash
     sudo apt-get update
     ```
   
   - **Upgrade installed packages**:
     
     ```bash
     sudo apt-get upgrade
     ```
   
   - **Install a software package** (e.g., `htop`):
     
     ```bash
     sudo apt-get install htop
     ```
   
   - **Remove a software package** (e.g., `htop`):
     
     ```bash
     sudo apt-get remove htop
     ```
   
   - **Remove a software package and its configuration files**:
     
     ```bash
     sudo apt-get purge htop
     ```
   
   - **Remove unused packages**:
     
     ```bash
     sudo apt-get autoremove
     ```

---

### Expected Output:

1. **Monitor processes**:
   - The `ps aux` command will display a list of all running processes.
   - The `top` command will show real-time system processes, including CPU and memory usage.

2. **Terminate processes**:
   - The `pidof` command will return the PID of the specified process.
   - The `kill` command will terminate the process with the given PID.
   - The `kill -9` command will forcefully terminate the process.

3. **Install, update, and remove software**:
   - The `sudo apt-get update` command will update the package list.
   - The `sudo apt-get upgrade` command will upgrade installed packages.
   - The `sudo apt-get install` command will install the specified software package.
   - The `sudo apt-get remove` command will remove the specified software package.
   - The `sudo apt-get purge` command will remove the software package and its configuration files.
   - The `sudo apt-get autoremove` command will remove unused packages.

---

### Screenshots:

1. **Output of `ps aux`**:
   
   ![image](https://github.com/user-attachments/assets/ps-aux-output.png)

2. **Output of `top`**:
   
   ![image](https://github.com/user-attachments/assets/top-output.png)

3. **Output of `apt-get` commands**:
   
   ![image](https://github.com/user-attachments/assets/apt-get-output.png)

---

### Notes:
- Ensure you have the necessary permissions to execute commands with `sudo`.
- Be cautious when using the `kill` command, especially with the `-9` option, as it forcefully terminates processes.
- Always double-check the package name before installing or removing software to avoid unintended actions.

This lab provides a hands-on approach to managing processes and software on a Linux system, which are essential skills for system administrators and developers.
