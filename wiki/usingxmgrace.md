XMGRACE
=========

If you have a file which contains the data (in 2 columns) to plot, example ```k_points.dat``` , type:

	::bash
	xmgrace k_points.dat

then, press ```Enter```. 


 If the file contains many columns, then type:

	::bash
	xmgrace

and press ```Enter```. 

Then go to ```Data``` then ```Import```, then ```ASCII```, then look for the file which contains data to plot and click on it.

Look at ```Load as ``` and change ```Single set``` to be ```Block data```, 

Then click on ```ok```.

Set type, example XY,

Choose X column, example ```1```, and Y column, example  ```2```.

Click on ```Apply```  to plot 1 Vs 2. If you want to plot many graphs, the depend on ```1```, then choose again on Y column for example ```3``` and click on ```Apply``` to plot also ```1 VS 3```, and so on. 

Then, click on ```Accept``` and on ```cancel``` of the ```Grace:Read sets```.

Click on Axis to set and to label them, or go to ```Plot``` then ```Axis properties.```

Do double click on the graph to put the ```Legend```.  Choose the set and put the legend, the Apply and Accept.

To move the ```legend```, press

	::bash
	Ctrl+Shift+L


To delete one graph, double click on the graphs, then  ```left click``` on the set to delete, then ```right click``` on it, chose ```Kill data```, then in the new window which appears, named ```Warndlg_popup```, click on ```Ok```.

 To add symbols press

	::bash
	Ctrl+E

To add the text, lines, arrows, box, ellipse to the graph, go to ```Window```, the ```Drawing objects```.

To divide ```xmgrace page```, go to ```Edit```, then ```Arrange graphs```. Choose the number of columns and rows, page offsets and spacing, then ```Apply```.


