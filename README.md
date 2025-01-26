Data Cleaning & Visualization Tour of the singers with mmd!

I stumbled upon a messy dataset and decided to work on it. Using Pandas, I cleaned it up, and finally, for better understanding and presentation, I visualized it with Matplotlib.
Stay with Mammad to explore the magic behind the code and see what’s happening! 

Steps in Data Cleaning:

The original dataset had some major issues that I needed to fix. Here's what I did:

Removing Unnecessary Columns:
I removed irrelevant columns like peak, all the time peak, ref, and year(s).
Also, I targeted duplicate rows and null values!
(Although nothing got removed, I kept this step as an educational reminder).

Renaming Columns:
I renamed columns like Actual Gross, Adjusted Gross, Average Gross, and Tour Title to shorter, clearer names.

Cleaning Column Values:
For columns like Total Earn, Profit (2022), and Average Earning, I stripped out all non-numeric characters, leaving only clean numbers behind.
These numbers were converted to strings for better readability.
For Tour Title, I kept only the tour names and removed unnecessary details.

Creating New Columns:
I extracted Start Year and End Year from the Year(s) column.
Here’s the cool part: if End Year was missing, I replaced it with the value of Start Year.
This way, tours with missing end years were assumed to have ended in their start year.

Visualization: Presenting Data Like a Pro

Using Matplotlib, I created several insightful charts:

Bar Chart: Total Earnings per Artist
This chart shows the total earnings (Total Earn) for each artist. Each bar represents an artist, and its height reflects how much money they made. 
Note: Artist names were rotated (rotation=45) to make them more readable.

Pie Chart: Profit Share in 2022
This pie chart visualizes each artist’s share of the 2022 profit (Profit (2022)). Imagine the profit as a pie, and each slice belongs to an artist.
Note: Percentages were displayed next to each slice, and the starting angle was adjusted (startangle=90).

Line Chart: Trend of Average Earnings in Tours
This chart illustrates the trend of average earnings (Average Earning) over the start and end years of tours.
Note: I added a grid (grid=True) for better visibility of the changes.

Scatter Plot: Profit vs. Number of Shows
This plot shows the relationship between the number of shows (Shows) and the 2022 profit (Profit (2022)). Each point represents an artist.
Note: The X-axis represents the number of shows, while the Y-axis represents the profit.
Histogram: Distribution of Number of Shows
I analyzed how many shows artists performed and how the numbers were distributed.

Summary:

First, I cleaned and organized the data by removing unnecessary columns, renaming them, and cleaning up the values.
Then, I used Matplotlib to create stunning visualizations, each revealing unique insights about the dataset.
Each chart tells a different story, making data analysis more straightforward and enjoyable!
