# Kickstarting with Excel

## Overview of Project
Louise's play "Fever" came close to its fundraising goal in a short amount of time. Now, she wants to know how different campaigns fared in relation to their launch dates and their funding goals.

### Purpose
The purpose of this analysis is to provide Louise with actionable information such that her project has the highest possible chance for success.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The below graph shows the relationship between campaign outcomes and month of launch. The numbers on the left-hand side represent number of Theater campaigns while the months corresponding to Launch Date are shown at the bottom. The three different color lines represent the outcomes, as indicated by the graph's legend on the right-hand side.

![Theater Outcomes vs Launch Date](https://github.com/cdeanatx/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The below graph shows the relationship between campaign outcomes and fundraising goal. The numbers on the left show the percentages of outcomes and the text at the bottom shows the range of fundraising goals.

![Theater Outcomes vs Fundraising Goal](https://github.com/cdeanatx/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
I really didn't encounter any difficulties while completing this project. However, I could see others struggling with creating "Deliverable 2." Specifically, creating the `countifs()` functions to pull in the relevant data.

It has always seemed strange to me that quantitative data is represented as a string within this Excel function. For example: `Kickstarter!$D:$D,">=25000",Kickstarter!$D:$D,"<30000"` represents "Goal is between 25,000 and 30,000" but `Kickstarter!$D:$D>=25000,Kickstarter!$D:$D<30000` would seem to make more sense.
 
## Results

**Based on the [Analysis of Outcomes Based on Launch Date](#analysis-of-outcomes-based-on-launch-date):**

- The best months to launch would be May or June, both of which have greater than 2:1 success to failure ratio.
- The worst months to launch would be December or October, both of which have less than 1.3:1 success to failure ratio.

**Based on the [Analysis of Outcomes Based on Goals](#analysis-of-outcomes-based-on-goals) and knowledge of Louise's project:**

- I would recommend maintaining a goal between $10,000 and $15,000. Since Louise's initial estimate that the play would cost $12,000, this should be a reasonable amount.

**This dataset has some considerable limitations:**

- We are compairing USD to foreign currencies, which create flawed analysis. It makes no sense to compare USD to foreign currencies on a 1:1 basis.
- Due to a lack of data points for campaigns with a fundraising goal above 15,000, we cannot be confident in the results of that analysis.

**Recommendations for additional/different data visualizations:**

- Change _Theater Outcomes Based on Launch Date_ to percentages and filter by US, since we have sufficient data points for each month in the US (ranges from 56 in December to 98 in June).
- Filter _Outcomes Based on Goal_ by US only and adjust fundraising goal ranges to fit the number of data points. We would like keep the first few ranges the same, as there are plenty of data points, but consider creating larger ranges for goals above $20,000.
- Add visualization to compare Outcomes vs. Completion Date (just like the Launch Date visualization).
- Add visualization to compare Outcomes vs. Length of Campaign (Completion Date - Launch Date).
