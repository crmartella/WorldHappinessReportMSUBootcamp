# Factors Impacting Global Happiness

## MSU AI Bootcamp: Project #2
## Team Happy Tree Pandas [insert image]

### Members:
* Cristian Goian
* Sean Kavanagh
* Christopher Martella
* Taylor Peterson

## Description

Building a program to study the factors that can contribute to a happier country over time. We will focus on the world’s top 25 saddest countries (based on 2023 data) to create a model to predict what factors have the most impact on influencing people of those countries to be happier over time. We are using data from the World Happiness Report that is available through Kaggle.

## Getting Started

### Installation

- Clone this repository to your local environment
- Open in Jupyter Notebook or VSCode

### Dependencies / Required Packages

- Python 3.10
- Pandas 
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Prophet

## Goals / Questions to be addressed
1. We will use data from **2005-2018** to predict happiness for **2019-2023**, and compare that to actual data from **2019-2023** to determine the validity of our predictive model.

2. We will predict what the happiness of the (top 25) saddest countries could look like between **2024 and 2034**.

3. Based on our findings, we will select other variables to run additional models on to study correlations further.

4. We will use those selected variables to predict how much of an impact those variables have on the outcome; with a goal of increasing a particular region's happiness score.

5. What would life be like with and without an economic crash (2008 and 2009) and COVID-19 Pandemic (2021 and 2022)? What would it look like in a "Utopia" or "Dystopia"?

## **Data Overview**

#### The __*World Happiness Report (WHR)*__ is a partnership of:
- Gallup 
- Oxford Wellbeing Research Centre
- UN Sustainable Development Solutions Network
- WHR’s Editorial Board

#### To obtain the happiness rankings of each country, the WHR is provided survey responses from the life evaluations of the __Gallup World Poll (GWP)__. Happiness rankings are based on the answers to the Cantril Ladder question:
> "Please imagine a ladder, with steps numbered from 0 at the
bottom to 10 at the top.  
The top of the ladder represents the best possible life
for you and the bottom of the ladder represents the worst possible life for you.  
On which step of the ladder would you say you personally feel you stand at this
time?”

#### Variable Definitions
#### Happiness Score (Life Ladder): 


- **Life Ladder**
: A happiness ranking on a scale of 0 to 10.

- **Country Name**
: Name of the country

- **Regional Indicator**
: Region in which the country is located

- **Log GDP Per Capita**
: The wealth of the country.

- **Social Support**
: A value that indicates how many people have family and friends that they can rely on in times of trouble.

- **Healthy Life Expectancy At Birth**
: Average life expectancy of a country. Based on data from the World Health Organization's (WHO) Global Health Observatory data repository.

- **Freedom To Make Life Choices**
: National average of the satisfaction with individual freedom to make life choices.

- **Generosity**
: Measure of how likely people are to donate to charity. 

- **Perceptions Of Corruption**
: Measure of national corruption. The GWP asked whether or not corruption was widespread throughout both government and business, on an individual level.

- **Positive Affect**
: Average of measures for laughter, enjoyment and doing interesting things.

- **Negative Affect**
: Average of measures for worry, sadness and anger.

- **Confidence In National Government**
: Institutional trust


### **Data Separation**

#### We split our data in a few different ways to make our comparisons. 
#### We first ran our analysis based on the **Region** each country was assigned to. This is the **'Regional Indicator'** column. 

#### Our Regions:
- Central and Eastern Europe	
- Commonwealth of Independent States	
- East Asia	
- Latin America and Caribbean	
- Middle East and North Africa	
- North America and ANZ	
- South Asia	Southeast Asia	
- Sub-Saharan Africa	
- Western Europe

#### We also considered historical points in time (in the range of our data set, 2005-2023) that may have affected global happiness scores. We decided on **two** major incidents:
- The global economic recession that impacted our world economy. This took place during 2008 and 2009.
- The global COVID-19 Pandemic. The impact of this is appparent in 2021 and 2022.

#### Here is a dictionary to explain the  organization of datasets:
- **Crash**
: 2008 & 2009.
- **COVID**
: 2021 & 2022.
- **Eutopia**
: No Crash and No COVID. The years 2008, 2009, 2021, and 2022 are dropped from the dataset. The flaws of our global history are essentially erased.
- **Dystopia**
: Only Crash and COVID years. All other years are dropped from the data set.
- **Actual**
: The entire .csv file, containing all years and corresponding data


## Conclusions
- Life Expectancy and per capita is highly correlated to happiness
- Corruption is very vague.

## Problems encountered
## Future Considerations

## Acknowledgments

- World Happiness Report (2005-2022) Kaggle Data Set  - [https://www.kaggle.com/datasets/usamabuttar/world-happiness-report-2005-present/data](https://www.kaggle.com/datasets/usamabuttar/world-happiness-report-2005-present/data)
- World Happiness Report (2023) Kaggle Data Set -  [https://www.kaggle.com/datasets/sazidthe1/global-happiness-scores-and-factors?select=WHR_2023.csv](https://www.kaggle.com/datasets/sazidthe1/global-happiness-scores-and-factors?select=WHR_2023.csv)
- Statistical Appendix: Latest version - March 13,2023 - [https://happiness-report.s3.amazonaws.com/2023/WHR+23_Statistical_Appendix.pdf](https://happiness-report.s3.amazonaws.com/2023/WHR+23_Statistical_Appendix.pdf)
- World Happiness Report Home - [https://worldhappiness.report/](https://worldhappiness.report/)
- 
