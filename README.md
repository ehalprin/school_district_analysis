# School_District_Analysis

## Overview of Project

This project was initiated by a request from Maria, the chief data scientist for a local school district. She requested help in analyzing test scores, budgets, and school size for fifteen schools in her district. This data will inform the district's decisions about budget and planning for coming years. This project was completed using Python and the Pandas library in Jupyter Notebook.

### Issue with Thomas High School Scores

After initial analysis was complete, the school board notified Maria that Thomas High School (THS) ninth graders had their reading and math scores altered dishonestly somehow. As a result, all of the reading and math scores for THS ninth graders were removed from the data set, and then the analysis was repeated. This report will identify all the changes that resulted in the removal of these scores.

#### Process to Remove Problematic Scores

To remove the scores in question, I used the loc method to identify all rows with the school name "Thomas High School" and the grade level "9th." I then set both their math and reading scores to "np.nan," or "Not a Number."

![Replace_THS_Math_Scores.png](https://github.com/ehalprin/school_district_analysis/blob/main/Resources/Replace_THS_Math_Scores.png)

#### Recalculating Passing Percentages

Later in the analysis process, I used the loc method again to count only the 10th-12th graders at THS. As I recalculated the new average reading and math scores, and passing percentages, I used only the 10th-12th graders in my calculation.

![Count_10th_to_12th_graders_THS.png](https://github.com/ehalprin/school_district_analysis/blob/main/Resources/Count_10th_to_12th_graders_THS.png)

## Results

The initial report can be found [here](https://github.com/ehalprin/school_district_analysis/blob/main/PyCitySchools.ipynb). In comparison, the follow-up report, with THS ninth graders' scores removed, can be found [here](https://github.com/ehalprin/school_district_analysis/blob/main/PyCitySchools_Challenge.ipynb).

### Effects from Removing Problematic Scores

- In the district summary:
  - The overall average math score fell from 79.0 to 78.9;
  - The percent passing math fell from 75% to 74.8%;
  - The percent passing reading fell from 86% to 85.7%; and
  - The overall percent passing fell from 65% to 64.9%.
- In the school summary:
  - THS's average math score fell from 83.42 to 83.35;
  - THS's average reading score increased from 83.85 to 83.89;
  - THS's percent passing math decreased from 93.27% to 93.19%;
  - THS's percent passing reading decreased from 97.31% 97.02%; and
  - THS's overall percent passing decreased from 90.95% to 90.63%.
- THS's performance compared to other schools did not change; they were still the second highest performing school based on overall passing percentage.
- In the comparison of average math and reading scores by grade level, Thomas High Schools' averages for the 9th grade were "NaN."
- There was no effect on the scores by spending range.
- There was no effect on the scores by school size.
- There was no effect on the scores by school type.

## Summary

Overall, the larger level initial analysis of the school district data held true, even when THS's 9th graders' scores were removed: there was no effect on the data when looking at scores by spending range, school size, or school type. However, the district summary's scores were affected, with a decrease in average math score, and percent passing math, reading, and both math and reading. Obviously THS's school summary was also very affected, though most of the changes were less than 1 unit (1 point or 1 percentage point). Interestingly, their average reading score actually increased with the removal of the 9th graders' scores, indicating that the 10th through 12th graders at THS performed very well on that test (presumably honestly). Despite the decrease in THS's scores in the follow-up analysis, they were still the 2nd highest performing school overall.
