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

This section examines how food trends emerge, peak, and decline over time using YouTube upload activtity and view counts.

![Weekly YouTube Uploads](Analysis_Plots/trend_plots.png)

</details>

---

<details id="geographic-diffusion">
<summary><strong>Geographic Diffusion of Trends</strong></summary>

Includes choropleth maps showing regional spread for:
- **Matcha** (global cultural adoption)  
- **Dubai Chocolate** (localized influencer-driven trend)  
- **Air Fryer** (utility-driven global adoption)  
- **Feta Pasta** (viral-burst trend originating in the U.S.)  

This section addresses:  
📌 *Where do trends originate? How do they travel across countries? Why do some remain local while others become global?*

</details>

---

<details id="sentiment-analysis">
<summary><strong>Sentiment Analysis</strong></summary>

Includes:
- VADER sentiment scoring  
- Distribution plots of positive/neutral/negative posts  
- Rolling sentiment over time  
- Comparisons across trends  

Key insights:
- **Matcha** → consistently positive, steady cultural integration  
- **Feta Pasta** → spike + rapid decline in sentiment after viral moment  
- **Dubai Chocolate** → rising sentiment due to growing novelty  
- **Air Fryer** → stable and neutral (utility-driven)  

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

---

<details id="cross-platform-comparison">
<summary><strong>Cross-Platform Comparative Analysis</strong></summary>

Includes synchronized weekly activity across:
- **Google Trends** (search interest)  
- **YouTube** (content creation + views)  
- **Reddit** (discussion + sentiment)  

Key conclusion:  
📌 Trends typically follow the sequence — **Search → Creation → Community Discussion**  

Examples:
- Dubai Chocolate: Search interest → YouTube uploads → Reddit conversations  
- Feta Pasta: Sharp synchronized viral spike across all platforms  
- Matcha + Air Fryer: Long-term slow growth across ecosystems  

This section ties everything together.

</details>

