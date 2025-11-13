🎬 Netflix Reviews Dataset – Data Cleaning & EDA Project

Welcome to my project! This repository contains the complete process of cleaning and exploring a dataset of Netflix mobile app reviews collected from the Google Play Store.
The goal? To transform raw, messy data into something clean, structured, and insight-ready. 🚀

 About the Dataset

The dataset includes thousands of real user reviews about the Netflix app. Each row represents one review with details like rating, review text, app version, and timestamp.

Columns Included :
Column	Description
reviewId	Unique identifier for each review
userName	Name of the person who wrote the review
content	Actual text of the review
score	Rating (1–5 stars)
thumbsUpCount	Number of likes on the review
reviewCreatedVersion	App version used while reviewing
at	Time and date when the review was posted
appVersion	Version of the app installed on the device
 Data Cleaning Process (What I Did)
 1. Handled Missing Values

Very few missing entries in content (only 6!).

Around 17.3% missing values in app version fields — expected, because many users don't include version details.

All other columns are fully complete.

 2. Removed Duplicates

Checked across all columns.

 No duplicate rows found — nice and clean!

 3. Cleaned & Standardized Text

Converted user names to Title Case for consistency.

Removed unnecessary spaces from review text and version columns.

Replaced "nan" strings with real NaN values.

4. Fixed Data Types

Converted the at column into proper datetime format.

Ensured numeric columns (score, thumbsUpCount) remain integers.

 5. Standardized Column Names

Converted all column headings to UPPERCASE for a clean, uniform look.

📊 Exploratory Data Analysis (Insights)
 Rating Distribution

Highest counts: 1-star and 5-star reviews.

This shows users are either very happy or very frustrated  with the app.

 Thumbs-Up Activity

Most reviews have 0 likes → low engagement.

A few reviews have thousands of likes (max = 8032 ).

 Common Review Themes

Top words appearing in reviews:

“netflix”, “good”, “movies”, “shows”, “watch”, “not”

Users frequently talk about:

Content quality

Streaming experience

App performance issues

📈 Key Takeaways

* The dataset is mostly clean and well-structured
* User ratings are extremely polarized
* Review text is rich with sentiment and app experience insights
* Great dataset for NLP, sentiment analysis, or dashboard building

🛠 Tools & Libraries Used

Python 🐍

Pandas

