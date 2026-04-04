# Yelp Hotel Reviews — Topic Modeling & Text Analytics

**Georgetown University MSBA | OPAN 6609: Text Analytics | Final Project**

**Team SAXA 3:** Mike Johnson, Kris Lederer, Sebastian Martinez, Ryan Mathis, Khushi Patel

---

## Overview

A hotel brand preparing to launch needs to understand what drives poor guest experiences. This project analyzes Yelp hotel reviews using NLP and topic modeling to surface the specific themes that unhappy customers write about, providing actionable intelligence for hotel operations and service design.

---

## Business Problem

> *You are leading a new branded hotel and you need to know what customers who give poor reviews of hotels tend to bring up. To minimize poor service, your analytics team will examine hotel reviews using topic modeling to identify what reviewers who give poor reviews actually write about in their experience — so your hotel focuses special attention on those domains.*

---

## Methodology

### 1. Exploratory Analysis
- Descriptive statistics on the review dataset
- Segmented reviews into **Positive** (4–5 stars), **Mixed** (3 stars), and **Negative** (1–2 stars) categories

### 2. N-Gram Analysis
- Extracted top unigrams and bigrams across all three sentiment segments
- Identified high-frequency language patterns distinguishing happy from unhappy reviewers

### 3. Latent Dirichlet Allocation (LDA) Topic Modeling
- Fit LDA models across three review subsets: all reviews, positive reviews, and negative reviews
- Identified 4 dominant topics per subset and assigned each review a dominant topic label

### 4. Behavioral Analysis
- Compared average review length between positive and negative reviewers
- Analyzed engagement (useful, cool, funny votes) across review sentiment categories

---

## Key Findings

### What unhappy customers write about (LDA Topics — Negative Reviews)

| Topic | Key Themes |
|---|---|
| 1 | Room service issues, small rooms, smoking |
| 2 | Room service, WiFi |
| 3 | Customer service, room cleanliness |
| 4 | Rooms not ready, maid service, bed size |

### What happy customers write about (LDA Topics — Positive Reviews)

| Topic | Key Themes |
|---|---|
| 1 | Great overall experience, great service |
| 2 | Room service, Bliss Spa, lake views |
| 3 | Location, staff, lobby bar, cleanliness |
| 4 | Good value, rooms, staff, location |

### Behavioral Insights
- **Unhappy reviewers write longer reviews** than happy reviewers
- **Positive reviews receive more engagement** (useful/cool/funny votes) from other users
- Happy and unhappy reviewers engage with the platform in meaningfully different ways

---

## Recommendations

**Short Term**
- Evaluate room service and cleaning operations — address bottlenecks and establish clear standards
- Establish customer service training standards
- Implement a strict no-smoking policy in rooms
- Implement a "Do Not Disturb" policy to reduce unwanted disturbances

**Long Term**
- Consider offering complimentary WiFi as a standard amenity
- Engage an interior designer to explore making rooms feel more spacious

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core programming language |
| pandas / numpy | Data manipulation |
| scikit-learn | `CountVectorizer`, `TfidfVectorizer`, `LatentDirichletAllocation` |
| matplotlib / seaborn | Data visualization |
| scipy | Statistical analysis |

---

## Repository Contents

| File | Description |
|---|---|
| `final_project.ipynb` | Full analysis notebook with code, visualizations, and commentary |
| `final_project_saxa3.html` | Rendered HTML export of the notebook |
| `Final Proj - Text Analytics final.pdf` | Slide deck presentation of findings |
| `hotel_final.csv` | Yelp hotel review dataset |

---

*README written with the assistance of [Claude Code](https://claude.ai/code) by Anthropic.*
