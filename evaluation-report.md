# **Movie Recommendation System - Evaluation Report**

---

## **1. Project Overview**

### **Objective**
The primary goal of this project was to **learn and practice data analysis skills** by building a **content-based movie recommendation system**.

### **Scope**
- **Web Scraping**: Gather movie data from IMDB website.
- **Data Processing and Cleaning**: Handle **missing**, **inconsistent**, and **dirty records** to simulate **real-world data challenges**.
- **Feature Engineering**: Transform and encode features into **numerical values** for similarity calculations.
- **Evaluation Metrics**: Assess system performance through **coverage**, **diversity**, and **serendipity testing**.
- **Visual Analysis**: Use **plots** and **visuals** to understand data distributions and similarity patterns.

---

## **2. Data Preparation**

### **2.1 Web Scraping**
- **Approach**: Collected movie data (titles, genres, ratings, descriptions, and durations) and exported it as a **CSV file** for offline analysis.
- **Why CSV?**:
  - To be easier to see the scraped data.
  - Avoid repeated web scraping.
  - Enable offline experimentation without dependency on live data.

---

### **2.2 Data Cleaning and Transformation**
- **Simulated Dirty Data**: Added **missing values** and **errors** to replicate **real-world scenarios**.
- **Steps involved**:
  - Removed **duplicates** and **invalid records**.
  - Converted **duration strings** (e.g., "PT2H22M") to **numeric values** in minutes.
  - Replaced **HTML entities** (e.g., `&apos;`) with standard characters.

---

### **2.3 Feature Engineering**
- **Movie Classification**:
  - Mapped ratings (e.g., **PG-13**, **NC-17**) into **user-friendly categories** (e.g., **Family-Friendly**, **Adult-Only**)
  - Added new columns for these categories to enhance **interpretability**.

- **Numerical Encoding**:
  - Applied **one-hot encoding** for categorical variables like **genres** and **ratings**.
  - Prepared data for **similarity matrix calculations**.

---

## **3. Evaluation and Insights**

### **3.1 Visual Analysis**

#### **Similarity Bar Plot**
- **Purpose**: Visualize the **Top-N similar movies** for the selected title.
- **Findings**:
  - Inputting the movie name **Lord of the Rings: The Return of the King** displayed as the most similar movie **Lawrence of Arabia**, a movie that I have not watched yet, but after a quick Google search, I found they are similar in multiple aspects. Will definitely watch it soon!

#### **Distribution Analysis**
- **Movie Duration**:
  - Most movies are **between 90 and 150 minutes** long.

- **Genre Distribution**:
  - **Drama** is the most common genre with more than 70% of the titles, followed by **Adventure** and **Crime**.
  - Genres like **Musical** and **Film-Noir** are the fewest ones.

---

### **3.2 Coverage Metrics**

- **Definition**: Measures how much of the dataset is represented in recommendations.
- **Result**:
  - **Coverage: High** — Indicates a **broad spread** across movies.
  - **Key Insight**: Recommendations are **not biased** toward a **small subset**.

---

### **3.3 Diversity Metrics**

- **Definition**: Measures whether recommendations are **varied** or **repetitive**.
- **Result**:
  - **Diversity Score: 0.68**—Highly diverse.
  - **Key Insight**: Recommendations have broad **variety** across genres and styles.

---

### **3.4 Serendipity Testing**

- **Definition**: Evaluates whether recommendations include **unexpected but relevant movies** to promote **exploration**.
- **Method**: Used **Jaccard Similarity** to measure **genre overlaps** between movies.


| Movie      | Recommendation               | Jaccard Similarity |
|------------|------------------------------|--------------------|
| The Matrix | Dune: Part Two               | 0.25               |
| The Matrix | Die Hard                     | 0.33               |
| The Matrix | Inception                    | 0.66               |
| The Matrix | Terminator 2: Judgment Day   | 0.66               |

- **Key Observations**:
  - **Low Similarity Scores (e.g., Dune: Part Two)** encouraged **exploration**.
  - **High Similarity Scores (e.g., Inception)** provided **reliable matches**.
  - System balanced **novelty** and **similarity** well.

- **Why Serendipity Matters?**
  - **Avoids Predictability**: Prevents repetitive suggestions.
  - **Encourages Discovery**: Promotes exploring **different genres** and **styles**.
  - **Keeps Recommendations Engaging**: Balances **familiarity** with **new experiences**.

---

## **4. Possible Improvements**

1. **Additional Features**:
   - Add **release year**, **directors**, and **actors** for richer similarity metrics.

2. **Hybrid Approach**:
   - Combine **content-based filtering** with **user preferences** to enhance recommendations.

3. **Randomness for Diversity**:
   - Introduce **random suggestions** in low-similarity ranges to **boost diversity**.

---

## **5. Final Thoughts**

This project provided valuable hands-on experience with **data analysis** and **recommendation systems**.

- **Key Takeaway**:
  - Recommendations were **relevant** and **engaging**, balancing **similarity** and **novelty** effectively.

- **Future Enhancements**:
  - Incorporate **user preferences** to build a **hybrid system** that combines **data insights** with **user feedback**.

> **Personal Reflection**:
> As a movie fan, I enjoyed seeing recommendations for titles I already love and discovering **hidden gems** based on their features. This project was a great way to **explore new movies** and **learn new skills** simultaneously.

---

## **6. Deliverables Checklist**

✅ **README.md** - Provides an overview of the project and serves as a quick reference guide.

✅ **Jupyter Notebook** - Includes code for scraping, processing, modeling, and evaluation.

✅ **Evaluation Report** - Documents findings, challenges, and suggestions for improvements.


