# Hypothesis: Are more goals scored in women's international soccer matches than men's?

## 🔗 Project Links
- [EDA and Hypothesis Testing on Jupyter Notebook](Hypothesis_Testing_with_Soccer_Matches.ipynb)

## 📖 Background
You're working as a sports journalist at a major online sports media company, specializing in soccer analysis and reporting. You've been watching both men's and women's international soccer matches for a number of years, and your gut instinct tells you that more goals are scored in women's international football matches than men's. This would make an interesting investigative article that your subscribers are bound to love, but you'll need to perform a valid statistical hypothesis test to be sure!

While scoping this project, you acknowledge that the sport has changed a lot over the years, and performances likely vary a lot depending on the tournament, so you decide to limit the data used in the analysis to only official FIFA World Cup matches (not including qualifiers) since 2002-01-01.

You create two datasets containing the results of every official men's and women's international football match since the 19th century, which you scraped from a reliable online source. This data is stored in two CSV files: __women_results.csv__ and __men_results.csv__.

The question you are trying to determine the answer to is:

    - Are more goals scored in women's international soccer matches than men's?

You assume a __10% significance level__, and use the following null and alternative hypotheses:

__Null Hypothesis__: The mean number of goals scored in women's international soccer matches is the same as men's.
__Alternative Hypothesis__: The mean number of goals scored in women's international soccer matches is greater than men's.

## 🔍 Results and Findings
1. There are 44,353 observations in the [men results dataset](men_results.csv) and 4884 observations in the [women results dataset](women_results).
2. For hypothesis testing, the datasets are filtered to only work on FIFA World Cup tournaments from year 2022 onwards. The filtered data consists of 384 observations in men dataset and 200 observations in women dataset.
3. The distribution of total number of goals scored in FIFA World Cup by men and women does not follow a normal distribution.
4. A non-parametric test called the __Wilcoxon-Mann-Whitney test__ is used for this hypothesis testing.
5. The p-value obtained from the test is lesser than the significance level of 0.1. Therefore, we will __reject the null hypothesis__ that the mean number of goals scored in women's international soccer matches is the same as men's.  


