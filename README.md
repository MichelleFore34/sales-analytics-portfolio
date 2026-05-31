# SaaS Sales Analytics

Exploratory analysis of a SaaS company's sales data to identify 
revenue drivers, profitability gaps, and discounting patterns 
across products and customer segments.

## Business Question

Which products and customer segments drive the most revenue — 
and where is profitability being eroded by discounting?

This is a question every SaaS revenue or analytics team needs 
to answer regularly. Discount creep and unprofitable products 
are two of the most common and costly problems in SaaS sales.

## Key Findings

- **SMB drives volume, Enterprise drives value**: SMB accounts 
  for the largest share of total revenue, but Enterprise deals 
  have the highest average sale and profit per transaction.

- **ContactMatcher has a discounting problem**: Average discount 
  of 35% — the highest in the portfolio — resulting in razor-thin 
  margins despite being the top revenue product.

- **Marketing Suite is structurally unprofitable**: The only 
  product with negative total profit. Even at a moderate 21% 
  average discount, it loses money on the average deal — 
  suggesting a pricing or cost issue, not just a sales behavior issue.

- **Alchemy is the star**: Low discounting (16%) and the highest 
  average profit per deal ($817). The pricing and sales motion 
  here should be the model for the rest of the portfolio.

## Tools

- Python 3
- pandas
- matplotlib
- seaborn
- Jupyter Notebooks

## How to Run

1. Clone the repo:
```bash
git clone https://github.com/MichelleFore34/sales-analytics-portfolio.git
cd sales-analytics-portfolio
```

2. Download the dataset from Kaggle and save it to `data/SaaS_Sales.csv`

3. Set up your environment:
```bash
python3 -m venv venv
source venv/bin/activate
pip install pandas matplotlib seaborn jupyter
```

4. Launch Jupyter:
```bash
jupyter notebook
```

5. Open `notebooks/01_exploration.ipynb` and run all cells

## Data

Download the [AWS SaaS Sales Dataset](https://www.kaggle.com/datasets/nnthanh101/aws-saas-sales) 
from Kaggle and save the file as `data/SaaS_Sales.csv` in the project root.

The data folder is excluded from this repo — the dataset is publicly available on Kaggle.

## Next Steps

- Regional analysis: which geographies are most and least profitable?
- Churn risk modeling: which customer profiles are highest risk?
- Discount threshold analysis: at what discount level do deals 
  become unprofitable by product?