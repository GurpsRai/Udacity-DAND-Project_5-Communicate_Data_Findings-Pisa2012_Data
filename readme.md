#  Factors Influencing Student Performance
## by Gurps Rai


## Dataset

> The Pisa assessment focuses on reading, mathematics, science, and problem solving, along with a whole host of other matrices, that are deemed to have an effect on educational achievement.
The complete Pisa dataset consisted of 636 separate features, for over 485K students. I decided to try and understand how some of these features in the dataset may influence student academic performance, of the three main subject disciplines which are included in the Pisa dataset; Mathematics, Reading and Science.
The factors I decided to focus on were:
- Country of student
- Wealth of student’s family
- Gender
- OECD membership of country
- Truancy
- Immigration status
- Student possession of textbooks


## Summary of Findings

### Main dependent variables of interest

> The three main scores were all very well 'normally' distributed and indicate the Pisa tests were of excellent technical quality, and the results were likely to be reliable indictors of student academic performance for each of the three subjects.

### Relationships observed between main features of interest.

> I a very strong positive linear correlation between my main dependent variables of mean scores. In other words, if you did well in one of the subjects you were likely to do well in the other subjects too. A weak positive correlation was also found between wealth and score.

> There were some interesting correlations between gender and the three subject scores. Female students did a lot better on the reading scores than male students, and this was seen to be true across the whole range of data. 
Male students seem to do slightly better than female students in the upper band of scores in mathematics and science (though also slightly worse in the lower range of scores in science), however, female students are more likely to achieve average score across all three subjects – i.e. they have less variance across the scores.
 
> Students having textbooks were highly correlated with higher scores for all three subjects. There is no doubting the improvement that textbooks made on scores. 

> Immigration status did not seem to be correlated to the scores for any of the subjects, and I decided not to follow up on this enquiry.

> A very strong correlation was found to exist between a country’s OECD membership and scores. OECD member countries had higher scores for all three subjects than non-members. This was interesting to me, as OECD member countries are understood to be richer than non-members, and how a country’s wealth may affect student scores, was one of my main initial enquiries.

> Truancy was found to be negatively correlated with student scores, the higher the truancy level, the lower the student was likely to score across all of the three subjects.


### Other interesting observations.

> On investigting the weak positive correlation I had initially found between country wealth and scores, I decided to take the average student wealth for each country, and each country’s corresponding maths scores. Mapping each country to a plot, I found some very interesting outliers. Vietnam for example, one of the poorest countries was found to have above average maths scores, and Qatar, one of the wealthiest countries was actually found to have one of the lowest maths scores in the data!

### Multivariate relationships observed. 

> The multivariate exploration confirmed some of my earlier findings, but also gave insights to other effects which were of interest to me.

> I found OECD membership is not only correlated to a country’s maths score, but also provides a good indicator of a country’s wealth.

> Truancy appeared to be correlated to scores and not wealth as I had thought.

> Some countries were found to buck the trend of gender in relation to score achieved across the three subjects. Female students were found to outperform male students in mathematics and science in some countries. However, this may also have been in part to male students underperforming in those countries.


### Surprising interaction of features.

> There seems to be a correlation of text book possession, gender of students, and the corresponding score of the three subjects.
In mathematics and science for example, female students had a greater increase of scores than male students, if they had textbooks, and male students improve their reading scores more than females if they were in possession of textbooks.


### References and Citations

Pisa 2012 Datafile - https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip&sa=D&ust=1554482573645000

Pisa 2012 Data Dictionary - https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554486256024000

Pisa 2012 Results in Focus Publication - https://www.oecd.org/pisa/data/pisa2012technicalreport.htm

What is an OECD? - https://www.economist.com/the-economist-explains/2017/07/05/what-is-the-oecd

Opening Latin encoded Pisa CSV datafile - Udacity Knowledge

Display all columns of a Pandas DataFrame - https://stackoverflow.com/questions/47022070/display-all-dataframe-columns-in-a-jupyter-python-notebook/47022213

Rename multiple column names in pandas DataFrame - https://chrisalbon.com/python/data_wrangling/pandas_rename_multiple_columns/

Visualise distributions of multiple variables - http://cmdlinetips.com/2019/02/how-to-make-histogram-in-python-with-pandas-and-seaborn/

Annotate single point in scatter plot with text - https://www.pythonmembers.club/2018/05/08/matplotlib-scatter-plot-annotate-set-text-at-label-each-point/

Scatter plot crosshairs for matplotlib - https://fcpython.com/visualisation/scatter-plots-crosshairs-in-matplotlib

Faceted heatmap - Udacity 'Diamonds' Example Project

