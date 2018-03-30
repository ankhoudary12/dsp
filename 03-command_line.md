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

> > * show current working directory path: **pwd**  
    * creating a directory: **mkdir**  
    * deleting a directory: **rm -r**  
    * creating a file using `touch` command: **touch file.txt**  
    * deleting a file: **rm**  
    * renaming a file: **mv oldname.txt newname.txt**  
    * listing hidden files: **ls -a**  
    * copying a file from one directory to another: **cp file.txt directory/**  
    * search files for lines: **grep searchterm** (case sensitive)  
    * find and replace text: **sed**  
    
    

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

> > `ls`: **list all files in directory**  
    `ls -a`: **list all files including hidden ones**   
    `ls -l`: **displays the long format listing**   
    `ls -lh`: **displays the long format listings in human readable format**   
    `ls -lah`: **displays all files (including hidden) in HRF**    
    `ls -t`: **displays files in order of timestamp**    
    `ls -Glp`: **displays in long format, NO group names, and directories with**  
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > `d`: **displays only directories**  
    `c`: **displays files by timestamp**  
    `r`: **displays files in reverse order**  
    `u`: **displays files by file access time**  
    `g`: **long format listing without the owner names**  

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > Basically, `xargs` reads data from **stdin** and executes the command given as argument one or more times based on the input. If no argument is given, `xargs` will mimic the`echo` command. In essence, `xargs` reads items from **standard input** as separated by blanks and executes a command for each argument. One very handy use of `xargs` is for searching through text files for a specific string of characters. To do this, the following command is used: 
`find -name "*.txt*" | xargs grep "abc"`
 

