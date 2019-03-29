
# Learning Linux



## Setting up a Linux Virtual machine (03/25)
* Download Ubuntu from https://www.ubuntu.com/download/desktop
* Download Virtual box from https://www.virtualbox.org/wiki/Downloads
    * LVM - Logical Volume Management - Allows to increase or decrease volumes later


## Shortcut Keys
* Ctrl+ A - go beginning of the command
* Ctrl+ E - go to the end of the command line
* Ctrl+ P - previous
* Cmd+ R - search the previous command
   
## Linux Basics

* pwd - print working directory
* ls - list files and folders in the folder
* ln - link - No 2 files but pointer to the file
* nano - edit a file
* cat - shows the file
* head - shows tyhe first XX lines
* tail - shows the last XX lines
* head tail -f options - Keeps the file open
* shutdown - r/h now - shutdown restart/halt now
* poweroff - shuts down the instance
* / - First slash is the root directory
* clear - clear the terminal
* cd to go up or down
* cd /- goes to the root directory
ubuntu@ip-172-31-82-245:/$ - Name@machinename: Dir


## Basics 2 (03/26)
https://www.youtube.com/watch?v=Lbh8Bh_SEzU&list=PLtK75qxsQaMLZSo7KL-PmiRarU7hrpnwK&index=4

* ls -a - shows hidden files
* $ is the bash for most of the linux versions
* cd ~ - short for the home
* touch filename - creates a file
* cat filename - prints the file
* mkdir dirname - creates a directory
* mv filename target - Move file to a folder
* rm filename - removes the file
* rmdir foldername - removes the folder
* rm -r - Removes recursively

### Basics continued
https://www.youtube.com/watch?v=ZeZVkA1zjWg&list=PLtK75qxsQaMLZSo7KL-PmiRarU7hrpnwK&index=5

* Anything after # will not be evaluated
* nano file - opens file in editor
* ln -s file linkfile - creates link of file

### More commands(03/27)
https://www.youtube.com/watch?v=EbOEqycEFeM&index=6&list=PLtK75qxsQaMLZSo7KL-PmiRarU7hrpnwK


* w - gives info on who all have logged in
* who - same as who but lesser information
* top - gives the details of the processes running
 * htop - gives the same as htop but better
* netstat - gives the network details
    * netstat -tupln - gives the needed details
    * sudo netstat -tupln gives more details as running on root
    
### Review Text editors
https://www.youtube.com/watch?v=fEGSA68uAR4&index=7&list=PLtK75qxsQaMLZSo7KL-PmiRarU7hrpnwK

* cp file1 file2 - copy file2 to file2
* man - help
* cat file1 file2 - concatenates file1 and file2

## Shell Features 03/28
https://www.youtube.com/watch?v=-Z5tCri-QlI&index=8&list=PLtK75qxsQaMLZSo7KL-PmiRarU7hrpnwK
### Redirection <, >, >>, 2>

* echo "STDIN -->0"
* echo "STDOUT -->1" dont have to specify as well. Redirects to the file
* echo "STDERR -->2"
* command < msg.txt - passed msg.txt to command
* (>>) concatenates 


### Pipes | 
    
* ps aus | less - displays but less makes it shows only one screen
* (#Q) - quits from less

https://www.youtube.com/watch?v=nLa6jAbULe8&list=PLtK75qxsQaMLZSo7KL-PmiRarU7hrpnwK&index=9

### Logical &&, cut, sort, uniq, grep

* prog1 && prog2 - It run prog2 only when prog1 is success
* cat file.txt | cut -d: -f2 - Cuts the file by the delimiter
* sort - bf - sorts
* uniq - unique values
* grep - search for some data
    * ubuntu@ip-172-31-82-245:~$ netstat >>netstat.txt
    * cat netstat.txt | uniq|grep bus | cut -d[ -f2


 










