Absolutely. I’ve based this plan on **Wes McKinney’s *Python for Data Analysis, 3rd Edition***, rather than treating it as a generic Python course. The book’s focus is specifically on the Python programming, libraries, and tools needed for data analysis, with major emphasis on **NumPy, pandas, data cleaning/wrangling, visualization, aggregation, and time series**. 

The book progresses through Python/Jupyter, built-in data structures, NumPy, pandas, data loading, cleaning, merging/reshaping, visualization, group operations, time series, modeling libraries, and real-world analysis examples.   

# 30-Day Python for Data Analysis Study Plan

### Overall goal

By the end of 30 days, you should be able to take a messy dataset and independently:

**Load → inspect → clean → transform → combine → analyze → visualize → explain findings**

You will also have completed a **portfolio-style final project**.

### Recommended daily commitment

**2–3 hours per day**

Use this structure every day:

| Activity                          |      Time |
| --------------------------------- | --------: |
| Read/study book                   | 30–45 min |
| Type and modify examples yourself | 30–45 min |
| Exercises                         | 45–60 min |
| Challenge                         | 30–45 min |
| Notes/review                      | 10–15 min |

**Important:** Don't just copy the book's code. Type it yourself, change the values, break it, fix it, and then solve the exercises without looking at the solution.

---

# WEEK 1 — Python Foundations

## Day 1 — Set up your data-analysis environment

**Book:** Chapter 1 + beginning of Chapter 2

### Learn

Understand:

* What Python is used for in data analysis
* NumPy
* pandas
* matplotlib
* IPython
* Jupyter
* Python environments
* Interactive/exploratory programming

The book specifically describes Jupyter/IPython as environments designed for interactive and exploratory computing. 

### Exercises

Create your first notebook.

Write code that:

1. Prints your name.
2. Prints your current Python version.
3. Creates three variables:

   * name
   * age
   * career_goal
4. Prints a sentence using those variables.
5. Performs:

   * addition
   * subtraction
   * multiplication
   * division
   * exponentiation

### Challenge

Create a small **personal data report**:

```text
Name
Age
Hours studied this week
Number of Python exercises completed
Number of SQL exercises completed
```

Calculate:

* average study hours per day
* percentage of exercises completed
* projected study hours after 30 days

### Goal outcome

You can open Jupyter and comfortably execute basic Python code.

---

# Day 2 — Python variables, types and operators

**Book:** Chapter 2

### Learn

Focus on:

* variables
* integers
* floats
* strings
* booleans
* `None`
* arithmetic
* comparisons
* type conversion
* assignment

### Exercises

Create:

```python
sales = 15000
expenses = 8500
customers = 120
```

Calculate:

* profit
* profit margin
* revenue per customer
* expense per customer

Then create a second scenario and compare them.

### Challenge

Create a **business calculator** that accepts:

```text
revenue
expenses
number_of_customers
```

and produces:

```text
profit
profit margin
revenue per customer
profit per customer
```

### Goal

You understand Python's basic building blocks rather than memorizing syntax.

---

# Day 3 — Conditions and control flow

**Book:** Chapter 2

### Learn

* `if`
* `elif`
* `else`
* comparison operators
* Boolean logic
* `and`
* `or`
* `not`
* `for`
* `while`

### Exercises

Create a program that categorizes customers:

```text
0–999       → Bronze
1,000–4,999 → Silver
5,000+      → Gold
```

Then create an age categorizer.

### Challenge

Create a **sales-performance analyzer**.

Given daily sales:

```python
sales = [1200, 850, 2300, 1750, 900, 3100, 2800]
```

Calculate:

* total sales
* average sales
* highest day
* lowest day
* number of days above average
* number of days below average

### Goal

You can use Python logic to answer basic questions about data.

---

# Day 4 — Lists, tuples, dictionaries and sets

**Book:** Chapter 3

The book covers tuples, lists, dictionaries, sets, sequence functions, and comprehensions in this chapter. 

