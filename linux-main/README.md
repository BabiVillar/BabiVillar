
<p style="text-align: left></p>
<h1 style="text-align: middle></h1>

<h1>PERMISSIONS IN LINUX</h1>	

<h2>Check file and directory details</h2>
<p>The screenshot demonstrates the specific directories and files of the system. <br>
<img src="Screenshot 2026-02-10 153602.png" alt="imagem 1" width="600"> <br>
The first line displays the command I entered, and the other lines the output. the code ls -la, list all contents of the project directory, include the details and the hidden files.
The first column represents the permissions set on each file or directory.<br></p>

<h2>Describe the permissions string</h2>
<p>The 10 character string determines who is authorized to access the file.<br>
<img src="Screenshot 2026-02-10 154223.png" alt="imagem 1" width="200"> <br>
- 1st character: represented by d,it indicates that it’s a directory or represented by hyphen (-), it’s a regular file. <br>
- 2nd-4th characters: represented by rwx, respectively read (r), write (w) and execute (x) permissions for the user. when one of these are represented by a hyphen (-) instead, indicate that permission is not granted to the user - the user creates the file. <br>
- 5th-7th characters: represented by rwx, respectively read (r), write (w) and execute (x) permissions for the user. when one of these are represented by a hyphen (-) instead, indicate that permission is not granted to the group - is a small group with the user include. <br>
- 8th-10th characters: represented by r-x, respectively read (r) and execute (x) permissions for the user. In this example the others don't have permission to write in this directory. Others are users of the system.</p>

<h2>Change directory permission</h2>
<p>The new definition is that only user can read, write and execute the directories and files. the group and the other can only read.
For this modifications have two ways, the first is: chmod g=r,o=r project-01. This command replaces existing permissions, leaving only the permission specified in the expression.<br>
<img src="Screenshot 2026-02-10 161342.png" alt="imagem 1" width="600"> <br>
The second way is: chmod g-wx,o-x project-02. This command removes the specified permissions.
<img src="Screenshot 2026-02-10 161937.png" alt="imagem 1" width="600"> <br>
The last modification is in the file read_me.txt. Always ensuring that the changes were made using the command ls -la. <br>
<img src="Screenshot 2026-02-10 162246.png" alt="imagem 1" width="600"> <br></p>
