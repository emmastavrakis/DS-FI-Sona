# DS-FI-Sona
Data Science for Industry Assignment 2

#1.  Introduction

In this assignment we will be conducting both predictive and descriptive analyses on the SONA dataset.  To this end we have:

1.  Built a neural network and a convolutional neural network to predict which president was the source when given a sentence of text 
2.  Assessed the performance of both the nn and cnn on unseen data and then compared and interpreted these results
3.  Conducted a desriptive analysis of the text in the speeches

The R-markdown workbook in this repo sets out the approach we took to conduct these analyses, decisions and choices that we made, what challenges we encountered and how we overcame these, as well as our interpretation of- and commentary on the results.

We were tasked to work in groups for this assignment and to advise how the workload was divided amongst the group members, as well as providing evidence of team collaboration on Git, which is what we have used this repository for.

#2.  Data preparation

The State of the Nation Address of the President of South Africa (SONA) is an annual event in which the President of South Africa reports on the status of the nation, normally to the resumption of a joint sitting of Parliament. In years that elections took place, a State of the Nation Address happens twice, once before and again after the election.

We were provided with full text of all State of the Nation Address (SONA) speeches, from 1994 through to 2018 on which to conduct our analyses.

Our approach to pre-processing the data centred primarily on using the **tidyverse** and **tidytext** libraries to wrangle the data and mine the text.

#3.  Exploratory Data Analysis

As part of the data preparation phase, we did some exploratory data analysis to see how the data was distributed and what type of trends were evident from the data.  We analysed the word counts, bigrams and trigrams.

#4.  Predictive Anaysis

For the predictive analysis we decided to build two models and compare their performance.  We started with a basic neural network (nn) and then built a convolutional neural network (cnn).  10-fold cros validation was used to validate the models' results

#5.  Comparison of results

The classic neural network achieved better performance on this data than the cnn, achieving >= 70% accuracy on the test dataset compared to the cnn's performance of approx 56%.  We conducted extensive tuning on both models, but were only able to significantly improve the performance of the classic neural network.

#6.  Descriptive Analysis

Lastly we performen a descriptive analysis of the data, including both a sentiment analysis and some topic investigation using a bag-of-words model to do topic modelling.  From the sentiment analysis we were able to describe each president's average sentiment and show how this varied over time, correlating to key events such as a spike in positive sentiment around the 2010 Soccer World Cup.  From the topic modelling analysis we were able to roughly define two broad topics : economic development and social development.  Although all presidents ultimately discussed relatively similar topics, this major distinction flavoured the SONA speeches from year to year.






