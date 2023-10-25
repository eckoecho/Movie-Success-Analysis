# Prediction of Movie Success

## Inspecting Movie Features to Predict Revenue

**Author: Echo Diaz**


My goal is to determine what movie attributes contribute to the success of a movie within the U.S.  Using up-to-date statistical data from IMDB movies, I determine the features contributing to the revenue-based success of a movie. 

This data analysis takes info from [IMDB](https://developer.imdb.com/non-commercial-datasets/).

For this analysis I've broken down the process of extracting, cleaning, filtering and exploratory data analysis into digestible parts:

* **Part 1:** Download several files from IMDB’s movie data set and filter out the subset of U.S. movies 
* **Part 2:** Use an API to extract box office revenue and profit data, add to the IMDB data and perform exploratory data analysis
* **Part 3:** Construct and export a MySQL database using the data.
* **Part 4:** Apply hypothesis testing to explore what makes a movie successful
* **Part 5 (Optional):** Produce a Linear Regression model to predict movie performance.

**Data Dictionaries:**
(*title.basics.tsv.gz)

| Variable Name | Description |
| --- | --- |
| **tconst (string)** | alphanumeric unique identifier of the title |
| **titleType (string)** | the type/format of the title (e.g. movie, short, tvseries, tvepisode, video, etc) |
| **primaryTitle (string)** | the more popular title / the title used by the filmmakers on promotional materials at the point of release |
| **originalTitle (string)** | original title, in the original language |
| **isAdult (boolean)** | 0: non-adult title; 1: adult title |
| **startYear (YYYY)** | represents the release year of a title. In the case of TV Series, it is the series start year |
| **endYear (YYYY)** | TV Series end year. ‘\N’ for all other title types |
| **runtimeMinutes** | primary runtime of the title, in minutes |
| **genres (string array)** | includes up to three genres associated with the title |


(*title.akas.tsv.gz)
| Variable Name | Description |
| --- | --- |
| **titleId (string)** | a tconst, an alphanumeric unique identifier of the title
| **ordering (integer)** | a number to uniquely identify rows for a given titleId
| **title (string)** | the localized title
| **region (string)** | the region for this version of the title
| **language (string)** | the language of the title
| **types (array)** | Enumerated set of attributes for this alternative title. One or more of the following: "alternative", "dvd", "festival", "tv", "video", "working", "original", "imdbDisplay". New values may be added in the future without warning
| **attributes (array)** | Additional terms to describe this alternative title, not enumerated
| **isOriginalTitle (boolean)** | 0: not original title; 1: original title