### Exercises

Create:

```python
customers = [
    {"name": "John", "age": 25, "sales": 1200},
    {"name": "Sarah", "age": 31, "sales": 2400},
    {"name": "Mike", "age": 22, "sales": 800}
]
```

Answer:

* Who generated the most sales?
* What is average age?
* What is total sales?
* Which customers generated more than R1,000?

### Challenge

Create a dataset containing **20 customers**.

Calculate:

* average age
* average sales
* maximum sales
* minimum sales
* number of customers above average sales

### Goal

You can represent structured data using native Python structures.

---

# Day 5 — Functions

**Book:** Chapter 3

### Learn

* functions
* parameters
* return values
* local/global scope
* lambda functions
* generators
* exceptions

### Exercises

Create:

```python
calculate_profit()
calculate_margin()
calculate_average()
categorize_customer()
```

### Challenge

Build a reusable:

**`sales_analyzer()`**

It should accept a list of sales and return:

```text
Total
Average
Minimum
Maximum
Number of sales above average
```

### Goal

You stop writing repetitive code.

---

# Day 6 — Files and error handling

**Book:** Chapter 3

### Learn

* opening files
* reading files
* writing files
* exceptions
* `try`
* `except`

### Exercise

Create a text file containing 20 sales values.

Read the file using Python.

Calculate:

* total
* average
* maximum
* minimum

### Challenge

Create a program that handles invalid data such as:

```text
1200
900
INVALID
1500
N/A
2200
```

Your program should identify invalid values rather than crashing.

### Goal

You can work with external data and handle errors.

---

# Day 7 — WEEK 1 TEST

### Don't read the book during this test.

Create a program that analyzes:

```text
20 customers
```

Each customer must have:

* name
* age
* gender
* city
* monthly spending

Your program must calculate:

1. Total customers
2. Average age
3. Average spending
4. Highest spender
5. Lowest spender
6. Customers above average spending
7. Customers below average spending
8. Number of customers by city

### Week 1 outcome

You should now understand:

**Python → variables → logic → collections → functions → files**

---

# WEEK 2 — NumPy + pandas

The book describes NumPy's `ndarray` as a central multidimensional numerical data structure and covers indexing, slicing, Boolean indexing, random generation, mathematical/statistical operations, sorting and more. 

---

# Day 8 — NumPy arrays

**Book:** Chapter 4

### Learn

* `numpy`
* arrays
* dimensions
* shape
* dtype
* indexing
* slicing

### Exercise

Create:

```python
import numpy as np

sales = np.array([1200, 1500, 900, 2200, 3100])
```

Calculate:

* total
* mean
* maximum
* minimum
* standard deviation

### Challenge

Create a 30-day sales array.

Analyze:

* weekly averages
* highest week
* lowest week
* days above average

### Goal

Understand why arrays are useful for numerical analysis.

---

# Day 9 — NumPy filtering and Boolean logic

### Learn

* Boolean arrays
* filtering
* fancy indexing
* sorting
* unique values
* conditional logic

### Exercise

Given:

```python
ages = np.array([18, 22, 35, 42, 19, 51, 27, 31])
```

Find:

* ages over 30
* ages under 25
* ages between 20 and 40
* oldest three people

### Challenge

Create a dataset containing:

```text
customer_id
age
income
spending
```

Find customers who satisfy:

```text
age > 25
AND
income > 15000
AND
spending > 3000
```

### Goal

You can filter numerical data efficiently.

---

# Day 10 — pandas Series and DataFrames

**Book:** Chapter 5

pandas is one of the book's primary focuses, particularly for structured/tabular data, cleaning, manipulation, selection, reshaping and aggregation. 

### Learn

* Series
* DataFrame
* columns
* indexes
* `head()`
* `tail()`
* `info()`
* `describe()`

### Exercise

Create:

