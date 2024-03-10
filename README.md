# AB_Testing_I
# Comparison of Conversion between Bidding Methods through A/B Testing

## Business Problem

Facebook recently introduced a new type of bid called "average bidding" as an alternative to the existing "maximum bidding" bid type.

One of our clients, bombabomba.com, decided to test this new feature to determine whether average bidding brings more conversions than maximum bidding through an A/B test.

The A/B test has been ongoing for 1 month, and now bombabomba.com expects you to analyze the results of this A/B test. The ultimate success metric for bombabomba.com is Purchase. Therefore, statistical tests should focus on the Purchase metric.

## Data Set Story

This dataset, containing a company's website information, includes data such as the number of ads seen and clicked by users, as well as the earnings from these actions. There are two separate datasets: Control and Test group. These datasets are located on separate sheets of the ab_testing.xlsx Excel file. Maximum Bidding has been applied to the Control group, and Average Bidding has been applied to the Test group.

### Variables

- Impression
- Click
- Purchase
- Earning

### Data

- 40 Observations
- 26 KB

Includes the number of ad impressions, the number of clicks on the displayed ad, the number of products purchased after clicking the ads, and the earnings obtained after purchasing the products.

## Project Tasks

### Task 1: Data Preparation and Analysis

#### Step 1:
Read the dataset consisting of control and test group data from ab_testing_data.xlsx. Assign the control and test group data to separate variables.

#### Step 2:
Analyze the control and test group data.

#### Step 3:
After the analysis process, use the concat method to merge the control and test group data.

### Task 2: Defining the Hypothesis of the A/B Test

#### Step 1:
Define the hypothesis.

- H0: M1 = M2
- H1: M1 != M2

#### Step 2:
Analyze the purchase (earning) averages for the control and test group.

### Task 3: Conducting the Hypothesis Test

#### Step 1:
Before conducting the hypothesis test, perform assumption checks. These are the Normality Assumption and Homogeneity of Variance. Test whether the control and test group meet the normality assumption separately based on the Purchase variable.

**Normality Assumption:**
- H0: The assumption of normal distribution is satisfied.
- H1: The assumption of normal distribution is not satisfied.
- p < 0.05 H0 REJECTED p > 0.05 H0 CANNOT BE REJECTED

Do the control and test groups satisfy the normality assumption based on the test results? Interpret the obtained p-value values.

**Homogeneity of Variance:**
- H0: The variances are homogeneous.
- H1: The variances are not homogeneous.
- p < 0.05 H0 REJECTED p > 0.05 H0 CANNOT BE REJECTED

Test whether the control and test group satisfy the homogeneity of variance based on the Purchase variable. Do the test results satisfy the normality assumption? Interpret the obtained p-value values.

#### Step 2:
Select the appropriate test based on the results of the Normality Assumption and Homogeneity of Variance.

#### Step 3:
Considering the p_value obtained from the test, interpret whether there is a statistically significant difference between the purchase averages of the control and test group.

### Task 4: Analysis of the Results

#### Step 1:
Indicate which test you used and the reasons for it.

#### Step 2:
Based on the test results you obtained, provide recommendations to the client.
