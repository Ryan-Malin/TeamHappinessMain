# TeamHappinessMain
Our team reviewed data from the past 5 years:
2021 --
2020 -- 
2019 -- 
2018 -- 
2017 -- 

The 2021 report ranked XX countries by how happy their citizens perceive themselves based on their evaluations of their own lives. The rankings of national happiness are based on a Cantril ladder survey. Nationally representative samples of respondents are asked to think of a ladder, the best possible life for them being a 10, and the worst possible experience is a 0. The question wording is  “Please imagine a ladder, with steps numbered from 0 at the bottom to 10 at the top. The top of the ladder represents the best possible life for you and the bottom of the ladder represents the worst possible life for you." They are then asked to rate their own current lives on that 0 to 10 scale. The report correlates the results with various life factors.

Factors that were analyzed:
**GDP**: GDP per capita is a measure of a country’s economic output that accounts for its number of people.
**Life Expectancy**: Healthy Life Expectancy is the average number of years that a newborn can expect to live in “full health” — in other words, not hampered by disabling illnesses or injuries.
**Freedom**: Freedom of choice describes an individual’s opportunity and autonomy to perform an action selected from at least two available options, unconstrained by external parties.
**Generosity**: is defined as the residual of regressing the national average of responses to the question, “Have you donated money to a charity in past months?” on GDP capita.

# #DATA CLEANING
# #identify the columns with no regional indicator
# #happiness_combined_df['Regional indicator'] == ''][['Country','Year']]
# #pd.pivot_table(happiness_combined_df, values='Country', columns='Year', aggfunc='count')
# before_clean_df = happiness_combined_df
# before_clean_df.pivot(index='Country', columns='Year', values='Country').to_csv('Resources/pivoted-for-missing-val.csv')
#looking at the pivoted data set, it was revealed the countries were named diffrently in
#diffrent years,to solve that, these countries were renamed to one consistent value across 
#years. Also, some countries did not have any data for some years. For instance, Belize, 
#Angola, Congo, Qatar are missing for most recent years. From our google research, it may be
#due to political situation and or high crime rate these countries.
