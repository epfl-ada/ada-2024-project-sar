
## Left in the shadows: Women’s Fight for Their Share of the Spotlight

**Abstract:**

We begin by analyzing the general position of women in cinema, focusing on trends in female representation. This initial analysis highlights industry disparities and progress, setting the stage for deeper exploration. Using tools like the Bechdel Test and trend analysis, we will assess the depth of female roles across genres and decades, offering insights into gender's cultural implications in film. Based on these insights, we will analyze factors such as age, height, ethnicity, and character type to identify the characteristics of a successful female lead, measured by box office revenue and critics. Our goal is to craft recommendations that maximize success while achieving a Bechdel Test score of 3. Ultimately, we aim to determine how specific female character types can enhance both commercial success and narrative quality, promoting gender inclusivity. This research will provide practical recommendations for casting and storytelling, contributing to a more inclusive cinematic future.

**Research questions:**
1. How has the role of women in the film industry evolved over the years?
2. How does the Bechdel Test score evolve over time, and what factors contribute to films achieving higher scores?
4. What is the current state of women's representation in the film industry?
5. Are female characters increasingly portrayed in roles that go beyond traditional stereotypes, and how does this affect audience reception?
7. What are the optimal attributes (age, height, ethnicity, character type) of a female lead to maximize box office revenue and critical ratings?
8. What is the correlation between achieving a Bechdel Test score of 3 and the financial and critical success of a film?
9. Is it really possible to predict the actress that could lead to the best movie succes while passing the Bechdel Test with the best score ? 

**Proposed additional datasets:**
1. IMDB Ratings
  This dataset was chosen to incorporate the ratings films received, which will be linked to revenue data (already available in the CMU movies database) to create a variable measuring a film’s success.

2. Bechdel Test Results
  This dataset contains Bechdel test scores, which provide insight into the interactions between women in films. By integrating these scores with other variables from the CMU movies dataset, we can analyze correlations between the Bechdel test results and other factors like ratings, revenue, and genre.

3. TMDB movies metadata
  This dataset contains information on 45,000 movies featured in the Full MovieLens dataset.
Features include posters, backdrops, budget, revenue, release dates, languages, production countries and companies.

6. Additional TVTropes entries for the movie
   List of trope names ocurring in each movie.
   
**Methods:**
- **Data collection and enrichment:** Gather data on movies, including box office revenue, critical ratings, budgets, genres, release years, and attributes of lead actors (age, height, ethnicity, character type). Collect Bechdel Test scores for films across different time periods and genres to evaluate the depth of female representation.
- **Comparative Analysis:** Examine male and female representation in similar roles to uncover hidden disparities.
- **Trend analysis:** Perform descriptive analysis to understand general trends in female representation across genres and decades. Analyze correlations between Bechdel Test scores, box office revenue, critical ratings, and other success metrics.
- **Regression analysis:** Build a predictive model to map actor attributes (age, height, ethnicity, character type) and film characteristics (budget, genre, release year) to success metrics like revenue and ratings. To explore the relationship between Bechdel test scores and other variables in the dataset, we primarily conducted linear regression analyses to identify potential patterns
- **Bechdel test analysis:** Evaluate the progression of female representation quality based on the depth of on-screen interactions.

**Proposed timeline:**

For Milestone 3, we plan to apply techniques from the "Handling Text Data" lectures. This will involve analyzing movie summaries to identify lexical fields associated with higher or lower Bechdel test scores, uncovering the language patterns linked to gender representation.
We will also add data to the tropes dataset to better predict the preferred character types, as the current tropes dataset is too small.
The next step involves performing propensity score matching to determine which variables act as confounders in these relationships.
There are several alternative approaches we can take to better understand the relationships in our data and identify the most important predictors of success.
One potential approach is recursive feature elimination (e.g., using linear regression or random forest), which recursively removes the least important features based on model performance. Additionally, decision tree-based models, such as Random Forest, can provide feature importance scores, which can be used to identify the most influential predictors.

**Organization within the team:**
Elsa: Handling text data
Mahdi: Decision tree-based models 
Maria: Recursive elimination
Alvaro: Propensity score and exploring the betchdel in details
Myriam: Additional tropes data analysis

Additional internal milestone : start the website site at least before the 4th od December

**Questions for TAs:**
1. What is the best method to predict the most successful female characters for a movie?
2. Given that the correlation for certain factors is low, are there alternative approaches we can use to improve our predictions?
3. How do you suggest handling missing or incomplete data, especially with categorical features like ethnicity or trope types?
4. What additional features or variables might be valuable to include in the model to predict the success of a female character ?

## How to use the library

```text
├── data                        <- All the data we have used for our analysis
│
├── src                         <- Source code
│   ├── Data_cleaning.ipynb     <- Code used for cleaning the data before usage in results.ipynb
│   ├── Data_merged.ipynb       <- Code used for merging the datasets
│
├── tests                       <- Tests not included in the results
│
├── results.ipynb               <- All the valuable results we have found to answer our main research questions
│
├── .gitignore                  <- List of files ignored by git
├── pip_requirements.txt        <- File for installing python dependencies
└── README.md

