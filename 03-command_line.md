# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

Show current working directory path: pwd

Create a directory: mkdir FILENAME

Deleting a directory:  rm -r directoryName

Creating a file using the 'touch' command: touch filename.txt

Deleting a file: rm filename.txt

Renaming a file mv old_filename.txt new_filename.txt

Listing hidden files: ls -a

Copying a file from one directory to another: cp sourceDir/file.txt destinationDir

Additional: copy all files in working directory into different directory: cp * destinationDir/

Additional: sort each line of a file name alphabetically, printing it to standard output: sort filename.txt



---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

'ls': lists all files and directories in working directory

'ls  -a': lists all files and directories including hidden files

'ls -l': lists all the content of a directory in long format

'ls -lh': lists all the content of a directory in long format with readable file size

'ls -lah': lists all the content of a directory, including hidden files, in long format with readable file size

'ls -t': order files and directories by the time they were last modified

'ls -Glp': lists all the content of a directory in long format while inhibiting the display of group information. Also, the command will 
indicate directories within the directory with a '/' ad the end.


---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

1. 'ls -r': displays files in reverse order

2. 'ls -d': displays only directories

3. 'ls -c': displays files by file timestamp

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

Answer: 'xargs' is a command that allows a user to build and execute other commands from the standard input. 



Here is an example of 'xargs' being used to separate an output of numbers:

Lets run say we ran the following: echo 1 2 3 4 5 6
we would get the following output: 
1 2 3 4 5 6

Now lets use 'xargs' to split the outputs into two items per line:echo 1 2 3 4 5 6| xargs -n 2
we would get the following output:

1 2

3 4

5 6




 

