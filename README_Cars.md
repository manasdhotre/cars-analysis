# Car market analysis 🚗

Exploratory data analysis on **428 car models** across makes, types, origins, and specifications — uncovering what drives car pricing, fuel efficiency, and performance characteristics.

---

## Project overview

This project analyses the Cars dataset to answer key questions:
- Which car origins (USA, Asia, Europe) dominate the market by volume?
- What is the relationship between engine size and price?
- Do more cylinders mean higher horsepower — and does that always mean higher price?
- Which car types (Sedan, SUV, Sports, etc.) have the best fuel efficiency?
- How do Asian, European, and American cars compare in price and specs?
- Which manufacturers (Make) offer the best horsepower-to-price ratio?

---

## Dataset

| Property | Detail |
|---|---|
| Source | Cars Dataset (Kaggle / SAS) |
| Rows | 428 car models |
| Columns | 15 (Make, Model, Type, Origin, DriveTrain, MSRP, Invoice, EngineSize, Cylinders, Horsepower, MPG_City, MPG_Highway, Weight, Wheelbase, Length) |
| Price range | $10,280 – $192,465 (MSRP) |

---

## Tools & libraries

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-teal)
![NumPy](https://img.shields.io/badge/NumPy-1.24-yellow)

---

## Key findings

- **Asian cars dominate by volume** — the largest share of models in the dataset originate from Asia
- **European cars have the highest average MSRP** — luxury brands like BMW and Mercedes skew the average up
- **More cylinders strongly correlate with higher horsepower** — 8-cylinder cars average nearly 2× the HP of 4-cylinder
- **Sedans are the most fuel-efficient** type on average in both city and highway MPG
- **SUVs are the heaviest** vehicle type and have the lowest fuel efficiency
- **Horsepower and MSRP are positively correlated** — higher performance comes at a premium
- **Hybrid/front-wheel drive cars** show better MPG than all-wheel or rear-wheel drive configurations

---

## Data cleaning steps

- Cleaned `MSRP` and `Invoice` columns — removed `$` symbols and commas, converted to numeric
- Handled missing values in `Cylinders` and `Horsepower` columns
- Filtered dataset to remove sports/wagon types for focused Sedan vs SUV comparison
- Converted price strings to integers for numerical analysis

---

## Project structure

```
cars-market-analysis/
│
├── Cars_Analysis.ipynb               # Main analysis notebook
├── Project+2+-+Cars+Dataset.csv      # Dataset
├── requirements.txt                  # Python dependencies
└── README.md                         # This file
```

---

## How to run

1. Clone this repository
   ```bash
   git clone https://github.com/ManasDhotre/cars-market-analysis.git
   cd cars-market-analysis
   ```

2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter and open the notebook
   ```bash
   jupyter notebook Cars_Analysis.ipynb
   ```

> **Note:** The dataset path in cell 2 has been updated from `/content/...` to `./Project+2+-+Cars+Dataset.csv` for local use.

---

## Author

**Manas Dhotre**
Aspiring Data Scientist | Python · Pandas · Data Analysis
📍 Pune, India

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://linkedin.com/in/manas-dhotre)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/ManasDhotre)

---

## Acknowledgements

Dataset sourced from [Kaggle – Cars Dataset](https://www.kaggle.com/datasets/CooperUnion/cardataset)
