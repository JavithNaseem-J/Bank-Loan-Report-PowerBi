# Bank Loan Data Analysis Project

## 1. ASK

### Key Questions:

1. **Monthly Trends by Issue Date**: To identify seasonality and long-term trends in lending activities.
2. **Regional Analysis by State**: To identify regions with significant lending activity and assess regional disparities.
3. **Loan Term Analysis**: To understand the distribution of loans across various term lengths.
4. **Employment Length Analysis**: How lending metrics are distributed among borrowers with different employment lengths, helping assess the impact of employment history on loan applications.
5. **Loan Purpose Breakdown**: A visual breakdown of loan metrics based on the stated purposes of loans, aiding in understanding the primary reasons borrowers seek financing.
6. **Home Ownership Analysis**: To assess how home ownership impacts loan applications and disbursements.

 **Good Loan v Bad Loan KPIs:**

- Good Loan:
  1. Good Loan Application Percentage
  2. Good Loan Applications

- Bad Loan:
  1. Bad Loan Application Percentage
  2. Bad Loan Applications

---

## 2. PREPARE
### Dataset:
- **id**: Unique identifier for each record.
- **address_state**: State where the loan applicant resides.
- **application_type**: Type of loan application (e.g., Individual).
- **emp_length**: Length of employment of the applicant.
- **emp_title**: Job title of the applicant.
- **grade**: Loan grade (related to creditworthiness).
- **home_ownership**: Applicant's home ownership status (e.g., RENT, MORTGAGE, OWN).
- **issue_date**: Date the loan was issued.
- **last_credit_pull_date**: Date when the applicant's credit was last checked.
- **last_payment_date**: Date of the last payment made.
- **loan_status**: Status of the loan (e.g., Fully Paid, Charged Off).
- **next_payment_date**: Date when the next payment is due.
- **member_id**: Member identifier of the loan applicant.
- **purpose**: Purpose of the loan (e.g., car, credit_card, etc.).
- **sub_grade**: Sub-category of the loan grade.
- **term**: Loan term (e.g., 36 months).
- **verification_status**: Whether the income has been verified or not.
- **annual_income**: Annual income of the applicant.
- **dti**: Debt-to-Income ratio.
- **installment**: Amount to be paid in each installment.
- **int_rate**: Interest rate of the loan.
- **loan_amount**: Amount of the loan.
- **total_acc**: Total number of credit accounts.
- **total_payment**: Total amount paid towards the loan so far.

---

## 3. PROCESS
- **Power BI**
- **DAX**
- **Power Query**
- **SQL**

### Data Cleaning:
- Remove duplicate loan applications.
- Handle missing data.
- Ensure consistent date formats.

### Transformation:
- Convert string-based dates to datetime for month-to-date and quarter-to-date calculations.

---

## 4. ANALYZE
#### KPIs:
- **Total Loan Applications** (with MTD and MoM)
- **Total Funded Amount** (with MTD and MoM)
- **Total Amount Received** (with MTD and MoM)
- **Average Interest Rate** (MTD and MoM)
- **Average Debt-to-Income Ratio** (MTD and MoM)

#### Key Metrics:
- **Total Loan Applications**: Number of loan applications received.
- **Total Funded Amount**: Sum of the loan amounts that have been approved and disbursed.
- **Total Amount Received**: Total payments received on the loans.
- **Average Interest Rate**: Mean interest rate charged on the loans.
- **Average DTI Ratio**: Mean debt-to-income ratio for loan applicants.
- **Loan MoM Growth**: Month-over-month growth in loan applications and funded amounts.

### 4.3. Calculated Fields/Parameters:

- **Total Loan Applications**: `COUNT([id])`
- **Total Funded Amount**: `SUM([loan_amount])`
- **Total Amount Received**: `SUM([total_payment])`
- **Average Interest Rate**: `CALCULATE(AVERAGE([int_rate]) * 100)`
- **Average DTI Ratio**: `CALCULATE(AVERAGE([dti]) * 100)`

- **Loan MoM**: `([Loan MTD] - [Loan PMTD]) / [Loan PMTD]`
- **Loan MTD**: `CALCULATE(TOTALMTD([Total Loan Applications], [Date Table].[Date]))`
- **Loan Fund MoM**: `([Loan Fund MTD] - [Loan Fund PMTD]) / [Loan Fund PMTD]`
- **Loan Fund MTD**: `CALCULATE(TOTALMTD([Total Funded Amount], [Date Table].[Date]))`
- **Loan Amt MoM**: `([Loan Amt MTD] - [Loan Amt PMTD]) / [Loan Amt PMTD]`
- **Loan Amt MTD**: `CALCULATE(TOTALMTD([Total Amount Received], [Date Table].[Date]))`

- **Loan Int MTD**: `CALCULATE(TOTALMTD([Average Interest Rate], [Date Table].[Date]))`
- **Loan DTI MTD**: `CALCULATE(TOTALMTD([Average DTI Ratio], [Date Table].[Date]))`
- **Loan DTI MoM**: `([Loan DTI MTD] / [Loan DTI PMTD]) / [Loan DTI PMTD]`

## 3. SHARE


https://github.com/user-attachments/assets/aa0dafe1-19ce-4833-8435-14c09167887d



