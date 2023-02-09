# Data Source Description

The dataset that we will use is the 2021 [Core Trends Survey](https://www.pewresearch.org/internet/dataset/2021-core-trends-survey/) put out by the [Pew Research Center](https://www.pewresearch.org/). In this survey, Pew asked respondents about their internet habits, including what social media sites they regularly used. 

From the full data, I have extracted and recoded the following variables for our use as an analytical dataset. To load this dataset in R, you just need to run the setup code chunk in the full_report.Rmd R Markdown document. The name of the dataset in R is `pew`. 

* **tiktok**: This variable indicates whether the respondent was a TikTok user. A value of "1" indicates that they were a TikTok user and a value of "0" indicates that they were not. I am coding it this way as a numeric value so that we can use it as the dependent variable in our final models. In those models, we can interpret all of the slope changes as the change in the probability that a person uses TikTok for a one unit change in the independent variable. However, for graphical and early analysis, you should treat this variable as a categorical variable by surrounding with the `factor` command like `factor(tiktok)`. This is the key dependent variable.
* **age**: Age of the respondent in years. This is our key independent variable.
* **gender**: Gender of the respondent as female, male, or non-binary.
* **degree**: Highest degree earned by the respondent.
* **employ_status**: The current employment status of the respondent.
