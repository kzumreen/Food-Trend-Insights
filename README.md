# Food-Trend-Insights
This is university capstone project exploring the lifecycle of digital food trends across YouTube, Reddit, and Google Trends. We focus on clear visual storytelling and this repo offers a polished summary of our core findings, key figures, and concise explanations.

**Authors:** Kadeeja Zumreen · Sriya Kondury · Sayalee Chivate  

---

## Table of Contents
- [Overview](#overview)
- [Data Sources](#data-sources)
- [Trend Lifecycle Analysis](#trend-lifecycle-analysis)
- [Geographic Diffusion](#geographic-diffusion)
- [Sentiment Analysis](#sentiment-analysis)
- [Topic Modeling (LDA)](#topic-modeling-lda)
- [Cross-Platform Comparison](#cross-platform-comparison)

---

<details id="overview">
<summary><strong>Overview</strong></summary>
  
Digital food trends increasingly emerge, spread, and decline through online platforms, shaping consumer behavior, cultural adoption, and global food discourse. Unlike traditional food movements, modern trends often follow nonlinear lifecycles driven by search behavior, content creation, influencer activity, and community discussion across social media ecosystems.

This project analyzes the lifecycle of four digital food trends — **Matcha**, **Baked Feta Pasta**, **Dubai Chocolate**, and **Air Fryer** — from 2015 to 2025 using data from **Google Trends**, **YouTube**, and **Reddit**. By examining temporal patterns, geographic diffusion, sentiment dynamics, and discussion themes, we investigate how trends originate, how quickly they scale, and whether they fade as short-lived viral phenomena or persist through long-term cultural and practical adoption.

Through a cross-platform, data-driven approach, this repository presents clear visual narratives that highlight distinct diffusion models, differences between viral and sustained trends, and the role of public curiosity, media amplification, and community engagement in shaping digital food lifecycles.

</details>

---

<details id="data-sources">
<summary><strong>Data Sources</strong></summary>

### YouTube Data  
Collected using YouTube Data API v3. Includes:
- Video metadata (titles, descriptions, duration)  
- Engagement metrics (views, likes, comments)  
- Upload timelines  

### Google Trends  
Collected via PyTrends. Includes:
- Weekly search interest (0–100 scale)  
- Global and country-level data (US, India, UAE, South Korea)  
- Region-by-region comparison for each trend

### Reddit Data  
Collected using PRAW. Includes:
- Post titles, scores, comments, timestamps  
- Subreddit distribution  
- Sentiment + topic modeling inputs  

</details>

---

<details id="trend-lifecycle-analysis">
<summary><strong>Trend Lifecycle & Temporal Patterns</strong></summary>

This section examines how food trends evolve over time by comparing public curiosity, creator adoption, and audience attention. Together, these signals distinguish short lived viral trends from those that achieve sustained cultural or practical relevance. 

### Public Interest Over Time
![Google Search Interest Over Time](Analysis_Plots/pytrends_searchInterest.png)
*Google Trends search interest (0-100) showing when public curiosity emerges, peaks, and declines for each trend.*

### Content Creation Dynamics
![Weekly YouTube Uploads](Analysis_Plots/trend_plots.png)
*Weekly YouTube video uploads highlighting differences between rapid viral adoption and gradual, sustained content growth.*

### Audience Attention and Reach
![Weekly Total Views per Trend](Analysis_Plots/trend_plots2.png)
*Weekly total YouTube views showing how audience attention scales and concentrates across different trend lifecycles.*

### Trend Lifecycle
![Trend Lifecycle Spiral](Analysis_Plots/trend_plots2.png)
*Spiral visualization summarizing the pace and duration of each trend's lifecycle, contrasting viral bursts with long term adoption*

</details>

---

<details id="geographic-diffusion">
<summary><strong>Geographic Diffusion of Trends</strong></summary>

We explored how digital food trends spread geographically and how adoption varies across regions. Using Google Trends data, we map relative search interest to identify each trend's regional concentration and degree of global diffusion.

### Regional Interest by Trend
![Matcha Geographic Diffusion](Analysis_Plots/Matcha%20Map.jpg)
*Geographic distribution of search interest for Matcha, showing widespread and sustained global adoption.*

![Dubai Chocolate Geographic Diffusion](Analysis_Plots/Dubai%20Chocolate%20Map.jpg)
*Search interest for Dubai Chocolate, highlighting strong regional concentration centered around its point of origin.*

![Baked Feta Pasta Geographic Diffusion](Analysis_Plots/Baked%20Feta%20Cheese%20Map.jpg)
*Geographic diffusion of Baked Feta Pasta, illustrating a short-lived viral spread with limited long-term regional adoption.*

![Air Fryer Geographic Diffusion](Analysis_Plots/Air%20Fryer%20Map.jpg)
*Regional adoption of Air Fryer searches, reflecting broad and sustained interest consistent with utility-driven diffusion.*

</details>

---

<details id="sentiment-analysis">
<summary><strong>Sentiment Analysis</strong></summary>

We used the VADER (Valence Aware Dictionary and Sentiment Reasoner) lexicon to analyze the tone of Reddit discussions. This allowed us to classify trends as long-term or short-lived based on whether community sentiment remained positive and diverse over time.

![Sentiment Distribution](Analysis_Plots/sentiment)
*This plot illustrates the VADER sentiment scores for each trend. You can see the high positive spikes for Baked Feta Pasta during its viral peak compared to the steady, neutral-to-positive sentiment for the Air Fryer.*

</details>

---

<details id="topic-modeling-lda">
<summary><strong>Topic Modeling (LDA)</strong></summary>

Includes:
- CountVectorizer preprocessing  
- LDA model (K=5 selected for interpretability)  
- Topic-word tables  
- Topic distribution across trends  

What this section reveals:
- What people **talk about most** for each trend  
- Whether discussions focus on recipes, purchasing, health, culture, etc.  
- How conversation themes evolve as trends grow or fade  

</details>