```python
df = pd.DataFrame({
    "name": ["John", "Sarah", "Mike", "Lisa"],
    "age": [25, 31, 22, 29],
    "sales": [1200, 2400, 800, 1900]
})
```

Explore the dataset.

### Challenge

Create a **50-row customer DataFrame**.

Use:

```python
df.info()
df.describe()
df.head()
df.tail()
```

and explain what each tells you.

### Goal

You can inspect a DataFrame without being dependent on someone else's code.

---

# Day 11 — pandas selection and filtering

### Learn

* selecting columns
* selecting rows
* `.loc`
* `.iloc`
* Boolean filtering
* sorting

### Exercises

Using your customer dataset:

Find:

* customers over 30
* customers spending over R2,000
* customers from Johannesburg
* top 10 customers
* bottom 10 customers

### Challenge

Answer 10 business questions about your dataset.

For example:

> Which customers spend more than the average?

> Which city has the highest-spending customers?

### Goal

You can retrieve exactly the data you need.

---

# Day 12 — pandas statistics

### Learn

* `mean()`
* `sum()`
* `min()`
* `max()`
* `median()`
* `std()`
* `count()`
* `value_counts()`
* correlation

### Exercise

Analyze:

```text
age
income
spending
```

Calculate descriptive statistics.

### Challenge

Investigate:

> Does income appear related to spending?

Calculate correlation and explain what the result means.

### Goal

You can turn raw columns into useful statistics.

---

# Day 13 — Loading real data

**Book:** Chapter 6

The book covers text/delimited files, JSON, HTML/XML, Excel, APIs and databases. 

### Practice files

Work with:

* CSV
* Excel
* JSON

### Exercise

Load a dataset and answer:

1. How many rows?
2. How many columns?
3. What are the data types?
4. Are there missing values?
5. Which columns are numerical?

### Challenge

Load **three different datasets**.

For each, create a short data-quality report.

### Goal

You can bring external data into Python.

---

# Day 14 — WEEK 2 PROJECT

Build:

## Customer Sales Analysis

Dataset:

**100 customers**

Columns:

```text
customer_id
name
age
gender
city
income
product
quantity
price
sales_date
```

Calculate:

* total revenue
* average order value
* highest-selling product
* highest-spending customer
* sales by city
* sales by gender
* sales by product

### Week 2 outcome

You should now be comfortable with:

**NumPy + pandas + DataFrames + filtering + statistics + loading data**

---

# WEEK 3 — Data Cleaning, Wrangling and Visualization

---

# Day 15 — Missing data

**Book:** Chapter 7

The book covers filtering missing data and filling missing data. 

### Exercise

Create a deliberately messy dataset:

```text
Name
Age
Income
City
Sales
```

Insert:

* missing ages
* missing income
* missing cities

Then investigate:

```python
df.isna()
df.isna().sum()
```

### Challenge

Try three approaches:

1. Remove missing rows.
2. Fill numerical values with a statistic.
3. Fill categorical values.

Compare the results.

### Goal

Understand that cleaning decisions affect analysis.

---

# Day 16 — Duplicates, replacement and outliers

### Learn

* duplicate detection
* removing duplicates
* replacing values
* renaming columns
* binning
* detecting outliers

### Exercise

Create duplicate customer records.

Find and remove them.

### Challenge

Find suspicious sales values.

Example:

```text
R100
R120
R150
R130
R125
R50,000
```

Investigate whether R50,000 should be treated as an outlier.

### Goal

You can identify potentially problematic data instead of blindly analyzing it.

---

# Day 17 — Strings and categorical data

### Learn

* string methods
* regular expressions
* pandas string operations
* categorical data

### Exercise

Clean:

```text
" johannesburg"
"JOHANNESBURG"
"Johannesburg "
"johannesburg"
```

into a consistent format.

### Challenge

Clean a customer dataset containing:

* inconsistent names
* inconsistent cities
* phone numbers
* email addresses
* product categories

### Goal

