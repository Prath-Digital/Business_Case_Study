# Business Case Study: Self Excercise - Chapter 1, Lecture 1.1

## Q1. What is Statistics, and how is it useful in real-world applications?

**Statistics** is the science of collecting, organizing, analyzing, interpreting, and presenting data to discover patterns, draw conclusions, and make decisions under uncertainty.

**Real-world usefulness**:

- Predicting weather & climate trends
- Quality control in manufacturing
- Medical research & drug testing
- Stock market analysis & risk assessment
- Election polling & public opinion research
- A/B testing in websites/apps
- Sports analytics
- Insurance premium calculation
- Crime trend analysis for policing
- Business decisions (pricing, inventory, customer segmentation)

Basically: Statistics helps us make **smarter decisions** when we have incomplete or uncertain information.

## Q2. How is Statistics applied in Data Science?

Statistics is one of the three main pillars of Data Science (together with programming & domain knowledge).

Main applications in Data Science:

- Exploratory Data Analysis (EDA) → summary statistics, distributions, visualizations
- Data cleaning → outlier detection, missing value treatment
- Feature selection & engineering
- Statistical hypothesis testing (t-tests, chi-square, ANOVA, etc.)
- Confidence intervals & margin of error
- Regression analysis (linear, logistic, polynomial…)
- A/B testing & experimentation
- Sampling & experimental design
- Model evaluation (p-values, confidence intervals, error metrics)
- Time series forecasting
- Bayesian statistics (increasingly popular in modern ML)

→ Statistics gives **validity, reliability and interpretability** to Data Science results.

## Q3. What is the difference between Data and Information in the context of Statistics?

| Aspect     | Data                           | Information                           |
| ---------- | ------------------------------ | ------------------------------------- |
| Definition | Raw, unprocessed facts/numbers | Processed, organized, meaningful data |
| State      | Unorganized, chaotic           | Organized, contextualized             |
| Example    | 23, 45, 19, 72, 31             | Average age = 38 years                |
| Meaning    | No inherent meaning by itself  | Has meaning and supports decisions    |
| Stage      | Input / collection stage       | After analysis & interpretation       |
| Analogy    | Ingredients                    | Cooked meal                           |

**In short**: Data is **raw material**, Information is **what we get after applying statistics** to the data.

## Q4. List a few real-life applications of Statistics in various fields

| Field         | Applications of Statistics                                |
| ------------- | --------------------------------------------------------- |
| Medicine      | Clinical trials, drug efficacy, disease outbreak modeling |
| Business      | Market research, customer segmentation, sales forecasting |
| Finance       | Risk management, portfolio optimization, fraud detection  |
| Sports        | Player performance analysis, strategy optimization        |
| Education     | Standardized test analysis, student performance tracking  |
| Psychology    | Personality research, experimental design                 |
| Agriculture   | Crop yield prediction, fertilizer effectiveness           |
| Environment   | Climate modeling, pollution trend analysis                |
| Government    | Census, economic indicators, policy evaluation            |
| Tech/Internet | Recommendation systems, A/B testing, spam detection       |

## Q5. What are the two main types of data in Statistics?

1. **Qualitative** (Categorical)
2. **Quantitative** (Numerical)

## Q6. Differentiate between Numerical Data and Categorical Data with examples

| Property         | Categorical (Qualitative)               | Numerical (Quantitative)                |
| ---------------- | --------------------------------------- | --------------------------------------- |
| Nature           | Represents categories/labels            | Represents measurable quantities        |
| Mathematical ops | Mostly counting, no true arithmetic     | Addition, subtraction, average possible |
| Examples         | Gender, color, city, blood type, yes/no | Height, weight, temperature, salary     |
| Subtypes         | Nominal, Ordinal                        | Discrete, Continuous                    |
| Visualization    | Bar chart, Pie chart                    | Histogram, Box plot, Line chart         |

## Q7. What is the difference between Discrete and Continuous numerical data?

| Property        | Discrete                                           | Continuous                                  |
| --------------- | -------------------------------------------------- | ------------------------------------------- |
| Nature          | Countable, distinct values                         | Can take any value in a range               |
| Possible values | Finite or countably infinite                       | Infinite (uncountable)                      |
| Examples        | Number of children, cars in parking lot, dice roll | Height, weight, temperature, time, distance |
| Measurement     | Usually counting                                   | Usually measuring                           |
| Graph type      | Bar chart (with gaps)                              | Histogram (no gaps), line chart             |

## Q8. What are some common methods of representing data visually?

Most popular visualization methods in Statistics:

- Bar Chart / Column Chart
- Pie Chart / Donut Chart
- Histogram
- Line Chart
- Box Plot (Box-and-Whisker Plot)
- Scatter Plot
- Heatmap
- Violin Plot
- Stem-and-Leaf Plot (less common today)
- Frequency Polygon
- Pareto Chart
- Time Series Plot

## Q9. Explain the use of bar graphs, line charts, and histograms in data representation

- **Bar Graphs**  
  → Compare **categories** or discrete groups  
  → Length/height of bars shows magnitude  
  → Good for: sales by product, votes by party, average score by class

- **Line Charts**  
  → Show **trends over time** or continuous variable  
  → Excellent for: stock prices, temperature changes, website traffic over months  
  → Can show multiple series on same chart

- **Histograms**  
  → Show **distribution** of **continuous numerical data**  
  → Displays frequency in intervals (bins)  
  → Helps see shape (normal, skewed, bimodal…), center, spread, outliers

## Q10. How can pie charts and box plots help in understanding the distribution of data?

**Pie Charts**

- Show **proportion/percentages** of categories that make up a whole (100%)
- Best when: small number of categories (≤5–7), focus is on relative size
- Helps quickly see which category is dominant
- Limitation: hard to compare similar-sized slices

**Box Plots** (Box-and-Whisker)

- Excellent summary of numerical data distribution
- Shows at once:
  - Median
  - Interquartile Range (IQR) → middle 50%
  - Range
  - Potential outliers
  - Skewness (position of median)
- Great for comparing distributions across multiple groups

## Q11. What is the difference between Population and Sample in statistics?

| Aspect            | Population                                 | Sample                           |
| ----------------- | ------------------------------------------ | -------------------------------- |
| Definition        | Entire group of interest                   | Subset/portion of the population |
| Size              | Usually very large (sometimes infinite)    | Much smaller, manageable         |
| Parameter vs Stat | Parameters (μ, σ, p) – true values         | Statistics (x̄, s, p̂) – estimates |
| Notation          | Greek letters (μ, σ, σ², p)                | Roman letters (x̄, s, s², p̂)      |
| Cost & Time       | Very expensive / impossible to study fully | Practical and affordable         |
| Accuracy          | Contains true value                        | Contains sampling error          |

## Q12. Why do data scientists often work with samples instead of entire populations?

Main reasons:

1. **Cost** – Collecting data from millions/billions is extremely expensive
2. **Time** – Impossible to measure entire population quickly
3. **Practicality** – Many populations are infinite or destructive sampling (e.g. crash testing cars)
4. **Sufficient accuracy** – A well-designed sample can give very accurate estimates
5. **Statistical inference** – We developed strong methods to make reliable conclusions from samples
6. **Feasibility** – Only realistic option in most real-world situations

Good sampling + correct statistical methods → we can make very good inferences about huge populations with only a few hundred/thousand observations.
