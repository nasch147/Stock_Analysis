# Stock_Analysis

## Overview of Project
The Client has asked for an analysis of the respective trading volumes and returns of 12 stocks in the green energy sector in 2017 and 2018. Originally, I prepared a macro to analyze this particular set of stocks.  Though the original macro performed the analysis much faster than manually manipulating the data, its run time gave rise to concerns regarding its scalability to larger data sets. the Client also expressed the interest to expand this macro to larger data sets. I was asked as to the ability to refactor the VBA code for the macro to reduce its run time. 

## Results
### Stock Performance
![2017_Returns](/Resources/2017_Returns.png)
![2018_Returns](/Resources/2018_Returns.png)

Overall, 2017 returns in the portfolio significantly outperformed returns for the same in 2018. The size of the returns in each year and the drastic differences between the two years suggests a high degree of volatility.  Such levels of volatility in the portfolio present a significant investment risk. Of course, this must be balanced against the opportunity for outsized returns. These investments would be appropriate in the context that they would be incorporated as a relatively underweighted portion of a much larger, more well-diversified portfolio.

### Script Performance
![2017_Refactored_Runtime](/Resources/2017_Runtime.png)
![2018_Refactored_Runtime](/Resources/2018_Runtime.png)

Overall, refactoring efforts resulted in approximately halving the macro's run time. 

![Refactored_Loop](/Resources/Refactored_Loop.png)

The improvement in performance was primarily generated from a more efficient construction of the script. A new loop structure was employed looping through the data in the workbook once as opposed to each row or ticker repetitively. The use of arrays and indexes were also utilized to enhance performance and enhance its utilization on a broader scale. 

## Summary
### Advantages and Disadvantages of Refactoring
The main advantage of refactoring code is to make the code more robust, more efficient, and easier to read and interpret. As is often the case, the first attempt in automating such an analysis through VBA can be inefficient and hastily constructed. As in the current instance, an original macro is often purpose-built to handle a specific scenario without thought to its application on a wider scale. The main disadvantage is the risk of corrupting the current code which works functionally well for its task at hand. It can also require an onerous level of coordination between the code development team. 

### Refactoring as it Relates to the Current Project
Following the incorporation of a more efficient loop structure, the macro ran significantly faster and would be much more appropriate for use in a larger data set. The code is also formatted and noted to be easier to read, understand, and build upon for future use. I did encounter several issues with the restructuring causing the script not to run which were eventually fixed with an amount of time and effort. 

---
# Green Stock Analysis Dataset - [VBA_Challenge_Workbook](VBA_Challenge.xlsm)
