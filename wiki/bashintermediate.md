Bash intermediate tutorial
==========================

Getting To know the Terminal
-----------------------------


###Command options

Most linux utilities and commands take options tat modify the behaviour of the output,
here are some  examples


####Command

    ::bash
    ls -l

This will cause the ```ls``` command to print the contents of a directory in ```long``` format. 
This will give output of this form:

    ::bash
    [asesma@comp32 test]$ ls -l
    total 4776
    -rw-rw-r--  1 asesma asesma   20480 Aug  1  2013 automated-0.1.b-alpha.tgz
    -rw-rw-r--  1 asesma asesma      55 May  7  2013 bands.in
    -rw-rw-r--  1 asesma asesma   30847 May  7  2013 bn.ps
    drwxrwxr-x 38 asesma asesma    4096 May  7  2013 BN.save
    -rw-r--r--  1 asesma asesma  306486 May  7  2013 B.pbe-n-van_ak.UPF
    -rw-r--r--  1 asesma asesma  270792 May  7  2013 N.pbe-van_ak.UPF
    -rw-rw-r--  1 asesma asesma      55 Apr 25 11:54 silicon.in
    drwxrwxr-x  2 asesma asesma    4096 Oct 28 17:10 test

The output is split into columns giving various pieces of information, this includes, permissions in the first column, the ownership,
then sizes, then a timestamp of the modification/creation date  followed by the name.

####Command

    ::bash
    cp  -r arg1 arg2

The ```cp``` command will normally not copy a directory, unless the ```-r``` option is passed in this case it will copy  the ```arg1``` directory
to the ```arg2``` name.


####Command

    ::bash
    cat file

The ```cat``` command is used to show the contents of a text file. Example

    ::bash
    [asesma@comp32 test]$ cat bands.in 
    &bands
        filband = 'bands.dat',
        prefix = 'BN'
    / 
    [asesma@comp32 test]$ 

This shows that the ```bands.in``` has 4 lines of text in it. The cat command can show line numbers if they are needed:

    ::bash
    &bands
      filband = 'bands.dat',
        prefix = 'BN'
    / 


####Command
  
    ::bash
    clear

This clears the screen.


####Command

    ::bash
    rm -r

This command removes a directory


##Vi basic commands

####How to create a file named ```new```

    ::bash
    vi new

Then press ```i``` to be in ```INSERT MODE``` in order to start typing
