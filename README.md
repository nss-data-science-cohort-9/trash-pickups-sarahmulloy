## Missed Trash Pickups

In this data question you will work with service request data related to missed trash pickups from [hubNashville](https://hub.nashville.gov), Metro Nashville government's comprehensive customer service system.

Your goal is to practice working with dates, times, and time-based aggregation in pandas while exploring patterns in missed pickups. You’ll also calculate fines based on missed pickups within a rolling time window.

**Step 1: Data Preparation**
1. Convert any date columns to datetime using pd.to_datetime().  
2. Create new columns for:  
    * year, month, day
    * day_of_week (or weekday name)
3. Filter the data so that you are only analyzing actual missed pickups.

**Step 2: Explore Time-Based Patterns**  
Answer these simpler questions first:  
1. Which day of the week has the highest number of missed pickups?
2. Missed pickups over time:  
    * Find the total number of missed pickups by month. Plot this with a line chart.  
    * Create a plot showing the number of missed pickups per day.  
    * Compute a rolling 30-day average of daily missed pickups. Visualize your results with a line chart to see trends.

**Step 3: Main Task – 180-Day Rolling Fine Calculation**  
Metro Nashville charges fines for excessive missed trash pickups. It uses the following method to fine the total fine:  A $1500 fine is charged for each missed pickup that is the third or subsequent one at the same address within a 180-day window. Multiple fines may apply to the same address.  
Your task is to calculate the total fines across all addresses.  
**Hint:** The rolling method can be use in combination with groupby.

**Step 4: Bonus Questions**
* What other types of complaints are there?
* Are there any geospatial patterns?
* How do metro crews compare to the contractor's performance?
* How much does each trash hauler owe?
* What were the total missed pickup by route?
