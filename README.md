<h1>Changing File Permissions in Linux</h1>

<h2>Project Description</h2>
The research team at my organization needs to update the file permissions for certain files and directories within the projects directory. The permissions do not currently reflect the level of authorization that should be given. Checking and updating these permissions will help keep their system secure. To complete this task, I performed the following tasks.
<br />

<h2>Check file and directory details</h2>

The following code demonstrates how I used Linux commands to determine the existing permissions set for a specific directory in the file system. <br/>

<p align="center">
<img width="624" height="204" alt="image" src="https://github.com/user-attachments/assets/4475fdeb-1989-4718-afef-ebda0592ac72" />

<br />The first line of the screenshot displays the command I entered, and the other lines display the output. The code lists all contents of the projects directory. I used the ls command with the -la option to display a detailed listing of the file contents that also returned hidden files. The output of my command indicates that there is one directory named drafts, one hidden file named .project_x.txt, and five other project files. The 10-character string in the first column represents the permissions set on each file or directory.

<h2>Changing File Permissions</h2>
<br />
The organization determined that other shouldn't have write access to any of their files. To comply with this, I referred to the file permissions that I previously returned. I determined project_k.txt must have the write access removed for other.

The following code demonstrates how I used Linux commands to do this:
 <br/>
<p align="center">
<img width="624" height="216" alt="image" src="https://github.com/user-attachments/assets/5573cb31-8f10-4eaf-8af2-9343c08338b3" />

<br />
The first two lines of the screenshot display the commands I entered, and the other lines display the output of the second command. The chmod command changes the permissions on files and directories. The first argument indicates what permissions should be changed, and the second argument specifies the file or directory. In this example, I removed write permissions from other for the project_k.txt file. After this, I used ls -la to review the updates I made.
<br />
  
<h2>Changing Hidden Files</h2>
<p align="center">
<img width="624" height="219" alt="image" src="https://github.com/user-attachments/assets/05d5e156-93d8-4bb8-9278-ac4acc421393" />

<br />
<h2>Change directory permissions</h2>
<p align="center">
<img width="624" height="216" alt="image" src="https://github.com/user-attachments/assets/3ea06ecf-f716-4020-976f-cda2ec66132a" />

<h2>Summary</h2>
<br />I changed multiple permissions to match the level of authorization my organization wanted for files and directories in the projects directory. The first step in this was using ls -la to check the permissions for the directory. This informed my decisions in the following steps. I then used the chmod command multiple times to change the permissions on files and directories.
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
