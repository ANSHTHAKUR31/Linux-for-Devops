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


