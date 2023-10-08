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

