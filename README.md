# The Art & Science of Data Visualization

Taking a dataset containing movie information, I set out with the goal of searching for some insights and bringing them to life with some good ol' data visualization. I made sure to incorporate design principles so that my visualization effectively conveys the insights I found.  

One of the things I wanted to find out was which director had directed the most critically acclaimed movies. Below are the results of my findings followed by the various ideas I took into account when designing the graph:

![Screenshot 2024-02-10 224838](https://github.com/khushil-sketch/Data-Visualization/assets/52947378/c54e0986-42b6-474c-9626-d5be4abbd275)

The barplot is designed to highlight the directors of the highest-rated films in the dataset, showcasing the number of acclaimed movies each has directed

The reason I chose a bar chart is that effective designs turn thinking principles into seeing principles- I wanted my audience to realize the excellence of a director by showing them how many top-rated films a certain individual has directed. Additionally, length is an effective channel to compare ordered attributes, hence I encoded my film_count data in bars.

I chose to use horizontal bars since that makes it much easier to discern differences in length. I performed the following transformations on my data: 
Grouping by directors
Counting the films a particular director has directed
Getting the mean Metascore of all the films a director has directed
Applying a filter to only include films greater than 70, which I chose as my threshold of excellence.

After doing these transformations, I remained with 17 rows in my data frame. By the principle of discriminability, I chose to pick the 10 directors who had directed the most 
highly rated films.

The x-axis represents the number of films (Quantitative Diverging) on a scale from 1 to 7, with 7 being the highest value. I did not extend my scale to 10 because that would have led to unnecessary white space on the graph. The y-axis represents the names of directors (Categorical), and since I included the number of directors in the title, I did not have to number them on the scale. The title of my bar chart conveys all the information the user needs to understand what the graph represents with the leas amount of friction. 

I chose to colour the top 5 bars blue and all the remaining grey since ‘Colour Hue’ is an effective identity channel. By visually filtering the bars, I get to direct the audience’s attention to the creme de la creme of directors, encoding even more information about the excellence of the directors through the use of colour. Additionally, by Steven’s Psychological Power Law, the perception of saturation is magnified by humans. 
Lastly, to enhance the visibility of each director's filmography volume, the film counts are displayed within the bars.

I wanted to also include the average film Metascore of the films a particular director had directed, however, I felt that having 2 quantitative values that convey different ideas would confuse the audience.
