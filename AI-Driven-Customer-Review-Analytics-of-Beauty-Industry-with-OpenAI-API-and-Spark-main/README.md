AI-Driven Customer Review Analytics of Beauty Industry with OpenAI API and Spark

# Contributors
Big thank to the wonderful team: 
### Technical
Xingyue Wang <wan01786@umn.edu>

Praveen Kumar G <govin098@umn.edu>

Paul Agbaje <agbaj004@umn.edu>
### Visualization
Claire Tsao <tsao0022@umn.edu>

Anurag Wadhwa <wadhw052@umn.edu>

Yumian Ding <ding0416@umn.edu>

# Executive Summary
### This project repository is created in partial fulfillment of the requirements for the Big Data Analytics course offered by the Master of Science in Business Analytics program at the Carlson School of Management, University of Minnesota.

Every year, the consumer product goods industry witnesses the introduction of around 30,000 new products, yet less than 10% of them manage to achieve true success, as revealed by the McKinsey Consumer Trend Study in 2019. Understanding customers precisely and timely for product development becomes one of the key strengths of consumer packaged goods (CPG) companies. 

Our project's primary objective is to establish a big-data-driven review intelligence and sentiment analysis pipeline, harnessing the capabilities of OpenAI, specifically tailored for the beauty industry. By leveraging LLM, we are able to think naturally again, effortlessly grasping the key information hidden in the data and conveying the business insights efficiently. 

## What is in the pipeline? 

We leverage Databricks, PySpark, and OpenAI APIs to scalably conduct unsupervised analysis of product reviews to extract topics and classify sentiments. By setting up 4 steps of prompts, we process the review data by batches and merge the resulting topics to get a bag of topics on the full scale of data. By labeling each review with topic and sentiment, we are able to generate a comprehensive dashboard of hieriarchical visualizations that is of great use in business settings. 

![alt text](https://github.com/Xingyue-Wang47/MSBA-2023-BDA-TrendsMktPlace-Team2/blob/main/Pipeline%20Flowchart)

## What are the values? 

### 1. Resolves the token limit of OpenAI prompt input and is able to handle large size of contents and generate topics on full scale of data. 
### 2. Generates nearly completely unsupervised topics results with no number of topics specified. 
### 3. Distinguished from traditional LDA by identifying topics based on its LLM training experience, not on the current dataset alone. 
### 4. Provides a more flexible sentiment analysis option, in which specific customized interest in sentiments can be analyzed easily (e.g. label the reviews that favor the color of this product as "positive in color")
### 5. Can be easily extended and transformed to many industries, as long as there is available review data
### 6. Leads to a comprehensive dashboard that provides analysis on different levels (category/subcategory/product)

### Link to the toy dataset: https://www.kaggle.com/datasets/jithinanievarghese/cosmetics-and-beauty-products-reviews-top-brands
### Link to the project video: https://youtu.be/yFQWXn-usTs
