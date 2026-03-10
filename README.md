# Discord App Review Sentiment Analysis

**Name:** Sultan Alamsyah Lintang Mubarok
**Student ID (NRP):** 5026231188

## Project Overview

This project aims to collect and analyze user reviews of the **Discord mobile application** from the **Google Play Store**. The collected reviews are used as a dataset for sentiment analysis, which helps identify users' opinions, experiences, and overall satisfaction with the application.

The dataset is obtained through web scraping using the **Google Play Scraper** library in Python. The scraped reviews are then stored in a CSV file to be used for further analysis.

---

## Project Objectives

The main objectives of this project are:

* To collect user review data from the Google Play Store for the Discord application.
* To build a dataset of user feedback for sentiment analysis.
* To understand user sentiment toward the Discord mobile application.
* To prepare data that can be used for further natural language processing (NLP) tasks.

---

## Methodology

The project follows several main steps:

### 1. Data Collection

User reviews are collected from the Google Play Store using the **google-play-scraper** Python library. The target application in this project is:

**Application Name:** Discord
**Application ID:** `com.discord`

The scraper retrieves review information such as:

* Review content
* Rating score
* Number of likes on the review
* Application version
* Review timestamp

### 2. Data Processing

The scraped data is converted into a **Pandas DataFrame** to make it easier to process and analyze.

### 3. Data Cleaning

The dataset is filtered to keep only relevant attributes needed for analysis, including:

* `content` – the text of the review
* `score` – rating given by the user
* `thumbsUpCount` – number of likes on the review
* `reviewCreatedVersion` – version of the app used by the reviewer
* `at` – review timestamp
* `appVersion` – application version

### 4. Data Export

The processed data is exported into a **CSV file** which will be used as the dataset for further sentiment analysis tasks.

---

## Technologies Used

* **Python**
* **Google Play Scraper**
* **Pandas**
* **Google Colab / Jupyter Notebook**

---

## Output Dataset

The scraping process generates a dataset in CSV format:

```
Review_App_Discord.csv
```

This dataset contains thousands of Discord user reviews collected directly from the Google Play Store.

---





