# Ashluxe Twitter Sentiment Analysis Using Twitter API V2

A data science project using the **Twitter API v2** to analyze sentiment around the **Ashluxe** fashion brand on Twitter, focusing on public opinion in Nigeria. This project provides insights into consumer perceptions, applying **Natural Language Processing (NLP)** to classify sentiment and visualize the distribution of opinions.

## Project Overview
This project uses **Twitter API v2** to retrieve recent tweets mentioning Ashluxe, classify them based on sentiment, and gain insight into the general perception of Ashluxe in the Nigerian fashion market. It explores the new capabilities of Twitter’s API while producing actionable insights for brand sentiment analysis.

## Video Demo
https://github.com/user-attachments/assets/171a5cd8-341d-4458-9caf-e6ea049fe845

## Features
- Real-time tweet retrieval using **Twitter API v2**
- Sentiment classification using **TextBlob** with categories: Positive, Neutral, Negative
- Sentiment percentage calculations and visualization
- Insightful metrics for brand sentiment analysis and market research


## Getting Twitter (X) API Keys

To run this project, you'll need access to Twitter’s API (X API). Follow these steps to create a developer account, set up a project, and obtain your API keys.

### 1. Create a Twitter Developer Account
   - Go to the [Twitter Developer Platform](https://developer.twitter.com/).
   - Click on **Sign Up** to create a Twitter Developer account (you’ll need a regular Twitter account to sign up).
   - Complete the sign-up form and agree to Twitter's terms and conditions.

### 2. Apply for Elevated Access
   - In the Developer Portal, create a new project by going to **Projects & Apps > Overview** and selecting **Create Project**.
   - Choose a project name, description, and intended use case for the API.
   - **Note**: Basic access gives you limited API functionality. To use more features like full search functionality, consider applying for **Elevated Access** if required.

### 3. Obtain API Keys and Access Tokens
   - Once your project is created, go to **Projects & Apps > Overview** and click on **+ Add App** under your project.
   - After creating your app, navigate to the **Keys and Tokens** tab.
   - Generate and save the following credentials:
     - **API Key**
     - **API Key Secret**
     - **Bearer Token**
     - **Access Token and Access Token Secret**

### 4. Secure Your Credentials
   - Treat these keys like passwords. Avoid sharing or exposing them publicly.

## Data Collection
Tweets were gathered with the following parameters:
- **Keyword**: "Ashluxe" and related terms
- **Location**: Nigeria (using relevant keywords to infer geographic location)
- **Language**: English
- **Filters**: Excluding retweets to focus on original opinions

The **Twitter API v2** was used to streamline data retrieval, with rate limit handling to ensure uninterrupted collection.

## Sentiment Analysis
Sentiment analysis was performed using **TextBlob**, a Python library that calculates the sentiment polarity of each tweet. Tweets were classified as:
- **Positive**: Sentiment score > 0
- **Negative**: Sentiment score < 0
- **Neutral**: Sentiment score = 0

## Results
The sentiment distribution revealed:
- **Neutral Sentiment**: 36.36% of tweets were neutral, suggesting balanced opinions.
- **Positive Sentiment**: 54.54% of tweets showed a positive sentiment, reflecting customer satisfaction.
- **Negative Sentiment**: 9.09% of tweets were negative, highlighting areas for potential improvement.

## Impact
These insights are valuable for:
- **Marketing Strategy**: Tailoring promotions and engagements based on positive sentiment drivers
- **Product Development**: Identifying areas needing improvement from negative feedback
- **Brand Monitoring**: Regular tracking of brand perception to adjust to evolving customer expectations

This project also serves as a case study for the effectiveness of **Twitter API v2** in sentiment analysis and brand management.

## Technologies Used
- **Python**: Programming language
- **Tweepy**: For connecting to the Twitter API
- **TextBlob**: For sentiment analysis
- **Pandas**: Data manipulation
- **Matplotlib**: Visualization of sentiment distribution

## Getting Started
1. **Clone the repository**:
   ```bash
   git clone https://github.com/tobibiggest/ashluxe-twitter-sentiment-analysis-using-twitter-api.git
   ```
2. **Install dependencies**:
   ```bash
   pip install tweepy textblob pandas matplotlib
   ```
3. **Configure Twitter API**: 
   - Create a **Twitter Developer account**.
   - Set up API credentials and add them to your script.

4. **Run the analysis**:
   - Use the provided code to fetch tweets, analyze sentiment, and visualize results.
