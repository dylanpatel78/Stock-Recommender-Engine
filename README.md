# Stock-Recommender-Engine

## Project Overview
This project is a stock analysis tool that helps users find stocks based on both their financial performance and public sentiment. The tool allows you to input a sector (e.g., Technology, Energy, Healthcare, etc.) and a budget, and it will rank the top stocks that you can afford, considering their recent stock performance and sentiment analysis from news articles.

## Key Features

* Dynamic Stock Analysis: The tool fetches stock data for multiple sectors like Technology, Energy, Healthcare, etc.
* Sentiment Analysis: Uses NewsAPI to pull the latest news articles for each stock and analyze the sentiment using TextBlob.
* Performance Evaluation: The tool evaluates the 1-month performance of each stock using the historical data from Yahoo Finance.
* Weighted Ranking: Combines stock performance (70%) and sentiment analysis (30%) into a score that ranks the stocks.
* Customizable Budget: You can input your own budget, and the tool will calculate how many shares you can afford based on the current stock prices.
  
## How It Works

* Input: The user enters the sector they are interested in (e.g., Technology, Healthcare) and their available budget.
* Stock Data Fetching: The program fetches stock data using the yfinance API, which provides historical prices and stock details.
* Sentiment Analysis: For each stock, the tool retrieves recent news articles and analyzes the sentiment (positive or negative) using TextBlob.
* Stock Ranking: The stocks are ranked based on a weighted score combining their sentiment and performance over the last month.
* Results: The top stocks are displayed, showing the company name, stock ticker, price per share, number of shares you can buy, and the overall score
