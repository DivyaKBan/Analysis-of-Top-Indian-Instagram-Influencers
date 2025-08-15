# Analysis of Top Indian Instagram Influencers

### Project Overview

This project performs an in-depth exploratory data analysis (EDA) on a dataset of the top 100 Instagram influencers in India. The primary goal is to uncover trends related to follower counts, engagement rates, and the most popular topics of influence to derive actionable insights for marketing strategies.

---

### Key Questions Answered

The analysis aims to answer the following questions:
* Who are the dominant influencers in the Indian market?
* What is the distribution of followers and engagement rates?
* Which influencer categories are the most common?
* Is there a relationship between an influencer's follower count and their engagement rate?
* Which influencer tiers (Micro, Macro, Mega) drive the highest engagement?

---

### Dataset

* **Source:** The dataset used is `instagram_data_india.csv`, containing a snapshot of the top 100 Indian Instagram influencers.
* **Key Columns:** `Name`, `Followers`, `ER` (Engagement Rate), `Topic of Influence`, `Potential Reach`.

---

### Analysis Workflow

1.  **Data Cleaning & Preparation:**
    * Loaded the dataset using Pandas.
    * Converted `Followers`, `Potential Reach`, and `ER` columns from string to numerical formats, handling suffixes like 'M' and '%'.
    * Cleaned and standardized the `Name` and `Topic of influence` columns.
    * Corrected data entry inconsistencies.

2.  **Feature Engineering:**
    * Created an `Influencer Tier` column (`Micro`, `Macro`, `Mega`) based on follower counts to enable deeper engagement analysis.

3.  **Exploratory Data Analysis (EDA) & Visualization:**
    * Analyzed the distribution of key metrics and visualized the relationships between variables using Matplotlib and Seaborn.

---

### Key Findings & Visualizations

#### 1. Follower Count Does Not Equal Higher Engagement
The analysis reveals a clear negative correlation **(-0.17)** between follower count and engagement rate. As an influencer's audience grows, the average engagement rate tends to decline.


![Follower vs Engagement Rate]

<img width="779" height="658" alt="Screenshot 2025-08-16 004434" src="https://github.com/user-attachments/assets/ae33e8cd-555b-4458-9b25-152cc76b89f0" />

#### 2. Micro-Influencers Drive the Highest Engagement
By categorizing influencers into tiers, it's evident that Mega-influencers have the lowest average engagement rate, while Micro-influencers have the highest. This suggests that smaller, niche audiences are often more interactive and dedicated.

![ER by Tier]

<img width="860" height="681" alt="Screenshot 2025-08-16 004504" src="https://github.com/user-attachments/assets/6fb6e5fc-a4a8-47c0-ae80-3bdbd79fcc90" />

#### 3. Entertainment and Acting are Dominant Topics
The Word Cloud shows that the Indian influencer landscape is heavily dominated by figures from the **Entertainment, Music, and Acting** industries. This highlights the strong influence of the film and music industry on social media.

![Topic Word Cloud]

<img width="1183" height="630" alt="Screenshot 2025-08-16 004526" src="https://github.com/user-attachments/assets/4371f0dd-a01f-42b2-b69d-b98b7e88af47" />
---


### Conclusion & Recommendations

This analysis provides several key takeaways:
* **Popularity vs. Engagement:** The most popular influencers are not necessarily the most engaging.
* **Industry Dominance:** The entertainment sector dominates the list of top influencers.
* **Niche Power:** Smaller, niche communities often lead to higher average engagement rates.

**Recommendations:**
* For a brand campaign focused on **maximum brand awareness**, partnering with a **Mega-influencer** is the most effective strategy due to their vast reach.
* For campaigns where the goal is **high user interaction and shares**, the data suggests that a strategy involving several **Micro-influencers** would yield a better return on investment and a more genuinely engaged audience.

---

### Tools and Libraries Used

* **Python**
* **Pandas:** For data manipulation and cleaning.
* **NumPy:** For numerical operations.
* **Matplotlib & Seaborn:** For data visualization.
* **WordCloud:** For topic visualization.
* **Jupyter Notebook:** As the development environment.

---

### How to Run This Project

1.  Clone the repository:
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  Install the required libraries:
    ```bash
    pip install pandas numpy seaborn matplotlib wordcloud jupyter
    ```
3.  Open and run the `pyth.ipynb` notebook in Jupyter Notebook or JupyterLab.
