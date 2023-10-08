![](/img/banner.JPG)<br />

# Movie Records Data Analysis Project
In this project, I explored a dataset containing movie records. The project is mearnt to The dataset was cleaned and transformed
in make it easy to work on and insights generated. 

### Dataset Source: 
The dataset was sourced from kaggle.com. It contains a single csv file with 10,866 records and 21 columns.
Below are the columns and their properties;
1.	imdb_id 10856 non-null object
2.	popularity 10866 non-null float64
3.	budget 10866 non-null int64
4.	revenue 10866 non-null int64
5.	original_title 10866 non-null object
6.	cast 10790 non-null object
7.	homepage 2936 non-null object
8.	director 10822 non-null object
9.	tagline 8042 non-null object
10.	keywords 9373 non-null object
11.	overview 10862 non-null object
12.	runtime 10866 non-null int64
13.	genres 10843 non-null object
14.	production_companies 9836 non-null object
15.	release_date 10866 non-null object
16.	vote_count 10866 non-null int64
17.	vote_average 10866 non-null float64
18.	release_year 10866 non-null int64
19.	budget_adj 10866 non-null float64
20.	revenue_adj 10866 non-null float64


### Technologies/Tools used:
* Python
* Jupyter Notebook
* Pandas
* Matplotlib


### Skills Demonstrated
In the course of this project, the following skills were demonstrated;
* Data Cleaning and Transformation using Python
* Data Exploration and Insight generation 

## Problem Statement
1.  Tidy up the dataset
2.  Transform the dataset to aid effective exploration
3.	What genre of movie is most produced in the last ten years?
4.	What are the first two most profitable movie genres in the last ten years?
5.	What range of movie runtime is more prefered by movie goers?
6.	Which production company made the largest profit within the time frame covered by the dataset?
7.	Which production company made more films within the time frame covered by the dataset?
8.	Which genre of movie is most produced by the company with the highest profit within the time frame covered by the dataset


## Data Cleaning and Transformation Processes

### Investigating the Dataset
The dataset was investigated and the following findings were made
1.	Missing data in some columns
![](/img/missing-data.JPG)<br />
*The image show each column with respective number of data missing*

2.	Remove duplicate record
![](/img/duplicate-data.JPG)<br />
*1 duplicate record exists*

3.	There is need to create a **Profit** column 
4.	Genres are moduled up together in one column seperated by "|"
5.	Production_companies are also moduled up together in one column seperated by "|"

![](/img/genre-production-companies.JPG)<br />
*Genre and Production_companies columns showing the data*

### Cleaning and Transformation operations
The follow operations were carried out on the dataset in other to make it clean and ready to be analyzed so as to answer the questions stated above
1.	**Missing data in some columns:** This was handled in two operations first the fields like homepage,tagline and keywords which contains over 1000 empty data were dropped from the dataset. This as well also took care of the fact that they columns were not necessary for the analysis to be carried out. On the other hand the missing data in the remaining text fields where filled with dummy data.
2.	**Remove duplicate record:** Just one duplicate record was discovered and it was deleted
3.	**Create a column for profit:** A "profit" column was added to the dataset since questions on profit were going to be answered.
4.	Genres are moduled up together in one column seperated by "|": In other to accurately analyze the genres there is need to unbundle the respective genres under which each movie falls under. This was done and a new csv file was created named **genre_cleaned.csv**. This is was done to be able to answer questions 1 and 2.
5.	**Production_companies** are also moduled up together in one column seperated by "|": Similarly, there was a need unbundle all of the production_companies which partook in the creation of each film in other to be able to effectively carry out analysis and answer questions which has to do with production_companies. A new csv **prodname_cleaned.csv** file was created from the original dataset. This is was done to be able to answer questions 4 and 5.
6.	**Genre and Production_companies analysis:** A third csv file was created from the genre file. This file is specifically created in other to be able to answer question 6 which will require the combine analsis of borth genre and production_companies.

