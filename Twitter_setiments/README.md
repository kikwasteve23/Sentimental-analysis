# Sentiment Analysis of Customer Tweets: Gaining Competitive Insights for Google and Apple Products

### Project Background
Ensemble Africa, an esteemed consultancy firm, collaborates closely with a prominent marketing agency driven by a singular objective: comprehending client product preferences through the lens of Twitter sentiments. This agency serves as a vital bridge between clients and their target audience, empowering them with consumer insights that are indispensable in today's competitive landscape.

The goal of this project is to develop a sentiment analysis model that accurately rates the sentiments of tweets about Apple and google products. By understanding the sentiments of customers' experiences, the marketing agency intends to identify areas where they can improve their services so as to enhance customer satisfaction and loyalty.

## Objectives
>- To build a specialized sentiment analysis model that can analyze twitter sentiments.
>- To establish if there is any differences in twitter sentiments between apple and google product
>- To find out the inclusive sentiment view towards apple and google products
>- To investigate the recurring topics of interest associated with negative or positive sentiments as seen by google and apple brands

## Stakeholders
Our stakeholder is a marketting agency seeking to understand client product needs based on their twitter sentiments. The client's aim is to also offer consumer insights with regards to the positive and negative mentions of the Google and Apple products.

## Hypothesis
H0: Our model's ability to accurately classify tweet sentiments between Google and Apple products is not significantly different from random chance.

H1: Our model's ability to accurately classify tweet sentiments between Google and Apple products is significantly better than random chance.

## Data Understanding
The dataset used is sourced from https://data.world/crowdflower/brands-and-product-emotions, consisting of 3 columns and 9093 rows. The columns include; tweet, sentiment and brand.

## Data Cleaning and Preparation
Steps used in data cleaning included: Renaming columns and removing duplicates aided in clarity and eliminating redundancy. Converting text to lowercase ensured uniformity, while imputing missing values maintained data integrity. In the NLP pre-processing phase, the removal of URLs, unnecessary terms, punctuation, and stopwords served to distill the text for sentiment analysis, resulting in a cleaner, more focused dataset primed for accurate emotion and sentiment extraction. The libraries used included, Pandas, NLTK, POS tagging. These provided efficient and specialized tools in text cleaning and manipulation for NLP tasks. 

## EDA

![image](https://github.com/kithinji007/Sentiments-Analysis/assets/128479803/72563985-0fba-48f6-9629-f02da7fa4f9e)


![image](https://github.com/kithinji007/Sentiments-Analysis/assets/128479803/5d6b68fe-dbaf-4e14-a7b1-a4fa9a38aebe)

From the visualiatin above, the product that recieved most tweets is google. The common trend is that most customers don't hold any emotion towards the product.


## Pre-processing for NLP

![image](https://github.com/kithinji007/Sentiments-Analysis/assets/128479803/305d37a3-7f2d-41da-a167-a659139c8955)

## Modelling
>- In our sentiment analysis project, we explored the effectiveness of various machine learning models in categorizing text-based data into sentiment classes. We employed a range of models to capture the nuances of sentiment expressed in textual content. 
>- The best performing models were Random forest and Neural Network respectively.


## Final Model
Our final model is the tuned Random forest with an accuracy of 98% on training data against an 86% on test data.
![image](https://github.com/kithinji007/Sentiments-Analysis/assets/128479803/ef1fe070-418f-46f6-b7ca-b9dc1c615359)



## Comparing it with Neural Network
The Neural Network performed really well with 85% accuracy. The plot showcasing the learning curve is ideal with both the training and validation curve accuracy increasing with the number of epochs and then later plateaus indicating that the model has learnt from the training data and generalizes well to new data.

The loss curve however, might indicate overfitting with an increasing number of epochs. This is seen as the loss decreases on the training data while increasing on validation data.
![download](https://github.com/kithinji007/Sentiments-Analysis/assets/110093196/918941e7-9dee-4092-8e09-6cf84e43eab1)

## Model Evaluation
The tuned Random Forest model appears to be a good candidate. It's yielding competitive accuracy on both the training and validation sets, and the accuracy drop is relatively small, indicating good generalization. It also has a high F1-Score 86% which shows a good balance between precision and recall.


## Conclusion
Google and Apple products are vastly used in the world. This study successfully achieved its objectives aimed at understanding the sentiment dynamics surrounding Google and Apple products on Twitter.

Through the development of a specialized sentiment analysis model, we discerned nuanced differences in sentiments between these two tech giants. Our best model was Random Forest Model since it displayed a high F1 Score of 86%; It yields a competitive accuracy on both the training and validation sets, and the accuracy drop is relatively small, indicating good generalization.

Our analysis revealed varying degrees of positivity and negativity in the Twitter discussions concerning their products, shedding light on the overall inclusive sentiment view towards both brands. Additionally, by investigating recurring topics associated with positive and negative sentiments using a word cloud for each sentiment, we gained valuable insights into the prevailing themes that influence public perception of Google and Apple. This research contributes to a deeper comprehension of how sentiments and topics converge to shape the online discourse surrounding these companies, offering a valuable resource for both academia and industry.

## Recommendations For Our Stakeholders
Craft marketing messages that align with the predominant sentiments expressed by consumers. Tailor your messages to resonate with the positive aspects and address concerns highlighted in sentiment analysis.

Collaborate with influencers who align with the positive sentiments around your brand. Their endorsement can amplify positive sentiment and reach a wider audience.

Regularly assess the impact of your marketing strategies on sentiment trends. Track changes in sentiment over time to gauge the effectiveness of your efforts and make data-driven adjustments

## NextSteps
Incorporate more advanced natural language processing techniques and machine learning algorithms to enhance the accuracy of sentiment classification. Note that the project is resource intensive, having GPUs will reduce model runtime

Extend the analysis over a longer time period to observe trends and changes in sentiment over time. This can provide deeper insights into the effects of product launches, events, and other external factors on public sentiment.

Collaborate with data scientists and NLP experts to continually refine the sentiment analysis model. This will ensure accurate classification of sentiment in tweets, enabling the agency to deliver high-quality insights to clients.

Analyze sentiment based on user demographics such as age, gender, and location. This helps tailor marketing strategies to specific consumer segments and craft messaging that resonates with different groups.


Develop predictive models to anticipate shifts in sentiment. This proactive approach allows the agency to advise clients on adjusting their strategies ahead of sentiment fluctuations.

Work closely with clients to integrate sentiment insights from customers into their marketing strategies. Collaborate on content creation, social media campaigns, and product messaging based on sentiment trends.
