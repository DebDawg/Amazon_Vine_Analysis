# Amazon Vine Analysis

## Overview of the analysis of the Vine program:
This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members. We have access to approximately 50 datasets, I chose to check the reviews for Wireless products from phone brands to cases, selfie sticks, and multiple additional products.  The analysis uses PySpark to perform the ETL process to extract the dataset and transform the data to connect to an AWS RDS instance.  Once connected the data loads the transformed data into pgAdmin and calculates different metrics.  Then we use PySpark again to determine if there is any bias from Vine members in our dataset.


## Results

**Total number of Vine reviews:**

- Total # of Paid Reviews

  ![image](https://user-images.githubusercontent.com/110787194/211240998-a34a57b0-b1d2-4dd7-8725-46bb25515bf1.png)

- Total # of Unpaid Reviews

  ![image](https://user-images.githubusercontent.com/110787194/211241041-02515ad9-2378-45e7-acc8-f06e1755c188.png)

- Total # of 5-star Paid Reviews

  ![image](https://user-images.githubusercontent.com/110787194/211241069-402468d3-3ba0-4695-8999-5b75b7df583b.png)
   
- Total # of 5-star Unpaid Reviews

  ![image](https://user-images.githubusercontent.com/110787194/211241471-1678d672-afbd-4e82-85be-691eca7b0107.png)

- The % of 5-Star Paid Reviews

  ![image](https://user-images.githubusercontent.com/110787194/211241925-9b0169f0-4f9e-4ced-ad3c-210b8904b903.png)
  
- The % of 5-Star Unpaid Reviews

  ![image](https://user-images.githubusercontent.com/110787194/211241731-7398f325-2b72-4cd7-be67-3767f66a34a9.png)


## Summary:

36% (222 reviews) out of a total of 613 reviews were paid.
47% (30,543 reviews) out of a total of 64,968 reviews were unpaid.

Both of the results were less than 50% which is not a positive review.  So these were not biased results.  
I myself cannot determine if these results could be considered biased, however if we were to do a statistical analysis that would allow us to figure out how or if these results are not biased.  



















Resources: [Amazon Review datasets](https://github.com/cedoula/Amazon_Vine_Analysis/blob/main/README.md#:~:text=Amazon%20Review%20datasets)
Software: AWS, Google Colab Notebook, PgAdmin 4, PostgresSQL 15, and PySpark  

