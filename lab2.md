# Lab Overview: Exploring `gedit` Man Page and `ext4` File-System Tuning

In this lab, we will explore the `gedit` man page, find the appropriate command for tuning `ext4` file-system parameters, and practice brace expansion to generate strings.

### Objective:
1. View the man page for the `gedit` command.
2. Use the `man -k ext4` command to search for a command to tune `ext4` file-system parameters.
3. Understand and demonstrate brace expansion to generate discretionary strings of characters.

---

### Input Commands:

1. **View the man page for `gedit`**:  
   To view the manual page for the `gedit` command, use the following command:
   
   ```bash
   man gedit

1. **Search for ext4 related tuning commands**:  
   Use the man -k ext4 command to search for all commands related to tuning ext4 file-system parameters:
   
   ```bash
   man -k ext4

1. **Brace Expansion**:  
   Demonstrate brace expansion with a sequence and a list:
   
   ```bash
   echo file{1..5}.txt

---

### Expected Output:

1. The output of man gedit will show you the manual page for gedit.

2. The output of man -k ext4 will list relevant man pages related to ext4.

3. The output of the brace expansion examples will be the expansion of the given patterns, such as file1.txt file2.txt file3.txt file4.txt file5.txt for the first example.
