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

#!/bin/bash
chmod --reference=olleh hello

#!/bin/bash
chmod +x -R */
script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.

#!/bin/bash
mkdir -m=751 my_dir
script that creates a directory called my_dir with permissions 751 in the working directory.

#!/bin/bash
chgrp school hello
change the group owner to school for the file hello

#!/bin/bash
chown vincent:staff *
changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.

#!/bin/bash
chown -h vincent:staff _hello
script that changes the owner and the group owner of _hello to vincent and staff respectively.

The file _hello is in the working directory
The file _hello is a symbolic link

#!/bin/bash
echo "Hello, World"
prints "Hello, World", followed by a new line to the standard output

#!/bin/bash
echo "\"(Ôo)'"
display a confuse smiley

#!/bin/bash
cat /etc/passwd
display the content of the /etc/passwd file

#!/bin/bash
cat /etc/passwd
display the content

#!/bin/bash
tail -n 10 /etc/passwd
display the last 10 lines

#!/bin/bash
head -n 10 /etc/passwd
display the first 10 lines

#!/bin/bash
head -n 3 iacta | tail -n 1
display the third line

#!/bin/bash
echo -e "Best School" > '\*\\'\''"Best School"\'\''\\*$\?\*\*\*\*\*:)'
shell script that creates a file named

#!/bin/bash
tail -1 iacta >> iacta 
duplicates the last line of the file iacta

#!/bin/bash
find . -type f -name "*.js" -delete   
deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders

#!/bin/bash
find . -type d -mindepth 1 | wc -l
counts the number of directories and sub-directories in the current directory.
The current and parent directories should not be taken into account
Hidden directories should be counted

#!/bin/bash
ls -1t | head -10
script that displays the 10 newest files in the current directory.
One file per line
Sorted from the newest to the oldest

#!/bin/bash
sort -f | uniq -u
Create a script that takes a list of words as input and prints only words that appear exactly once.

Input format: One line, one word
Output format: One line, one word
Words should be sorted

#!/bin/bash
grep root /etc/passwd
display the lines containing the pattern root from the file

#!/bin/bash
grep -c bin /etc/passwd
display the number of lines that contain the pattern bin the in the file

#!/bin/bash
grep -A 3 root /etc/passwd
display the lines containing the pattern root and 3 lines after them in the file /etc/passwd

#!/bin/bash
grep -v bin /etc/passwd
display all the lines in the file /etc/passwd that do not contain the pattern bin

#!/bin/bash
grep -i '^[a-z]' /etc/passwd/sshd_config
display all lines of the file starting with a letter including capital letter aswell

#!/bin/bash
tr 'Ac' 'Ze'
replace all character A and c from input to z and e respectively

#!/bin/bash
tr -d 'cC'
remove all letters c and C from input

#!/bin/bash
ver 
reverse its input

#!/bin/bash
alias ls='rm -f *'
create a script that create an alias

#!/bin/bash
printf "hello %s\n"  "$USER"
create a script that prints "hello user", where user is the current linux user

#!/bin/bash
export PATH="$PATH:/action"
Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.

#!/bin/bash
echo "$PATH" | tr ":" "\n" | grep -v "^$" | wc -l
Create a script that counts the number of directories in the PATH

#!/bin/bash
printenv
createa script that lists environnement variables

#!/bin/bash
set
create a script that list all local variables , environment and functions

#!/bin/bash
BEST="School"
create a new local variable

#!/bin/bash
export BEST="School"
create a new global variable

#!/bin/bash
echo $((TRUEKNOWLEDGE + 128))
prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line.

#!/bin/bash
echo $((POWER/DIVIDE))
script that prints the result of power divided by divide, followed by a new line

#!/bin/bash
echo $((BREATH ** LOVE))
script that display the result of BREATH to the power LOVE


#!/bin/bash
echo $((2#$BINARY))
script that converts a number from base 2 to base 10

#!/bin/bash
echo {a..z}{a..z} | tr " " "\n" | grep -v oo
script that prints all possible combinations of two letters, except oo.

Letters are lower cases, from a to z
One combination per line
The output should be alpha ordered, starting with aa
Do not print oo
Your script file should contain maximum 64 characters

#!/bin/bash
printf "%.2f" "$NUM"
 script that prints a number with two decimal places, followed by a new line.
  
