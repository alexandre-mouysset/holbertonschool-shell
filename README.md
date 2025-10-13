#!/bin/bash
pwd
this script print the absolute path name of the current working directory

#!/bin/bash
ls
this script displays the contents list of the current directory

#!/bin/bash
cd
this script changes the working directory

#!/bin/bash
ls -s
this script display the current directory contents in a long format

#!/bin/bash
ls -la
this script display the current directory contents, including hidden files

#!/bin/bash
ls -lan
this script display current directory contents

#!/bin/bash
mkdir /tmp/my_first_directory
this script create a directory named my_first_directory in the /tmp/ directory

#!/bin/bash
mv /tmp/betty /tmp/my_first_directory/
this script move the file betty from /tmp/ to /tmp/my_first_directory

#!/bin/bash
rm /tmp/my_first_directory/betty
this script remove betty

#!/bin/bash
rm -r /tmp/my_first_directory
this script remove the directory

#!/bin/bash
cd -
this script change de working directory to the previous one

#!/bin/bash
ls -la . .. /boot/    
Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format.

#!/bin/bash 
file /tmp/iamafile
Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script.

#!/bin/bash
ln -s /bin/ls __ls__

#!/bin/bash
cp -u *.html ../
Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.

#!/bin/bash
mv [A-Z]* /tmp/u/  
Create a script that moves all files beginning with an uppercase letter to the directory /tmp/u

#!/bin/bash
rm -rf *~
create a script that deletes all files in the current working directory that end with the character ~

#!/bin/bash
mkdir -p welcome/to/school
Create a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory.two spaces allowed

#!/bin/bash
su betty
switches the current user to the user betty

#!/bin/bash
whoami
print the effective username of the current user

#!/bin/bash
groups
prints all the groups the current user is part of

#!/bin/bash
chown betty hello
changes the owner of the file hello to the user betty

#!/bin/bash
touch hello
create an empty file called hello

#!/bin/bash
chmod u+x hello
add execute permission to the owner of the file hello

#!/bin/bash
chmod ug+x,o+r hello
adds execute permission to the owner and the group owner, and read permission to other users, to the file hello

#!/bin/bash
chmod +x hello
adds execution permission to the owner, the group owner and the other users, to the file hello

#!/bin/bash
chmod 007 hello
Write a script that sets the permission to the file hello as follows:

Owner: no permission at all
Group: no permission at all
Other users: all the permissions

#!/bin/bash
chmod 753 hello
script that sets the mod of the file hello
