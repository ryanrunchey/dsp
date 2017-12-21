# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

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

* [pwd] show current working directory path
* [mkdir] creating a directory
* [rm -r directoryname] delete a directory by recursively deleting all folders and files within the directory
* [touch filename.ext] creating a file using touch command
* [rm] deleting a file
* [-r] stands for recursive (i.e. rm -r deletes a directory and all of its child directories.)
* [mv] renaming a file or folder since renaming is interpretted by the system as moving the file
* [ls] list all files and directories in the current directory 
* [-a] show hidden files (i.e. ls -a shows all contents in a directory including hidden files)
* [cp] copying a file from one directory to another
* [sort] takes a filename or standard input and orders each line alphabetically, printing it to a standard output.
* [mv] moves a file or directory taken as an input in the first argument to the location of the directory in the second argument

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

* [ls] lists all files and folders in the current working directory.  
* [ls -a]  lists all files and folders including hidden files in the current working directory
* [ls -l]  lists all contents in the directory in long format
* [ls -lh]  lists all contents in the directory in long format and human readable sizes (i.e. 1K, 234M)
* [ls -lah]  lists all contents in the directory in long format, including hidden files, and human readable sizes (i.e. 1K, 234M)
* [ls -t] lists all contents in the directory by the time they were last modified 
* [ls -Glp]  lists all contents in the directory, highlights different file types with different colors, in long format, and Display a slash (‘/’) immediately after each pathname that is a directory.



---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

* -a	Displays all files.
* -p	Displays directories with /
* -R	Displays subdirectories as well.
* -t	Displays newest files first. (based on timestamp)
* -1	Displays each entry on a line.

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

* What is the xargs command in UNIX?
The xargs command in UNIX is a command line utility for building an execution pipeline from standard input. Whilst tools like grep can accept standard input as a parameter, many other tools cannot. Using xargs allows tools like echo and rm and mkdir to accept standard input as arguments. - https://shapeshed.com/unix-xargs/

* The most common usage of xargs is to use it with the find command. This uses find to search for files or directories and then uses xargs to operate on the results. Typical examples of this are removing files, changing the ownership of files or moving files. 

find /tmp -mtime +14 | xargs rm

* finds and removes files in the directory /temp that are two weeks or older

 

