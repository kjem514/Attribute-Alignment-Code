# Attribute-Alignment-Code
This repository holds code which can be used to calculate attribute alignment, which models the coexistence of attributes within lower-level components of a complex multilevel system.

To use this code, first download Anaconda Navigator, which is free (https://www.anaconda.com/products/distribution)
Then, open Jupyter Notebook
Upload your data in .csv form and the "Python Attribute Alignment Code - Github - 1-23-23.asciidoc" file from this repository. 
Fill in the variable names of interest from your file where indicated, specifically
  1. Add the name you use to separate your teams where "Overall GroupID" appears. This is the variable that will divide members into team 1, team 2, etc. 
  2. Add a dependent variable where "DV" appears
  3. Add attributes you are interested in calculating alignment values for 
  4. Make sure there is no missing data in your .csv file.
  5. If you need to include teams with missing data, including “na.rm=TRUE” to the following line may work:
 return(sqrt(rowSums((attribute_1_matrix - attribute_2_matrix) ** 2,na.rm=TRUE)))

Also, in newer versions of Python, you may have to change "data_matrix = all_data.as_matrix()" to "data_matrix = all_data.values"

Finally, note that this code is subject to an MIT Open Source License (see Legal.txt)

Good luck with your research!
