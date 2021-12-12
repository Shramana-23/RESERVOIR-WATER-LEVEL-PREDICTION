RESERVOIR-WATER-LEVEL-PREDICTION
Auto Regression model of Harangi Reservoir, Karnataka- This is a model made for the Wave2Web Hackathon organised by WRI India powered by Microsoft and Blackrock.

DATASET
1. The dataset is Harangi_mod.csv. The columns are - YEAR,WEEK,FLOW_DATE,PRESENT_TORAGE_TMC,RES_LEVEL_FT,INFLOW_CUSECS,OUTFLOW_CUSECS,STORAGE_CONSD_IN_OUT.In there the column
  'STORAGE_CONSD_IN_OUT' is a calculated column in TMC. It is calculated by the formula (PRESENT_STORAGE_TMC*9505x10^5+INFLOW_CUSECS-OUTFLOW_CUSECS)/9504X10^5. The factor 
  9504x10^5 is the multiplication factor of converting TMC to CUSECS. For Harangi Reservoir the MDDL(minimum drawn down level) is 2788.66 FT. GROSS-STORAGE=8.50 TMC DEAD-STORAGE
  =0.427 TMC
2.The following graphs are plotting to get an idea of time- series analysis -
   WEEK-WISE plot of RESERVOIR WATER LEVEL in FT DIVIDED into subplots according to years.
   LINE PLOT OF RESERVOIR WATER LEVEL with YEAR.
   Plot of the stationary dataset's STORAGE_CONSD_IN_OUT.


AUTO REGRESSION MODEL
1.The dataset is trained on the above model splitting into training and test data(80:20) ratio.
AutoReg adds the ability to specify exogenous variables, include time trends,
and add seasonal dummies.
The mean-squared error is 0.0467
2. Graphs of prection and test data for 'RES_LEVEL_FT' and 'STORAGE_CONSD_IN_OUT' are plotted. 
