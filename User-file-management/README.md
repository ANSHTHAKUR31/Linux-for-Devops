<<<<<<< HEAD
##            Users & Files Management

. System-level commands

uname

=> It tells about the operating system 

uptime

=> shows how long the system has been running along with load average.

Date

=> It shows current system date and time 

Who, whoami

=>The who command shows which users are currently logged into the system and what terminal they are using with how long they have been logged in.

=> The whoami command shows the username of the current logged-in user.


Which
=> The which command shows the full path of a command/executable that will run when you type a command.

Id
=> The id command shows user identity information such as:
User ID (UID)
Group ID (GID)
Groups the user belongs to

 

Sudo
=> It allows a normal user to run commands with superuser (root) privileges.

Shutdown
=> The shutdown command is used to turn off the system safely.

Reboot
=>The reboot command is used to restart the system.

Apt
=> It is used to install, update, upgrade, and remove software packages on Debian/Ubuntu systems.

Yum
=> YUM is a package manager used in RHEL-based Linux systems.
CentOS (older versions)
Amazon Linux (older)

DNF
=> DNF is the modern replacement for YUM.

Pacman
=> Pacman is the package manager for Arch Linux.

Portage
=> Portage is the package management system used by Gentoo Linux.


Users & Group Management

Sudo
Useradd
=> sudo user add -m Jethalal 
-m makes sure user add in the same directory
whoami
Su
=> switch user


passwd
=> it will show the list of users for cat etc/passwd
Sudo passwd jethalal , will set the password for jethalal user
Cat /etc/passwd

userdel
=> sudo userdel jethalal

groupadd
=> sudo groupadd devops
Cat etc/group

gppasswd -a , -M 
=> sudo gppasswd -a jethalal devops 
Here -a denotes add jethalal user to devops group

And -M to add multiple user such as , 
Sudo gppasswd -M Iyer , Bhide , Pappu devops

Verify :- cat etc/group

groupdel
It is use to delete the group
=> sudo groupdel devops





File permission commands

Umask
=> user file creation mode
=> by default permission to file when any new file added 




ls -l 
=> to list with permission 


chmod
=> it is use to change the permission of file and directory

chown commands
=> sudo chown jethalal file.txt 

chgrp command
=> sudo chgrp devops file.txt 

compression commands

Zip , gunzip , and gzip commands
=> zip -r compress.zip  new folder
	Unzip compress.zip 

Tar,  untar command
=> tar -cvzf compress.tar.gz new folder
	tar -xvzf compress.tar.gz

.file transfer command

Scp command ( copy files )

=> scp -i “linuxServer.pem" secret.txt ubuntu@ec2-13-233-75-0.ap-south-1.compute.amazonaws.com:home/ubuntu

scp -i “linuxServer.pem" -r ubuntu@ec2-13-233-75-0.ap-south-1.compute.amazonaws.com:home/ubuntu/newfolder .


Rsync command
=> rsync -e  “ssh -I “linuxServer.pem” -avz  newfolder ubuntu@ec2-13-233-75-0.ap-south-1.compute.amazonaws.com:home/ubuntu/newfolder 



=======
 
>>>>>>> f22e126 (networking added)
