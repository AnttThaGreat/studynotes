
to check for the presence of files or folders use 
_-f_  :checks for file
_-d_  checks for directory

_EX: if [ -f ~/myfile]_  
will then for that file
else
then

use _fi_ to end the if statement

##### use cases that come to mind are:
check to see if something got save where i wanted or just make sure its there

checking to see if a password doc exists 
and copy it to another location

to check if a certain key file is present before running a program or terminating one

if there is a folder open and view the contents then erase it.



EX2: 
command =/user/bin/htop 
if [ -f $command ]
then
	echo "$command is available, let's run"
else
	echo "$command not present, installing it...""
	sudo apt update && sudo apt install -y htop
	
$command

#### Use cases that come to mind

-y to just answer without a confirm prompt

setting variable to common file name that contains information then checking if that file exists on remote machine

setting variable to a common directory that can contain information on a remote machine

check to see if a program is installed and install it and run it EX2:
IE: check if ssh is available
check to see if ufw is installed and allow something



