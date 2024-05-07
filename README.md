# mgt4250spring2024final
Author(s): Tyler Vining (tvining@elon.edu)

## Project Description
This repository is for the class project of MGT 4250 at Elon University.

In light of the compelling evidence supporting the critical need for equitable compensation practices, this project embarks on a detailed examination of the underlying factors influencing employee salaries. By leveraging a comprehensive, public dataset from Kaggle (Employee_Salaries.csv) and applying a multifaceted analytical approach, the aim is to unravel the complexities of salary disparities within the county of Montgomery, MD. This endeavor not only seeks to address the immediate concerns highlighted by prior research but also to pave the way for actionable insights that can drive organizational and societal change toward fairness and transparency in compensation. 
### Questions of Interest 
- Q1: Are there any signs of a gender pay gap within specific departments?
- Q2: How does pay vary and do some departments or job grades have wider salary ranges than others?
- Q3: How much do employees rely on overtime across different departments or genders and how does this affect their total earnings?
### Importance Statement 
These questions and their accompanying visualizations are *especially* **important** because:
1. By comparing the average salaries between genders within each department and grade level using grouped bar charts, Figure 1a aims to highlight any disparities in base pay that could exist even within the same roles or levels. Figure 1b takes this analysis one step further, accounting for the effects overtime pay has on wage disparities as well. To do so, a calculated field summing Base Pay and Overtime Pay was created. 
2. By utilizing a box plot at the departmental level and a box and scatter plot at the grade level, the distribution of salaries across different departments and grade levels can be displayed. This will aid in understanding the compensation structure and variance within the employment system. By plotting each employee’s salary against their department, the spread and concentration of salaries within each department can be visually inspected. This helps in understanding if certain departments are inherently paid more or less, potentially due to the nature of the work, market demand for specific skills, or historical biases. By incorporating an average salary line within each grade level scatter plot, a clear measure of central tendency is provided, allowing for comparative analysis of how many employees earn above or below this mark. This reference line is crucial for exploring which grade levels typically exceed the average and identifying significant deviations that may require further investigation.
3. By creating scatter plots that compare base salary against overtime pay for all employees, categorized by gender and segmented by department, it becomes clear how overtime reliance differs across various organizational sectors and between genders, as well as its effect on total compensation. This visualization not only highlights discrepancies in overtime allocation but also helps in understanding how these disparities contribute to the overall earnings of different employee groups, thereby informing more equitable compensation strategies.

## Data Description
### Source and Collection Methodology 
The dataset created by Sahir Maharaj and titled “Employee_Salaries.csv” encompasses a comprehensive array of data points across 10,291 records, reflecting the diverse and complex landscape of employee compensation within Montgomery County. It spans a broad spectrum of departments and divisions, indicating a rich variety of job functions and responsibilities captured within 42 distinct departments and further detailed across 627 unique divisions. This granularity facilitates an in-depth exploration of compensation structures and disparities, not just at a broad organizational level but also within specific operational units.

Capturing a detailed snapshot of the workforce’s gender distribution (58% Male, 42% Female), the dataset acts as a vital tool for examining gender-based salary discrepancies. It offers a comprehensive view of employee compensation, blending both fixed salaries and variable earnings such as overtime and longevity pay. Notably, the salary range—stretching from $11,147.24 to $292,000.00—reveals the organization’s diverse compensation strategies and underscores the urgency of investigating potential inequities. Thus, the detailed compensation data in "Employee_Salaries.csv" from Kaggle will facilitate a focused examination of gender pay gaps across roles, salary variations by department and grade, and the impact of overtime on overall compensation, spotlighting areas where disparities demand attention and action.

### Data Characteristics 
- *Department* (string): Abbreviation representing the department to which the employee belongs (e.g., ABS for Alcohol Beverage Services).
- *Department_Name* (string): Full name of the department.
- *Division* (string): Specific division within the department.
- *Gender* (string, binomial, categorical): Employee’s gender (M or F).
- *Base_Salary* (float): Employee’s base annual salary in USD.
- *Overtime_Pay* (float): Annual overtime pay received by the employee in USD.
- *Longevity_Pay* (float): Additional pay received by employees based on the length of their service.
- *Grade* (string): Grade level within the organization, indicating the job level or classification.
 
## Interpreting Visualizations
### 1. Gender Pay Gap Bar Charts
As aforementioned, Figure 1a aims to highlight any disparities in base pay that could exist even within the same roles or levels, while Figure 1b takes this analysis one step further by accounting for the effects of overtime pay on wage disparities. Before conducting the analysis, departments with only females or males—specifically BOA, IGR, ORE, and ZAH—were removed, leaving 38 out of the total 42 departments available for gender comparison.

