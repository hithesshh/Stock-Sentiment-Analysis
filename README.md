# Stock-Sentiment-Analysis
Sentiment analysis performed on news headlines regarding stocks to predict the overall condition of the stock market
Extracting stock sentiment from news headlines is a pivotal aspect of modern financial analysis. It involves employing advanced computational techniques to sift through vast quantities of news articles and headlines related to specific stocks or the broader financial market. The goal is to discern the prevailing sentiment surrounding a particular stock, be it positive, negative, or neutral. 
By leveraging natural language processing (NLP) and sentiment analysis algorithms, analysts can gain a deeper understanding of market sentiment and potential shifts in investor sentiment.
Algorithm	
1. Data Retrieval
➢	Import the necessary libraries, such as feedparser, to fetch news headlines from an RSS feed.
➢	Define the RSS feed URL (e.g., Google News RSS for stock market news).
➢	Create a function retrieve_google_news_headlines to fetch news headlines from the RSS feed, considering pagination to collect a specified number of headlines.
2. Data Storage:
➢	Define an output CSV file name to store the collected headlines.
➢	Create a function save_headlines_to_csv to save the fetched headlines to a CSV file.
3. Sentiment Analysis:
➢	Import libraries like numpy, pandas, and nltk for data processing and sentiment analysis.
➢	Download the VADER sentiment lexicon for sentiment analysis.
4. Loading Data:
➢	Load the headlines from the CSV file into a pandas DataFrame for further analysis.
5. Sentiment Analysis Loop:
➢	Initialize counters for positive, negative, and neutral headlines.
➢	Create a loop to iterate through each headline.
➢	Use the VADER sentiment intensity analyzer to analyze the sentiment of each headline.
➢	Determine the sentiment label (positive, negative, or neutral) based on the compound sentiment score.
6. Sentiment Analysis Results:
➢	 Print the headline and its sentiment label (e.g., "Positive (+0.75)") for each headline.
➢	 Update the counters based on the sentiment label.
7. Overall Sentiment:
➢	Calculate the overall market sentiment based on the majority sentiment category (positive, negative, or neutral).
