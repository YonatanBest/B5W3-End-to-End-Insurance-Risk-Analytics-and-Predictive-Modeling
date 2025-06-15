# B5W3: End-to-End Insurance Risk Analytics & Predictive Modeling

## Project Overview
This project aims to analyze historical car insurance claim data for AlphaCare Insurance Solutions (ACIS) in South Africa. The goal is to optimize marketing strategies and discover low-risk segments for premium reduction, using advanced analytics and predictive modeling.

## Objectives
- Perform exploratory data analysis (EDA) to uncover risk and profitability patterns.
- Statistically validate or reject key business hypotheses about risk drivers.
- Build predictive models for claim severity and premium optimization.
- Establish reproducible, auditable data pipelines using DVC.
- Deliver actionable insights and recommendations for ACIS's marketing and pricing strategy.

## Data Description
- **Time Range:** Feb 2014 to Aug 2015
- **Key Columns:**
  - Policy & Transaction: UnderwrittenCoverID, PolicyID, TransactionMonth
  - Client: IsVATRegistered, Citizenship, LegalType, Title, Language, Bank, AccountType, MaritalStatus, Gender
  - Location: Country, Province, PostalCode, MainCrestaZone, SubCrestaZone
  - Car: ItemType, Mmcode, VehicleType, RegistrationYear, Make, Model, Cylinders, Cubiccapacity, Kilowatts, Bodytype, NumberOfDoors, VehicleIntroDate, CustomValueEstimate, AlarmImmobiliser, TrackingDevice, CapitalOutstanding, NewVehicle, WrittenOff, Rebuilt, Converted, CrossBorder, NumberOfVehiclesInFleet
  - Plan: SumInsured, TermFrequency, CalculatedPremiumPerTerm, ExcessSelected, CoverCategory, CoverType, CoverGroup, Section, Product, StatutoryClass, StatutoryRiskType
  - Payment & Claim: TotalPremium, TotalClaims

## Project Structure
- `data/` - Raw and processed data files (tracked with DVC)
- `notebooks/` - Jupyter notebooks for EDA, modeling, and reporting
- `src/` - Source code for data processing, modeling, and utilities
- `reports/` - Generated reports and visualizations
- `dvc.yaml` - DVC pipeline definitions
- `README.md` - Project documentation

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/YonatanBest/B5W3-End-to-End-Insurance-Risk-Analytics-and-Predictive-Modeling.git
   cd B5W3-End-to-End-Insurance-Risk-Analytics-and-Predictive-Modeling
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Install DVC:
   ```bash
   pip install dvc
   dvc init
   ```
4. Configure DVC remote storage as per instructions in Task 2.

## Deliverables
- **Task 1:** EDA & Stats (Branch: `task-1`)
- **Task 2:** Data Version Control with DVC (Branch: `task-2`)
- **Task 3:** Hypothesis Testing (Branch: `task-3`)
- **Task 4:** Predictive Modeling (Branch: `task-4`)