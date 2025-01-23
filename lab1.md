# Lab Overview: Creating Files and Directories Using the touch Command

In this lab, we are practicing the creation of empty files and directories using the touch command, a basic and commonly used Linux/Unix command. The objective is to understand how to create multiple files at once, as well as how to organize them into subdirectories.

### Objective:
1. Create six files with the following naming conventions:
   - songX.mp3
   - snapX.jpg
   - filmX.avi
   Where X is a number ranging from 1 through 6.
   
2. Create three subdirectories to organize the files, named:
   - friends
   - family
   - work

3. Use a single command to create all three subdirectories simultaneously.

---

### Input Commands:

To achieve the above objectives, we used the following commands:

1. **Create files**:  
   
bash
   touch song{1..6}.mp3 snap{1..6}.jpg film{1..6}.avi

2. **Create subdirectories**
   
bash
   mkdir friends family work


3. **Organize files into subdirectoires**
   
bash
   mv song1.mp3 song2.mp3 song3.mp3 friends
   mv snap1.jpg snap2.jpg snap3.jpg family
   mv film1.avi film2.avi film3.avi work

---

### Expected Output:

1. The given six files will be created in our current directory.

2. Three new directories will be created.

3. The files will be moved into their respective subdirectories.
   
---

### Screenshots:

![image](https://github.com/user-attachments/assets/59844fde-0e13-429d-b15f-c236206bc3df)

![image](https://github.com/user-attachments/assets/8e31a1c9-87a1-4f35-9a71-f86af1a95297)

![image](https://github.com/user-attachments/assets/ceee828e-48e4-4d5d-94ac-dd36860bed1d)

![image](https://github.com/user-attachments/assets/f7378d5c-ec8d-478c-8e31-70a73df4e463)

