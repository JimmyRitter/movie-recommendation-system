# Movie Recommendation System

## Objective
Create a movie recommendation system that suggests films based on user preferences, leveraging web scraping, data processing, and recommendation algorithms. This project will involve multiple stages, from data collection to algorithm implementation.

## Requirements

### 1. Web Scraping
- **Task:** Scrape movie data such as titles, genres, ratings and other useful information.
- **Tools:** Use `BeautifulSoup` or `Scrapy` to extract data from a website like IMDb or Rotten Tomatoes.
- **Deliverable:** A CSV file containing a clean dataset with relevant movie attributes. (This step is not mandatory. Use only to easily see the scraped data.)

### 2. Data Processing with Pandas
- **Task:** Clean and preprocess the scraped data.
- **Key Steps:** Handle missing values, remove duplicates, and standardize formats.
- **Deliverable:** A well-structured Pandas DataFrame ready for analysis.

### 3. Feature Engineering with Pandas and NumPy
- **Task:** Convert categorical data (like genres) into numerical features.
- **Steps:**
  - Apply one-hot encoding for categorical variables.
  - Create a content-based feature matrix.
- **Deliverable:** A matrix ready for similarity calculations.

### 4. Recommendation Algorithm
- **Task:** Implement a recommendation system using collaborative filtering or content-based filtering.
- **Steps:**
  - Use cosine similarity or another similarity measure for recommendation.
  - Implement the algorithm using Pandas and NumPy.
- **Deliverable:** A function or set of functions that generate movie recommendations based on user input.

### 5. Evaluation
- **Task:** Assess the **performance and quality** of the recommendation system using **qualitative methods** and **alternative metrics** suitable for **content-based filtering**.
- **Key Metrics:** Focus on **visual analysis**, **coverage**, and **diversity**, instead of traditional metrics like **MSE** or **MAE**, which require **user interaction data**.
- **Steps:**
  1. **Visual Analysis**:
     - Test recommendations for selected movies.
     - Verify whether suggested movies share logical similarities based on genres, ratings, and durations.

  2. **Coverage and Diversity Metrics**:
     - Measure the percentage of movies covered by recommendations.
     - Assess the system’s ability to recommend **diverse movies** across genres and attributes.

  3. **Serendipity Testing**:
     - Evaluate whether the system offers **unexpected yet relevant recommendations**.
     - Focus on **surprise factor** while maintaining relevance.

- **Deliverable:**
  - An **evaluation report** or notebook section summarizing:
    1. Observations from visual analysis and testing.
    2. Metrics for **coverage** and **diversity**.
    3. Challenges faced and suggestions for improvement.

## Instructions
1. Document your progress and methodology in a Jupyter notebook or a series of notebooks.
2. Include comments and markdown cells to explain your code and thought process.
3. At the end of the project, summarize your findings and any challenges you encountered.

---

## Evaluation Report
This can be found here [Evaluation Report](./evaluation-report.md)