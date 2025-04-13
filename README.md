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

    Taghreed20@Ubuntu5:~$ cd docs
    Taghreed20@Ubuntu5:~/docs$ pwd
    /home/Taghreed20/docs
    Taghreed20@Ubuntu5:~/docs$ readlink -f mycv
    /home/Taghreed20/docs/mycv
    Taghreed20@Ubuntu5:~/docs$ 
  
  5-  Copy the /etc/passwd file to your home directory making its name is mypasswd :

    Taghreed20@Ubuntu5:~$ sudo cp /etc/passwd ~/mypasswd
    
  6-  Rename this new file to be oldpasswd :
  
    Taghreed20@Ubuntu5:~$ sudo mv ~/mypasswd ~/oldpasswd 
  
  7- You are in /user/bin , list four ways to go to your home directory :
  
    Taghreed20@Ubuntu5:~$ cd bin
    Taghreed20@Ubuntu5:~/bin$ cd ~
    Taghreed20@Ubuntu5:~$ cd bin 
    Taghreed20@Ubuntu5:~/bin$ cd $HOME
    Taghreed20@Ubuntu5:~$ cd bin
    Taghreed20@Ubuntu5:~/bin$ pushd ~
    ~ ~/bin
    Taghreed20@Ubuntu5:~$ cd bin
    Taghreed20@Ubuntu5:~/bin$ cd .. 
    
  8- List Linux commands in /usr/bin that start with letter w :

    Taghreed20@Ubuntu5:~/bin$ ls /usr/bin | grep '^w'
    w
    wall
    watch
    watchgnupg
    wc
    wdctl
    wget
    whatis
    whereis
    which
    which.debianutils
    whiptail
    who
    whoami
    whoopsie
    whoopsie-preferences
    wireplumber
    word-list-compress
    wpa_passphrase
    wpctl
    wpexec
    write
    wsdd

  9- Display the first 4 lines of /etc/passwd :

    Taghreed20@Ubuntu5:~$ head -4 /etc/passwd
    root:x:0:0:root:/root:/bin/bash
    daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
    bin:x:2:2:bin:/bin:/usr/sbin/nologin
    sys:x:3:3:sys:/dev:/usr/sbin/nologin

  10-Display the last 7 lines of /etc/passwd : 

    Taghreed20@Ubuntu5:~$ tail -7 /etc/passwd
    polkitd:x:987:987:User for polkitd:/:/usr/sbin/nologin
    rtkit:x:116:119:RealtimeKit,,,:/proc:/usr/sbin/nologin
    colord:x:117:120:colord colour management daemon,,,:/var/lib/colord:/usr/sbin/nologin
    gnome-initial-setup:x:118:65534::/run/gnome-initial-setup/:/bin/false
    nm-openvpn:x:119:121:NetworkManager OpenVPN,,,:/var/lib/openvpn/chroot:/usr/sbin/nologin
    gdm:x:120:122:Gnome Display Manager:/var/lib/gdm3:/bin/false
    Taghreed20:x:1000:1000:Taghreed20:/home/Taghreed20:/bin/bash
    
  11-Display the man pages of passwd the command and the file sequentially in one command : 

    Taghreed20@Ubuntu5:~$ man passwd && man 5 passwd 
![image](https://github.com/user-attachments/assets/65dd8a2b-13ad-439d-b9de-1076b2100918)

  12- Display the man page of the passwd file : 

    Taghreed20@Ubuntu5:~$ man 5 passwd
  ![image](https://github.com/user-attachments/assets/70a2f15b-53f3-4a2a-a5d0-6ce7a91716f8)

  13-  Display a list of all the commands that contain the keyword passwd in their man page :  

    Taghreed20@Ubuntu5:~$ man -k etc/passwd
    
    pam_localuser (8)    - require users to be listed in /etc/passwd
    update-passwd (8)    - safely update /etc/passwd, /etc/shadow and /etc/group

  14-Using vi write your CV in the file mycv. Your CV should include your name, age, school, college, experience,.. : 

    Taghreed20@Ubuntu5:~$ vi mycv
  ![image](https://github.com/user-attachments/assets/4f6dfd52-d130-4fd6-a9a7-7ede4a6dfb9f)

  16- st the available shells in your system : 
  
    Taghreed20@Ubuntu5:~$ cat /etc/shells
    # /etc/shells: valid login shells
    /bin/sh
    /usr/bin/sh
    /bin/bash
    /usr/bin/bash
    /bin/rbash
    /usr/bin/rbash
    /usr/bin/dash


  

   
