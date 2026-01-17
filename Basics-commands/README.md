BASICS LINUX COMMANDS 
1. --------->     Ls     <----------
=> to list all the items in the directory

Ls -l 
=> gives all the info of the  creation date , permissions ..etc.

B. ls -a
=> gives all the info about the hidden files 

C. ls -t
=> sort on the basis of time 

Command	Use
ls -lh	=  Detailed + readable size
ls -ltr	=  Oldest file last
ls -la  = 	Hidden + details
ls -lhS	=  Size + readable

<img width="1450" height="996" alt="image" src="https://github.com/user-attachments/assets/01e8280f-6f8a-4def-83f6-c02ad4b607d4" />

2. --------->  Cd     <----------
=> uses for changing the directory 

Cd ~
=> direct to the home directory 
B. Cd ..
=> direct it to the previous directory 

<img width="1362" height="664" alt="image" src="https://github.com/user-attachments/assets/fb7be5a1-ce55-4c24-85c6-dee7f2be6786" />



3. --------->  Pwd   <----------
=> gives path to the directory from the root
<img width="1528" height="664" alt="image" src="https://github.com/user-attachments/assets/2ba8ecda-a52e-4187-bfd0-527b4777a863" />



4.  --------->  Mkdir     <----------
=> to create new folders or directory 

A. mkdir directory_name
=> for creating a single directory 
B. mkdir dir1 dir2 dir3
=> for creating multiple folders or directory at the same time 
C. mkdir -p
=> creates parent as well as child directory too even if parent doesn’t exist .
mkdir -p DevOps/Linux/Basics
Agar DevOps aur Linux exist nahi karte, to bhi ban jaayenge
Error nahi aata

D.mkdir -v.      Verbose mode (batata hai kya create hua)
mkdir -v test
Output:
mkdir: created directory 'test'

E. mkdir -m 777 dir1
=> creating directory with permission 

<img width="1566" height="1842" alt="image" src="https://github.com/user-attachments/assets/ec2bdfa6-b794-4a21-9246-6608e7cedcf8" />


5.  --------->  Delete directory    <----------
Rmdir -> for deleting the empty directory
Rmdir -r => for deleting the directory with its content 
Rmdir -rf => with content + forcefully 
Rmdir -ri => with content + will ask the permission to delete

<img width="1566" height="1028" alt="image" src="https://github.com/user-attachments/assets/16b97a91-1269-4fc6-ad97-2d99077fd645" />

E. rm file_name => Single file delete karta hai
F. Rm -I => will ask the permission to delete the file
G. Rm -f => by force 
H. Rm *txt => via the pattern 

<img width="2844" height="1068" alt="image" src="https://github.com/user-attachments/assets/770d610b-ff67-4de1-85e4-3d1cd26ce706" />


Important thing to note here is that backup file end with numbers that’s why rm *backup.txt didn’t worked.
That’s why starting with rm backup*.txt worked.

6.  --------->  Cat , Zcat    <----------
=> cat command is used to show the content of files as well as to merge multiples file and it also creates new files.
And Zcat is use to show the content of the compressed file(.gz)without uncompressing it.

Cat file.txt => will display the content of the files 
Cat file1.txt  file2.txt => will display both files content 
Cat > file.txt  => will create the new file ( control +d)to save it.
Cat >> file.txt => adding new content to existing file
Cat -n file.txt  => will display the content with  line number 
Zcat file.gz => will display the content of that compressed file

<img width="1684" height="1304" alt="image" src="https://github.com/user-attachments/assets/3bb86064-d77a-49de-bdfd-2741eadb9545" />

7.    --------->  Touch    <----------
=> to create the files 

A. Touch file.txt => will create the file 

8.    --------->   Head    <----------
=> use to display the first 10 lines of file by default 

Head file.txt   => will display 10 line of the file 
Head -n 5 file.txt   => will display 5 lines only 
Head -c 20 file.txt  => will display the 20 byte only

<img width="1684" height="1430" alt="image" src="https://github.com/user-attachments/assets/8c444061-fd88-4f32-9428-1631995fc0bb" />


9.    --------->  Tail , tail -f    <----------
=> use to display the last 10 lines of file by default 

Tail file.txt  => will display the last 10 lines of the files
Tail -n 5 file.txt.   => will display the last 5 lines only 
Tail -c 10 file.txt. => will display the 10 byte of file
Tail -f file.txt  => whenever any new line added in the file it will show on the terminal

<img width="1684" height="1008" alt="image" src="https://github.com/user-attachments/assets/8c216428-c7b5-46bf-b1c9-197bd8403230" />

10.  --------->  Less , more    <---------- 
=> more is a basic pager used to display the long file , but it limitation is you can go forward only.
 whereas less is advanced pages it can go forward and backward .



11.   --------->   Cp   <---------- 
=> cp is use to copy the files and directories. cp source destination 

File copy
=> cp file1.txt    file2.txt

B.  Copy file into directories 
=>. cp file.txt  destination 

c.  Multiple files in one directory
=> cp    f1    f2    f3     newfolder

D. Directory copy  (-r required)
=>  cp    -r   A1    newfolder
Option	Use
-r	Directory copy
-i	Confirm overwrite
-f	Force overwrite
-p	Preserve attributes
-v	Show progress
-u	Update only

<img width="1684" height="1236" alt="image" src="https://github.com/user-attachments/assets/5f1ae9d0-e256-4e06-ba59-67375f9ccde7" />




