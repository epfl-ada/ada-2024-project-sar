# Left in the shadows: Women’s Fight for Their Share of the Spotlight

## Abstract:

Cinema has long reflected societal norms, yet gender representation remains a critical issue, with women often confined to stereotypes and underrepresented in leading roles. This study introduces an Inclusivity Score, combining metrics such as the Bechdel Test, actress proportion, and script allocation to women, to assess inclusivity in films. Despite decades of analysis, there is little evidence of significant improvement. A newly developed Success Metric, combining revenue and ratings, reveals no meaningful correlation between inclusivity and success, highlighting that inclusivity is a societal choice rather than a commercial constraint.

The study demonstrates that creating inclusive and successful films is possible, offering actionable recommendations such as diversifying female roles, enriching characters with emotional depth, and promoting leadership narratives. This framework proves that inclusivity and compelling storytelling can coexist, paving the way for more equitable cinema.

All results can be found on [this webpage](https://elsahtz2.github.io/SAR-ADA_website/)

## Research questions:

1. What is the current state of women's representation in the film industry? Has it evolved over the years?
2. How to measure the success and the inclusivity of a film?
3. Is it possible to make an inclusive movie and still be a success? How to achieve this goal?
4. How does the Bechdel Test score evolve over time, and what factors contribute to films achieving higher scores? What is the correlation between achieving a Bechdel Test score of 3 and the financial and critical success of a film?
5. Are female characters increasingly portrayed in roles that go beyond traditional stereotypes, and how does this affect audience reception?

## Additional datasets:

1. **IMDB Ratings**:
   This dataset was chosen to incorporate the ratings films received, which will be linked to revenue data (already available in the CMU movies database) to create a variable measuring a film’s success.
   The dataset is available on this [this website]('https://developer.imdb.com/non-commercial-datasets/')

2. **Bechdel Test Results**
   This dataset contains Bechdel test scores, which provide insight into the interactions between women in films. By integrating these scores with other variables from the CMU movies dataset, we can analyze correlations between the Bechdel test results and other factors like ratings, revenue, and genre. The dataset can be obtained by doing a request to [this url]('http://bechdeltest.com/api/v1/getAllMovies').

3. **TMDB movies metadata**
   This dataset contains information on 45,000 movies featured in the Full MovieLens dataset.
   Features include posters, backdrops, budget, revenue, release dates, languages, production countries and companies.
   This dataset was obtained trought a Wikidata query using [this url](https://query.wikidata.org)

4. **Film dialogue from The Pudding**:
   This dataset contains the distribution of the script to the different actors of the movie. The dataset is used to compute the share of the script given to women actress and is available to download on this [github page](https://github.com/matthewfdaniels/scripts/)

## Methods:

- **Data collection and enrichment:** Gather data on movies, including box office revenue, critical ratings, budgets, genres, release years, and attributes of lead actors (age, height, ethnicity, character type). Collect Bechdel Test scores for films across different time periods and genres to evaluate the depth of female representation.
- **Comparative Analysis:** Examine male and female representation in similar roles to uncover hidden disparities.
- **Trend analysis:** Perform descriptive analysis to understand general trends in female representation across genres and decades. Analyze correlations between Bechdel Test scores, box office revenue, critical ratings, and other success metrics.
- **Bechdel test analysis:** Evaluate the progression of female representation quality based on the depth of on-screen interactions.

## Organization within the team:

- Elsa: Creation of website + creation inclusivity metric and analysis
- Mahdi: Decision tree-based models + research feature
- Maria: Synopsis analysis + High level analysis
- Alvaro: Bechdel analysis
- Myriam: Website design + Investigation of possible prediction

## Files organisation

```plaintext
📂 Project Root
│
├── README.md
├── requirements.txt              # Dependencies required to run the project
├── milestone2.ipynb              # Milestone 2 hand-in
├── results_milestone3.ipynb      # Final results used for the analysis
│
├── 📂 data                       # Contains datasets used in the project
│   ├── 📂 original_datasets      # Raw datasets
│   │   ├── Budget_data
│   │   ├── CMU_dataset
│   │   ├── IMDB_data
│   │   └── Script_data
│   └── 📂 preprocessed_datasets  # Processed datasets used for analysis
│
├── 📂 figures                    # Visualizations and figures generated during analysis
│
├── 📂 src                        # Source code and notebooks
│   ├── Data_cleaning.ipynb       # Notebook for cleaning merged data
│   └── Data_merged.ipynb         # Notebook for merging datasets for analysis
│
└── 📂 tests                      # Test scripts whe investigating data during milestone2
    └── Tropes_tests.ipynb        # Notebook for analysis on tropes
```
