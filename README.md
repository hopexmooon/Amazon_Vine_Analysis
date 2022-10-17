## Amazon Vine Analysis

### Overview of the analysis: 

The purpose of this analysis is to further my skills and knowledge on performing ELT on a large dataset. I was able to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. From the 50 datasets available I selected Gift Card reviews Dataset to analyze. I pulling specific data from the dataset, transforming it on a Colab Notebook, conncecting it to an AWS RDS, and finally load the transformed data into pgAdmin. Further analysis was done using Pandas. 


### Results: 

* How many Vine reviews and non-Vine reviews were there?

There are a total of 149,086 reviews. Out of all the reviews there are zero Vine reviews. All the reviews for Gift Cards are made up of non-Vine reviews. Because of this further analysis on Vine reviews will be omitted because there are no Vine reviews. 

<img width="284" alt="Screen Shot 2022-10-17 at 1 32 09 PM" src="https://user-images.githubusercontent.com/108151049/196244305-fe13170e-1af7-4361-9ab2-018439e6d630.png">

<img width="404" alt="Screen Shot 2022-10-17 at 1 37 47 PM" src="https://user-images.githubusercontent.com/108151049/196245255-0bd975a0-2b1d-424e-930d-6fa3425f8f5f.png">


* How many non-Vine reviews were 5 stars?

The image below is a screenshot from the Jupyter notebook where I used Pandas to further analyze the data. On it I created a few dataframes to filter the information further. I used vine_unpaid.df to collect all the reviews where there was no Amazon Vine program payment. From that dataframe I filtered further to find out of the non-Vine reviews how many were 5 stars (vine_unpaid_star) and used len() to find the total. From the analysis there are a total of 87 5-star non-Vine reviews for Gift Cards.

<img width="671" alt="Screen Shot 2022-10-17 at 1 43 47 PM" src="https://user-images.githubusercontent.com/108151049/196246357-81d1cf77-19f2-4069-b8da-d32683fadb14.png">


* What percentage of non-Vine reviews were 5 stars?

We can do simple math to figure out the percentage of 5-star non-Vine reviews. We find that 25.58% of non-Vine reviews recieved 5 stars.


### Summary: 

Because we did not have any data to compare non-Vine reivews vs Vine reviews there is no way to judge for any positivity bias resulting from the Vine program. We have no way of analyzing the effectiveness of the Vine program. 
