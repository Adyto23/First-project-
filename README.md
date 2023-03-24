# 27th Club Real or Myth
**Ady Toledano**  
**IronHack, Remote Course, Berlin 24 Mar 2023**

## Overview

* Is the avarage life expectancy of Famous Artists is lower than other Occupations ? - 27th Club Real or Myth

Used:

	* Python
	* Statistical analysis
  * Hypothesis Testing 
	* Data visualization
	* Jupyter Notebook
	* Tableau
  
  ## Data Preparation

### Overview: 
* Data Title: Age dataset: life, work, and death of 1.22M people

	* [dataset](https://www.kaggle.com/datasets/imoore/age-dataset)
  
* 10 columns 
* 1222997 rows 
* columns:
* 
| Initial Column | Comments | New Column |
Id - Wikidata Id
Name - Full Name
Short description - Will detail the Profession of the person and should they have more than one it will be listed in this column, in this column I have tried to sum it to one Profession in order to get a more clear view
Gender - Gender / Sex
Country - Country / historical region, deleted in this column countries after the charecter ";" in order to get a better overview in the data
Occupation - Occupation title
Birth year - Birth year
Death year - Death year, limiting this column to years above 1930
Manner of death - Such as suicide, natural causes or capital punishment
Age of death - Age of death , changing the range to between 18-100
AgeRange - New column created for ranges: 18-29, 30-39, 40-49, 50-59, 70+

 
### Data Wrangling and Cleaning
  
- Overall Data description
- Deleting  columns with unique values: Id, Name 
- Looking for outliers column by column, please see above to more information about the changes
- Dealing with Nan Values for each column
- Checking for correlation with target feature
- checking Hypothesis with the age of 27 and with the mean of artists compared to non artist Occupations


### Data Storage

* As the Dataset is quite large you will be able to access:
* Use [Link](https://drive.google.com/drive/folders/1wGRChf85LullaU3Weyo1u2WpIUJbrXlo)

## Data Analysis

* Use [tableau](https://public.tableau.com/app/profile/ady.toledano/viz/Book2_16794783401290/Story1?publish=yes)

### Data Exploration and Visualization
Used Tableau to visualize the Project data data and ppt for the [presentation][(https://docs.google.com/presentation/d/1uV481vZeN0vXxO3m2vl5otSgrpAx9hq-1uts1mDUKk4/edit#slide=id.g1f9b3e5b7c1_4_75)]

### Hypothesis Testing: 
1. death , famous people project - 

##The null hypothesis (H0): mean age_of_death of singer = 27
##The alternative hypothesis: (H1): age_of_death of singer ≠ 27

Used confidence interval and stat, pval in order to reject H0

2. exp.generalinfo - 
##The null hypothesis (H0): the age_of_death of all others is lower or equals to all artists  , in this case we took the mean of 64 of the artists as a limit
##The alternative hypothesis: (H1): the the age_of_death is higher than artists

Used the mean age of artists which was 64 and a DataFrame that contained all rows that Occupations are not artists. 
As before used confidence interval and stat, pval in order to reject H0


## Conclusion

In both Hypotesis Testing H0 was rejected and the age of death was higher than 27 for singers and more than 64 for all other Occupations
 
