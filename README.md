# Movie Success Analysis
 

In this project, I created a MySQL database combining a subset of IMDB's and TMDb's data on movies. The objective was to analyze the key drivers of a movie's success and provide actionable recommendations to stakeholders.

Throughout the project, the following key steps were undertaken:

**Part 1:** Downloaded and filtered IMDB movie data as requested by the stakeholders.

**Part 2:** Leveraged The Movie Database (TMDb)'s open API to extract box office revenue and profit data, enriching the IMDB dataset. This additional information was then used for comprehensive exploratory data analysis.

**Part 3:** Constructed and exported a MySQL database, incorporating the collected data, for efficient storage and retrieval.

**Part 4:** Employed hypothesis testing to delve into the critical factors that influence a movie's success.


# EDA
## To prepare this data, the data was cleaned, and the following processes were performed:

During the exploratory data analysis, a mixture of barplots, boxplots, and histograms were visualized for each datatype column.

<img width="621" alt="Screenshot 2023-11-18 at 3 25 31 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/02d01313-c52d-4090-8349-a726ada06075">

The histogram shows the majority of US movies are rated R, followed by PG-13, and PG.

<img width="607" alt="Screenshot 2023-11-18 at 3 41 37 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/c3510877-dec6-4ead-9fdc-4ed686f25517">

The boxplot reveals that G-rated movies generate the highest revenue, with PG-13 and PG-rated films following closely in revenue rankings. Boxplots depict the range and median of movie genres, with a black bar indicating the distribution. Notably, G-rated movies exhibit a wider revenue range compared to R-rated films.

<img width="992" alt="Screenshot 2023-11-18 at 4 01 01 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/1bf40634-8f87-4ccb-931d-834763808b63">

Based on the provided data, the exploratory data analysis (EDA) findings reveal notable variations in revenue and budget across different movie ratings. Specifically, G-rated movies tend to have higher median revenues (7.34e+07) compared to their median budget (2.38e+07). In contrast, R-rated movies exhibit a lower median revenue (1.53e+07) in relation to their median budget (9.50e+06). This suggests that, on average, G-rated movies achieve a more favorable revenue-to-budget ratio compared to R-rated movies. The analysis highlights the potential importance of movie rating in understanding the financial performance of films in the dataset.

# Hypothesis Testing Results

## Hypothesis: Does the MPAA rating of a movie (G/PG/PG-13/R) affect how much revenue the movie generates?
<img width="617" alt="Screenshot 2023-11-19 at 7 45 22 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/371a1053-f385-4593-8e27-3dd65b26480e">

This boxplot visualizes the median revenue per genre, revealing that G-rated movies exhibit the highest revenue. Through hypothesis testing, statistical significance is established, leading to the rejection of the null hypothesis. This underscores the conclusion that a movie's rating significantly influences its financial success.

<img width="533" alt="Screenshot 2023-11-19 at 8 28 15 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/fbe32f25-e297-41e5-843e-4a46e0e886e1">

Statistically, there is a significant difference in revenue between G and R-rated movies, and the negative mean difference implies that, on average, G-rated movies have higher revenue than R-rated movies.Therefore, I reject the null hypothesis and choose the alternative hypothesis: There is a significant difference revenue between genres.

## Hypothesis: Does the release month have an effect on revenue?

<img width="541" alt="Screenshot 2023-11-19 at 8 53 59 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/6842b5c7-bbe7-4855-b3b8-d3033df8ea77">

Based on the Tukey results, we reject the null hypothesis and accept the alternative hypothesis: The month a movie is released has a signifcant difference in revenue.

<img width="615" alt="Screenshot 2023-11-19 at 8 55 08 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/fe7f1015-e0d1-4302-a09a-2821988d70ca">

The test results suggest that the release month of a movie is a determining factor in its revenue success. Different months exhibit significant differences in mean revenue, indicating that the timing of a movie's release can impact its financial performance. For example, movies released in months like May, June, July, November, and December tend to have higher revenue compared to movies released in other months.

## Hypothesis: Is there a significant difference in revenue between movies that belong to a collection and those that do not?


<img width="736" alt="Screenshot 2023-11-19 at 11 45 17 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/259af2f3-8902-46d3-baa7-c4cb16777615">

In this analysis, it is evident that movies belonging to a collection outperform those that do not. The rejection of the null hypothesis supports the conclusion that there is a statistically significant difference in revenue between collection and non-collection movies.
