# Customer_Segmentation_Using_RFM_Model
The more effectively we understand our customers, the more likely it is that we will raise brand/product awareness, sales, and ROI. This project is focused on segmenting our client base into categories that, among other things, reflect their purchasing power and pinpointing key commercial prospects.
This Readme section is to walk you through my codes and processes and will be useful to Data Analysts and Scientist. For For the Stakeholder's report and insights, check the Stakeholders Report PDF or watch the presentation https://www.canva.com/design/DAFIO0lN758/MR_jKf-fQXgfbdxMxuZw5g/watch?utm_content=DAFIO0lN758&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink


The is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail was used for this analysis.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.
Segmenting their client base into categories that, among other things, reflect their purchasing power and pinpointing key commercial prospects was the focus of this project.
By segmenting their consumers into Low, Mid, and High value segments, I will help them target their customers effectively and maintain customer acquisition and retention, i.e. avoid higher churn rate. This data set was provided by a UK-based and registered non-store online retailer.


# Methodology
-Cleaning the data by deleting necessary rows or/and columns, getting the relevant insights, and representing the data set using the most effective visualization charts
-Group the data into Recency, Frequency and Monetary clusters by deploying the KMeans Clustering algorithm and creating a new DataFrame to host the new columns generated.
-Interpret the results of analysis and proffer business strageties and recommendations tailored to increased revenue and ROI.


# Data Cleaning & EDA
This project was conducted using Jupyter Notebook. After loading the appropriate libraries, I found the missing cells and made the necessary adjustments by removing them. I then verified that the columns were of the necessary types, although for this project, the CustomerID and InvoiceDate columns' data types were altered to accomplish our primary goal.
I then calculated the Recency, Frequency, and Monetary Values of each consumer. I only included the customer's most recent purchase in my calculations for recency, the total number of purchases for frequency, and the monetary amount of all of their past transactions combined for value. A new data frame called RFM received the new columns.
The relationships between the metrics, the greatest and lowest values for each metric, as well as outliers like the reasons why certain clients had negative financial value, were among the patterns I discovered. It turns out that customers received a clear return policy, and those who returned their purchases suffered financial losses. 
The limited correlation between each variable suggested that, in contrast to Bayes' theorem, the results of one measure did not necessarily alter the results of the other. Please refer to the jupyter file for more technical details.
I then used boxplots, bar plots, histograms, box plots, and heatmaps to visualize the data.


# Deploying the KMeans  Model
5 clusters were created for each metric (0,1,2,3,4) which when put together gives a overall score of 12. Using the KMeans algorithm, I fit the data for training and predicted the
 scores for reach of the metrics. I also created a function order_cluster to ensure there was a consistent order for the cluster numbers that will be the output of the KMeans prediction.
 I went on to obtain the overall score of the cusotomers and performed some visualizattion and analysis.
 
 
 # Conclusion
 Based on the recommendations and insights in the Stakeholders report, if implemented, the company stand to generate even more revenue and create brand awareness for their services.
 






