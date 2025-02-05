# 🛡 File Permissions in Linux  

## 📌 Project Overview  
This project explores file and directory permissions in Linux, focusing on how to view, modify, and secure files. Using Linux commands, I learned to:  

✅ Check file and directory details  
✅ Understand and interpret permission strings  
✅ Modify file and directory permissions with `chmod`  
✅ Secure hidden files by adjusting their access permissions  

These concepts are essential for Cybersecurity Analysts to protect system files and manage access control.  

---

## 🔍 Checking File and Directory Details  
To check the current directory and list files with their permissions, I used:  

- `pwd` – Displays the current working directory  
- `ls -l` – Lists files along with their permissions  
- `ls -la` – Lists all files, including hidden ones

<img src="https://i.imgur.com/VqPYfyW.png" alt="Linux File Permissions" width="600">

## Navigating to projects Directory
Listing the contents and permissions of the projects directory

<img src="https://i.imgur.com/VqPYfyW.png" alt="Linux File Permissions" width="600">



  

---

## 📝 Understanding File Permission Strings  
Each file has a permission string that looks like this:
<br>  <span style="color:red; font-weight:bold;">`-rw--w---- 1 researcher2 research_team   46 Feb  5 17:04 .project_x.txt`</span>
This string represents file ownership and access permissions for the user, group, and others.

---
## 🔧 Changing File Permissions
The goal here was to check to see if any files had write permissions for "others" and i found:
<br><span style="color:red; font-weight:bold;">`-rw-rw-rw- 1 researcher2 research_team   46 Feb  5 17:04 project_k.txt`</span> <br/>

To remove write permissions for others i used:
<br><span style="color:red; font-weight:bold;">`chmod o-w project_k.txt`</span> <br/>

As we can see now, others dont have write permission:
<img src="https://i.imgur.com/Q6pm9lY.png" alt="Linux File Permissions" width="600">

Similarly, I changed another file's permissions so only the user could read it:
<br><span style="color:red; font-weight:bold;">`chmod 440 .project_x.txt
`</span> <br/>

Now we can see it's updated to only "read" for everyone
<img src="https://i.imgur.com/4UqUOBR.png" alt="Linux File Permissions" width="600">


























