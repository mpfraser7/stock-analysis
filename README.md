# stock-analysis
## VBA Challenge

### Overview of Project
Initially, I wrote a VBA code that analyzes a list of 12 stocks. The analysis provides the daily volume and return % for each stock, based on the fiscal year provided in a message box. The purpose of the challenge was to refactor the code and make it run quicker. Instead of going through the entire database 12 times, once for each stock, the refactored code only goes through the database once while storing the important values in variables. The result of the refactored code is explained below.

https://github.com/mpfraser7/stock-analysis/blob/main/VBA_Challenge.xlsm

### Results
First, let's talk about the stock performance, comparing year 2017 with 2018. The average volume and total volume for all stocks is very similar from year to year. However, the return % is drastically different. In 2017, the average return is 67%, compared to -9% in 2018. The best performing stock in 2017 was DQ. The best performing stock in 2018 was RUN.
![](https://github.com/mpfraser7/stock-analysis/blob/main/Stock%20Performance%20Comparison.png)



Now, let's talk about the difference between the old code and the refactored code. There was a massive increase in performance for both years. Referring to the screenshots below, the refactored shaved approximately 90% from the original code. It was approximately 8 to 9 times faster. This is mostly due to the fact that the refactored code only had to go through the database once, rather than 12 times.

Original 2017

![](https://github.com/mpfraser7/stock-analysis/blob/main/Original%202017.png)

Original 2018

![](https://github.com/mpfraser7/stock-analysis/blob/main/Original%202018.png)

Refactored 2017

![](https://github.com/mpfraser7/stock-analysis/blob/main/2017%20Refactored.png)

Refactored 2018

![](https://github.com/mpfraser7/stock-analysis/blob/main/2018%20Refactored.png)
### Summary

Refactoring a code is a fine balance. It can save a lot of processing time, but it can also be very tedious and laborious. Before deciding on refactoring a code, you have to think if it is worth the effort. Using this code as an example, saving less than a second for a code that would be ran once a day at the most, might not be worth it. It would take way too many years to reach the break even point. However, if the code went from taking 10 minutes to less than a second, then it would be very well worth it. Before refactoring a code, you have to take into account the volume of the data, run time, velocity, frequency, and other variables. In hindsight, I would not have refactored the code in the stock analysis challenge.
