# Bank Term Deposit Subscription Prediction

## About Dataset

### Context

Term deposits are a major source of income for a bank. A term deposit is a cash investment held at a financial institution, where the money is invested for an agreed rate of interest over a fixed period. Banks use various outreach plans, including email marketing, advertisements, telephonic marketing, and digital marketing, to sell term deposits to their customers.

Telephonic marketing campaigns are still one of the most effective ways to reach people, but they require substantial investment in large call centers. Therefore, it's crucial to identify customers most likely to convert beforehand so that they can be specifically targeted via calls.

The dataset is related to direct marketing campaigns (phone calls) of a Portuguese banking institution. The classification goal is to predict if the client will subscribe to a term deposit (the variable y).

### Content

The data is related to the direct marketing campaigns of a Portuguese banking institution, primarily based on phone calls. Often, multiple contacts with the same client were required to determine whether the client would subscribe to the bank term deposit ('yes') or not ('no'). The dataset includes two files:

- `train.csv`: Contains 45,211 rows and 18 columns, ordered by date (from May 2008 to November 2010).
- `test.csv`: Contains 4,521 rows and 18 columns, representing 10% of the examples (4,521), randomly selected from `train.csv`.
The two csv files have been merged into a single file named `bank-additional-full.csv`

### Detailed Column Descriptions

#### Bank Client Data:

1. **age**: Age of the client (numeric).
2. **job**: Type of job (categorical): "admin.", "unknown", "unemployed", "management", "housemaid", "entrepreneur", "student", "blue-collar", "self-employed", "retired", "technician", "services".
3. **marital**: Marital status (categorical): "married", "divorced", "single" (note: "divorced" means divorced or widowed).
4. **education**: Education level (categorical): "unknown", "secondary", "primary", "tertiary".
5. **default**: Has credit in default? (binary): "yes", "no".
6. **balance**: Average yearly balance in euros (numeric).
7. **housing**: Has housing loan? (binary): "yes", "no".
8. **loan**: Has personal loan? (binary): "yes", "no".

#### Related to the Last Contact of the Current Campaign:

9. **contact**: Contact communication type (categorical): "unknown", "telephone", "cellular".
10. **day**: Last contact day of the month (numeric).
11. **month**: Last contact month of the year (categorical): "jan", "feb", "mar", …, "nov", "dec".
12. **duration**: Last contact duration in seconds (numeric).

#### Other Attributes:

13. **campaign**: Number of contacts performed during this campaign and for this client (numeric, includes the last contact).
14. **pdays**: Number of days that passed after the client was last contacted from a previous campaign (numeric, -1 means the client was not previously contacted).
15. **previous**: Number of contacts performed before this campaign and for this client (numeric).
16. **poutcome**: Outcome of the previous marketing campaign (categorical): "unknown", "other", "failure", "success".

#### Output Variable (Desired Target):

17. **y**: Has the client subscribed to a term deposit? (binary): "yes", "no".


## Data Analysis and Machine Learning Model

In this project, a comprehensive analysis of the dataset has been conducted, and a machine learning model has been built to predict whether clients will subscribe to a term deposit based on various features. The goal is to provide insights and predictions to help optimize marketing campaigns and improve subscription rates.

The analysis includes exploratory data analysis (EDA), feature engineering, data preprocessing, model selection, training, evaluation, and fine-tuning. The final model's performance metrics are reported, and the model is ready for deployment in a production environment.

### Questions Answered in the Analysis

The following questions were addressed in the analysis using the `bank-additional-full.csv` dataset:

1. What profiles (age / job / marital status / etc.) are the most likely to respond positively?
2. Does the financial situation of people have an impact on how they answer?
3. Do the timing (date / duration) and type of contact matter significantly? How? Is it the same for all groups of people?
4. What is the best number of contacts to reach an agreement? What is the best delay? Are people more likely to agree to the campaign if they have already agreed in the past?
5. Does the economy (Employment variation rate / Consumer Price Index / Consumer Confidence Index / Euribor / etc.) have an impact? How? Is it the same for everybody?
6. Any interesting insights to add?

Feel free to explore the Jupyter Notebook and code for detailed information about the data analysis and machine learning pipeline.
