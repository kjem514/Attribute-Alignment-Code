# Attribute-Alignment-Code
This repository holds code which can be used to calculate attribute alignment, which models the coexistence of attributes within lower-level components of a complex multilevel system.

**To use Python code calculating 2-attribute alignment**, first download Anaconda Navigator, which is free (https://www.anaconda.com/products/distribution)
Then, open Jupyter Notebook. Then, upload your data in .csv form (one team member per row) and the "2 Attribute Alignment Code 3-6-23.ipynb" file from this repository. 

To download a file from Github: Click on the file you wish to download from GitHub to open the individual file. From there, right click the Raw button at the top of the file, select Save Link As… , choose the location on your computer where you want to save the file, and select Save.

Then, fill in your variable names where indicated, specifically
  1. Fill in the name of your data set, including ".csv" after "DATA_FILE =" 
  2. Fill in "base_column" and "comparison_columns" with you attributes of interest. 
  3. Set distance_type = 2 to calculate the Euclidean distance between attribute vectors. Set distance_type = 'cosine' to calculate the cosine of the angle between vectors. These methods are described in detail in Emich et al., 2022, ORM. 

**To use the Python code, which calculates all 3+ alignment types at once**, follow the previous steps, but instead download the "Python Attribute Alignment Code - Github - 3-6-23.ipynb" file from this repository and upload it to Jupyter Notebook. 
Then, fill in the variable names of interest from your file where indicated, specifically
  1. Add the name you use to separate your teams where "Overall GroupID" appears. This is the variable that will divide members into team 1, team 2, etc. 
  2. Add a dependent variable where "DV" appears
  3. Add attributes you are interested in calculating alignment values for 
  4. Make sure there is no missing data in your .csv file.
  5. If you need to include teams with missing data, including “na.rm=TRUE” to the following line may work:
 return(sqrt(rowSums((attribute_1_matrix - attribute_2_matrix) ** 2,na.rm=TRUE)))

Also, in newer versions of Python, you may have to change "data_matrix = all_data.as_matrix()" to "data_matrix = all_data.values" or to "all_data.to_numpy()"

The R-code is presented in the "R-code-potentialenergy.ipynb", " ", and " " files, along with several brief examples. 

Finally, note that this code is subject to an MIT Open Source License (see Legal.txt)

Good luck with your research!

References: 

For a description of 2-attribute alignment:
Emich, K.J., Lu, L., Ferguson, A.J., Peterson, R.S., & McCourt, M. (2022). Team Composition Revisited: A Team Member Attribute Alignment Approach. Organizational Research Methods, 25, 642-672. 

For an example of 2-attribute alignment:
Emich, K.J., Lu, L., Ferguson, A.J., Peterson. R.S., Martin, S.R., McClean, E., Woodruff, T., & McCourt, M. Control and Change Together: Conscientiousness and Proactivity Alignment Improve Team Performance. Accepted at Academy of Management Discoveries.

For a description of 3+ attribute alignment: 
Emich, K.J., McCourt, M., Lu, L., Ferguson, A.J., & Peterson, R.S. (Accepted). Team Composition Revisited: Expanding the Team Member Attribute Alignment Approach to Consider Patterns of More than Two Attributes. Organizational Research Methods.
