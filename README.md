
**Title:**

**Abstract:**

We begin by examining the general position of women in cinema, analyzing the general trends in female representation. This first analysis highlights the disparities and progress in the industry, setting the stage for deeper exploration. Through tools like the Bechdel Test and trend analysis, we will evaluate the depth and importance of female roles across genres and decades, offering insights into the broader cultural implications of gender in film. 
Building on these insights, we will conduct a data analysis to identify the optimal characteristics of a female lead such as age, height, ethnicity, and character type that contribute to a movie's success in terms of box office revenue and critical acclaim. Taking these factors into account, we aim to craft recommendations that not only maximize film success but also achieve a Bechdel Test score of 3. By the end of the project, our goal is to determine how incorporating certain types of female characters can elevate both the commercial and narrative quality of films, while promoting gender inclusivity.
This research will show gender dynamics within the film industry and provides practical recommendations for casting and storytelling that resonate with audiences and contribute to a more inclusive cinematic future.

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

**Questions for TAs:**
How to find a good method to predict the best women for the success of the movie? Since the correlation for some factors are too low, is there another way to deduce our predictions 
