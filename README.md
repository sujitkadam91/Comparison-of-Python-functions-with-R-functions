# Comparison-of-Python-functions-with-R-functions
###Subscribe this YouTube Channel Data/Fun
## How to install and load Package

install.packages("dplyr")

library(dplyr)

## For Checking working Directory

getwd()


## For setting new working directory for reading CSV file 

setwd("E:\\Data Sets")

## For checking list of files in a directory

dir()


## For reading csv file 
#https://www.kaggle.com/c/titanic/data

df<- read.csv("train.csv")

## For Checking structure of Data frame

str(df)


## For Summarise dataframe

summary(df)

## For checking how many rows in df

nrow(df)


## For checking how many coloumns in df

ncol(df)



## For checking dimentions of df

dim(df)


## For checking column names of df

colnames(df)

## For checking row names of df

rownames(df)

## For view top 10 rows of df

head(df,10)

## For view bottom 10 rows of df

tail(df,10)

## For selecting random 7 rows from df

library(dplyr)

sample_n(df,7)

## For Selecting Colums from df

DF1<-select(df,Age,Survived)

colnames(DF1)


## Drop colums

DF_drop_Age_Sur<-select(df,-c(Age,Survived))

names(DF_drop_Age_Sur)

## For select random 25% rows from df

df_25per<- sample_frac(df,0.25)

dim(df_25per)


## For checking Missing values

is.na(df$Age)

## For sorting df by specific column

DF_Arrange_Age<-arrange(df,Age)# Defalut is Accending order

head(DF_Arrange_Age)

DF_Arrange_Age_Des<-arrange(df,desc(Age))## Descending

head(DF_Arrange_Age_Des)


## For Filtering data

df_filter_Age<-filter(df, Age >= 40)

head(df_filter_Age)

dim(df_filter_Age)

## How to rename column 

New_df<- rename(df,New_Age= Age)

names(New_df)
############Subscribe this YouTube Channel Data/Fun############

************************* PYHON CODES ******************************************************************************************
###Subscribe this YouTube Channel Data/Fun
## How to install and load Package
!pip install numpy       #install 
!pip pandas numpy
import numpy as np
import pandas as pd

## For Checking working Directory

import os
os.getcwd()


## For setting new working directory for reading CSV file 


os.chdir("E:\\Data Sets")

## For checking list of files in a directory

os.listdir()

#Subscribe this YouTube Channel Data/Fun
## For reading csv file 
#https://www.kaggle.com/c/titanic/data

df = pd.read_csv("train.csv")

#Subscribe this YouTube Channel Data/Fun
## For Checking structure of Data frame

df.info()

## For Summarise dataframe

df.describe()

#Subscribe this YouTube Channel Data/Fun
## For checking number of rows indf

df.shape[0]

## For Checking number of colums in df

df.shape[1]

#Subscribe this YouTube Channel Data/Fun
## For checking dimentions of df

df.shape

#Subscribe this YouTube Channel Data/Fun
## For checking column names of df

df.columns

## For checking row names of df

df.index

#Subscribe this YouTube Channel Data/Fun
## For view top 10 rows of df

df.head(10)

## For view bottom 10 rows of df

df.tail(10)

#Subscribe this YouTube Channel Data/Fun

## For selecting random 7 rows from df

df.sample(7)

## For Selecting Colums from df

DF1=df[["Age","Survived"]]
DF1.columns
#Subscribe this YouTube Channel Data/Fun
## Drop colums

DF_drop_Age_Sur= df.drop(["Age","Survived"],axis=1)
DF_drop_Age_Sur.columns

## For select random 25% rows from df

df_25per=df.sample(frac=0.25)
df_25per.shape

#Subscribe this YouTube Channel Data/Fun
## For checking Missing values

pd.isnull(df.Age)

## For sorting df by specific column

DF_Arrange_Age=df.sort_values(['Age'])
DF_Arrange_Age.head()

DF_Arrange_Age_Des=df.sort_values(['Age'],ascending=False)

#Subscribe this YouTube Channel Data/Fun
## For Filtering data

df_filter_Age=df.query('Age>=40')
df_filter_Age.shape

## How to rename column

New_df = df.rename(columns={"Age":"New_Age"})
New_df.columns

############Subscribe this YouTube Channel Data/Fun############
***************************PYTHON CODES************************************************

## How to install and load Package

!pip install numpy       #install 

!pip pandas numpy

import numpy as np

import pandas as pd

## For Checking working Directory

import os
os.getcwd()


## For setting new working directory for reading CSV file 


os.chdir("E:\\Data Sets")

## For checking list of files in a directory

os.listdir()


## For reading csv file 

#https://www.kaggle.com/c/titanic/data

df = pd.read_csv("train.csv")


## For Checking structure of Data frame

df.info()

## For Summarise dataframe

df.describe()


## For checking number of rows indf

df.shape[0]

## For Checking number of colums in df

df.shape[1]

## For checking dimentions of df

df.shape

## For checking column names of df

df.columns

## For checking row names of df

df.index


## For view top 10 rows of df

df.head(10)

## For view bottom 10 rows of df

df.tail(10)



## For selecting random 7 rows from df

df.sample(7)

## For Selecting Colums from df

DF1=df[["Age","Survived"]]

DF1.columns


## Drop colums

DF_drop_Age_Sur= df.drop(["Age","Survived"],axis=1)

DF_drop_Age_Sur.columns

## For select random 25% rows from df

df_25per=df.sample(frac=0.25)

df_25per.shape

## For checking Missing values

pd.isnull(df.Age)

## For sorting df by specific column

DF_Arrange_Age=df.sort_values(['Age'])

DF_Arrange_Age.head()

DF_Arrange_Age_Des=df.sort_values(['Age'],ascending=False)


## For Filtering data

df_filter_Age=df.query('Age>=40')

df_filter_Age.shape

## How to rename column

New_df = df.rename(columns={"Age":"New_Age"})

New_df.columns

############Subscribe this YouTube Channel Data/Fun############



