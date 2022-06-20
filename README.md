# School_District_Analysis

## Overview of Project

This project was initiated by a request from Maria, the chief data scientist for a local school district. She requested help in analyzing test scores, budgets, and school size for fifteen schools in her district. This data will inform the district's decisions about budget and planning for coming years. This project was completed using Python and the Pandas library in Jupyter Notebook.

### Issue with Thomas High School Scores

After initial analysis was complete, the school board notified Maria that Thomas High School ninth graders had their reading and math scores altered dishonestly somehow. As a result, all of the reading and math scores for Thomas High School ninth graders were removed from the data set, and then the analysis was repeated. This report will identify all the changes that resulted in the removal of these scores.

#### Process to Remove Problematic Scores

To remove the scores in question, I used the loc method to identify all rows with the school name "Thomas High School" and the grade level "9th." I then set both their math and reading scores to "np.nan," or "Not a Number."

![Replace_THS_Math_Scores.png](https://github.com/ehalprin/school_district_analysis/blob/main/Resources/Replace_THS_Math_Scores.png)

#### Recalculating Passing Percentages

Later in the analysis process, I used the loc method again to count only the 10th-12th graders at Thomas High School. As I recalculated the new average reading and math scores, and passing percentages, I used only the 10th-12th graders in my calculation.

![Count_10th_to_12th_graders_THS.png](https://github.com/ehalprin/school_district_analysis/blob/main/Resources/Count_10th_to_12th_graders_THS.png)

## Results

The initial report can be found [here](https://github.com/ehalprin/school_district_analysis/blob/main/PyCitySchools.ipynb). In comparison, the follow-up report, with Thomas High School ninth graders' scores removed, can be found [here](https://github.com/ehalprin/school_district_analysis/blob/main/PyCitySchools_Challenge.ipynb).

### Effect on District Summary

### Effect on School Summary

### Effect on Thomas High School Performance

### Effect on Math & Reading Scores by Grade

### Effect on Scores by School Spending

### Effect on Scores by School Size

### Effect on Scores by School Type

## Summary
