#What are Various Popular Tech YouTubers Saying? A Topic Modeling Approach to Tech YouTube Transcripts

## Overview

This project aims to perform topic modeling on a Kaggle dataset "YouTuber's Saying Things" containing user-written transcripts, YouTuber-made scripts, and auto-generated subtitles. The goal is to analyze the data and extract useful insights from it. 

## Methodology

1. Download the Kaggle dataset "YouTuber's Saying Things" (I've also provided the exact data I've used)
2. Convert the CSV file into a pandas DataFrame for easier cleanup and filter it by "Tech, Tech,Comedy, Tech, Informative, and Tech,News".
3. Combine all the Transcript values into one long string.
4. Use NLTK to remove all "STOPWORDS" from the text to remove words that are not helpful in topic modeling.
5. Utilize a python script to tokenize the reviews and generate text tokens based on the reviews, clean the tokens of stopwords that will negatively impact the analysis, then lemmatize the tokens and join the lemmatized words together.
6. Using the gensim python module, generate the LDA model for analysis based on the number of topics and plot the topics as a bar graph.
7. Plot the models on a graph with respect to changing the number of topics that go into generating the model using pyLDAvis.
8. Note that the dataset contains a combination of user-written transcripts, YouTuber-made scripts, and auto-generated subtitles from text-to-speech, so some results may not be entirely accurate. However, given the limitations of data on human-written transcripts, we must use the available data to have a useful corpus for Topic Modeling.

## Conclusion

This project is aimed at analyzing the Kaggle dataset "YouTuber's Saying Things" and extracting useful insights from it using topic modeling. By performing the above-mentioned methodology, we can visualize the topics of the data and analyze the results to gain insights. Note that the results may not be entirely accurate due to the limitations of the dataset.
