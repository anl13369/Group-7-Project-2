# Group-7-Project-2

# Group 7 Team Members:
1. Andrea Lam [@anl13369](https://github.com/anl13369)
2. Sierra Cross-Thompson [@sierract](https://github.com/sierract)
3. Meghana Kottapalli [@meghanakottapalli03](https://github.com/MeghanaKottapalli03)
4. Cecilia Rizo-Patron [@cecirp](https://github.com/cecirp)

# Describing your data set and what data it contains:

# 2 questions relevant to our data set and why they are interesting and important:
**1. Which licensees rely most heavily on promotional deductions relevant to the revenue?**

Importance: Promotional deductions (bonuses, free spins, etc.) significantly impact the revenue generated from players, it allows licensees to see how heavily their profitability relies on these deductions, and they could then use to this to adjust/optimize their promotional strategies

Relation to data set: We pulled the “Licensee,” “Promotional Deductions,” and “Total Gross Gaming Revenue” columns to compare the promotional deductions to the total gross gaming revenue

**2. How do each licensee’s total wagers compare to Patron Winnings across different years?**

Importance: Each licensee can see during what time of year they are spending the most money on online gambling, and they can then use this information to adjust their budget for gambling expenses

Relation to data set: We used the “Licensee”, “Month Ending”, “Wagers”, and “Patron Winnings” columns to compare different licensees’ wagers across multiple time periods

# The manipulations applied to the data set as part of the analysis:

We altered the dataset to exclude the notes column, finding that most of the observations did not report a value. Across all the rows, only one row contained a single piece of quantitative data. The data set also lacks a clear explanation of what the value achieves or reports, meaning that the column lacks analytical value.

# Analysis and Results:
**1. Which licensees rely most heavily on promotional deductions relevant to the revenue?**
![image](https://github.com/user-attachments/assets/3626a7a2-2a50-4e63-8b31-add46762d304)
This graph shows the ratio of promotional deductions to total gaming revenue, which gives us a clearer view of how dependent each licensee is on incentives to drive their business but relative to what they earn rather than in cash terms.
- MPI Master Wagering License CT, LLC leads with the highest ratio at 9.71%, meaning nearly 10 cents of every dollar earned comes from promotions. This shows a strong dependence on bonuses and similar strategies to attract or keep players.
- Mohegan Digital, LLC follows with 8.01%, also showing a fairly high reliance, though slightly more conservative than MPI.
- MPTN On-Reservation sits at 7.42%, still relatively high, especially considering their smaller overall revenue. This might suggest they’re trying to stay competitive with bigger players through aggressive promotions.
- Mohegan Tribe On-Reservation comes in lowest at 5.15%, suggesting a more modest and potentially sustainable promo strategy.

**Data Transformations Relevant to Question 1**
A calculated field was introduced to determine the percentage of revenue affected by promotional deductions.
This metric helps quantify the financial significance of these deductions on total gross revenue.

Calculation Process:
- Formula: Promotional Deductions ÷ Total Gross Gaming Revenue
- Labeled as DeductToRevenue in the dataset for reference.

Purpose & Impact:
- Measures the extent to which promotions influence revenue.
- Helps evaluate financial performance and reliance on promotional deductions.
- Supports informed decision-making regarding promotional strategies and optimization.

**Implications:**
Looking at these ratios helps licensees understand how much they are spending and how that spending is truly impacting their financial performance.
A higher ratio may indicate more player engagement in the short term, but it also may lead to higher costs and thinner margins since the company supplies the promotional credits. 
A lower ratio may indicate a more sustainable model, relying less on constant incentives. But, this may reduce the frequency of gameplay since users are not as incentivized to play.
This means that the insights from our analysis can help licensees determine whether their current promotion strategy is worth the trade off, or if there is room to scale back while keeping revenue steady. 

**2. How do each licensee's total wagers compare to Patron Winnings across different years?**



# Tableau Packaged Workbook:
