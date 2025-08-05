# Student Social Media Addiction: An Exploratory Data Analysis

### An exploratory data analysis of how social media usage patterns correlate with the academic performance, sleep quality, and mental well-being of students.

---

## 📊 Project Overview

This project performs an in-depth Exploratory Data Analysis (EDA) on the "Students' Social Media Addiction" dataset. The primary goal is to uncover patterns, correlations, and insights into how different aspects of social media engagement affect students' lives. We investigate the relationships between daily usage hours, preferred platforms, and key life-quality indicators such as mental health scores, hours of sleep, academic performance, and interpersonal conflicts.

The analysis aims to answer questions like:
- Is there a correlation between the hours spent on social media and a student's mental health score?
- How does social media usage impact sleep patterns and academic performance?
- Do relationship statuses or gender play a role in social media addiction and its effects?
- What are the most common social media platforms among students in this dataset?

## 💾 Dataset

The data for this project was sourced from the [Students' Social Media Addiction dataset on Kaggle](https://www.kaggle.com/datasets/adilshamim8/social-media-addiction-vs-relationships).

The dataset contains the following features:
- **`Age`**: Age of the student.
- **`Gender`**: Gender of the student.
- **`Academic_Level`**: The current academic level (e.g., Undergraduate, Graduate).
- **`Country`**: The country of the student.
- **`Avg_Daily_Usage_Hours`**: Average hours spent on social media per day.
- **`Most_Used_Platform`**: The social media platform used most frequently.
- **`Affects_Academic_Performance`**: Self-reported impact on academics (Yes/No).
- **`Sleep_Hours_Per_Night`**: Average hours of sleep per night.
- **`Mental_Health_Score`**: A self-reported score from 1-10 indicating mental well-being.
- **`Relationship_Status`**: The student's relationship status (e.g., Single, In Relationship).
- **`Conflicts_Over_Social_Media`**: A score indicating the frequency of conflicts due to social media.
- **`Addicted_Score`**: A self-reported score from 1-10 indicating the level of addiction.

Two CSV files are included in this repository:
1.  `Students Social Media Addiction.csv`: The original, raw dataset.
2.  `studentsSocialMedia_cleaned.csv`: A cleaned and preprocessed version of the dataset used for the analysis.

## 📈 Analysis & Key Findings

The analysis was conducted in the `EDA-Project-1_Sushant.ipynb` Jupyter Notebook. Key findings from the exploration include:

* **Strong Negative Correlation between Usage and Well-being**: There is a clear negative correlation between the average daily hours spent on social media and students' mental health scores and hours of sleep. As usage increases, mental health and sleep tend to decline.
* **Impact on Academics**: Students who reported that social media affects their academic performance tend to have significantly higher daily usage hours.
* **Addiction Score Insights**: The `Addicted_Score` is strongly correlated with `Avg_Daily_Usage_Hours` and `Conflicts_Over_Social_Media`, indicating that higher usage is linked to a greater sense of addiction and more interpersonal friction.
* **Platform Popularity**: Instagram, TikTok, and Facebook were among the most used platforms by the students in this dataset.
* **Linear Relationships**: Many of the core relationships (e.g., usage vs. sleep) appear to be linear, suggesting that linear regression models could be effective for future predictive tasks.

## 🛠️ Technologies Used

This project was implemented using Python 3 and the following libraries:
- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical operations.
- **Matplotlib**: For creating static, foundational visualizations.
- **Seaborn**: For creating more advanced and aesthetically pleasing statistical visualizations.
- **Jupyter Notebook**: For interactive analysis and documentation.

## 🚀 How to Use

To replicate this analysis, please follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/Student-Social-Media-Analysis.git](https://github.com/your-username/Student-Social-Media-Analysis.git)
    cd Student-Social-Media-Analysis
    ```

2.  **Install the required libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn jupyterlab
    ```

3.  **Launch Jupyter Notebook:**
    ```bash
    jupyter lab
    ```

4.  **Open and run the notebook:**
    Open the `EDA-Project-1_Sushant.ipynb` file and run the cells sequentially to see the full analysis.

## 🔮 Conclusion & Future Work

This EDA successfully highlights the significant, and often negative, impact of high social media usage on a student's life, particularly concerning mental health, sleep, and academics.

Potential next steps for this project include:
* **Predictive Modeling**: Build a linear regression model to predict a student's `Mental_Health_Score` or `Addicted_Score` based on their usage patterns.
* **Statistical Testing**: Apply more rigorous statistical tests (e.g., Spearman's correlation for non-linear relationships, t-tests for group comparisons) to validate the observed correlations.
* **Addressing Bias**: Acknowledge and potentially develop methods to account for the self-report bias inherent in the survey data.
* **Advanced Modeling**: Explore non-linear models or clustering algorithms to identify distinct groups of users (e.g., "Casual Users," "Power Users," "At-Risk Users").
