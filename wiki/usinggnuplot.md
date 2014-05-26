GNUPLOT
===========

If you have a file which contains the data to plot, example ```file.dat``` , type ``` gnuplot``` to the terminal and press ```Enter```. 

On the new line wich appears, type


     p "file.dat" u 1:2 w lp


This ```p``` means to plot for the ```file.dat```, ```u```: use, ```1:2```: plot column 1 vs column 2, ```w```: write, ```lp```: line and points.
Then, name the graph for example  ```image01.png```by typing the following comands


    set term png
    
    set output "image01.png"


Then, set the y label, x label and title to be for exapmle ``` Energy, Lattice consant, and Optimized lattice constant``` respectivelly by



    set ylabel "energy"

    set xlabel "Lattice constant"

    set title "Optimized lattice constant"

You can also set the x range, y range and x tics by typing the following comands


    set xrange [4.5, 9.5] 

    set yrange [-260.5, -260.1]

    set xtics (4.5,5.0,5.5,6.0,6.5,7.0,7.5,8.0,8.5,9.0,9.5)


After to put the all needed comands, then replot and exit by typing


     replot


     exit


To se the plotted image, type


      gwenview image01.png

or 
 
      eog image01.png