You can turn messy text into standardized analytical data.

---

# Day 18 — Merge datasets

**Book:** Chapter 8

### Learn

* merge
* join
* concatenate
* database-style joins
* index-based merging

The book specifically discusses database-style DataFrame joins and merging on indexes. 

### Exercise

Create:

**customers.csv**

```text
customer_id
name
city
```

and

**orders.csv**

```text
order_id
customer_id
product
amount
```

Merge them.

### Challenge

Create a third dataset:

```text
customer_id
customer_segment
```

Combine all three.

### Goal

Understand how multiple datasets become one analytical dataset.

---

# Day 19 — Reshaping data

### Learn

* hierarchical indexes
* long format
* wide format
* pivoting

### Exercise

Create monthly sales data.

Transform:

```text
Month | Product | Sales
```

into:

```text
Month | Product A | Product B | Product C
```

### Challenge

Create both:

**long format**

and

**wide format**

of the same dataset.

Explain why each format could be useful.

### Goal

You understand data structure, not just commands.

---

# Day 20 — Visualization

**Book:** Chapter 9

The book covers matplotlib figures/subplots, labels, annotations and saving plots, followed by pandas/seaborn visualization including line, bar, histogram, scatter and categorical plots. 

### Learn

Create:

* line chart
* bar chart
* histogram
* scatter plot
* box plot

### Exercise

Using your sales dataset:

Create:

1. Monthly sales line chart
2. Sales by product bar chart
3. Sales distribution histogram
4. Income vs sales scatter plot

### Challenge

For each chart, write:

> What does this chart tell us?

Do not merely create charts.

### Goal

You begin communicating insights visually.

---

# Day 21 — WEEK 3 PROJECT

Create a complete:

# Sales Dashboard Notebook

Your notebook should contain:

### Section 1 — Data

Load the dataset.

### Section 2 — Data quality

Show:

* missing values
* duplicates
* incorrect values
* data types

### Section 3 — Cleaning

Document what you changed.

### Section 4 — Analysis

Calculate:

* revenue
* averages
* product performance
* customer performance

### Section 5 — Visualization

Create at least:

* 2 bar charts
* 1 line chart
* 1 histogram
* 1 scatter plot

### Week 3 outcome

You can now perform a basic **real-world data-cleaning and EDA workflow**.

---

# WEEK 4 — Advanced Analysis

# Day 22 — GroupBy

**Book:** Chapter 10

The book describes group operations using the **split → apply → combine** approach and covers summary statistics, transformations, pivot tables and cross-tabulations. 

### Learn

```python
df.groupby()
```

Practice:

* sum
* mean
* count
* min
* max
* multiple aggregations

### Exercise

Calculate:

```text
sales by city
sales by product
sales by gender
average sales by city
average sales by product
```

### Challenge

Find:

> Which product performs best in each city?

### Goal

You can answer grouped business questions efficiently.

---

# Day 23 — Advanced aggregation

### Learn

* multiple aggregation functions
* `agg()`
* `apply()`
* transformations
* quantiles
* group-specific calculations

### Exercise

For each product calculate:

```text
total sales
average sales
minimum
maximum
standard deviation
```

### Challenge

Create customer segments:

```text
Low spender
Medium spender
High spender
```

based on spending.

Then compare each segment.

### Goal

You can perform more sophisticated group analysis.

---

# Day 24 — Pivot tables and cross-tabulation

The book covers `pivot_table` and `crosstab` for summarizing grouped data.

### Exercise

Create a pivot table:

```text
Rows    = City
Columns = Product
Values  = Sales
```

### Challenge

Create a cross-tabulation showing:

```text
Gender × Product
```

Then:

```text
City × Product
```

### Goal

You can create reporting-style summaries.

---

# Day 25 — Time series

**Book:** Chapter 11

### Learn

* datetime
* converting strings to datetime
* date ranges
* time-series indexing
* shifting
* periods
* resampling

