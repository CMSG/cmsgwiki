

Bash beginer tutorial
======================

Starting a terminal
-----------------------

### In Gnome 2

    Goto Applications ->  System Tools -> Terminal

### In KDE: 

    Goto Menu -> System Terminal

### Others:

    For Unity/Gnome 3,   search for "terminal" under the launcher

## Usage

Terminals will usually present a prompt for you to type and this prompt will appear as "$" 
this  means the terminal is ready to receive commands.

### First Steps

In this section i will show a command and its output:

####Command :

    ::bash 
    ls

The output will appear as such

    ::bash
    [asesma@cmsg tmp]$ ls
    cu.save  cu.wfc1  ni.save  ni.wfc1

You can ignore the part that says [asesma....]  this is unique to the computer and will be different on yours.
Here the  output of the command ```ls``` is the list that follows on the new line. In this case ```ls``` simply  gives us the
contents of the current directory.

####Command:

    ::bash
    pwd

the output will appear as such


    ::bash
    [asesma@cmsg ~]$ pwd
    /home/luke

This command ```pwd```  means ``` print directory tree``` it is used to show the current location of the terminal on the 
directory tree.

####Command: 
    
    ::bash
    mkdir

example usage:

    ::bash
    [asesma@comp32 ~]$ mkdir  test

If you now check the contents of the current directory  you will see a new directory named  ```test``` created, this command 
is used to create directories.

####Command

    ::bash
    cd

Example usage,

    ::bash
    [asesma@comp32 ~]$ cd test
    [asesma@comp32 test]$ 

This is used to change the current location of the terminal to another location, so if you type ```pwd``` you should see your new location
thats different from you previous location, see below  for another illustration

    ::bash
    [asesma@comp32 ~]$ pwd
    /home/asesma
    [asesma@comp32 ~]$ cd test
    [asesma@comp32 test]$ pwd
    /home/asesma/test

In this example the terminal is first located at ```/home/asesma```  but after changing directory its moved to ```/home/asesma/test```

####Command
    
    ::bash
    cp 

Example usage:

    ::bash
    [asesma@comp32 lesson]$ cp bands.in  silicon.in
    [asesma@comp32 lesson]$ ls
     bands.in  silicon.in

The ```cp``` command creates a copy of an existing file with the new name thats passed as the second parameter, in this case ```bands.in```
was copied to ```silicon.in```, a listing of the contents of the directory with ```ls``` shows the two files.

####Command

    ::bash
    mv

Example usage:

    ::bash
    [asesma@comp32 lesson]$ mv silicon.in  simple.in
    [asesma@comp32 lesson]$ ls
    bands.in  simple.in

The ```mv``` command moves a file from one location to another location, but can also be  used as a simple way to rename files. Below is a 
more comprehensive example:

    ::bash
    [asesma@comp32 lesson]$ mkdir crystal
    [asesma@comp32 lesson]$ ls
    bands.in  crystal  simple.in
    [asesma@comp32 lesson]$ mv simple.in  crystal/
    [asesma@comp32 lesson]$ ls
    bands.in  crystal
    [asesma@comp32 lesson]$ ls crystal/
    simple.in

We first create a directory named crystal, then move the file  ```simple.in``` to  it, using ```ls``` along the way to see  the effect of  each command.

####Command

     ::bash
     rm

Example usage:

    ::bash
    [asesma@comp32 lesson]$ ls
    bands.in  crystal
    [asesma@comp32 lesson]$ rm bands.in
    [asesma@comp32 lesson]$ ls
    crystal

The ```rm``` command is used to remove/delete files, it can not delete non-empty directories without  the recursive flag as see below:

    ::bash
    [asesma@comp32 lesson]$ ls
    crystal
    [asesma@comp32 lesson]$ rm -r crystal/


####Command:

    ::bash
    rmdir

Example usage:

    ::bash
    [asesma@comp32 lesson]$ ls
    crystal
    [asesma@comp32 lesson]$ ls crystal/
    [asesma@comp32 lesson]$ rmdir crystal/
    [asesma@comp32 lesson]$ ls
    [asesma@comp32 lesson]$ 

Here we see a directory that is itself empty, the command ```ls crystal``` shows the contents of the ```crystal``` directory,  the command ```rmdir``` is then usedto delete the directory.
