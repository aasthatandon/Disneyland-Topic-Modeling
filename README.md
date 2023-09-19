# Disneyland-Topic-Modeling

### Problem Statement : 
Customer feedback plays a pivotal role in the service industry, and Disneyland, being one of the world's most renowned theme park chains, recognizes the significance of analyzing online customer reviews. The objective of this research is to employ topic modeling techniques to comprehensively analyze customer reviews of Disneyland branches in California, Paris, and Hong Kong. The aim is to identify the key topics that contribute to both positive and negative reviews, explore variations in these topics across different months and seasons, and ultimately utilize this information to enhance visitor satisfaction, improve services, and make informed, data-driven decisions.

### Research Questions:
- What are the key topics mentioned in positive and negative customer reviews across different branches and the factors associated to it ?
- How do these topics vary across different months in each branch ?
- How do these topics vary across different seasons in each branch ?
- How can this information be used to enhance the customer experience and address any issues affecting customer satisfaction ?

### Data source:
Dataset is available on Kaggle at the following link :
https://www.kaggle.com/datasets/arushchillar/disneyland-reviews.

### Data Preparation :

We began by cleaning the dataset, retaining 40K reviews (18K - California, 12K - Paris, 9K - Hong Kong), excluding rows with missing Year_Month entries. We then parsed "Year" and "Month," grouping them into "Seasons" (Fall, Winter, Spring, Summer). Several preprocessing step were performed including sentence-to-word tokenization, stemming, stop word and common word removal, iteratively enhancing data quality.

### Analysis and Insights :
#### Identifying Key topics mentioned in positive and negative customer reviews : 
Performed separate branch-wise analyses using a 1 to 5 rating scale, categorizing reviews as Negative (1-3) and Positive (4-5). Employing LDA topic modeling, we extracted distinct topics from Positive feedback, indicating customer-attracting themes, and Negative feedback, identifying issues potentially detrimental to the business.

#### Identifying topics varying across different months in each branch : 
Conducted comprehensive reviews analysis for each branch, extracting K distinct topics. By computing monthly average topic distributions (from January to December) across all reviews, we tracked topic dynamics, allowing us to delve into the reasons behind evolving themes over time.

#### Identifying topics varying across different seasons in each branch : 
Similar to monthwise analysis. Analyzed branch reviews, identified K topics, and computed average topic distributions for each season (Fall, Summer, Winter, Spring) to uncover seasonal topic shifts and their underlying reasons.


### Files Overview:
- ```Disneyland_Review_Exploratory_Analysis.ipynb```: EDA on combined Disneyland reviews from Paris, HongKong, and California
- ```Disneyland_Review_Topic_Modeling_CA.ipynb```: Topic Modeling on Disneyland Reviews of California branch
- ```Disneyland_Review_Topic_Modeling_HK.ipynb```: Topic Modeling on Disneyland Reviews of HongKong branch
- ```Disneyland_Review_Topic_Modeling_Paris.ipynb```: Topic Modeling on Disneyland Reviews of Paris branch
- ```Disneyland_Review_Technical_Report.pdf``` : Technical Report of combined analysis of all three branches
- ```Disneyland_Review_Presentation.pdf``` : Presentation of combined analysis of all three branches