Of these 38 departments analyzed in Figure 1a, women were found to have a higher average base salary in only 14 departments, representing 36.84% of the department sample. By integrating average overtime pay into the salary analysis, Figure 1b further illustrates gender wage disparities. That is, accounting for overtime pay exacerbated the disparity already discovered, resulting in only 9 out of the 38 departments—23.68% of the sample—showing women being paid more. This significant decrease from 36.84% to 23.68% suggests that overtime pay significantly favors men, leading to an increase in their overall average earnings compared to women.

To illustrate this point further, consider specific department abbreviations where this trend is notable. Departments such as CEC, COR, DGS, DOT, and FRS are prime examples where overtime pay appears to disproportionately benefit men, resulting in higher overall average earnings for male employees compared to their female counterparts.

These findings underscore the need for targeted interventions to address gender-based pay disparities, particularly in the context of overtime pay distribution. Organizations should consider conducting thorough audits of their compensation practices, implementing transparent salary structures, providing training to mitigate biases in decision-making processes, and promoting gender diversity in leadership positions. Additionally, ongoing monitoring and evaluation are crucial to ensure that these measures effectively promote gender equity in compensation.

![image](https://github.com/tvining9/mgt4250spring2024final/assets/168783531/fdbad73e-f5c3-4c18-91f7-d7a1429e4e59)

### 2. Departmental and Grade-Level Salary Box and Scatter Plots
The visualizations, Figure 2a and Figure 2b, aim to provide insights into salary distribution across departments and grade levels, aiding in understanding compensation structures and variances within the employment system.

Figure 2a utilizes a box plot at the departmental level to display the distribution of salaries. Notable observations include the lowest paying department, OAG, with a base salary of $11,147 for males and the highest paying department, CEX, with a male employee earning $292,000 and a female employee earning $22,526. CEX exhibits the largest pay variance among departments, followed by CAT, HHS, and OMB, indicating significant salary ranges.

An important aspect of Figure 2a is the anomaly detection and distribution analysis. Out of 29 potential anomalies requiring further review, only 10 are female, representing 34.48% of the anomalies. This disparity highlights the need for deeper examination of gender-related pay discrepancies.

Further insights from Figure 2a reveal that 9 out of 21 employees below $40,000 base salary are female. Additionally, approximately 44% of employees below the average salary line are female, compared to 38% above the average line. Moreover, only about 35% of employees earning above $200,000 are female, with no females earning above $240,000. These findings underscore potential gender-related disparities in salary distribution.

![image](https://github.com/tvining9/mgt4250spring2024final/assets/168783531/8fd046d9-a549-48cd-960b-9174dcc2cd31)

Figure 2b sheds light on salary determinants at the grade level, showing that salary tends to be influenced by grade. That is, salary and grade level positively correlate, and as such, the higher in the company the more money one makes. However, disparities exist due to large salary ranges among certain grade levels, particularly executive grades (e.g., EX1, EX3), manager grades (e.g., M2, MD3), and those without a designated grade. The large range of employees without a designated grade is most likely due to the inability to access relative experience, skills, or credentials (hence no grade level assigned). Another explanation of the variance could be due to a lack of payment structure for "un-graded" employees, thus resulting in other factors like bias playing large roles in forming compensation structures for those without a designated grade. Other possible contributing factors to these disparities may include the ability of upper management to influence the wages they or others receive, or the potentially large disparity between relative experience and credentials among upper management (thus reflected in their pay).   

![image](https://github.com/tvining9/mgt4250spring2024final/assets/168783531/e6e216c6-be45-47b8-a864-206382154936)


### 3. Overtime Impact Scatter Plots
Figure 3 showcases a scatter plot juxtaposing base salary against overtime pay, focusing on five specific departments: COR, FRS, DOT, POL, and SHF. These departments were chosen because, among all 38 departments available for gender pay-gap analysis, they demonstrate the highest reliance on overtime pay. This selection highlights the significant disparity between men and women in their reliance on overtime pay, a finding consistent with the notable observation emphasized in Figure 1b: overtime pay disproportionately benefits males over females. That is, despite males and females earning similar average annual base salaries across highlighted departments such as COR, FRS, DOT, POL, and SHF, males receive considerably more in average overtime pay than females. This disparity highlights a gender-based pay gap, evident not only in base salary but also in overtime pay.
![image](https://github.com/tvining9/mgt4250spring2024final/assets/168783531/f9726992-0d52-4a07-9aa8-03ef0315cd43)

## Discussion & Summary
The examination of salary disparities, particularly the gender pay gap, is substantiated by extensive research demonstrating that wage differences persist across genders within similar roles, grades, and departments, a finding highlighted by Blau and Kahn in their 2017 study published in the *Journal of Economic Literature*. This issue not only poses ethical concerns but also has broader implications for economic equality, like the impact of gender equality on economic growth (Fluchtmann et al., 2024). Furthermore, the importance of understanding compensation variance across departments and grades is reinforced by principles of public administration that advocate for equitable and transparent compensation systems to maintain fairness and reduce turnover, a perspective championed by Rainey in his 2009 work, *Understanding and Managing Public Organizations*.

The role of overtime in compensation, governed by regulations such as the Fair Labor Standards Act, presents legal and well-being considerations, suggesting that a thorough analysis of its impact on total earnings is crucial for organizational practices, as noted by the U.S. Department of Labor. The call for transparency in pay practices is supported by research from Bamberger and Belogolovsky in 2010, which found that such transparency significantly affects individual task performance, as detailed in their study in *Personnel Psychology*.

On a legal front, adherence to equitable compensation practices is not merely ethical but is mandated by laws like the Equal Pay Act of 1963 and Title VII of the Civil Rights Act of 1964, with the Equal Employment Opportunity Commission providing guidance on compliance (Equal Pay Act of 1963, n.d.; Protections Against Discrimination and Other Prohibited Practices, 2013). This legal framework underscores the necessity of analyzing and addressing pay disparities to foster an inclusive workplace culture.

Moreover, the societal and economic benefits of equitable compensation practices extend beyond organizational boundaries, contributing to reducing poverty, supporting family stability, and enhancing economic growth through increased consumer spending. The Credit Suisse Research Institute's 2016 report, *The CS Gender 3000: The Reward for Change*, elaborates on these broader implications, linking equitable pay practices to significant economic and social advantages.

Through this lens, the comprehensive analysis of salary factors not only addresses immediate concerns of fairness and legal compliance but also aligns with wider objectives of promoting gender equality, economic stability, and social justice, reflecting a deep understanding of the interconnectedness of organizational practices and societal well-being.

### AI and Article Insights 
When prompted the three questions analyzed in this project, ChatGPT 4 provided the following insightful output: 
- "Q1: Analysis of salary data reveals disparities between genders within departments, with women often earning less than men in comparable roles.
- Q2: A review of salary structures across departments and job grades demonstrates varying pay scales, with some departments or higher job grades showing wider salary ranges compared to others. For example, roles with variable performance-based incentives or commission structures often feature wider salary ranges to accommodate fluctuations in earnings based on individual performance levels.
- Q3: Data on overtime usage among employees in different departments and genders illustrates differential reliance, influencing total earnings. For instance, men might engage in more overtime work, thereby potentially increasing their total earnings compared to women in similar roles."

The visualizations in my study, particularly Figures 1a, 1b, and 3, corroborate both the literature review and the insights provided by ChatGPT 4. These figures effectively highlight gender-based disparities in base and overtime pay, reflecting the findings from the discussed academic studies and generative AI analysis. Furthermore, while Figures 2a and 2b highlighted varying pay scales for Executives and Managers and ChatGPT 4 did not, the AI was able to provide a viable reason for large salary ranges not yet considered: variable performance-based incentives or commission structures. Conjoined, the consistency among these insights not only validates the visual representation used in the project but also emphasizes the significance of visual tools in understanding and communicating complex data patterns. Expanding on this, the visualizations serve as a powerful narrative device that reinforces the interconnected nature of organizational practices and societal impacts, illustrating how there are still inequitable compensation practices that must be proactively addressed to drive broader economic and social benefits in the future.

### References
1. AG, C. S. (2016, September). Credit Suisse Research Institute Releases the CS Gender 3000: The Reward for Change Report Analyzing the impact of Female Representation in Boardrooms and Senior Management. https://www.prnewswire.com/news-releases/credit-suisse-research-institute-releases-the-cs-gender-3000-the-reward-for-change-report-analyzing-the-impact-of-female-representation-in-boardrooms-and-senior-management-300332558.html
2. Bamberger, P., & Belogolovsky, E. (2010). The impact of pay secrecy on individual task performance. Personnel Psychology, 63(4), 965–996. https://doi.org/10.1111/j.1744-6570.2010.01194.x
3. Blau, F. D., & Kahn, L. M. (2017). The Gender Wage Gap: Extent, Trends, and Explanations. Journal of Economic Literature, 55(3), 789–865. https://doi.org/10.1257/jel.20160995
4. Equal Pay Act of 1963. (n.d.). US EEOC. Retrieved April 3, 2024, from https://www.eeoc.gov/history/equal-pay-act-1963
5. Fluchtmann, J., Keese, M., & Adema, W. (2024). Gender equality and economic growth: Past progress and future potential (OECD Social, Employment and Migration Working Papers 304; OECD Social, Employment and Migration Working Papers, Vol. 304). https://doi.org/10.1787/fb0a0a93-en
6. Protections Against Discrimination and Other Prohibited Practices. (2013, July 16). Federal Trade Commission. https://www.ftc.gov/policy-notices/no-fear-act/protections-against-discrimination
7. Rainey, H. G. (2009). Understanding and Managing Public Organizations, Fourth Edition (4th ed.). Jossey- Bass.



![image](https://github.com/tvining9/mgt4250spring2024/assets/168783531/6e5e64ed-101f-437e-b303-23c80a0aadf9)

[Elon University](https://www.elon.edu/)
