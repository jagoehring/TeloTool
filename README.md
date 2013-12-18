TeloTool - Step-by-Step instructions 
========
<ol>
  <li> TeloTool can only be used on a 64bit Windows Platform.  </li>
  <li> Please download and install the 64bit MATLAB Compiler Runtime (MCR) (version 7.17 (R2012a), freely available at the Mathworks webpage http://www.mathworks.com/products/compiler/mcr/).</li>
  <li> Start TeloTool.</li>
  <li> Load a TRF gel (in .tif format) via ‘Load Image’.</li>
  <li> [Optional] Invert via ‘Invert Image’, so that the image has a dark background.</li>
  <li> Press ‘Calculate Lanes’. White rectangles will appear in the main axis, which represent the automatically recognized lanes. </li>
  
    <ol>
      <li> [Optional] The parameters for the recognition can be changed via the two sliders underneath the main axis           called ‘Filter for Lane Number’ and ‘Filter for Lane Width’. [Optional] Manual adjustment of the lanes is           possible via pressing the button ‘Adjust Lanes’. </li>
      <li> [Optional] Lanes can be equalized via ‘Constant Lanes’.</li>
    </ol>

  <li>Press ‘Lane Profiles’ to fill the list box with intensity profiles of the recognized lanes.</li>
  <li> Press ‘left ladder’ within the list box. The intensity profile of the left ladder will be displayed in the profile axis next to the main axis. The y-axis represents the pixel position. </li> 
  <li> Press ‘Ladder Values’ to open a GUI with the values of the ladder. Here, it is also possible to load the text-file containing the ladder values in the format [max value;intermediates;min value]. Press ‘Apply Ladder Values’. TeloTool will always automatically remember the last ladder used. </li> 
  <li> Press ‘Adjust Ladder’. A new GUI will open, which displays the left and the right ladder with the automatically recognized extrema as red dots. </li> 
    <ol>
      <li>If there are wrongly recognized extrema, press ‘Delete Extrenum’ and click and drag into the axis to remove it (it may take 2-3 seconds until the program reacts). Press ‘Reset’ to remove the selection.</li> 
      <li> It is necessary that the same number of peaks is recognized in both ladders. The 'ladder values' also need to have the same number of elements. </li> 
      <li>‘Apply and Close’</li> 
    </ol>
  <li>[Optional] The ladder is automatically fitted with a polynomial fit of the 3rd order. Press ‘Ladder Fit’ to change and compare the fits. </li> 
  <li>Now any other lane within the list box can be displayed. </li> 
    <ol>
      <li>The probe intensity corrected data and corresponding Gaussian fit is displayed within the profile axis. Press the check box ‘raw’ to display the uncorrected data. </li> 
      <li>The fit qualities of the Gaussian fit to the intensity profile can be found underneath the profile axis. </li> 
    </ol>
  <li>Please switch between the ratio buttons ‘raw’ and ’corr’ underneath the background options to change the display of the results. 
    <ol>
      <li>The maximum intensity of the lane profile is displayed as red dot within the main axis.</li> 
      <li>Please find the mean TRF, the standard deviation and the range for the selected lane beneath it. </li> 
    </ol>
  <li>Press ‘Get Result’ to open a new GUI which displays the results of all lanes.</li> 
    <ol>
      <li>The table holds the statistics and the graph a visual representation.</li> 
      <li>The user can switch between the ‘raw’ and the ‘corr’ data via the ratio buttons.</li> 
      <li>A threshold for the fit quality can be chosen (the standard is 80%). All fits which have a quality less than that treshhold are displayed in red. </li> 
      <li>[Optional] The user may exclude lanes from the graph by choosing a particular lane via the drop down menu and pressing ‘Exclude Lane’. </li> 
      <li>Data of the current table can be saved as .xls file via ‘Save Table’. All tables can be saved by pressing ‘Save All’.</li> 
      <li>The graphical representation may be saved via ‘Export diagram’. To save it as .pdf or .eps indicated      open-source programs has to be installed.</li> 
    </ol>
</ol>
