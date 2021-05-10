# Module 4 Python and Pandas Challenge: School District Analysis
---
A supervisor in charge of evaluating the school district budget for the following year has asked for a school district analysis using Pandas in Python. In order to make the best decisions for the budget for the coming year, it is important to omit any results regarding the math and reading scores of ninth grade students at Thomas High School as to not skew the data. Likewise, it is important to compare each school's budget with the math, reading, and overall grade outcomes of the students based on different factors like the school size, type of school, and etc.
---
## District Summary
![School_District Analysis](https://github.com/mbroad1/School_District_Analysis/blob/main/School%20District%20Summary%20DF_Updated.png)
- The **district summary** is unaffected by the new analysis shown above because there were no new scores of reading or math added in this analysis, and no existing scores of reading or math were removed in this analysis.
- The only difference between the new analysis and the older analysis is the formatting of the numbers (see the below image to see the format of the older analysis' numbers)
![School_District Analysis](https://github.com/mbroad1/School_District_Analysis/blob/main/School%20District%20Summary%20DF_Original.png)
---
## School Summary
![School_District Analysis](https://github.com/mbroad1/School_District_Analysis/blob/main/School%20Summary%20DF_Updated.png)
- The only part of the **school summary** analysis that is affected are Thomas High School's "% Passing Math", "% Passing Reading", and "% Overall Passing" values.
  - These values were affected because in the original analysis (shown in the image below), the 9th graders of Thomas High School were included in the total student count; however, the math scores and reading scores of the 9th graders at Thomas High School are **all** missing.
![School_District Analysis](https://github.com/mbroad1/School_District_Analysis/blob/main/School%20Summary%20DF_Original.png)
- Since these values are missing, the original calculations for "% Passing Math", "% Passing Reading", and "% Overall Passing" are all skewed to be lower because not all students included in the total for the division to get these percentages have scores (aka, the 9th graders do not have scores).
- Therefore, when you convert the math and reading scores of the 9th graders from Thomas High School to "NaN" (null scores) and exclude the 9th graders in the total student count to get the percentages for math, reading, and overall passing, you will get the true values of what the "% Passing Math", "% Passing Reading", and "% Overall Passing" are actually supposed to be in Thomas High School.
- In the original analysis for Thomas High School:
  - % Passing Math = 66.91
  - $ Passing Reading = 69.66
  - % Overall Passing = 65.08
- In the updated analysis for Thomas High School:
  - % Passing Math = 93.27
  - $ Passing Reading = 97.31
  - % Overall Passing = 90.95
