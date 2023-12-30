<h1>Analyze netflix movie data if movie duration is getting shorter over time</h1>

See workspace here: [Notebook](workspace.ipynb)👀

<h2> Approach to this project: </h2>

- I've loaded the netflix_data.csv file into a pandas DataFrame so I can inspect and analyze the data.
- I've subset the DataFrame to only include the rows where "type" is equal to "Movie". This filters out TV Shows and other types to just focus on movies
- I've then selected only the columns that seem relevant to the analysis which are; title, country, release_year, duration, and listed_in (genres).
- To look at duration, I've filtered the DataFrame to only include movies that are at least 60 minutes long as standard full-length movies tend to be at least 60 minutes.
- I've assigned different colors to the unique genre values. This will let us see trends by genre on the plot.
- Lastly, I've created a scatter plot of duration on the y-axis versus release_year on the x-axis, using the genre colors.

Looking at the plot, there does seem to be a slight downward trend in the median movie duration over the years shown from around 2010 onwards, with most titles clustering closer to the 90 minute range now versus longer before. However, the trend isn't very strong and there's a lot of variation between genres and individual titles. In summary, this project was an initial exploration of the question but did not result in a conclusive yes or no answer about movies shortening due to limitations of the single data source analyzed.
