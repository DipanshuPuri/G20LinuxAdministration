# Lab Overview: Managing User Accounts in Linux

In this lab, we will practice creating and managing user accounts in a Linux environment. The objective is to create multiple users, set their passwords, update user comments, and remove a user from the system.

### Objective:
1. Create the `operator1` user and confirm its existence.
2. Set the password for `operator1`.
3. Create additional users `operator2` and `operator3` and set their passwords.
4. Update the comment for the `operator1` user account using the `usermod -c` command.
5. Remove the `operator3` user from the system.

---

### Input Commands:

To achieve the above objectives, we used the following commands:

1. **Create `operator1` user and set password**:
   
bash
   sudo useradd operator1
   sudo passwd operator1

2. **Create `operator2` and `operator3` users and set passwords**:
   
bash
   sudo useradd operator2
   sudo passwd operator2
   sudo useradd operator3
   sudo passwd operator3

3. **Update the comment for `operator1`**:
   
bash
   sudo usermod -c "Primary Operator" operator1

4. **Remove `operator3` user**:
   
bash
   sudo userdel operator3

---

### Expected Output:

1. The `operator1`, `operator2`, and `operator3` users will be created.
2. Passwords will be set for all three users.
3. The comment for `operator1` will be updated to "Primary Operator".
4. The `operator3` user will be removed from the system.

---

### Screenshots:

![image](https://github.com/user-attachments/assets/59844fde-0e13-429d-b15f-c236206bc3df)

![image](https://github.com/user-attachments/assets/8e31a1c9-87a1-4f35-9a71-f86af1a95297)

![image](https://github.com/user-attachments/assets/ceee828e-48e4-4d5d-94ac-dd36860bed1d)

![image](https://github.com/user-attachments/assets/f7378d5c-ec8d-478c-8e31-70a73df4e463)
