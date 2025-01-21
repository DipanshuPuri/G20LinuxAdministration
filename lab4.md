# Lab Overview: File Permissions and umask Configuration

In this lab, we will practice creating directories, modifying file permissions, and setting up the default umask for users. We will explore both symbolic and octal methods for changing file permissions, and demonstrate how to configure the `umask` for a specific user to control file access.

### Objective:
1. Create the `/home/consultants` director
2. Add write permission to the `consultants` group using the symbolic method.
3. Forbid others from accessing files in the `/home/consultants` directory using the octal method.
4. Change the default `umask` for the `operator1` user to prohibit all access for users that are not in their group.
5. Confirm that the `umask` is changed.

---

### Input Commands:

1. **Create the `/home/consultants` directory**:  
   Use the `mkdir` command to create the directory `/home/consultants`:
   
   ```bash
   sudo mkdir /home/consultants

2. **Add write permission to the consultants group using the symbolic method**
  Use the chmod command to add write permission to the consultants group for the /home/consultants directory. This can be done using the symbolic method (g+w):

  ```bash
  sudo chmod g+w /home/consultants
  ```

3. **Forbid others from accessing files in the /home/consultants directory using the octal method**
   Use the chmod command with the octal method (chmod 770) to set the permissions for /home/consultants so that others cannot access the directory:

   ```bash
   sudo chmod 770 /home/consultants

4. **Change the default umask for the operator1 user**
   To change the default umask for the operator1 user, edit their profile configuration file (such as .bashrc or .profile depending on the shell). Add or modify the line to set the umask value to 0770:

   ```bash
   sudo nano /home/operator1/.bashrc
   ```
   Add the following line at the end of the file:
   umask 0770

5. **Confirm that the umask is changed**
   To confirm that the umask has been successfully changed, log in as operator1 and run the following command to display the current umask setting:

   ```bash
   umask
   ```

---

### Expected Output:   

1. Created the After creating the /home/consultants directory.

2. Add write permission to the consultants group.

3. Forbid others from accessing the /home/consultants directory.

4. Change the default umask for operator1.
