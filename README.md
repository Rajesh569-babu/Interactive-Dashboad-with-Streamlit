Sentiment Analysis Dashboard
Overview

This project is a Streamlit-based interactive dashboard for analyzing the sentiment of Twitter data. Users can explore tweets related to airlines, view sentiment distributions, visualize tweet locations, and generate word clouds based on tweet sentiment.

The dashboard provides:

Interactive visualizations of tweet sentiments.

Filtering of tweets by time, airline, and sentiment.

Word cloud generation for specific sentiments.

Real-time mapping of tweet locations.

Features

Random Tweet Display

Select a sentiment (positive, neutral, negative) from the sidebar.

Display a random tweet corresponding to that sentiment.

Sentiment Visualization

Shows the distribution of tweets by sentiment.

Available visualization types: Histogram and Pie chart.

Tweet Time & Location Analysis

Filter tweets by the hour of the day.

Visualize tweet locations on a map.

Option to show raw tweet data.

Airline-wise Sentiment Breakdown

Select airlines to compare sentiment counts.

Visualized as a histogram with facets for each sentiment.

Word Cloud Generation

Generate word clouds for positive, neutral, or negative tweets.

Automatically filters out URLs, mentions, and retweets.

Installation
Prerequisites

Python 3.7+

Pip package manager

Required Libraries

Install all dependencies with pip:

pip install streamlit pandas numpy plotly matplotlib wordcloud

Dataset

The dashboard uses a CSV dataset named Tweets.csv containing airline tweets.

Columns of interest:

text → Tweet text

airline_sentiment → Sentiment label (positive, neutral, negative)

tweet_created → Timestamp of the tweet

airline → Airline name

tweet_location / coordinates → Optional location data for mapping

How to Run

Place the Tweets.csv file in the same directory as the app script.

Run the Streamlit app:

streamlit run app.py


Open the URL provided in the terminal (usually http://localhost:8501) in a web browser.

Usage Instructions

Sidebar Controls

Show random tweets: Select sentiment to view a random tweet.

Visualization type: Choose Histogram or Pie chart to display sentiment counts.

Filter by hour: Use slider to see tweets posted in a specific hour.

Select airlines: Compare sentiment across multiple airlines.

Word Cloud: Generate word cloud for selected sentiment.

Main Dashboard

Displays charts, maps, and word clouds based on sidebar selections.

Hover over charts to view detailed data points.
