# Group-7-Project-2

# Group 7 Team Members:
1. Andrea Lam [@anl13369](https://github.com/anl13369)
2. Sierra Cross-Thompson [@sierract](https://github.com/sierract)
3. Meghana Kottapalli [@meghanakottapalli03](https://github.com/MeghanaKottapalli03)
4. Cecilia Rizo-Patron [@cecirp](https://github.com/cecirp)

# Describing your data set and what data it contains:

We found our data from the US Data Catalog which displays information collected from online casino gaming in Connecticut. The spreadsheet is a mix of qualitative and quantitative data to explain the different earnings, promotions and wagers that occurred per month.

The **qualitative data** includes the four different licensees in the state of Connecticut, the fiscal year of operation and the month ending in which data was recorded.

The **quantitative data** records many different aspects key to earnings of both players and the casino:

**Wagers** records the total amount bet by patrons, or players of the online casino games.

**Patron Winnings** is the total amount won by players and represents the amount the casino games must pay out to the players.

**Cancelled Wagers** are bets that are voided or cancelled for reasons like technical issues or user cancellation.

**Online Casino Gaming Win or Loss** records the net win or loss for each licensee.

**Promotional Coupons or Credits Wagered** represents the value of promotions that are used as marketing tools to get people to gamble. This can be anything from free spins on games or credits given on the game that transfers to money.

**Promotional Deduction** is also a marketing tool used to get people to gamble but is different from coupons or credits as it is the monetary cost of giving a player a bonus. In other words, it is the cost of providing a bonus. For example, if a bonus of $50 is given out to a player, and this causes the casino to pay out an additional $150 to a player, the $150 is recorded as a deduction here from their gross revenue.

**Total Gross Gaming Revenue** is the revenue recorded before any promotional costs. This is simply the patron winnings subtracted from the wagers. The total is what the casino retains after paying customers.

**Payments** refers to the number of payments made to customers that month. This is not completely clear in the data, but it can be inferred when the data is compared to the other quantitative data.

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
<p align="center">
<img src="https://github.com/user-attachments/assets/3626a7a2-2a50-4e63-8b31-add46762d304" width="600">
</p>

The graph shows promotional deductions as a percentage of total gaming revenue, highlighting each licensee’s reliance on incentives.
- MPI Master Wagering License CT, LLC leads at 9.71%, showing strong dependence on promotions.
- Mohegan Digital, LLC follows at 8.01%, maintaining a high but slightly more conservative reliance.
- MPTN On-Reservation, at 7.42%, likely uses aggressive promotions to compete despite smaller revenue.
- Mohegan Tribe On-Reservation ranks lowest at 5.15%, suggesting a more modest, sustainable strategy.

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

These ratios help licensees assess spending and its impact on financial performance.
- A higher ratio may boost short-term engagement but increase costs and tighten margins due to promotional credits.
- A lower ratio suggests a more sustainable model with fewer incentives but could reduce gameplay frequency.
- Insights from this analysis help licensees decide whether to maintain or adjust their promotion strategy while sustaining revenue.

**2. How do each licensee's total wagers compare to Patron Winnings across different years?**
<p align="center">
<img src="https://github.com/user-attachments/assets/53800f2f-d927-4fa3-8818-fd694cddfa67" width="600">
</p>

Licensee Wager Trends (2021–2025)
- Red and blue lines represent the top two licensees by wager volume.
- Both show strong growth from 2021 to 2024, indicating increasing player engagement.

- Sharp decline in 2025 likely due to:
  - An In-Progress/Incomplete year (partial data)
  - Seasonal or market factors

- Nearly identical trends suggest:
  - Similar market conditions
  - Competitive strategies or parallel responses to industry changes

<p align="center">
<img src="https://github.com/user-attachments/assets/98d14cb8-0a85-47ed-aeca-a5301838753a" width="500">
</p>

  In contrast, the licensees represented by the orange and teal lines report significantly lower wager volumes throughout all years. Their relatively flat trajectories imply steady but minimal activity, which could reflect niche markets, localized player bases, or more limited promotional strategies. Despite their small scale, these licensees remain consistent over time, showing no dramatic spikes or drops.
  
Overall, the charts provide clear insights into how each licensee is evolving independently over time, with larger operators showing aligned growth trends and smaller entities maintaining a low but steady presence.

<p align="center">
<img src="https://github.com/user-attachments/assets/e58ff31c-d203-4e22-bd90-48782e02640a" width="650">
</p>

The graph compares total wagers to player winnings across five time points, highlighting overall betting activity and return behavior.
- Mohegan Digital, LLC and MPI Master Wagering License CT, LLC show similar trends - steady growth through mid-years, then a decline in the latest data.
- Mohegan Tribe On-Reservation lacks 2021 data but peaks in 2023, later aligning with industry payout trends.
- MPTN On-Reservation starts lowest in 2021 but rises to match others by 2023, possibly indicating slower growth or lower engagement.
- All licensees experience a recent drop in wagers and winnings, likely due to an incomplete year, seasonal patterns, or shifts in promotional strategies.

**Data Transformations Relevant to Question 2**

A new calculated field was introduced to analyze the relationship between total wagers and patron winnings.
This ratio helps identify betting trends and assess profitability across licensees.

Calculation Process:
- Formula: Wagers ÷ Patron Winnings
- Labeled as WagersToWinnings in the dataset for reference.

Purpose & Impact:
- Reveals how wagering behavior compares to winnings over different periods.
- Helps evaluate financial performance and betting patterns for each licensee.
- Provides insights that support strategic decisions regarding player incentives and revenue optimization.

**Implications:**

Understanding the relationship between how much players wager and how much they win back gives valuable insight into overall player engagement, game performance, and payout structure.
- When winnings closely match wagers, it shows a stable return environment, which can build player trust and encourage continued play. But it also means margins may be tighter, as more money is returned to players.
- If winnings dip below wagers significantly, licensees might see higher revenue, but risk creating a less appealing experience,  which could hurt long-term engagement if players feel returns are too low.
- The drop in both wagers and winnings in 2025 may reflect seasonality or changes in player behavior, making it a critical time for licensees to evaluate their current strategies and monitor if engagement rebounds later in the year.

# Tableau Packaged Workbook:

[Group Project 2 .zip](https://github.com/user-attachments/files/19914265/Group.Project.2.zip)
