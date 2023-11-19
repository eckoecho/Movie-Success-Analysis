# Movie Success Analysis
 

In this project, I created a MySQL database combining a subset of IMDB's and TMDb's data on movies. The objective was to analyze the key drivers of a movie's success and provide actionable recommendations to stakeholders.

Throughout the project, the following key steps were undertaken:

**Part 1:** Downloaded and filtered IMDB movie data as requested by the stakeholders.

**Part 2:** Leveraged The Movie Database (TMDb)'s open API to extract box office revenue and profit data, enriching the IMDB dataset. This additional information was then used for comprehensive exploratory data analysis.

**Part 3:** Constructed and exported a MySQL database, incorporating the collected data, for efficient storage and retrieval.

**Part 4:** Employed hypothesis testing to delve into the critical factors that influence a movie's success.


## To prepare this data, the data was cleaned, and the following processes were performed:

During the exploratory data analysis, a mixture of barplots, boxplots, and histograms were visualized for each datatype column.

<img width="621" alt="Screenshot 2023-11-18 at 3 25 31 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/02d01313-c52d-4090-8349-a726ada06075">

The histogram shows the majority of US movies are rated R, followed by PG-13, and PG.

<img width="607" alt="Screenshot 2023-11-18 at 3 41 37 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/c3510877-dec6-4ead-9fdc-4ed686f25517">

The boxplot reveals that G-rated movies generate the highest revenue, with PG-13 and PG-rated films following closely in revenue rankings. Boxplots depict the range and median of movie genres, with a black bar indicating the distribution. Notably, G-rated movies exhibit a wider revenue range compared to R-rated films.

<img width="992" alt="Screenshot 2023-11-18 at 4 01 01 PM" src="https://github.com/eckoecho/Movie-Success-Analysis/assets/43970023/1bf40634-8f87-4ccb-931d-834763808b63">

Based on the provided data, the exploratory data analysis (EDA) findings reveal notable variations in revenue and budget across different movie ratings. Specifically, G-rated movies tend to have higher median revenues (7.34e+07) compared to their median budget (2.38e+07). In contrast, R-rated movies exhibit a lower median revenue (1.53e+07) in relation to their median budget (9.50e+06). This suggests that, on average, G-rated movies achieve a more favorable revenue-to-budget ratio compared to R-rated movies. The analysis highlights the potential importance of movie rating in understanding the financial performance of films in the dataset.

