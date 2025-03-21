# Lab Overview: Writing Shell Scripts for System Information and Mathematical Calculations

In this lab, we will practice writing shell scripts to perform tasks such as printing system information, performing basic mathematical calculations, and using redirection operators to store command outputs. The objective is to understand scripting fundamentals and output redirection in Linux.

### Objective:
1. Write a shell script to print system information (e.g., hostname, OS, memory, disk usage).
2. Write a shell script to perform basic mathematical calculations (e.g., addition, subtraction, multiplication, division).
3. Use redirection operators (`>`, `>>`) to store the output of commands into files.

---

### Input Commands:

To achieve the above objectives, we used the following commands and scripts:

1. **Shell script to print system information**:
   
bash
   #!/bin/bash
   echo "System Information:"
   echo "Hostname: $(hostname)"
   echo "Operating System: $(uname -s)"
   echo "Memory Usage: $(free -h | grep Mem | awk '{print $3 "/" $2}')"
   echo "Disk Usage: $(df -h / | grep / | awk '{print $3 "/" $2}')"

2. **Shell script to perform basic mathematical calculations**:
   
bash
   #!/bin/bash
   echo "Enter two numbers:"
   read num1 num2
   echo "Addition: $(($num1 + $num2))"
   echo "Subtraction: $(($num1 - $num2))"
   echo "Multiplication: $(($num1 * $num2))"
   echo "Division: $(($num1 / $num2))"

3. **Using redirection operators to store output**:
   
bash
   ./system_info.sh > system_info.txt
   ./math_calculations.sh >> calculations.log

---

### Expected Output:

1. The `system_info.sh` script will display:
   - Hostname
   - Operating System
   - Memory Usage
   - Disk Usage

2. The `math_calculations.sh` script will:
   - Prompt for two numbers
   - Display the results of addition, subtraction, multiplication, and division

3. The output of the scripts will be stored in:
   - `system_info.txt` for system information
   - `calculations.log` for mathematical calculations

---

### Screenshots:

![image](https://github.com/user-attachments/assets/)

![image](https://github.com/user-attachments/assets/)

![image](https://github.com/user-attachments/assets/)

![image](https://github.com/user-attachments/assets/)
