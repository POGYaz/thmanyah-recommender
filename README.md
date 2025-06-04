# 🎧 Thmanyah Recommender System

This project was developed as part of the **Thmanyah Data and AI Assignment**.  
It analyzes podcast listening behavior and builds a content-based recommendation system using Python.

---

## 🎯 Project Objectives

- Load and clean user, episode, and listening log data
- Analyze user engagement across categories, genders, and countries
- Build a simple recommender function based on user preferences
- Visualize key trends and share recommendations

---

## 📁 Files Included

| File Name                         | Description                                 |
|----------------------------------|---------------------------------------------|
| `thmanyah_recommender_project.ipynb` | Jupyter Notebook with all analysis and code |
| `users.csv`                      | User demographic information                |
| `episodes.csv`                   | Podcast metadata (title, category)          |
| `listens.json`                   | Listening log (user_id, episode_id, duration) |
| `README.md`                      | This file — summary of the entire project   |

---

## ✅ Tasks Completed

1. **Data Cleaning & Merging**
   - Removed all sessions with 0-second durations
   - Merged all datasets on `user_id` and `episode_id`

2. **Behavior Analysis & Visualizations**
   - Top episode categories
   - Listening duration by gender
   - Episode count per user
   - Listening time by country

3. **Recommender System**
   - Function recommends 3 new episodes based on favorite category
   - Already-played episodes are excluded
   - Works with any user ID from the dataset

---

## 📊 Questions from the Assignment (and Answers)

### 1. **Which episode categories are listened to the most?**

Estimated from the bar chart titled *Top Episode Categories*:

| Category      | Approx. Count |
|---------------|----------------|
| Society      | 29            |
| Sports    | 28            |
| News       | 13            |
| Religion      | 9             |
| Politics       | 4             |
| Technology       | 4             |

These categories had the highest listening frequency in the dataset.

---

### 2. **What is the difference in average listening time between males and females?**

From the *Average Listening Duration by Gender* bar chart:

| Gender  | Avg Duration (seconds) |
|---------|------------------------|
| Male    | ~620                   |
| Female  | ~900                   |

Males had slightly longer average listening durations than females.

---

### 3. **What is the average number of episodes a user listens to?**

The average number of unique episodes per user is:  
**`4.42 episodes/user`**

---

### 4. **What is one additional useful analysis for understanding user behavior? Why?**

> I added an analysis of **total listening time by country**.

Estimated Top Countries by Engagement:

| Country         | Total Listening (seconds) |
|------------------|---------------------------|
| Jordan     | ~19,500                   |
| Morocco           | ~19,000                    |
| Saudi Arabia            | ~12,000                    |
| Egypt          | ~10,000                    |
| UAE          | ~6,000                    |

This shows where the most active listeners are and helps the team localize or prioritize based on region.

---

## ▶️ How to Run This Project

1. Clone this repository or download the ZIP
2. Open the notebook in Jupyter or Google Colab
3. Run all cells top to bottom
4. Test the recommender function by calling `recommend_episodes(user_id)`

---

## 👤 Author

Made by **Yazan Alkamal**  
Submitted for the **Thmanyah Data & AI Internship Program**

