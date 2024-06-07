# datafun-06-eda

#### I created a new repo in Github

#### I added the README.md file when creating the new repo

#### I opened the Documents folder in File Explorer since that is where I wanted this project to be stored

#### I cloned the new repo to the Documents folder with the following command

```shell

git clone site_URL

```

## Opening project and adding files in VS Code

#### I opened the new project in VS Code

#### I added a .gitignore file

#### I added a requirements.txt file

#### I created a virtual environment using the code below

```shell
py -m venv .venv
.venv\Scripts\Activate

```

## Install packages in Virtual Envvironment

#### The code below installs pandas and pyarrows in the requirements.txt file
```shell

pip install jupyterlab pandas pyarrow matplotlib seaborn
python -m pip freeze > requirements.txt

```

## Git add my recent changes to my github
```shell

Git add .

```

## Git commit my recent changes to my github

```shell

git commit -m "Start New Project"

```

## Push recent changes to my github

```shell

git push origin main

```

## Tips Data Set

This data set contains records representing the tipping behavior of customers.
It includes data such as tip, sex, smoker, day and size.

Link to the data set:
https://github.com/mwaskom/seaborn-data/blob/master/tips.csv


## Imported dependencies and loaded my data set using the code below

```shell

#Import Dependencies
import matplotlib.pyplot as plt
import pandas as pd
import seaborn as sns
import pyarrow as pa

# Load the tips dataset into DataFrame
df = sns.load_dataset('tips')

# Inspect first rows of the DataFrame
print(df.head())

```

## Performed Initial Inspection of the Data Set

#### By pulling the first 10 rows I'm looking for trends or patterns in the data

```shell

print(df.head(10))
print(df.shape)
print(df.dtypes)

```

## DataFrame Describe to Display Summary Statistics

#### This gives a high level overview of the statistics and numbers in the dataset

```shell

print(df.describe())

```

## Plot Histogram for total_bill Column and all numerical columns

I created multiple histograms to analyze and decipher the data in the numercial and categorical columns.

## Plot Counts for Each Categorical Column

I created multiple plots to analyze the data for all of the categorical columns in the data set.

## Data Transformation and Feature Engineering

I transformed the data by renaming two columns and adding a new column to the data set.

## Initial Visualizations

I created different graphs and charts to visualize the data and answer the three following questions:
1. How do the different numercial columns in the tips data set correlate with each other?
2. How do the tip amount and total_bill amount vary between the different days of the week?
3. How do the tip amount and total_bill amount vary between different genders?

## Push final changes to my github

```shell

git add .
git commit -m "Final Commit"
git push origin main

```

## Created Project 6 EDA Notebook based on the source below:
https://github.com/denisecase/datafun-06-spec