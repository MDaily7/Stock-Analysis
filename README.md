# Stock Analysis
## Overview of Project
### Background and Purpose
Our client Steve has just recieved his degree in finance and is now helping his parents with stock investments. He has asked for help with setting up VBA macros to quickly analyze data for a variety of stocks. We began by setting up a simple macro to analyze the DQ stock that his parents were interested in, but we quickly progressed to creating a macro to anlayze all of the stocks Steve had compiled data for. Finally, we have refactored the All_Stocks_Analysis code so that it runs more efficiently and will be better suited for larger amounts of stocks for Steve to analyse in the future. 
## Results
Steve will be able to show his parents that, despite doing quite well in 2017, DQ was the worst performing stock in 2018 of the stocks he compiled data for as can be seen in [2018 Stock Data](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/Resources/VBA_Challenge_2018_StockData.png). However, when comparing [2017 Stock Data](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/Resources/VBA_Challenge_2017_StockData.png) to the previous image, its clear that almost all stocks did better in 2017 with the exception of "RUN" which had a significantly better return in 2018. It may be difficult for Steve to conclude much without more data for each of the stocks, but using only what we have, it seems safer to go with "RUN" for investment purposes. The "ENPH" stock also did well in 2018, but it is down roughly 50% from the previous years return, so it may be a riskier option. Luckily, thanks to the code provided to Steve, he will easily be able to add additional years of data and quickly analyze them. This will work no matter the amount of rows of data he has for any particular year thanks to the dynamic way in which the row end was coded as a RowCount [RowCount Code](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/Resources/RowCountCode.png). However, he will need to have any new  tickers he wishes to analyze added to the [ticker array](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/Resources/tickersArray.png). Fortunately, analyzing additional stocks should continue to be a quick process thanks to the refactored code which performs much faster than the original code as can be seen by comparing the execution times of the [2017 Original Execution Time](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/Resources/VBA_Original_2017.png) and [2018 Original Execution Time](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/Resources/VBA_Original_2018.png) to the [Refactored 2017 Execution Time](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/Resources/VBA_Challenge_2017.png) and [Refactored 2018 Execution Time](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/Resources/VBA_Challenge_2018.png). 
## Summary
### General Advantages and Disadvantages of Refactoring Code
In general, the advantages seem to outweigh the disadvantages when refactoring code. The purpose of refactoring is to make the code more efficient and or more readable. A more efficient code means that it can carry out its task more quickly with larger amounts of data by taking less steps or using less memory. The refactored code in this analysis was approximately .66 seconds faster than the original code. However, the data set being looked at was fairly small only encompassing twelve stock tickers. The roughly 6.4 times increase in speed could be tremendous as more tickers are added. Furthermore, creating more readable code would be hugely beneficial in a more collaborative environment as it would be far more conducive to working together. In the scenario for this analysis, both sets of code were annotated quite thoroughly, but the importance of readability can still be highlighted. For example, if Steve ever wanted to change the starting row of data, he could easily do so by going to the part of code annotated as defining the [rowStart](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/Resources/rowStart%20definition%20annotation.png) and changing that variable accordingly. As far as I can tell, the only real disadvantage of refactoring code is the time invested into doing it. If the data set being worked on was never expected to become larger, then perhaps this time investment would not be worth it. Once again using our refactored code as an example, the execution time difference is insignificant if no additional data or tickers are expected to be added. In which case, refactoring the code would not really have been worth the time investment. In conclusion, it is probably best to consider the purpose of the code and determine if making it more efficient or readable will be worth the time investment of refactoring. 
### Advantages and Disadvantages of Refactoring this Projects Code
As was already touched upon previously, refactoring the original code for this project did make the macro faster. However, it did take several hours to refactor and resulted in a fairly marginal decrease in elapsed time practically speaking. If the data set is never expected to expand to include more tickers, then it may have not been worth it in the end. However, the benefit of refactoring the code will increase every time an additional ticker is added. Another disadvantage of refactoring the code in this scenario is that it might be more confusing to Steve to utilize on his own. Ideally, the annotations should overcome this problem, but this may not be the case if he is not very familiar with VBA. This could be true for the original script as well, but it is slightly less technical and there are fewer adjustments that need to be made when adding additional tickers.
## Resources
All images can be found in the [ResourcesFolder](https://github.com/MDaily7/Stock-Analysis/tree/main/Challenge/Resources), and the data and code can be found in  
[VBA_Challenge](https://github.com/MDaily7/Stock-Analysis/blob/main/Challenge/VBA_Challenge.xlsm)
