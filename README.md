@DTU SVT 2025

@Jan Jastrzebski, Xiao Chen

============
Introduction
============

This is a README for the Blade Damage Map software, which allows for visualization and subsequent analysis of inspections performed on wind turbine blades in wind turbine farms as well as single blade wind turbines from tests performed in research or testing facilities.

============
LICENSE
============

MIT License

Copyright © 2025 Technical University of Denmark, Department of Wind and Energy Systems.
For full license text, see license.txt.

============
Installation
============

A Win8+ computer with a valid MATLAB license is required.

============
Functionality
============

'View Blade Damage Map database':
Access the 'database.mat' file in order to display the sets of data which have been ingested into the BDM.
By then accessing the database the connected images, locations or otherwise information pertaining to the database is displayed.

'Add to Blade Damage Map database':
Queries the user to specify which Case is being dealt with and after making the correct choice implement the 
data into the database structure, so that the dataset can be then displayed through 'View available BDM'.

Case 1 requires an image folder containing images of the documented damages, which have a naming convention which can be recovered with the cases
second requirement, an .xlsx sheet containing information required for establishing a digital twin of the farm and the connected damages.

Case 2 requires images of the damages to be saved in individual folders where the damage progression is saved by the images chronologically in a "YYYYMMDD-HHMM" format. 
When ingested the folders and the damage locations are loaded in an alphabetical order.

Whichever case is added to the 'database.mat' file, the resulting folder which contains the project is saved and any additional information 
necessary for the loading and display is saved in the individual 'meta.mat' file.

============
Resources
============

'functions' folder containing:

All functions related to creating and display of 'Case 1', 'Case 2' and additional 'util' functions for software utility such as unpacking data

'examples' folder containing:

'Wind Farm Inspection' an example of Case 1 use case of the software, including the dataset .excel sheet and associated photographs of the damages. Viewable through 'View Blade Damage Map database'

'Single Damage Inspection' an example of Case 2 use case, images of single blade test performed in a research facility.

In the root directory:

'virtual.asc' file containing all data required for visualizations, such as wind turbine blade point cloud

'Example_structure_case1.xlsx' excel sheet for providing a comparison of how the BDM software expects the rows for ingestion of Case 1 to be formatted

'database.mat' file containing all the information relating to the stored datasets

