For Use with SPUDSIM v2-2 and tested on January 2017, 2025
The excel macro method makes it easier to develop input files needed to drive USDA-ARS Adaptive Cropping Systems Laboratory crop models.  Each model uses a similar excel macro, although slight differences with respect to cultivar coefficients and initial field conditions exist.

A user-manual is not available at this time. Hence, users are strongly encouraged to reach out to ACSL staff for assistance. For SPUDSIM, please contact Dr. David Fleisher (David.fleisher@usda.gov) for assistance.

This version includes irrigation file changes, which include options for selecting irrigation time and ponding, and N2O gas fluxes from soil surface.  

To use:

(1) The example_input folder contains two files.  One is a *.xls file, called a template file, which summaries data associated with a field trial at a farm in Nebraska. In general, each row of the spreadsheet would represent a different field or scenario to be simulated. The first tab, "Description" is used to identify and provide names to the different types of input data. Only one row (one field) is provided in this example, but the user could easily add additional rows for the same field which could vary for example, by N fertilizer amount or application timing, cultivar differences, weather data, planting dates, and etc.  Each spreadsheet tab represents a different class of data.

The second file, *.crp, contains weather data used in the model. Currently, the weather has to be provided by the user (i.e. no option at this point in the excel macro to download weather data from online sources).  

(2) After input data is entered into the template.xlsx file (step (1)),  the '*.xlsm' file can be opened.  The first six rows of this file, (Column A1-6) are used to indicate where different files are situated on the hardrive.  This includes location of the template file, weather data, and etc. It may be easier for users to maintain the same file structure as in the version provided in GitHub.

(3) When ready, clicking on the  'Select ID's and run macros' will let the macro read in the template file.  A list will appear corresponding to each row in Description tab of the template.xlsx file. User can click on the row in the popupbox, and the interface will proceed to create the input files, each in the folder specified by the user.

(4) In the current setup, execution should just take a few seconds.  In the 'example input' folder, you will see new files created.  Double click the 'grid1.bat' file as a final step.  This will create the matching soils information for the field location.

(5) You are now able to use the input data for the SPUDSIM potato model.  Again, for SPUDSIM assistance or help with this macro, please contact Dr. David Fleisher (David.fleisher@usda.gov).

(6) Note the 'prerun_example_input' folder provides the results from a successful macro run...