12.   --------->  Mv    <---------- 
=> mv is use to move the files or directories and to rename it .

Basic Syntax.  => mv source destination

  File rename  => mv file1.txt file2.txt
  Move File Into Directory  =>  mv file.txt newfolder
  Directory move  => mv  dir1  dir2

  <img width="1684" height="1012" alt="image" src="https://github.com/user-attachments/assets/f2fa8594-411e-4b43-bee2-70e329eea9d7" />




13 .    --------->  Wc   <----------
=> It is use to count the lines words and characters of file.
Basic Syntax      =>    wc    file.txt
Output format	    =>      lines  words  characters  filename
A.   Lines count 		=>	 wc -l file.txt
B.   Word count 		=>	 wc -w file.txt
C.   Character count 	=>	 wc -m file.txt
D.   Bytes count 		=>	 wc -c file.txt
E.   With pipe 		=>     ls | wc -l

<img width="1684" height="616" alt="image" src="https://github.com/user-attachments/assets/831564e5-a59d-40ae-be83-0356511db521" />





14.   --------->   Vi editor in unix and Linux operating system   <----------
 => Its a terminal based text editor which creates or edit the files  






15.   --------->   ln ( hard link and soft link )   <----------
=> it is use to create links (shortcuts)

Hard link 
=> share the same index node 
 .   it is safe even after the deletion of original files.
 .   not for directory normally 
 .   not for different file system

Basic syntax   =>   ln   		original.txt     hardlink.txt
Proof               =>   ls   -li 	original.txt    hardlink.txt


Soft link
=> Different index node 
.    Not safe after the deletion of original files.
.    Allowed for directory
	
Basic syntax   =>  ln -s original.txt softlink.txt
Proof               =>  ls -l softlink.txt

<img width="1684" height="1006" alt="image" src="https://github.com/user-attachments/assets/3d50e782-d57b-4ff0-94d6-8f2f745d5107" />





16.   --------->  cut    <----------
=> It is use to engrave the  column / character out of the specific output or files.

. cut command delimiter ke basis par file se specific fields ya fixed position characters extract karti hai.

file.txt =>    Ansh:21:Delhi    Ravi:22:Mumbai     Neha:20:Pune

   Single field nikalna (-d + -f)
=>     cut -d ":" -f 1 data.txt

Output :    Ansh Ravi Neha


B.     Multiple fields nikalna
=>    cut -d ":" -f 1,3 data.txt

Output :  Ansh:Delhi   Ravi:Mumbai   Neha:Pune
C.     Character-wise cut (-c)
=>	 cut -c 1-4 name.txt

Output :   Ansh		Ravi

<img width="1684" height="1006" alt="image" src="https://github.com/user-attachments/assets/900e16fa-f196-4d41-8160-c28c0a5a4910" />




17.    --------->   Tee    <---------- 
=>	it  show the output in terminal and save it in the file

 Simple output save + display
=>  ls | tee files.txt

Output  terminal  => A1 backup1.txt 	file4.txt 	newfolder
Output  files.txt   => A1 backup1.txt 	file4.txt 	newfolder

B.  Append mode (-a)
=>  date | tee -a time.log

Output  terminal  => Tue Jan 16 22:45:10 IST 2026
Output  time.log  => Tue Jan 16 22:45:10 IST 2026


<img width="1684" height="1340" alt="image" src="https://github.com/user-attachments/assets/d5f9d3ff-50fd-4bc7-8d6f-600b3295ec92" />






18.   --------->   Sort    <---------- 
=> It sort the text line by line (Default: alphabetical order, ascending)

Names.txt
Ravi
Ansh
Neha
Kunal

A. Simple sort (alphabetical)
=>   sort names.txt
output
Ansh
Kunal
Neha
Ravi

B. Reverse sort (-r)
=> sort -r names.txt

output
Ravi
Neha
Kunal
Ansh

C. Numeric sort (-n) 
=> sort -n marks.txt

D. Sort + unique (-u)
=> sort -u city.txt

E. Sort by specific column (-k)
=> sort -k3 -n students.txt


<img width="1684" height="1274" alt="image" src="https://github.com/user-attachments/assets/2b5fb6c4-c95b-4a46-b281-8ab1139b9ff0" />





 19.    --------->   Clear    <---------- 
=> it is use to clear the terminal 

20. Diff 
=> it helps to identify the difference between two files and directory

Diff   f1.txt  f2.txt   => normal difference 
Diff -y f1.txt f2.txt => will show the diff with side view 



<img width="1684" height="1378" alt="image" src="https://github.com/user-attachments/assets/23adb79a-91b3-4186-baec-e560dd678277" />


*Login related commands 
Ssh

=>   SSH (Secure Shell) is a command used to securely connect to a remote computer/server over a network.

*Disk usage 
Df => show the used and free space of disk 
Du => it tell about the size of files/directories



<img width="1684" height="1676" alt="image" src="https://github.com/user-attachments/assets/f3695e99-44fb-41ec-8e0c-ebb944f5ccaa" />

*process
Ps        => Shows currently running processes.
Top      => Shows real-time running processes + CPU &          memory usage.

Fuser   => Shows which process is using a file, directory, or   port. 

Kill       => Stops a running process using PID.
nohup => Runs a command in background even after logout.

Free         =>  Shows memory (RAM + swap) usage.
Vmstat     =>  Shows memory, CPU, processes, I/O stats.










