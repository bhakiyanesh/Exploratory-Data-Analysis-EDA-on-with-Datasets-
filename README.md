# Aim:  
To Perform exploratory data analysis (EDA) on with datasets like email data set. 
# Procedure: 
Exploratory Data Analysis (EDA) on email datasets involves importing the data, cleaning it, visualizing 
it, and extracting insights. Here's a step-by-step guide on how to perform EDA on an email dataset using 
Python and Pandas 
## 1. Import Necessary Libraries: 
Import the required Python libraries for data analysis and visualization. 
## 2. Load Email Data: 
Assuming you have a folder containing email files (e.g., .eml files), you can use the email library to 
parse and extract the email contents. 
## 3. Data Cleaning: 
Depending on your dataset, you may need to clean and preprocess the data. Common cleaning 
steps include handling missing values, converting dates to datetime format, and removing duplicates. 
## 4. Data Exploration: 
Now, you can start exploring the dataset using various techniques. Here are some common EDA tasks: 
Basic Statistics: 
Get summary statistics of the dataset. 
Distribution of Dates: 
Visualize the distribution of email dates. 
## 5. Word Cloud for Subject or Message: 
Create a word cloud to visualize common words in email subjects or messages. 
## 6. Top Senders and Recipients: 
Find the top email senders and recipients. 
Depending on your dataset, you can explore further, analyze sentiment, perform network analysis, or 
any other relevant analysis to gain insights from your email data. 
#Program: 
''' # Import necessary libraries 
import pandas as pd 
import matplotlib.pyplot as plt 
import seaborn as sns 
#Load the dataset 
df = pd.read_csv('D:\ARCHANA\dxv\LAB\DXV\Emaildataset.csv') 
#Display basic information about the dataset 
print(df.info()) 
#Display the first few rows of the dataset 
print(df.head()) 
#Descriptive statistics 
print(df.describe()) 
#Check for missing values 
print(df.isnull().sum()) 
#Visualize the distribution of numerical variables 
sns.pairplot(df) 
plt.show() 
#Visualize the distribution of categorical variables 
sns.countplot(x='label', data=df) 
plt.show() 
#Correlation matrix for numerical variables 
correlation_matrix = df.corr() 
sns.heatmap(correlation_matrix, annot=True, cmap='coolwarm') 
plt.show() 
#Word cloud for text data (if you have a column with text data) 
from wordcloud import WordCloud 
text_data = ' '.join(df['text_column']) 
wordcloud = WordCloud(width=800, height=400, random_state=21, 
max_font_size=110).generate(text_data) 
plt.figure(figsize=(10, 7)) 
plt.imshow(wordcloud, interpolation="bilinear") 
plt.axis('off') 
plt.show()'''
# Output

<img width="627" height="416" alt="Screenshot 2026-02-02 202551" src="https://github.com/user-attachments/assets/d2c88cc9-50b8-40b7-890f-a61e1d029ad9" />

<img width="597" height="602" alt="Screenshot 2026-02-02 202649" src="https://github.com/user-attachments/assets/fbafd9d1-f277-4e58-ba33-0844ca70c69e" />

<img width="486" height="529" alt="Screenshot 2026-02-02 202719" src="https://github.com/user-attachments/assets/ddbf8ce1-4829-4af7-bb1a-fd4b80be6bfa" />

<img width="515" height="456" alt="Screenshot 2026-02-02 202809" src="https://github.com/user-attachments/assets/ea82192a-b464-404b-a1ca-5737293ccda9" />
# RESULT: 
Thus the above working with numpy, pandas, matplotlib has been completed successfully. 
