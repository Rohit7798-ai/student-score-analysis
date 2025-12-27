# Student Score Analysis

> A  data analysis project examining the relationships between student demographics, family background, study habits, and academic performance across 30,000+ student records.

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-Complete-success.svg)

---

## Overview

This project analyzes educational data to understand the factors that influence student academic performance. By examining various demographic, socioeconomic, and behavioral variables, we identify significant patterns and correlations that affect student success in Math, Reading, and Writing.

### Research Questions

- How does parental education level impact student performance?
- What role do study hours play in academic achievement?
- Are there gender-based differences in subject performance?
- Does socioeconomic status (indicated by lunch type) affect grades?
- Do family structure variables influence academic outcomes?

---

## Key Findings

### 1. Parental Education Impact

Students whose parents hold higher educational degrees demonstrate significantly better academic performance across all subjects.

- **Master's degree holders' children**: Math 72.3 | Reading 75.8 | Writing 76.4
- **High school graduates' children**: Math 64.4 | Reading 67.2 | Writing 65.4
- **Performance gap**: Approximately 8-11 points across subjects

**Conclusion**: Parental education level shows a strong positive correlation with student achievement.

### 2. Study Hours Correlation

Weekly study time demonstrates a clear relationship with academic performance.

- **More than 10 hours/week**: Math 68.7 | Reading 70.4 | Writing 69.8
- **5-10 hours/week**: Math 66.9 | Reading 69.7 | Writing 68.6
- **Less than 5 hours/week**: Math 64.6 | Reading 68.2 | Writing 67.1

**Conclusion**: Increased study time correlates with improved academic outcomes.

### 3. Gender Performance Patterns

Analysis reveals distinct performance patterns between male and female students.

- **Female students**: Math 64.1 | Reading 72.9 | Writing 72.9
- **Male students**: Math 69.1 | Reading 65.9 | Writing 63.9

**Conclusion**: Female students excel in language-based subjects while male students show strength in mathematics.

### 4. Socioeconomic Indicators

Lunch type serves as a proxy for family income and shows significant performance differences.

- **Standard lunch**: Math 70.7 | Reading 72.2 | Writing 71.5
- **Free/reduced lunch**: Math 58.9 | Reading 64.2 | Writing 62.7
- **Performance gap**: 9-12 points across subjects

**Conclusion**: Socioeconomic factors significantly influence academic performance.

### 5. Non-Significant Factors

The following variables showed minimal or no correlation with academic performance:

- Parental marital status
- Number of siblings
- Birth order (first child vs. others)

---

## Dataset Information

**Total Records**: 30,641 students  
**Features**: 15 variables per student  
**Missing Data**: Present in several columns, handled appropriately in analysis

### Dataset Structure

**Demographic Variables**:
- Gender
- Ethnic Group (Groups A-E)

**Family Background**:
- Parent Education Level
- Parent Marital Status
- Number of Siblings
- First Child Status

**Socioeconomic Indicators**:
- Lunch Type (Standard vs. Free/Reduced)
- Transportation Method

**Academic Behavior**:
- Weekly Study Hours
- Test Preparation Course Completion
- Sports Practice Frequency

**Performance Metrics**:
- Math Score (0-100)
- Reading Score (0-100)
- Writing Score (0-100)

---

## Technical Implementation

### Technologies Used

- **Python 3.7+** - Core programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical graphics

### Analytical Approach

1. **Data Exploration**: Initial inspection of dataset structure and quality
2. **Data Cleaning**: Identification and handling of missing values
3. **Descriptive Statistics**: Summary statistics for all variables
4. **Group Analysis**: Performance comparisons across different categories
5. **Visualization**: Creation of charts and heatmaps for pattern identification

---

## Installation and Setup

### Prerequisites

- Python 3.7 or higher
- pip package manager

### Installation Steps

**1. Clone the Repository**
```bash
git clone https://github.com/yourusername/student-score-analysis.git
cd student-score-analysis
```

**2. Install Dependencies**
```bash
pip install -r requirements.txt
```

**3. Prepare Dataset**
- Place your CSV file in the project directory
- Update the file path in `analysis.py`:
```python
df = pd.read_csv("Expanded_data_with_more_features.csv")
```

**4. Execute Analysis**
```bash
python analysis.py
```

---

## Project Structure

```
student-score-analysis/
│
├── analysis.py                          # Main analysis script
├── Expanded_data_with_more_features.csv # Dataset (not included)
├── README.md                            # Project documentation
├── requirements.txt                     # Python dependencies
└── .gitignore                          # Git ignore rules
```

---

## Visualizations Generated

The analysis produces the following visualizations:

- **Count Plots**: Gender and ethnic group distributions
- **Heatmaps**: Correlation between categorical variables and scores
- **Box Plots**: Score distributions for Math, Reading, and Writing
- **Bar Charts**: Comparative performance across different groups
- **Pie Charts**: Ethnic group representation

---

## Data Quality Notes

The dataset contains missing values in several columns:

- EthnicGroup: 1,840 missing (6.0%)
- ParentEduc: 1,845 missing (6.0%)
- TransportMeans: 3,134 missing (10.2%)
- TestPrep: 1,830 missing (6.0%)
- Other variables have less than 5% missing data

Analysis methods account for these missing values appropriately.

---

## Use Cases

This project is valuable for:

- **Educational Researchers**: Understanding factors affecting student success
- **Data Science Students**: Learning practical data analysis techniques
- **Policy Makers**: Identifying areas requiring educational intervention
- **Educators**: Recognizing patterns in student performance
- **Data Analysts**: Practicing exploratory data analysis

---

## Contributing

Contributions are welcome and appreciated. To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/Enhancement`)
3. Commit your changes (`git commit -m 'Add new analysis'`)
4. Push to the branch (`git push origin feature/Enhancement`)
5. Open a Pull Request

### Contribution Ideas

- Additional statistical tests
- Machine learning predictive models
- Interactive visualizations
- Code optimization and documentation
- Extended analysis of specific variables

---

