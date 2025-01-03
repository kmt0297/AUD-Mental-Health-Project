# Analytics with Unstructured Data: Mental Health Project

## Project Guidelines
- **What is the problem statement? What are you trying to show or study?**  
- **Why is the problem important/interesting?**  
- **What is (are) the data source(s)?**  
  - Avoid Facebook & LinkedIn (too risky to scrape)  
  - X API not free anymore (so forget tweets)  
- **How much data is available?**  
  - Sometimes not enough data is available  
- **What type of analysis will be conducted?**  
- **What could be possible results?**  
- **"Aha" moments (aka "moments of truth")?**  

My team and I chose to scrape mental health subreddits.

---

## Project Overview: Unmasking Emotions  
### Sentiment and Trends in Mental Health Forums  

This project explores how unstructured data from Reddit can help identify and analyze trends in mental health discussions, with a focus on sentiment and potential crisis identification. By scraping data from mental health subreddits, we aimed to uncover insights that could guide mental health interventions and resource allocation.

---

## Problem Statement and Goal
The primary issue addressed was the lack of proactive measures and monitoring for mental health crises on forums. With reactive interventions being the norm, our goal was to:  
- Develop analytical tools for early detection of crises.  
- Analyze sentiment trends to identify critical patterns.  
- Explore ways to prioritize posts requiring immediate attention.  

---

## Methods
### Data Collection:
- Scraped data from subreddits like **r/need_support** and **r/suicidewatch**.  
- Filtered posts by flair ("Need Support") and time, removing duplicates.  
- Converted timestamps into human-readable formats for analysis.  

### Analytics:
- **Sentiment Analysis**: Measured sentiment polarity of posts to gauge emotional tone. Median sentiment scores showed **r/suicidewatch** was consistently more negative than **r/need_support**.  
- **Topic Modeling**: Identified family, job, and social/loneliness issues as recurring themes.  
- **Day-of-Week Trends**: Examined fluctuations in post frequency and sentiment across the week.  

### Crisis Classification:
- Used logistic regression to predict posts needing professional attention, treating **r/suicidewatch** posts as a positive class.  

---

## Findings
### Sentiment Trends:
- Posts on **r/suicidewatch** had consistently negative sentiment, signaling the need for immediate attention.  
- Sentiment for **r/need_support** fluctuated, with peaks on Monday and Thursday.  

### Thematic Insights:
- Family issues were consistent, while job and loneliness topics varied more.  
- Day-of-week trends revealed potential opportunities for targeted interventions.  

### Crisis Detection:
- While the model showed potential, the false-negative rate highlighted areas for improvement.  
