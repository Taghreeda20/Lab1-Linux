# Lab1-Linux
  2- What is the difference between cat and more command?
  ![Image Alt](https://github.com/Taghreeda20/Lab1-Linux/blob/c3b99842333eefbf6ebddd7a8bbdfb961e39500f/Screenshot%202025-04-05%20222828.png)
  3- What is the difference between cat and more command?
  ![Image Alt](https://github.com/Taghreeda20/Lab1-Linux/blob/b7fb229ce67238b1dee93b456247bbb5f1714b58/Screenshot%202025-04-05%20225134.png)
  4-Create the following hierarchy under your home directory:
  
    Taghreed20@Ubuntu5:~$ mkdir dir1
    Taghreed20@Ubuntu5:~$ mkdir dir1/dir11
    Taghreed20@Ubuntu5:~$ mkdir dir1/dir12
    Taghreed20@Ubuntu5:~$ touch dir1/dir11/file1
    Taghreed20@Ubuntu5:~$ mkdir docs
    Taghreed20@Ubuntu5:~$ touch docs/mycv
    Taghreed20@Ubuntu5:~$ ls
    Desktop  docs       Downloads  Pictures  snap       Videos
    dir1     Documents  Music      Public    Templates
    Taghreed20@Ubuntu5:~$ ls dir1
    dir11  dir12

  b- remove dir12 using rmdir –p command : 

    Taghreed20@Ubuntu5:~$ cd dir1
    Taghreed20@Ubuntu5:~/dir1$ rm dir11
    rm: cannot remove 'dir11': Is a directory
    Taghreed20@Ubuntu5:~/dir1$ rm -r dir11
    Taghreed20@Ubuntu5:~/dir1$ ls dir1
    ls: cannot access 'dir1': No such file or directory
    Taghreed20@Ubuntu5:~/dir1$ ls
    dir12
    Taghreed20@Ubuntu5:~/dir1$ rmdir -p dir12

  c- The output of the command pwd was /home/user. Write the absolute and relative path for the file mycv :   
  
  5-  Copy the /etc/passwd file to your home directory making its name is mypasswd :
  6-  Rename this new file to be oldpasswd :
  7- list four ways to go to your home directory :
  9- Display the first 4 lines of /etc/passwd :
  10-Display the last 7 lines of /etc/passwd : 
  11-Display the man pages of passwd the command and the file sequentially in one command : 



  

   
