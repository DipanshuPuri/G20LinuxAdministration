# Lab Overview: Editing Files with Vim and Nano

In this lab, we will use `vim` and `nano` to edit a text file, `editing_final_lab.txt`, using a shell variable. The goal is to explore text editing modes in Vim, practice visual mode, and modify file contents based on specific instructions.

### Objective:
1. Use `vim` and `nano` to edit the `editing_final_lab.txt` file.
2. Define and use the `lab_file` shell variable for the file.
3. Enter Vim’s visual mode.
4. Remove the last seven characters from the first column on the first line.
5. Preserve only the first four characters of the first column.

---

### Input Commands:

1. **Define the shell variable for the file**:  
   Define a variable for the file that you will edit. You can use the following command to store the file name in a shell variable:
   
   ```bash
   lab_file="editing_final_lab.txt"

2. **Edit the file with Vim**
   Use the vim command to open and edit the editing_final_lab.txt file:

   ```bash
   vim $lab_file

3. **Use Visual Mode in Vim**
   Enter visual mode to highlight text:
   Press v to start visual mode.
   Use the arrow keys to move the cursor and select the text that you want to delete or modify.

4. **Remove the last seven characters from the first column**
   In visual mode, select the last seven characters of the first column, and then delete them.
   Use the arrow keys to move the cursor to the beginning of the text you wish to delete.
   Press d to delete the selected text.

5. **Preserve only the first four characters of the first column**
   Use visual mode to select the first four characters of the first column.
   Press y to copy the selected characters.
   Paste them back in if needed.

6. **Edit the file using Nano**
   Alternatively, you can use nano to edit the same file:

   ```bash
   nano $lab_file
   ```
   Navigate through the file using the arrow keys and delete or modify the text as needed.

---

### Expected Output:

After performing the required operations
   ```bash
   abcd
   hijk
   opqr
   ```
   
