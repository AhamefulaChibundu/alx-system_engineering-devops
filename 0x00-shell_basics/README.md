# SHELL BASICS AND BASH SCRIPT

This project is simply about bash script and shell basics.

### WHAT IS BASH SCRIPT?

Bash script is a series of command written in a file which are read and executed by the bash program. The program is usually executed line by line.
Example of a bash script is #!/bin/bash (program to be executed) 

### WHAT IS SHELL BASICS

These are basic human-readable commands by a user which the shell understands and converts into something the karnel can understand. we would be covering some of such examples and we would be doing it using bash script, they are as follows:

1. A command that prints the absolute path name of the current working directory. The command for this is 'pwd'. We can make this a bash script by creating a file (e.g file1) and saving these in it: #!/bin/bash pwd 
After saving, we need to make our files exectable by using the command chmod u+x (filename); in this example, since the name of our file is file1, we use chmod u+x file1. Finally, to execute the code, we type ./file1 and it prints our current working directory.
<br>

```
$ ./file1  
 
/root/project/shell-basics/  
 
$
``` 
<br>
Moving on, we follow same stepsin example1

2. A script that displays the contents list of your current directory: `#!/bin/bash ls`
3. A script that changes the working directory to the user’s home directory: `#!/bin/bash cd /root`
4. A script that displays current directory contents in a long format: `#!/bin/bash ls -l`
5. A script that displays current directory contents, including hidden files (starting with .): `#!/bin/bash ls -la`
6. A script that displays current directory contents in long format, with user and group IDs displayed numerically and also hidden files: `#!/bin/bash ls -na`
7. A script that creates a directory in another directory: ``#!/bin/bash mkdir /tmp/file1``
8. A script that moves one directory to another: ``#!/bin/bash mv /tmp/dir1 /tmp/dir2``
