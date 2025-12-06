## 🎯 Business Objective
Your employer, **AlphaCare Insurance Solutions (ACIS)**, is committed to developing cutting-edge risk and predictive analytics in car insurance planning and marketing in South Africa. As a newly joined marketing analytics engineer, your first project is to analyze historical insurance claim data to:

- **Optimize marketing strategy**
- Discover **"low-risk" targets** for premium reduction
- Create opportunities to attract new clients
- Build smart models that optimize premiums

---

## 🚀 Project Motivation
This challenge sharpens skills in three key areas:
- **Data Engineering (DE)**
- **Predictive Analytics (PA)**
- **Machine Learning Engineering (MLE)**

The tasks simulate real-world pressures and deadlines typical in financial analytics, improving your ability to:
- Manage complex datasets
- Adapt to challenges
- Think creatively
- Apply hypothesis testing and predictive analytics in insurance

---

## 📊 Data Description
**Historical Data Period**: February 2014 to August 2015  
**Data Location**: [Provided data file - raw_data.txt]

### Data Structure Categories:

#### 1. Insurance Policy Columns
- `UnderwrittenCoverID`, `PolicyID`

#### 2. Transaction Date
- `TransactionMonth`

#### 3. Client Information
- `IsVATRegistered`, `Citizenship`, `LegalType`, `Title`, `Language`, `Bank`
- `AccountType`, `MaritalStatus`, `Gender`

#### 4. Client Location
- `Country`, `Province`, `PostalCode`, `MainCrestaZone`, `SubCrestaZone`

#### 5. Car Insured
- `ItemType`, `Mmcode`, `VehicleType`, `RegistrationYear`, `Make`, `Model`
- `Cylinders`, `Cubiccapacity`, `Kilowatts`, `Bodytype`, `NumberOfDoors`
- `VehicleIntroDate`, `CustomValueEstimate`, `AlarmImmobiliser`, `TrackingDevice`
- `CapitalOutstanding`, `NewVehicle`, `WrittenOff`, `Rebuilt`, `Converted`
- `CrossBorder`, `NumberOfVehiclesInFleet`

#### 6. Insurance Plan
- `SumInsured`, `TermFrequency`, `CalculatedPremiumPerTerm`, `ExcessSelected`
- `CoverCategory`, `CoverType`, `CoverGroup`, `Section`, `Product`
- `StatutoryClass`, `StatutoryRiskType`

#### 7. Payment & Claim
- `TotalPremium`, `TotalClaims`

---

## 🎓 Learning Outcomes
By completing this project, you will demonstrate proficiency in:

1. **Data Understanding & Insight Extraction**
   - EDA techniques, statistical distributions, sampling, visualization
   - Data structure and algorithm understanding in ML pipelines

2. **Software Engineering Best Practices**
   - Modular and object-oriented Python code
   - Python package building

3. **Statistical Modeling & Analysis**
   - Statistical models for A/B test outcomes
   - Logistic regression, chi-squared tests

4. **A/B Testing Design & Implementation**
   - Robust A/B test design with clear metrics
   - Sample size determination, control/test group selection

5. **Data Versioning**
   - Dataset and analysis result version management
   - DVC (Data Version Control) implementation

---

## ✅ Project Tasks

### **Task 1: Git, GitHub & EDA**
- Create Git repository with good README
- Git version control & CI/CD with GitHub Actions
- Exploratory Data Analysis (EDA) with statistical thinking
- **Minimum Essential**: Create `task-1` branch, commit 3x daily, perform comprehensive EDA

### **Task 2: Data Version Control (DVC)**
- Establish reproducible data pipeline using DVC
- Initialize DVC with local remote storage
- Version control datasets for auditability
- **Minimum Essential**: Merge `task-1` to main, create `task-2` branch, DVC setup

### **Task 3: A/B Hypothesis Testing**
- Statistically validate/reject key hypotheses about risk drivers
- Test 4 null hypotheses about risk differences across provinces, zip codes, gender
- **Minimum Essential**: Statistical testing with clear business recommendations

### **Task 4: Statistical Modeling**
- Build predictive models for dynamic, risk-based pricing
- Claim Severity Prediction (Risk Model)
- Premium Optimization (Pricing Framework)
- **Minimum Essential**: Data preparation, model building, evaluation, SHAP/LIME interpretation

📁 Project Structure
insurance-analytics-predictive-modeling/
├── data/
│   ├── raw/                   # Original data files (gitignored)
│   │   └── raw_data.txt      # 500MB insurance data
│   └── processed/            # Processed datasets (gitignored)
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_eda_analysis.ipynb
│   ├── 03_hypothesis_testing.ipynb
│   └── 04_modeling.ipynb
├── src/
│   ├── __init__.py
│   ├── data_preprocessing.py
│   ├── hypothesis_testing.py
│   └── modeling.py
├── .github/workflows/
│   └── python-ci.yml         # CI/CD pipeline
├── README.md                 # This file
├── requirements.txt          # Python dependencies
└── .gitignore               # Git ignore rules