# Website Traffic Analysis

## 📌 Project Overview

This project analyzes website traffic and user interaction data to understand website engagement, traffic patterns, landing page performance, and user behavior. It was completed during my Data Analytics Internship at Alfido Tech through InternSpark.

The objective was to clean the website event data, calculate key traffic and engagement metrics, visualize user behavior, and uncover insights that can help improve website engagement and conversion performance.

---

## 🎯 Problem Statement

The business wants to know:

- How much website traffic is generated?
- How many sessions and estimated users are recorded?
- How do users interact with the website through pageviews, previews, and clicks?
- Which landing pages receive the most traffic?
- Which pages may be causing user drop-off?
- What is the website's bounce rate and click-through rate?
- Which countries contribute the most website traffic?
- Where are the opportunities to improve user engagement and conversions?

---

## 📊 Dataset

A website traffic/event log dataset containing information about user interactions, dates, locations, artists, albums, tracks, and link identifiers.

**Dataset Size:** 226,278 rows × 9 columns

**Key columns:** event, date, country, city, artist, album, track, isrc, linkid

**Event Types:**
- Pageview
- Click
- Preview

**Note:** the dataset does not contain a unique user ID or timestamp information. Therefore, user count is estimated using unique link IDs, and true average session duration cannot be calculated accurately.

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- Jupyter Notebook

---

## 🔍 Analysis Performed

### 1. Data Loading & Exploration

- Loaded the website traffic dataset using Pandas
- Checked the dataset structure using `head()`, `info()`, `shape`, and `describe()`
- Examined data types, unique values, and basic statistics

### 2. Data Cleaning

- Checked for missing values
- Checked and removed duplicate records
- Converted the `date` column into datetime format
- Created `Year`, `Month`, `Day`, and `Weekday` columns
- Handled missing values in country, city, artist, album, and track fields
- Standardized text-based fields
- Verified event categories
- Checked `linkid` values

### 3. Event Analysis

Analyzed the distribution of:

- Pageviews
- Clicks
- Previews

### 4. Website Traffic Metrics

Calculated key website performance metrics:

- Estimated Sessions
- Estimated Users
- Bounce Rate
- Click-Through Rate (CTR)

Average Session Duration was not calculated because the dataset contains dates but does not provide start and end timestamps.

### 5. Exploratory Data Analysis & Visualization

Created visualizations for:

- User Flow Funnel
- Event Distribution
- Top 10 Entry Pages
- Top Exit Pages
- Daily Website Traffic Trend
- Top 10 Countries by Traffic

---

## 📈 Key Findings

**KPIs**

| KPI | Value |
|---|---:|
| Estimated Sessions | 3,839 |
| Estimated Users | 3,839 |
| Bounce Rate | 40.45% |
| Click-Through Rate (CTR) | 39.24% |

**Event Distribution**

| Event Type | Count |
|---|---:|
| Pageview | 142,015 |
| Click | 55,732 |
| Preview | 28,531 |

**Insights**

- **High Traffic but Moderate Engagement:** Pageviews make up the largest share of website activity, while a smaller proportion of visitors proceed to previews and clicks. This indicates opportunities to improve user engagement.

- **Bounce Rate:** The estimated bounce rate is **40.45%**, meaning a significant portion of landing pages received pageviews without further click or preview interactions.

- **Click-Through Rate:** The calculated CTR is **39.24%**, showing that a considerable portion of recorded pageviews resulted in a click action.

- **Landing Pages:** A small number of landing pages receive a disproportionately large share of website traffic. These high-performing entry pages should be prioritized for optimization.

- **Exit Pages:** Several pages receive pageviews but generate no click interactions, indicating possible user drop-off and opportunities to improve content, navigation, and calls-to-action.

- **International Reach:** Website traffic comes from more than 200 countries. Saudi Arabia, India, and the United States contribute some of the highest traffic volumes.

- **Traffic Trends:** Daily pageviews fluctuate across the observation period, indicating variations in visitor activity that can be used for campaign and content planning.

---

## 💡 Business Recommendations

- Optimize high-traffic landing pages by improving page design, content structure, loading speed, and call-to-action placement.
- Strengthen CTA elements with clear and compelling actions such as "Get Started", "Request a Demo", or "Contact Us".
- Analyze high-bounce pages and improve their content quality, navigation, and user experience.
- Target high-traffic countries such as Saudi Arabia, India, and the United States with region-specific content and marketing campaigns.
- Conduct A/B testing on headlines, CTA placement, page layouts, and promotional messages.
- Use daily traffic trends to plan content publishing and marketing campaigns around high-traffic periods.
- Monitor engagement metrics regularly to identify pages where users are dropping off.

---

## 📁 Files

- `Website_Traffic_Analysis.ipynb` – Complete analysis notebook
- `cleaned_website_traffic.csv` – Cleaned dataset generated during the analysis
- `traffic.csv` – Original dataset
- `README.md` – Project documentation

---

## 👩‍💻 Author

**Vaishnavi Tiwari**

B.Tech – Computer Science & Artificial Intelligence | Aspiring Data Analyst

- GitHub: [vaishnavitiwari1109](https://github.com/vaishnavitiwari1109)
