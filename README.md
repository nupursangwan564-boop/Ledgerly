Ledgerly 💳
Detecting Forgotten and Recurring Subscriptions from Transaction Data
Ledgerly is a transaction-analysis platform designed to help users understand and monitor their recurring expenses.

It processes transaction data, identifies recurring payment patterns, tracks subscription history, detects increases in recurring charges, and highlights potentially dormant or forgotten subscriptions.

🎯 Problem Statement
CS03 – Detecting Forgotten and Recurring Subscriptions from Transaction Data

People often have multiple recurring payments and subscriptions, making it difficult to keep track of where their money is going. Some subscriptions may be forgotten, while recurring charges may increase without being noticed.

Ledgerly aims to analyze transaction history and provide meaningful insights into these recurring expenses.

💡 Solution
Ledgerly analyzes transaction records and performs rule-based transaction analysis to:

Identify merchants from transaction descriptions
Group transactions by merchant
Detect recurring payment patterns
Track recurring payment history
Calculate recurring monthly spending
Detect increases in recurring charges
Identify potentially dormant or forgotten recurring payments
Generate spending insights and alerts
Visualize recurring expenditure
Workflow
Transaction Data
       ↓
Data Loading
       ↓
Data Cleaning & Merchant Extraction
       ↓
Merchant & Category Identification
       ↓
Recurring Payment Detection
       ↓
Subscription Analysis
       ↓
Price-Hike / Dormant Charge Detection
       ↓
Insights & Alerts
       ↓
Visualization
🛠️ Technologies Used
Python
Pandas – Transaction data processing
Regex (re) – Merchant extraction and text processing
Matplotlib – Data visualization
CSV – Transaction data storage
⚙️ How It Works
1. Transaction Data Loading
Ledgerly loads transaction records from a CSV dataset and converts transaction dates into a suitable format for analysis.

2. Merchant Extraction
Transaction descriptions are cleaned using regular expressions and keyword-based logic to identify merchants.

3. Recurring Payment Detection
Transactions are grouped according to merchants. Merchants having repeated transactions are analyzed as potential recurring payments.

4. Subscription Analysis
For recurring payments, Ledgerly analyzes the latest payment amount, payment history, and total recurring expenditure.

5. Price-Hike Detection
The latest recurring payment amount is compared with the earlier amount to identify increases in subscription charges.

6. Dormant Charge Detection
Certain recurring charges can be flagged as potentially dormant or forgotten based on the available transaction information.

7. Visualization
Recurring expenditure and detected alerts are represented using charts for easier understanding.

📊 Sample Transaction Categories
The current prototype works with transaction examples such as:

Netflix
Spotify
Cult.fit
Adobe
Uber
Blinkit
The dataset contains both recurring subscriptions and one-time transactions for analysis.

📈 Key Features
Recurring payment detection
Subscription history tracking
Merchant identification
Recurring spending analysis
Price-hike detection
Dormant/forgotten charge identification
Spending summaries
Visual representation of recurring expenditure
Alert generation
🚀 Future Scope
Ledgerly can be further enhanced with:

Real bank statement integration
Support for multiple transaction formats
More advanced subscription detection
Machine-learning-based pattern detection
Personalized spending recommendations
Automated subscription cancellation assistance
Interactive web dashboard
Larger and more diverse transaction datasets
🧪 Current Implementation
The current prototype uses rule-based transaction analysis rather than a machine-learning model.

The system currently demonstrates the core concept using transaction data stored in CSV format.

👥 Team
Team AKIRA
Problem Statement: CS03
Theme: FinTech
Project: Ledgerly

🔗 Project
Ledgerly Website:
https://price-hike-detector.preview.emergentagent.com/

📚 References
Pandas Documentation
Matplotlib Documentation
Research and open-source projects related to financial transaction analysis and recurring payment detection
📌 Project Status
Prototype / Hackathon Project

Ledgerly is currently being developed and enhanced with additional transaction history and features.
