TeloTool - Step-by-Step instructions (with example gel)
========

1)	TeloTool can only be used on a 64bit Windows Platform. 
2)	Please download and install the 64bit MATLAB Compiler Runtime (MCR) (version 7.17 (R2012a), freely available at the Mathworks webpage http://www.mathworks.com/products/compiler/mcr/).
3)	Start TeloTool.
4)	Load the example membrane via ‘Load Image’.
5)	Invert via ‘Invert Image’, so that the image has a dark background.
6)	Press ‘Calculate Lanes’. White rectangles will appear in the main axis, which represent the automatically recognized lanes. 
a.	[Optional] The parameters for the recognition can be changed via the two sliders underneath the main axis called ‘Filter for Lane Number’ and ‘Filter for Lane Width’. [Optional] Manual adjustment of the lanes is possible via pressing the button ‘Adjust Lanes’. 
b.	[Optional] Lanes can be equalized via ‘Constant Lanes’. 
7)	Press ‘Lane Profiles’ to fill the list box with intensity profiles of the recognized lanes.
8)	Press ‘left ladder’ within the list box. The intensity profile of the left ladder will be displayed in the profile axis next to the main axis. The y-axis represents the pixel position. 
9)	Press ‘Ladder Values’ to open a GUI with the values of the ladder. The standard has the sizes [10000;8000;6000;5000;4000;3500;3000;2500;2000]. Here, it is also possible to load the text-file ‘standard_ladder_for_example_gel.txt’. Press ‘Apply Ladder Values’. TeloTool will always automatically remember the last ladder used. 
10)	Press ‘Adjust Ladder’. A new GUI will open, which displays the left and the right ladder with the automatically recognized extrema as red dots. 
a.	The left ladder has one wrongly recognized extremum, press ‘Delete Extrenum’ and click and drag into the axis to remove it (it may take 2-3 seconds until the program reacts). Press ‘Reset’ to remove the selection.
b.	The right ladder has ten peaks, whereas the left has only nine extremas. In order to have the same number of elements in both ladders, the peak on the far right has to be removed (the band with the lowest molecular weight)
c.	‘Apply and Close’
11)	[Optional] The ladder is automatically fitted with a polynomial fit of the 3rd order. Press ‘Ladder Fit’ to change and compare the fits. 
12)	Now any other lane within the list box can be displayed. 
a.	The probe intensity corrected data and corresponding Gaussian fit is displayed within the profile axis. Press the check box ‘raw’ to display the uncorrected data. 
b.	The fit qualities of the Gaussian fit to the intensity profile can be found underneath the profile axis. 
13)	Please switch between the ratio buttons ‘raw’ and ’corr’ underneath the background options to change the display of the results. 
a.	The maximum intensity of the lane profile is displayed as red dot within the main axis.
b.	Please find the mean TRF, the standard deviation and the range for the selected lane beneath it. 
14)	Press ‘Get Result’ to open a new GUI which displays the results of all lanes
a.	The table holds the statistics and the graph a visual representation.
b.	The user can switch between the ‘raw’ and the ‘corr’ data via the ratio buttons.
c.	A threshold for the fit quality can be chosen (the standard is 80%). All fits which have a quality less than that treshhold are displayed in red. 
d.	[Optional] The user may exclude lanes from the graph by choosing a particular lane via the drop down menu and pressing ‘Exclude Lane’. 
e.	Data of the current table can be saved as .xls file via ‘Save Table’. All tables can be saved by pressing ‘Save All’.
f.	The graphical representation may be saved via ‘Export diagram’. To save it as .pdf or .eps indicated open-source programs has to be installed.