The chapter covers date/time data, date ranges, frequencies, shifting, time zones, periods, resampling and moving-window functions. 

### Exercise

Convert:

```text
2026-01-15
2026-02-21
2026-03-12
```

into datetime values.

Extract:

* year
* month
* day
* weekday

### Challenge

Analyze **daily sales for six months**.

Calculate:

* daily sales
* weekly sales
* monthly sales
* monthly growth
* rolling average

### Goal

You can analyze data across time.

---

# Day 26 — Modeling foundations

**Book:** Chapter 12

The book introduces:

* Patsy
* statsmodels
* linear models
* time-series processes
* scikit-learn

but deliberately treats these as introductions rather than a complete machine-learning course. 

### Exercise

Take your sales dataset.

Investigate whether:

```text
income
age
quantity
```

are related to:

```text
sales
```

### Challenge

Build a simple regression model.

Don't focus on becoming an ML engineer yet.

Focus on understanding:

**features → target → model → result**

### Goal

Understand how your pandas workflow connects to modeling.

---

# Day 27 — Real-world analysis

**Book:** Chapter 13

The book's examples include:

* Bitly/USA.gov data
* MovieLens
* US baby names
* USDA food data
* Federal Election Commission data. 

### Exercise

Choose **one** dataset.

Perform:

1. Load
2. Inspect
3. Clean
4. Transform
5. Analyze
6. Visualize

### Challenge

Do the entire analysis without following the book's code line-for-line.

### Goal

Move from exercises to independent analysis.

---

# Day 28 — Advanced NumPy + performance day

**Book:** Appendix A

The appendix covers advanced array manipulation, broadcasting, advanced ufunc usage, structured arrays, sorting and performance topics. 

### Exercises

Practice:

* reshaping
* broadcasting
* concatenation
* splitting
* sorting

### Challenge

Take a calculation you previously performed using a Python loop.

Rewrite it using NumPy vectorized operations.

Compare the approaches.

### Goal

Understand why vectorized numerical operations are important.

---

# Day 29 — FINAL PROJECT: Data Analyst Challenge

Now pretend you have been given a completely unfamiliar business dataset.

Use this workflow:

## Step 1 — Understand

Answer:

> What does this dataset represent?

## Step 2 — Inspect

Check:

```python
shape
columns
dtypes
head()
describe()
```

## Step 3 — Clean

Check:

```text
missing values
duplicates
incorrect types
outliers
inconsistent strings
```

## Step 4 — Transform

Create useful columns.

For example:

```text
profit
profit_margin
customer_segment
month
year
```

## Step 5 — Combine

If you have multiple datasets, merge them.

## Step 6 — Analyze

Use:

```text
groupby
aggregation
pivot_table
crosstab
correlation
```

## Step 7 — Visualize

Produce at least:

**5 meaningful charts**

## Step 8 — Explain

Write:

### Finding 1

What did you discover?

### Finding 2

What did you discover?

### Finding 3

What did you discover?

### Finding 4

What did you discover?

### Finding 5

What did you discover?

### Goal

Complete an analysis without needing step-by-step instructions.

---

# Day 30 — Final assessment

Today you don't learn new material.

You prove that you can use what you've learned.

## Part A — Python test

Without the book:

* variables
* lists
* dictionaries
* loops
* functions
* conditions

## Part B — NumPy test

Create an array and:

* filter it
* calculate statistics
* sort it
* reshape it

## Part C — pandas test

Given a CSV:

```text
Load
Inspect
Filter
Sort
Group
Aggregate
```

## Part D — Cleaning test

Identify:

* missing values
* duplicates
* inconsistent categories
* outliers

## Part E — Visualization test

Create:

* bar
* line
* histogram
* scatter

## Part F — Business questions

Answer at least **10 questions** about the dataset.

---

# Your 30-Day Skill Progression

