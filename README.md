Below is the revised GitHub README documentation for your Power BI project, with the "Dashboard Features" section removed and replaced with a "Questions Answered" section. This section highlights key questions that the Power BI report can help answer based on the dataset and the visuals provided in the images.

---

# Bank Loan Report - Power BI Project

## 📊 Project Overview

The **Bank Loan Report** is a Power BI project designed to analyze and visualize loan application data for a financial institution. The dashboard provides insights into loan applications, funding amounts, loan statuses, interest rates, debt-to-income (DTI) ratios, and more. It is divided into three main pages: **Summary**, **Overview**, and **Details**, each offering a different level of granularity for stakeholders to monitor loan performance and trends.

This project aims to assist bank managers, financial analysts, and decision-makers in understanding loan portfolios, identifying trends, and making data-driven decisions.

---

## 📊 Dataset Description

The dataset used in this project contains detailed information about loan applications. It includes the following key columns:

- **id**: Unique identifier for each loan application.
- **address_state**: The state where the applicant resides (e.g., CA, TX, NY).
- **application_type**: Type of application (e.g., Individual).
- **emp_length**: Employment length of the applicant (e.g., < 1 year, 10+ years).
- **emp_title**: Job title of the applicant (e.g., Ryder, American Airlines).
- **grade**: Loan grade assigned (e.g., A, B, C).
- **home_ownership**: Ownership status (e.g., RENT, MORTGAGE, OWN).
- **issue_date**: Date the loan was issued.
- **last_credit_pull_date**: Date of the last credit pull.
- **last_payment_date**: Date of the last payment.
- **loan_status**: Status of the loan (e.g., Charged Off, Fully Paid, Current).
- **next_payment_date**: Date of the next scheduled payment.
- **member_id**: Unique identifier for the member.
- **purpose**: Purpose of the loan (e.g., car, wedding).
- **sub_grade**: Sub-grade of the loan (e.g., A1, B2).
- **term**: Loan term (e.g., 36 months, 60 months).
- **verification_status**: Verification status (e.g., Source Verified, Not Verified).
- **annual_income**: Annual income of the applicant.
- **dti**: Debt-to-income ratio.
- **installment**: Monthly installment amount.
- **int_rate**: Interest rate of the loan.
- **loan_amount**: Loan amount requested.
- **total_acc**: Total number of accounts.
- **total_payment**: Total payment made.

The dataset includes 38,576 loan applications with a total funded amount of $436M and a total amount received of $473M.

---

## ❓ Questions

This Power BI report helps answer the following key questions for stakeholders:

1. **What is the overall performance of the loan portfolio?**  

2. **How many loans are classified as good vs. bad?**  

3. **What is the distribution of loan statuses?**  

4. **How do interest rates and DTI ratios vary by loan status?**  

5. **What are the trends in loan applications over time?**  

6. **Which states have the highest number of loan applications?**  

7. **What are the most common purposes for loans?**  

8. **How do loan terms (e.g., 36 months vs. 60 months) compare?**  

9. **What is the distribution of loan applications by employment length?**  

10. **How does home ownership impact loan applications?**  

11. **What are the details of individual loan applications?**  


---

## 🛠️ Prerequisites

To run this Power BI project, you need the following:
- **Power BI Desktop**: Download and install the latest version of Power BI Desktop from [Microsoft's official website](https://powerbi.microsoft.com/desktop/).
- **Dataset**: The dataset file (e.g., `loan_data.csv`) containing the loan application data.

---

## ⚙️ Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/bank-loan-report.git
   cd bank-loan-report
   ```

2. **Download Power BI Desktop**:
   - If you don't have Power BI Desktop installed, download it from [here](https://powerbi.microsoft.com/desktop/) and install it on your system.

3. **Load the Dataset**:
   - Place the dataset file (`loan_data.csv`) in the project directory.
   - Open Power BI Desktop.
   - Click on **Get Data** > **Text/CSV** and select the `loan_data.csv` file.
   - Load the data into Power BI.

4. **Open the Power BI File**:
   - Open the `Bank_Loan_Report.pbix` file in Power BI Desktop.
   - If the dataset is already connected, the dashboard will load automatically. Otherwise, reconnect the dataset as described above.

5. **Explore the Dashboard**:
   - Navigate through the **Summary**, **Overview**, and **Details** pages using the tabs on the left.

---

## 🚀 Usage

- **Filter Data**: Use the filters on the left sidebar (State, Grade, Purpose) to drill down into specific subsets of the data.
- **Interact with Visuals**: Click on charts, maps, or tables to interact with the data and see cross-filtered results.
- **Analyze Trends**: Use the visuals to identify trends in loan applications by month, state, or purpose.
- **Detailed Insights**: Use the detailed table to view individual loan records for in-depth analysis.

---

## 📸 Screenshots

### Summary Page
![Screenshot 2025-03-27 014155](https://github.com/user-attachments/assets/8339f108-3f35-48ad-a6d5-c515082af9d9)

### Overview Page
![Screenshot 2025-03-27 014230](https://github.com/user-attachments/assets/601d73b5-ef41-42fd-868b-376d2496ac6c)


### Details Page
![Screenshot 2025-03-27 014255](https://github.com/user-attachments/assets/291ce60b-7a5b-49de-80ff-a3a97d930496)

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
