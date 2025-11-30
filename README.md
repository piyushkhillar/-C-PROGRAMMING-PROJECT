Loan EMI Calculator – C Project

This is a small C programming project where the user can check if they are eligible for a loan based on their CIBIL score. If they qualify, the program shows different loan tenure options along with the interest rates, and then calculates the EMI, total interest, and total payable amount.

The logic is based on common banking practices (inspired by RBI guidelines), but simplified so it’s easy to understand for learning purposes.

Features
Takes CIBIL score as input

Shows eligibility (CIBIL < 650 → Not eligible)

If eligible:

Takes loan amount

Shows multiple tenure options (12, 24, 36, 60 months)

Shows interest rates for each tenure

Calculates:

Monthly EMI

Total interest

Total amount to be paid

#How Interest Rate is Decided Based on CIBIL Score

650–699 → +2% extra interest

700–749 → +1% extra interest

750+ → No extra interest

Based on Loan Tenure

1–12 months → 10% per year

13–36 months → 11.5% per year

37+ months → 13% per year

Final interest = base rate + CIBIL risk add-on.

** EMI Formula Used 𝐸 𝑀 𝐼
𝑃 ⋅ 𝑟 ⋅ ( 1 + 𝑟 ) 𝑛 ( 1 + 𝑟 ) 𝑛 − 1 EMI= (1+r) n −1 P⋅r⋅(1+r) n​

Where:

P = loan amount

r = monthly interest rate

n = number of months

How to Run
Compile and run using GCC:

gcc loan_emi.c -o loan_emi ./loan_emi

Or just run directly in CodeBlocks / Dev-C++.

📂 Files loan_emi.c // Main C program README.md // Project documentation
CODE:
<img width="1356" height="3066" alt="code 2" src="https://github.com/user-attachments/assets/124da7b4-3769-4da9-8b43-d4c06bc1c5ba" />

OUTPUT:

<img width="1830" height="790" alt="Screenshot (3)" src="https://github.com/user-attachments/assets/59aa2064-a418-4311-bee0-7b50a6b619cd" />
