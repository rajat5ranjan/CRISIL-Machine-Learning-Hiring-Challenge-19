# CRISIL Machine-Learning Hiring Challenge-19

CRISIL Machine Learning Hiring Challenge'19 organised by Hackerearth

# Extract Financial Statement Values

Financial statement analysis is critical to every organization to enable companies to make better economic decisions that yields more income in the future. For a given financial statement, a rulebook is followed to extract the values associated with accrual, audit status, balance sheet, measurement date and pension plans as shown (refer rulebook & sample data here)

## Task:

* Build an NLP model which analyzes each document, looks for relevant financial terms (described below)

* The NLP Model should learn on Documents available under Training data folder using Rules listed here

* Apply the same model on Test Data documents to extract relevant financial information

* The results need to be updated & uploaded in the sheet provided: ‘Results.csv’ (download dataset)

Note: No training labels are explicitly available for this problem statement. You will be able to test your model's accuracy by submitting values extracted for Test data.


## Data Description:

|Columns | Description of Values|
|---|---|
|Credit Name, State, Security ID, Org ID, FYE|Identifiers from Documents provided to you already in “Results.csv”|
|Accounting Basis|Identify ‘Basis of Accounting’ as [‘Accrual’, ‘Cash’, ‘Modified Accrual’, ‘Modified Cash’, ‘Regulatory’]|
|Pension Plan 1 Name*|Pension Plan Identifier for Pension Plan with highest Total Pension Liability (0 if no date is specified) |
|Pension Plan 1 Measurement Date|Reporting Date for Pension Plan 1 (0 if no date is specified) [DD/MM/YYYY]|
|Pension Plan 1 Total Pension Liability|Total Pension Plan liability for Pension Plan 1 (0 if no liability is specified) [int64]|
|Balance Sheet Cash|Total value of Balance sheet-Governmental funds under ‘Cash & Cash Equivalents’ row. This will include all other row items as well which have been highlighted in the rules for cash and cash equivalent.  (0 if no balance sheet amount is specified) [int64]|
|Pension Plan 2 Name*|Pension Plan Identifier for Pension Plan with second highest Total Pension Liability (0 if no date is specified)|
|Pension Plan 2 Measurement Date|Reporting Date for Pension Plan 1 (0 if no date is specified) [DD/MM/YYYY]|
|Pension Plan 2 Total Pension Liability|Total Pension Plan liability for Pension Plan 1 (0 if no date is specified) [int64]|

**Note: *- Map Pension Plan Names to Industry Standards as specified here**

### Data Volume:

Train Data: 479 Documents, 1.5GB
Test Data: 98 Documents, 373.7MB
Submission Format: You need to update Results.csv provided here, with your predictions and upload it online.
Data Files: Download Dataset (~1.7GB)

### Evaluation Metric:

[ML_Model] accuracy_score

### Leaderboard score = 100 * mean(accuracy\_score[columns])

[Offline] Source Code, Models/Logic used

# Leaderboard
[Problem Link](https://www.hackerearth.com/challenges/hiring/crisil-ml-hiring-challenge-2019/machine-learning/extract-financial-statement-values/)

[Leaderboard Link](https://www.hackerearth.com/challenges/hiring/crisil-ml-hiring-challenge-2019/leaderboard/extract-financial-statement-values/)

# Rank 1
