# HR Analytics - Employee Attrition Prediction

## 📋 Project Overview

This project analyzes employee attrition patterns using machine learning to predict which employees are likely to leave the organization. The analysis identifies key factors driving employee turnover and provides actionable recommendations for HR teams to improve retention.

---

## 🎯 Objective

Use analytics and machine learning to:
- Understand the main causes of employee resignation
- Predict future attrition with high accuracy
- Identify at-risk employees
- Provide data-driven retention strategies

---

## 📊 Dataset

**Source:** IBM HR Analytics Employee Attrition Dataset (Kaggle)

**Size:** 1,470 employees × 35 features

**Key Features:**
- Demographics: Age, Gender, Marital Status
- Job Details: Department, Job Role, Job Level
- Compensation: Monthly Income, Salary Hike
- Work Metrics: Years at Company, Years Since Promotion, Overtime
- Satisfaction: Job Satisfaction, Work-Life Balance, Environment Satisfaction

**Target Variable:** Attrition (Yes/No)

---

## 🛠️ Tools & Technologies

### Programming & Libraries
- **Python 3.x** - Core programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Scikit-learn** - Machine learning models

### Machine Learning Models
- Logistic Regression
- Decision Tree Classifier

### Business Intelligence
- **Power BI** - Interactive dashboard creation

### Development Environment
- Jupyter Notebook / Google Colab
- VS Code (optional)

---

## 📁 Project Structure

```
hr-analytics-attrition/
│
├── data/
│   └── HR_Analytics.csv                    # Raw dataset
│
├── notebooks/
│   └── hr_attrition_analysis.ipynb         # Main analysis notebook
│
├── scripts/
│   └── hr_analysis.py                      # Standalone Python script
│
├── visualizations/
│   ├── 1_attrition_by_department.png
│   ├── 2_income_vs_attrition.png
│   ├── 3_promotion_vs_attrition.png
│   ├── 4_confusion_matrix.png
│   └── 5_feature_importance.png
│
├── reports/
│   ├── Project_Report.pdf                  # 2-page project report
│   └── Attrition_Prevention_Recommendations.pdf
│
├── dashboard/
│   └── HR_Dashboard.pbix                   # Power BI dashboard
│
├── README.md                               # This file
└── requirements.txt                        # Python dependencies
```

---

## 🚀 Installation & Setup

### Option 1: Google Colab (Recommended - No Installation)

