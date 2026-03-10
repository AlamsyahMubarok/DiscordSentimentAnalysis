# Discord App Review Sentiment Analysis

**Name:** Sultan Alamsyah Lintang Mubarok
---
**NRP:** 5026231188
---


## 1. Project Overview

This project focuses on collecting and preparing user review data from the **Discord mobile application** available on the **Google Play Store**. The dataset collected in this project will be used for **sentiment analysis and Natural Language Processing (NLP)**.

User reviews provide valuable insights into user satisfaction, complaints, and suggestions regarding the application. By collecting and analyzing these reviews, we can better understand how users perceive the performance and quality of the Discord application.

The data collection process is conducted using **web scraping techniques** through the Python library **google-play-scraper**.

---

## 2. Project Objectives

The objectives of this project are:

1. To collect user review data from the Google Play Store.
2. To build a dataset of Discord application reviews.
3. To prepare the dataset for sentiment analysis.
4. To analyze user feedback related to the Discord mobile application.

---

## 3. Target Application

| Application | Platform          | Application ID |
| ----------- | ----------------- | -------------- |
| Discord     | Google Play Store | `com.discord`  |

Google Play Store link:
https://play.google.com/store/apps/details?id=com.discord

---

## 4. Methodology

The methodology of this project consists of several stages.

### 4.1 Data Collection

User reviews are collected from the Google Play Store using the **google-play-scraper** Python library.

The scraping process collects review information such as:

* Review content
* Rating score
* Number of likes on the review
* Application version
* Review timestamp

The collected data represents user feedback about the Discord mobile application.

---

### 4.2 Data Processing

The scraped data is converted into a **Pandas DataFrame** to facilitate data processing and manipulation.

This step helps transform raw data into a structured dataset suitable for analysis.

---

### 4.3 Data Cleaning

Only relevant attributes are selected to ensure the dataset remains concise and useful for analysis.

The selected columns include:

| Column               | Description                                     |
| -------------------- | ----------------------------------------------- |
| content              | User review text                                |
| score                | Rating score given by the user                  |
| thumbsUpCount        | Number of likes received by the review          |
| reviewCreatedVersion | Version of the application used by the reviewer |
| at                   | Timestamp when the review was created           |
| appVersion           | Version of the application                      |

---

### 4.4 Data Export

After processing and cleaning, the dataset is exported into a **CSV file**.

```
Review_App_Discord.csv
```

This dataset will be used for further sentiment analysis.

---

## 5. Project Workflow

```
Google Play Store
        │
        ▼
Web Scraping (google-play-scraper)
        │
        ▼
Raw Review Data
        │
        ▼
Data Processing (Pandas)
        │
        ▼
Data Cleaning
        │
        ▼
CSV Dataset
        │
        ▼
Sentiment Analysis
```

---

## 6. Technologies Used

The technologies used in this project include:

* Python
* Google Play Scraper
* Pandas
* Jupyter Notebook / Google Colab

---

## 7. Dataset Output

The scraping process generates a dataset in CSV format:

```
Review_App_Discord.csv
```

The dataset contains thousands of user reviews collected from the Google Play Store and will be used for sentiment analysis.

---

## 8. Project Structure

```
discord-sentiment-analysis
│
├── notebook
│   └── scraping_discord_reviews.ipynb
│
├── dataset
│   └── Review_App_Discord.csv
│
├── README.md
│
└── requirements.txt
```

---

## 9. Notes

The data collected in this project is sourced from publicly available user reviews on the Google Play Store and is intended solely for **educational and research purposes**.
