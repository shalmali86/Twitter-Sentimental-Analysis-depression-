# **MDD Analysis from Tweets**

This project analyzes tweets to identify patterns and relationships between user behavior and the likelihood of Major Depressive Disorder (MDD). It uses natural language processing, statistical techniques, and data visualization to uncover insights from textual data.

---

## **Features**

1. **Text Preprocessing:**
   - Splits tweet content into individual words using specific delimiters.
   - Identifies and counts frequently used words.

2. **Analysis of Tweet Content:**
   - Analyzes the frequency of the word "Depression" in tweets.
   - Evaluates the relationship between mentioning "Depression" and MDD diagnosis using a Chi-square test.

3. **Statistical Insights:**
   - Computes risk ratios (RR) to quantify the likelihood of MDD among users tweeting "Depression."
   - Provides a 95% confidence interval for the risk ratio to assess statistical significance.

4. **Data Visualization:**
   - Visualizes MDD-related trends across weekdays using stacked bar charts.
   - Displays a heatmap comparing MDD likelihood between users who tweeted "Depression" and those who did not.

---

## **Technologies Used**

- **Python Libraries:**
  - **Pandas**: For data manipulation and preprocessing.
  - **NumPy**: For numerical computations and statistical calculations.
  - **Seaborn & Matplotlib**: For data visualization (heatmaps, bar charts).
  - **Scipy**: For statistical analysis (Chi-square test).
- **Jupyter Notebook** (Optional): For interactive data exploration.

---

## **How to Use**

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/mdd-tweets-analysis.git
   cd mdd-tweets-analysis
   ```

2. **Install Dependencies:**
   Ensure you have Python 3.7+ installed. Then, install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy
   ```

3. **Run the Program:**
   - Load your dataset (e.g., a CSV file containing tweet data).
   - Run the script in your Python environment or Jupyter Notebook.

4. **Expected Input:**
   - A dataset with columns:
     - `post_text`: The tweet content.
     - `MDD`: A binary column indicating MDD status (1 for positive, 0 for negative).

5. **Output:**
   - Stacked bar charts for MDD trends across weekdays.
   - A heatmap comparing MDD risk between "Depression" tweeters and non-tweeters.
   - Statistical insights, including risk ratio and confidence interval.

---

## **Example Workflow**

1. **Preprocessing and Word Analysis:**
   - Splits tweets into words.
   - Counts frequently used words, filtering for meaningful ones (≥3 characters).

2. **Weekly MDD Trends:**
   - Groups tweets by weekdays and calculates proportions of MDD-related tweets.
   - Visualizes trends using a stacked bar chart.

3. **Heatmap and Risk Analysis:**
   - Compares MDD status between users who tweeted "Depression" and those who did not.
   - Visualizes the relationship with a heatmap.
   - Calculates and interprets the risk ratio and its confidence interval.

---

## **Statistical Insights**

- **Risk Ratio:** Users tweeting the word "Depression" are approximately 2 times more likely to have MDD compared to those who do not.
- **Confidence Interval:** The risk ratio's 95% confidence interval is provided to assess the reliability of this observation.

---

## **Customization**

- Modify the word of interest (`Depression`) in the analysis for alternative keywords.
- Adjust data visualization styles by changing the Seaborn or Matplotlib parameters.

---

## **Future Enhancements**

- Incorporate advanced NLP techniques (e.g., sentiment analysis, topic modeling).
- Add support for multilingual tweet analysis.
- Explore temporal patterns (hourly, seasonal trends) for more granular insights.

---

## **License**

This project is licensed under the [MIT License](LICENSE).

---

## **Contributing**

Contributions are welcome! Feel free to submit a pull request or open an issue for any suggestions or improvements.

---

## **Acknowledgments**

Special thanks to the open-source community for the tools and libraries that made this analysis possible.
