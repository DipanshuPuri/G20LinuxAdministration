# Lab Overview: Managing File Permissions and Ownership Using `chown` and `chmod`

In this lab, we will practice managing file permissions and ownership in a Linux environment using the `chown` and `chmod` commands. The objective is to change file ownership, modify file permissions, and understand the impact of these changes.

### Objective:
1. Change the ownership of a file using the `chown` command.
2. Modify file permissions using the `chmod` command with different options.
3. Verify the changes in ownership and permissions.

---

### Input Commands:

To achieve the above objectives, we used the following commands:

1. **Change ownership of a file**:
   
bash
   sudo chown operator1:operator1 example.txt

2. **Change file permissions using symbolic mode**:
   
bash
   chmod u+rwx,g+rx,o+r example.txt

3. **Change file permissions using numeric mode**:
   
bash
   chmod 754 example.txt

4. **Verify ownership and permissions**:
   
bash
   ls -l example.txt

---

### Expected Output:

1. The ownership of `example.txt` will be changed to `operator1` for both user and group.
2. The file permissions will be updated to:
   - **Symbolic mode**: `rwxr-xr--` (user: read, write, execute; group: read, execute; others: read).
   - **Numeric mode**: `754` (user: read, write, execute; group: read, execute; others: read).
3. The `ls -l` command will display the updated ownership and permissions for `example.txt`.

---

### Screenshots:

![image](https://github.com/user-attachments/assets/)

![image](https://github.com/user-attachments/assets/)

![image](https://github.com/user-attachments/assets/)

![image](https://github.com/user-attachments/assets/)
