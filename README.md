# 🎧 Thmanyah Recommender System

This project was developed as part of the **Thmanyah Data and AI Assignment**.  
It analyzes podcast listening behavior and implements a content-based recommendation system using Python and pandas.

---

## 🎯 Project Objectives

- Load and clean podcast-related datasets (users, episodes, and listening logs)
- Analyze user engagement across categories, genders, and countries
- Visualize behavioral insights using graphs and statistics
- Build a simple recommendation function that suggests new episodes based on user preferences

---

## 📁 Files Included

| File Name                         | Description                                  |
|----------------------------------|----------------------------------------------|
| `thmanyah_recommender_project.ipynb` | Jupyter Notebook with all analysis and code |
| `users.csv`                      | User demographic information                 |
| `episodes.csv`                   | Podcast metadata (title, category)           |
| `listens.json`                   | Listening log (user_id, episode_id, duration)|
| `README.md`                      | Project summary and documentation            |

---

## ✅ Summary of Tasks Completed

### 1. Data Cleaning & Integration
- Removed all records with 0-second listening durations
- Merged the three datasets using `user_id` and `episode_id`

### 2. Data Analysis & Visualization
- Identified most popular podcast categories
- Analyzed listening behavior by gender
- Calculated the average number of episodes per user
- Measured engagement by country

### 3. Recommender System
- Implemented a function that recommends 3 new episodes to a user
- Recommendations are based on the user’s most listened-to category
- Episodes the user has already heard are excluded

---

## 📊 Questions from the Assignment — Answered

### 1. What are the most listened-to episode categories?

Estimated from the bar chart (*Top Episode Categories*):

| Category     | Approx. Count |
|--------------|---------------|
| Society      | 29            |
| Sports       | 28            |
| News         | 13            |
| Religion     | 9             |
| Politics     | 4             |
| Technology   | 4             |

> "Society" and "Sports" were the most frequently listened-to categories.

---

### 2. What is the difference in average listening time between males and females?

From the *Average Listening Duration by Gender* chart:

| Gender  | Avg Duration (seconds) |
|---------|------------------------|
| Male    | ~620                   |
| Female  | ~900                   |

> On average, **females listened longer than males** per session.

---

### 3. What is the average number of episodes a user listens to?

> Based on grouped counts of unique `episode_id` per `user_id`:

**📌 Average: `4.42 episodes/user`**

---

### 4. What additional analysis could help understand user behavior?

> An analysis of **total listening time by country** was added to identify the most engaged audiences by region.

Estimated total listening durations by country:

| Country        | Total Listening (seconds) |
|----------------|---------------------------|
| Jordan         | ~19,500                   |
| Morocco        | ~19,000                   |
| Saudi Arabia   | ~12,000                   |
| Egypt          | ~10,000                   |
| UAE            | ~6,000                    |

> This insight helps prioritize localization efforts and audience-specific strategies.

---

## ▶️ How to Run This Project

You can run the notebook in two ways:

### 🟢 Option 1: Google Colab (Recommended)

Open the notebook directly in Google Colab:  
👉 [Open in Google Colab](https://colab.research.google.com/drive/1FcRtHNy4gAWQ2hFmAkpo8iZw5HS6U5uL?usp=sharing)

### ⚙️ Option 2: Run Locally

1. Clone or download this repository
2. Open `thmanyah_recommender_project.ipynb` in Jupyter Notebook
3. Run all cells in order to load the data, generate insights, and test the recommender function

---

## 👤 Author

Made by **Yazan Alkamal**  
Submitted for the **Thmanyah Data & AI Internship Program** ✨