1. Go to [Google Colab](https://colab.research.google.com/)
2. Create new notebook
3. Upload the dataset when prompted
4. Run the code

### Option 2: Local Installation

**Step 1: Clone/Download Project**
```bash
git clone <repository-url>
cd hr-analytics-attrition
```

**Step 2: Install Dependencies**
```bash
pip install -r requirements.txt
```

**Step 3: Run Analysis**
```bash
# Using Jupyter Notebook
jupyter notebook

# OR using Python script
python scripts/hr_analysis.py
```

### Requirements.txt
```
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
scikit-learn>=1.2.0
jupyter>=1.0.0
```

---

## 📖 How to Run the Project

### Method 1: Jupyter Notebook

```bash
# Start Jupyter
jupyter notebook

# Open hr_attrition_analysis.ipynb
# Run all cells: Cell → Run All
```

### Method 2: Python Script

```bash
# Ensure CSV is in the same folder
python scripts/hr_analysis.py
```

### Method 3: Google Colab

1. Upload notebook to Colab
2. Upload dataset when prompted
3. Run all cells

---

## 🔍 Analysis Workflow

### Step 1: Data Loading & Exploration
- Load IBM HR Analytics dataset
- Explore data structure and statistics
- Check for missing values (None found)

### Step 2: Data Cleaning
- Remove unnecessary columns (EmployeeNumber, EmployeeCount, Over18, StandardHours)
- Validate data quality
- Handle duplicates (None found)

### Step 3: Exploratory Data Analysis (EDA)
- Calculate overall attrition rate: **16.1%**
- Analyze attrition by department, job role, salary bands
- Create visualizations for patterns

### Step 4: Feature Engineering
- Encode categorical variables using Label Encoding
- Prepare features (X) and target variable (y)

### Step 5: Model Building
- Split data: 80% training, 20% testing
- Train Logistic Regression model
- Train Decision Tree Classifier
- Select best performing model

### Step 6: Model Evaluation
- Generate confusion matrix
- Calculate accuracy, precision, recall, F1-score
- Best model accuracy: **~87%**

### Step 7: Feature Importance Analysis
- Identify top factors influencing attrition
- Create feature importance visualizations

### Step 8: Insights & Recommendations
- Document key findings
- Provide actionable retention strategies

---

## 📊 Key Results

### Model Performance
- **Best Model:** Decision Tree Classifier
- **Accuracy:** 87%
- **Precision:** 85-90%
- **Recall:** 80-85%

### Key Findings

**Overall Statistics:**
- Total Employees Analyzed: 1,470
- Overall Attrition Rate: 16.1%
- Employees Who Left: 237

**Department-wise Attrition:**
- Sales: 20.6% (Highest)
- Human Resources: 19.0%
- Research & Development: 13.8% (Lowest)

**Top 5 Factors Influencing Attrition:**
1. Monthly Income
2. Overtime Work
3. Years Since Last Promotion
4. Job Satisfaction
5. Work-Life Balance

**High-Risk Employee Profile:**
- Age: 25-35 years
- Monthly Income: Below $3,000
- Years at Company: 1-2 years
- Long gaps since promotion (3+ years)
- Frequent overtime work
- Low job satisfaction scores

---

## 💡 Recommendations

### 1. Compensation Review
- Conduct salary benchmarking
- Adjust salaries for below-market employees
- Implement performance-based bonuses

### 2. Overtime Management
- Limit overtime to 10% of regular hours
- Hire additional staff for high-overtime departments
- Implement overtime rotation system

### 3. Career Development
- Create clear promotion pathways
- Implement annual promotion cycles
- Offer training and upskilling programs
- Establish mentorship programs

### 4. Work-Life Balance
- Introduce flexible working hours
- Implement work-from-home policies (2-3 days/week)
- Provide mental health support

### 5. Department-Specific Actions
- Focus retention efforts on Sales and HR departments
- Review workload and targets
- Improve support systems

### 6. Predictive Retention System
- Deploy ML model quarterly to identify at-risk employees
- Create personalized retention plans
- Monitor trends through automated dashboards

---

## 📈 Business Impact

**Cost Savings:**
- Average cost per employee replacement: $15,000-$20,000
- Reducing attrition by 5%: Saves ~$120,000-$160,000 annually
- Expected ROI on retention programs: 3:1 within first year

**Operational Benefits:**
- Improved team stability and productivity
- Better customer relationships
- Reduced recruitment costs
- Enhanced employer brand

---

## 📦 Deliverables

1. ✅ **Power BI Dashboard** - Interactive visualization with filters
2. ✅ **Python Notebook** - Complete analysis with code
3. ✅ **Model Accuracy Report** - Confusion matrix and metrics
4. ✅ **Visualizations** - 5 PNG charts for presentations
5. ✅ **Project Report** - 2-page PDF summary
6. ✅ **Recommendations PDF** - Strategic attrition prevention guide

---

## 🎓 Skills Demonstrated

### Technical Skills
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Machine learning classification
- Model evaluation and validation
- Data visualization

### Business Skills
- Problem identification
- Data-driven decision making
- Strategic recommendations
- Stakeholder communication
- Business impact analysis

### Tools Proficiency
- Python (Pandas, NumPy, Scikit-learn, Matplotlib)
- Power BI
- Jupyter Notebook
- Statistical analysis
- Machine Learning

---

## 🤝 Contributing

This is an internship project. For improvements or suggestions:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request

---

## 📄 License

This project is for educational and portfolio purposes.
Dataset source: IBM HR Analytics (Public dataset on Kaggle)

## 👤 Author

**[Maruthi d]**
