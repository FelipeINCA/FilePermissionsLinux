# File Permissions in Linux
<body>
  <a>**File permissions in Linux
Project description
Authorization is the concept of granting access to specific resources in a system. It's important because without authorization any user could access and modify all files belonging to other users or system files. This would certainly be a security risk.
In Linux, file and directory permissions are used to specify who has access to specific files and directories. You’ll explore file and directory permissions and change the ownership of a file and a directory to limit who can access them.
As a security analyst, setting appropriate access permissions is critical to protecting sensitive information and maintaining the overall security of a system
Check file and directory details
TASK 1: In this task, you must explore the permissions of the projects directory and the files it contains. The lab starts with /home/researcher2 as the current working directory. This is because you're changing permissions for files and directories belonging to the researcher2 user.

The command ls displays the names of files and directories in the current working directory, in addition to the command -l shows the permissions of any file or directory.
Describe the permissions string
a 10-character string begins each entry and indicates how the permissions on the file are set. For instance, a directory with full permissions for all owner types would be drwxrwxrwx:
The 1st character indicates the file type. The d indicates it’s a directory. When this character is a hyphen (-), it's a regular file.
The 2nd-4th characters indicate the read (r), write (w), and execute (x) permissions for the user. When one of these characters is a hyphen (-) instead, it indicates that this permission is not granted to the user.
The 5th-7th characters indicate the read (r), write (w), and execute (x) permissions for the group. When one of these characters is a hyphen (-) instead, it indicates that this permission is not granted for the group.
The 8th-10th characters indicate the read (r), write (w), and execute (x) permissions for the owner type of other. This owner type consists of all other users on the system apart from the user and the group. When one of these characters is a hyphen (-) instead, that indicates that this permission is not granted for other.
The second block of text in the expanded directory listing is the user who owns the file. The third block of text is the group owner of the file.
Change file permissions


In order to change the permissions of files in the current directory, we use the command chmod that allows changed permissions on files and directories, adding the command g-r, we are denying read permissions for the owner group in the project_m.txt file.
Change file permissions on a hidden file


With the purpose to see the hidden files or directories, We use the command ls -la that displays the hidden files and directories, and list the permissions of these. Then, We allow to change the permissions of hidden files with the command chmod u-w, g+r in the .project_x.txt. For this case, We are changing the permissions to the .prohect_x.txt file denegated write authorization for users and adding read permissions to the group.
Change directory permissions


To change directory permissions, We use the command chmod g-x drafts/ that allows the group to have execute permissions in the drafts directory.
Summary
The permissions of the projects directory and the files it contains. The lab starts with /home/researcher2 as the current working directory. This is because you're changing permissions for files and directories belonging to the researcher2 user.

Determine whether any files have incorrect permissions and then change the permissions as needed. This action will remove unauthorized access and strengthen security on the system.

Determine if a hidden file has incorrect permissions and then change the permissions as needed. This action will further remove unauthorized access and strengthen security on the system.

Change the permissions of a directory. First, you’ll check the group permissions of the /home/researcher2/projects/drafts directory and then modify the permissions as required. 


**</a>
</body>
