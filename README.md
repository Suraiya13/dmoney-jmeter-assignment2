# Dmoney JMeter Assignment 

## Topic
JMeter

## Description
This project contains a JMeter test plan (`dmoney.jmx`) for simulating transaction scenarios in the Dmoney API.

### Scenario
1. **Deposits:** 5 agents perform deposits for 10 customers.
2. **Send Money:** 5 customers send money to another 10 customers.
3. **Payments:** 5 customers make payments to 2 merchants.

### Implementation Details
- **Admin login:** A single login is used to generate a token for all threads.
- **CSV Data Files:** 
  - `deposit.csv` → agents and customers for deposits
  - `sendMoney.csv` → customers for sending money
  - `payment.csv` → customers and merchants for payments
- **Dynamic Amounts:** Random Variable Controller used to generate transaction amounts.
- **Thread Settings:** 
  - 3 threads for each type of transaction
  - Ramp-up time: 120 seconds
- **Assertions:** Added to ensure all transactions are successful.



### How to Run
1. Open `dmoney.jmx` in JMeter.
2. Make sure CSV files are in the `Resources/` folder.
3. Run the test plan (non-GUI recommended for large tests).
4. View results in the generated HTML report.

### HTML Reports 

<img width="1910" height="926" alt="Screenshot (107)" src="https://github.com/user-attachments/assets/2313be44-2c0a-4790-a86a-6200f69e16a5" />
