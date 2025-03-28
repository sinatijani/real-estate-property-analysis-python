# US Real Estate Data: Cleaning It Up!

Okay, so I got my hands on this US real estate dataset. It was a mess! My goal was to clean it up and make it usable, like if I was running a real estate agency. Here's what I did:

## The Messy Data

* **First Look:**
    * I loaded the data into Pandas, called it "df".
    * Right away, I saw tons of duplicates. Like, 86% of the data was exactly the same!
    * The "full address" column was overkill, so I just kept the city and state.
* **More Duplicates:**
    * Even after that, there were still 772 more duplicates based on the address.
    * I sorted the data by address, price, size, and sold date, then got rid of the extras.
    * Ended up with "df4", which was clean of address duplicates and had no nulls.

## Dealing with Crazy Prices

* **Outliers:**
    * The prices were all over the place. I used charts and stats to find the outliers (the super low or high prices).
    * I used the IQR method to find the right cut-off points, and got rid of the outliers.
    * This gave me "df5", my main clean dataset.
* **Fixing Nulls:**
    * "df5" still had some missing values in beds, baths, size, etc.
    * I filled those with the median values.
    * Left the missing "sold date" alone, because it means the property hasn't sold yet, which is useful info.
* **Final Check:**
    * Did a final check on the stats.
    * Found a few more outliers, but decided to leave them because I didn't want to lose too much data.
    * Did a correlation analysis and a heat map.
    * Saved the clean data as an Excel file.

## Why This Matters

* **Clean Data is Key:**
    * You can't do good analysis with bad data.
    * This project shows I can handle messy data and get it ready for analysis.
* **Real Estate Insights:**
    * I also looked at some basic stats, like average prices, to see how they could be used in a real estate context.
    * For example, the mean price helps give a general idea of the market.
* **Libraries:**
    * Used Pandas, Numpy, Seaborn, Scipy, and Matplotlib.

## The Result

* The final dataset "df5" is about 12.5% of the original data.
* I also did some basic analysis, like property values by state and sales trends, but the cleaning was the main focus.

* Kindly read the report for the full breakdown