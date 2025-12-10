# Customer Satisfaction Prediction

A machine learning project to predict customer satisfaction ratings from support ticket data.

## About

This project analyzes customer support tickets to understand what factors influence satisfaction and builds predictive models. It's part of my Data Science internship work.

## Dataset

The dataset contains ~8,500 customer support tickets with information like:
- Customer demographics (age, gender)
- Product purchased
- Ticket details (type, subject, priority, channel)
- Resolution time
- Satisfaction rating (1-5)

## Project Structure

```
├── Customer_Satisfaction_Prediction.ipynb   # Main analysis notebook
├── customer_support_tickets.csv             # Dataset
├── outputs/
│   ├── cleaned_data.csv                     # Processed data
│   ├── model_results.csv                    # Model comparison
│   ├── feature_importance.csv               # Feature rankings
│   └── visualizations/                      # All plots
│       ├── 01_satisfaction_distribution.png
│       ├── 02_satisfaction_by_category.png
│       ├── 03_customer_demographics.png
│       ├── 04_ticket_analysis.png
│       ├── 05_resolution_time.png
│       ├── 06_correlation_matrix.png
│       ├── 07_satisfaction_heatmap.png
│       ├── 08_model_comparison.png
│       ├── 09_confusion_matrix.png
│       ├── 10_feature_importance.png
│       └── 11_dashboard.png
├── requirements.txt
└── README.md
```

## What I Did

1. **Data Cleaning** - Handled missing values, converted dates, removed duplicates
2. **Feature Engineering** - Created new features like resolution time, age groups, description length
3. **EDA** - Explored patterns through 11 visualizations
4. **Modeling** - Trained 5 different ML models:
   - Logistic Regression
   - Decision Tree
   - Random Forest
   - Gradient Boosting
   - K-Nearest Neighbors
5. **Evaluation** - Compared models and analyzed feature importance

## Key Findings

- Average customer satisfaction is around 3/5
- Resolution time and product type are important predictors
- All support channels (email, phone, chat, social media) are roughly equally used
- Technical issues generate the most tickets

## How to Run

1. Clone this repo
2. Install dependencies: `pip install -r requirements.txt`
3. Open the notebook and run all cells
4. Check the `outputs/` folder for results

## Requirements

- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Results

The models achieved around 20-22% accuracy on this 5-class classification problem. This is actually reasonable given:
- 5 classes to predict
- Random baseline would be 20%
- The data has inherent noise

See the dashboard (`outputs/visualizations/11_dashboard.png`) for a summary of all findings.

## Contact

Feel free to reach out if you have questions or suggestions!

---
*This project was completed as part of a Data Science internship.*
