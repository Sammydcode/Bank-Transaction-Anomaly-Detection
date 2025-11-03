# Bank Transaction Anomaly Detection

## Project Overview
This project focuses on developing a machine learning model to detect anomalous transactions in bank transfer data. The system analyzes various transaction features to identify potentially fraudulent activities and flag suspicious transactions for further investigation.

## Objectives
1. **Data Curation and Processing**: Clean, preprocess, and explore bank transaction data
2. **Machine Learning Model Development**: Build and train anomaly detection algorithms
3. **Model Evaluation**: Assess performance using precision, F1 score, and other relevant metrics

## Dataset
The project uses a comprehensive bank transactions dataset (`bank_transactions_data_2.csv`) containing 2,512 records with 16 features including:

### Key Features:
- `TransactionID`: Unique identifier for each transaction
- `AccountID`: Customer account identifier
- `TransactionAmount`: Monetary value of transaction
- `TransactionDate`: Date and time of transaction
- `TransactionType`: Debit/Credit classification
- `Location`: Geographic location of transaction
- `DeviceID`: Device used for transaction
- `IP Address`: IP address of transaction origin
- `MerchantID`: Merchant identifier
- `Channel`: Transaction channel (ATM, Online, Branch)
- `CustomerAge`: Age of customer
- `CustomerOccupation`: Occupation category
- `TransactionDuration`: Duration of transaction process
- `LoginAttempts`: Number of login attempts
- `AccountBalance`: Current account balance
- `PreviousTransactionDate`: Timestamp of last transaction

## Technical Implementation

### Technologies Used
- **Python 3.13.4**
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Data visualization
- **Datetime**: Date/time handling
- **Jupyter Notebook**: Interactive development environment

### Key Analysis Steps

#### 1. Data Loading & Initial Inspection
- Loaded dataset with 2,512 transactions and 16 features
- Performed initial data exploration and statistical analysis
- Created backup of raw data for reference

#### 2. Data Cleaning & Preprocessing
- Converted date columns to proper datetime format
- Checked for duplicates and missing values
- Validated data integrity and format consistency

#### 3. Exploratory Data Analysis (EDA)
- **Transaction Amount Distribution**: Highly right-skewed with most transactions below ₦250
- **Hourly Transaction Patterns**: Peak activity at 4:00 PM (~1,300 transactions)
- **Time-based Analysis**: Transaction frequency analysis across different hours

#### 4. Feature Engineering
- Time-based features extraction
- Transaction pattern analysis
- Customer behavior profiling

## Key Insights

### Transaction Patterns:
- **Peak Hours**: Highest transaction volume occurs at 4:00 PM
- **Amount Distribution**: Majority of transactions are small-value (<₦250)
- **Activity Decline**: Transaction frequency decreases steadily after peak hours

### Data Quality:
- No missing values or duplicates found
- Clean dataset with proper formatting
- Consistent data types across features

## Model Development (Planned)

### Anomaly Detection Approaches:
- Isolation Forest
- Local Outlier Factor (LOF)
- One-Class SVM
- Autoencoders

### Evaluation Metrics:
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix Analysis

## Project Structure

bank-transaction-anomaly-detection/
├── bank_transaction_anormaly_detction.ipynb
├── bank_transactions_data_2.csv
├── README.md
└── requirements.txt



## 🛠️ Installation & Setup

### Prerequisites
- Python 3.7+
- Jupyter Notebook
- Required Python packages (see requirements.txt)

### Installation Steps
```bash
# Clone the repository
git clone https://github.com/Sammydcode/Bank-Transaction-Anomaly-Detection.git

# Navigate to project directory
cd Bank-Transaction-Anomaly-Detection

# Install required packages
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook
```

### Usage
- Open bank_transaction_anormaly_detction.ipynb in Jupyter Notebook

- Run cells sequentially to reproduce the analysis

- Modify parameters and experiment with different anomaly detection algorithms

- Evaluate model performance on the transaction dataset

### Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for suggestions and improvements.


### Authors
[Amadasun Samuel] - Initial work and development

### Acknowledgments
- Dataset provided for educational purposes

- Inspired by real-world financial fraud detection systems

- Built using open-source Python data science libraries

  
#### This README provides:
- Clear project overview and objectives
- Comprehensive dataset description
- Technical implementation details
- Key findings and insights
- Setup and usage instructions
- Professional structure for GitHub presentation
