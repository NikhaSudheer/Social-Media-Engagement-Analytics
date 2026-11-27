PROJECT DOCUMENTATION -- Social_Media_Engagement_Analytics

PROJECT OVERVIEW

This project analyzes 5,000 social media posts using Python to understand how likes, comments, shares, impressions and watch time vary across post types, categories, countries, devices and user groups, helping identify which content and audiences perform best.

TOOLS USED

1.Python

2.NumPy

3.Pandas

4.Matplotlib

5.Seaborn

6.Plotly

DATASET

Source: social_media_engagement_5000.csv 

Data contains: User ID, Age, Gender, Country, Post ID, Post type,Likes, Comments, Shares, Watch time, Posted date,Follower count,Device type,Engagement rate etc.

STEPS FOLLOWED

1.Imported the CSV with Pandas, checked data types and converted posted_at to datetime

2.Used NumPy arrays for basic array operations

3.Cleaned the data: detected missing values, filled them with the median (numeric) or mode (categorical), demonstrated forward/backward fill, removed duplicates, 
fixed data types, standardized gender labels, corrected unrealistic likes, comments and shares, and extracted hashtag count

4.Explored the data with head(), tail(), info(), describe(), value counts, correlation and groupby()

5.Created new fields (engagement_score, hashtag_count) and group summaries by post type, country and sentiment

6.Calculated mean, median, mode, standard deviation, variance and percentiles

7.Built 12 Matplotlib and Seaborn plots and 4 interactive Plotly charts

8.Final insights and wrote a one-page summary

KEY INSIGHTS

Highest engagement by post type: Reels have the highest average engagement score (about 11,986 likes + comments + shares per post), followed by images (11,975), videos (11,905) and text (11,903). The four types are within 1% of each other. By engagement rate, video is highest (0.454) and reel lowest (0.417).

Best content category: Music has the highest average engagement score (about 12,132); fashion is lowest (11,749). By engagement rate, fitness is highest (0.463).

Country with the highest average engagement rate: Australia (0.492), then UAE (0.469) and Japan (0.460). India is lowest (0.397).

Age: the correlation between age and engagement is close to zero (about -0.03). Users under 50 average about 12,040 to 12,130 engagement score; users aged 50 and over average about 11,580, roughly 4% lower. Engagement rate barely changes across age groups (0.434 to 0.447).

Verified accounts: verified accounts do not perform better. They average 11,518 engagement score against 11,988 for non-verified accounts (about 4% lower) and a rate of 0.420 against 0.441. Verified posts are only 483 of 5,000, so this is a small group.

FILES INCLUDED

1.Social_Media_Engagement_Analytics.ipynb — Python notebook with the code, outputs, charts, final insights and one-page summary

2.README.md — Project description

