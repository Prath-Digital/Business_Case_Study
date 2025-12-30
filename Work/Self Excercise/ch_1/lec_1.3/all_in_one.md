# Statistics Basics: Questions & Answers

Friendly explanations of key concepts in descriptive and inferential statistics  
(Prepared on December 30, 2025)

---

## Q1. What is a Gaussian (Normal) Distribution in statistics?

A **Gaussian** or **Normal distribution** is a continuous probability distribution that is symmetric and bell-shaped.  
It is completely defined by two parameters:

- **Mean (μ)** – the center of the distribution
- **Standard deviation (σ)** – the spread or width of the curve

Many natural phenomena (heights, test scores, measurement errors, etc.) tend to follow this distribution.

---

## Q2. What are the key characteristics of a normal distribution curve?

- **Symmetric** around the mean (left and right halves are mirror images)
- **Bell-shaped** and unimodal (one peak)
- **Mean = Median = Mode**
- **Defined by mean (μ) and standard deviation (σ)**
- **68-95-99.7 rule** (Empirical Rule):
  - ~68% of data within **±1σ**
  - ~95% within **±2σ**
  - ~99.7% within **±3σ**
- Asymptotic tails (never touches the x-axis but approaches it)
- Total area under the curve = 1 (probability)

---

## Q3. Why is the normal distribution important in data analysis and machine learning?

It’s important because:

- Many real-world variables are approximately normal (or can be transformed to be)
- **Central Limit Theorem**: Sample means from large samples tend to be normally distributed, regardless of the original population
- Many statistical tests (t-test, ANOVA, linear regression, etc.) assume normality
- Simplifies modeling in machine learning (e.g., Gaussian Naive Bayes, z-scores, standardization)
- Enables powerful tools like confidence intervals and hypothesis testing

---

## Q4. What is a percentile, and how is it used in data interpretation?

A **percentile** tells you the relative standing of a value within a dataset.  
The **P**-th percentile is a value below which **P%** of the observations fall.

Examples:

- 25th percentile = 25% of data is below this value
- 90th percentile = you’re in the top 10%

Used for: comparing scores (e.g., “Your test score is at the 85th percentile”), identifying outliers, setting benchmarks, and summarizing distributions.

---

## Q5. Define quartiles. How are Q1, Q2, and Q3 calculated?

**Quartiles** divide a sorted dataset into four equal parts:

- **Q1** (first quartile) = 25th percentile
- **Q2** (second quartile) = 50th percentile = **median**
- **Q3** (third quartile) = 75th percentile

**Calculation** (for a sorted dataset):

1. Find the position:
   - Q1 position = (n + 1) × 0.25
   - Q2 position = (n + 1) × 0.5
   - Q3 position = (n + 1) × 0.75
2. If the position is not an integer → interpolate between adjacent values  
   (There are several accepted methods; software like Python’s NumPy or R may differ slightly.)

---

## Q6. What is the Interquartile Range (IQR), and what does it represent?

**IQR = Q3 − Q1**

It represents the **middle 50%** of the data (the range where the central half of observations lie).

Advantages:

- Robust measure of spread (not heavily affected by outliers)
- Used to identify outliers (see Q9)

---

## Q7. What are the components of a Five-Number Summary?

1. **Minimum** (smallest value, excluding outliers)
2. **Q1** (first quartile, 25th percentile)
3. **Q2** (median, 50th percentile)
4. **Q3** (third quartile, 75th percentile)
5. **Maximum** (largest value, excluding outliers)

These five numbers give a concise overview of the dataset’s center and spread.

---

## Q8. Explain how a boxplot represents a dataset using the five-number summary.

A **boxplot** (box-and-whisker plot) visualizes the five-number summary:

- **Box**: spans from Q1 to Q3 (middle 50% of data)
- **Line inside box**: median (Q2)
- **Whiskers**: extend to the smallest/largest values that are **within 1.5 × IQR** of Q1/Q3
- **Points beyond whiskers**: plotted as individual dots (potential outliers)

---

## Q9. How does a boxplot help in identifying outliers?

Outliers are typically defined as values that fall outside:  
**Lower fence** = Q1 − 1.5 × IQR  
**Upper fence** = Q3 + 1.5 × IQR

Any data point below the lower fence or above the upper fence is plotted as an individual point (dot) and considered a potential outlier.

---

## Q10. What is Inferential Statistics? How is it different from Descriptive Statistics?

| Aspect        | Descriptive Statistics                   | Inferential Statistics                                               |
| ------------- | ---------------------------------------- | -------------------------------------------------------------------- |
| **Purpose**   | Summarize and describe the data you have | Make predictions or generalizations about a population from a sample |
| **Data used** | Entire dataset                           | Sample only                                                          |
| **Examples**  | Mean, median, standard deviation, charts | Hypothesis testing, confidence intervals                             |
| **Goal**      | Describe what **is**                     | Infer what **might be** true for the population                      |

---

## Q11. What is a sample in inferential statistics, and why is it used?

A **sample** is a smaller subset of the entire **population** that we actually collect and analyze.

Why use samples?

- Populations are often too large or inaccessible (e.g., all voters, all fish in an ocean)
- Saves time and money
- With proper sampling, we can make reliable inferences about the population

---

## Q12. Name and explain two common methods used in inferential statistics (e.g., hypothesis testing, confidence intervals).

1. **Confidence Intervals**  
   A range of values that is likely to contain the true population parameter (e.g., mean) with a specified level of confidence (usually 95%).  
   Example: “We are 95% confident that the true average height is between 168 cm and 172 cm.”

2. **Hypothesis Testing**  
   A method to decide whether there is enough evidence to reject a null hypothesis (H₀) in favor of an alternative hypothesis (H₁).  
   Steps:
   - State H₀ and H₁
   - Choose significance level (α, often 0.05)
   - Calculate test statistic and p-value
   - Decide: reject H₀ if p-value ≤ α  
     Example: Testing whether a new drug is more effective than placebo.