| Days  | Main skill                       | Target |
| ----- | -------------------------------- | ------ |
| 1–3   | Python basics                    | ⭐      |
| 4–7   | Python data structures/functions | ⭐⭐     |
| 8–9   | NumPy                            | ⭐⭐     |
| 10–12 | pandas                           | ⭐⭐⭐    |
| 13–14 | Data loading                     | ⭐⭐⭐    |
| 15–17 | Data cleaning                    | ⭐⭐⭐    |
| 18–19 | Data wrangling                   | ⭐⭐⭐⭐   |
| 20–21 | Visualization                    | ⭐⭐⭐⭐   |
| 22–24 | GroupBy/aggregation              | ⭐⭐⭐⭐   |
| 25    | Time series                      | ⭐⭐⭐⭐   |
| 26    | Modeling introduction            | ⭐⭐⭐⭐   |
| 27    | Real-world analysis              | ⭐⭐⭐⭐⭐  |
| 28    | Advanced NumPy                   | ⭐⭐⭐⭐⭐  |
| 29–30 | Portfolio project                | ⭐⭐⭐⭐⭐  |

# The datasets I recommend using

Don't use the same dataset for everything. Rotate datasets so that you learn to deal with different structures.

### Dataset 1 — Sales

Columns:

```text
order_id
customer_id
product
category
quantity
price
city
order_date
```

Use for:

**pandas + cleaning + groupby + visualization**

### Dataset 2 — Customers

```text
customer_id
age
gender
income
city
customer_segment
```

Use for:

**filtering + statistics + segmentation**

### Dataset 3 — Movies

```text
movie_id
title
genre
rating
year
```

Use for:

**grouping + aggregation + visualization**

### Dataset 4 — Financial transactions

```text
transaction_id
date
account
category
amount
transaction_type
```

Use for:

**time series + aggregation + cleaning**

### Dataset 5 — Your own project dataset

Use something you're genuinely interested in.

This is important because the book itself progresses toward real-world data analysis examples rather than stopping at isolated programming exercises. 

---

# Your daily challenge rule

For every exercise, follow this process:

**1. Try it yourself for 15 minutes.**

**2. If stuck, reread the relevant section.**

**3. Try again without copying.**

**4. Only then look at an example.**

**5. Close the example.**

**6. Rebuild the solution yourself.**

**7. Change the problem.**

For example, if the exercise says:

> Find average sales by city.

After solving it, change it to:

> Find average sales by city and product.

Then:

> Find the highest-selling product in each city.

Then:

> Find the percentage contribution of each product to city sales.

That progression is what will turn knowledge of pandas into actual **data-analysis ability**.

---

# Final outcome after 30 days

If you complete the exercises rather than simply reading the chapters, your target capability is:

```text
                    DATASET
                       ↓
                   LOAD DATA
                       ↓
                 INSPECT DATA
                       ↓
                  CLEAN DATA
                       ↓
                TRANSFORM DATA
                       ↓
                 MERGE DATA
                       ↓
             GROUP / AGGREGATE
                       ↓
                ANALYZE DATA
                       ↓
               VISUALIZE DATA
                       ↓
             FIND INSIGHTS
                       ↓
              COMMUNICATE RESULTS
```

That is the core workflow I would want you to be able to perform independently after the 30 days.

The book itself emphasizes that its purpose is to equip the learner with Python, libraries, and tools for becoming an effective data analyst, rather than attempting to teach all data-analysis methodology or advanced data science in one book. 

**One important adjustment for you:** since you're also learning SQL/data analysis, I would make the exercises deliberately connect **Python/pandas concepts to SQL concepts**. For example, `WHERE` → pandas filtering, `GROUP BY` → `groupby()`, `JOIN` → `merge()`, and SQL aggregations → pandas aggregations. That will make the two skills reinforce each other rather than feeling like two separate courses.

---

If you want, I can:

* Create Day 1 Python code examples
* Design Week 4 Day 22 GroupBy practice code
* Outline the Final Project steps
