# Instacart Association Rule Mining

A comprehensive market basket analysis project using the Instacart dataset to discover product purchase patterns and association rules through the Apriori algorithm.

## 📋 Overview

This project performs association rule mining on Instacart's e-commerce transaction data to uncover meaningful product relationships and co-purchase patterns. The analysis helps identify which products are frequently bought together, enabling data-driven recommendations and business insights.

## 🎯 Objectives

- Analyze customer purchase behavior using market basket analysis
- Extract frequent itemsets using the Apriori algorithm
- Generate association rules with support, confidence, and lift metrics
- Provide actionable business insights for e-commerce optimization

## 📊 Dataset

The project uses the **Instacart Market Basket Analysis** dataset, which includes:

- **aisles.csv**: Aisle information (134 aisles)
- **departments.csv**: Department information (21 departments)
- **products.csv**: Product details (49,688 products)
- **orders.csv**: Order metadata (3.4M+ orders)
- **order_products__prior.csv**: Prior order products (32M+ records)
- **order_products__train.csv**: Training order products (1.4M+ records)

### Sample Size
The analysis uses a sample of **20,000 orders** containing **210,733 product transactions** across **21,948 unique products**.

## 🛠️ Technologies & Libraries

- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computations
- **mlxtend**: Apriori algorithm and association rule mining
- **networkx**: Graph-based analysis (optional)
- **matplotlib**: Data visualization

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/ParsaHaghighatgoo/instacart-association-rule-mining.git
cd instacart-association-rule-mining
```

2. Create a virtual environment (recommended):
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install required dependencies:
```bash
pip install -r requirements.txt
```

## 🚀 Usage

Run the Jupyter notebook to perform the complete analysis:

```bash
jupyter notebook main.ipynb
```

### Analysis Pipeline

1. **Data Loading**: Load and explore the Instacart dataset
2. **Data Preprocessing**: 
   - Filter orders with at least 2 products
   - Merge product names with transaction data
   - Sample 20,000 orders for analysis
3. **Basket Creation**: Transform transactions into market baskets
4. **Apriori Algorithm**: Extract frequent itemsets with different support thresholds
5. **Association Rules**: Generate rules with confidence and lift metrics
6. **Visualization**: Create charts and graphs for insights
7. **Business Interpretation**: Translate findings into actionable recommendations

## 📈 Key Findings

### Frequent Itemsets
- **min_support = 0.01**: 128 frequent itemsets (max size: 2)
- **min_support = 0.05**: 7 frequent itemsets (max size: 1)

### Top Association Rules

The strongest associations (by lift) include:
- **Organic Raspberries → Organic Strawberries** (lift ≈ 2.95)
- Strong co-purchase patterns among organic fruits
- High correlation between complementary produce items

### Metrics Explained

- **Support**: Frequency of itemset occurrence in transactions
- **Confidence**: Conditional probability of consequent given antecedent
- **Lift**: Strength of association (lift > 1 indicates positive correlation)

## 💼 Business Applications

1. **Product Recommendations**: Real-time suggestions based on cart contents
2. **Cross-Selling & Bundling**: Create "Frequently Bought Together" offers
3. **Targeted Promotions**: Offer discounts on associated products
4. **Website Optimization**: Place related products closer together
5. **Inventory Management**: Forecast demand for associated products

## 📁 Project Structure

```
instacart-association-rule-mining/
├── main.ipynb                              # Main analysis notebook
├── requirements.txt                        # Python dependencies
├── README.md                               # Project documentation
├── .gitignore                              # Git ignore rules
├── EC-hw3.pdf                              # Assignment description
├── instacart_association_rule_mining_doc.pdf  # Detailed documentation
├── e_commerce_HW3_dataset/                 # Dataset folder
│   ├── aisles.csv
│   ├── departments.csv
│   ├── products.csv
│   ├── orders.csv
│   ├── order_products__prior.csv
│   └── order_products__train.csv
├── Docs/                                   # Analysis documentation
│   ├── Task3_questions.md
│   ├── Task4_Association Rules Analysis.md
│   ├── Task5_BusinessInterpretation.md
│   ├── Task5_Question2.md
│   └── Task5_Question3.md
└── figures/                                # Visualization outputs
    ├── 1.png
    ├── 2.png
    ├── 3.png
    ├── 4.png
    └── top_items.png
```

## 📚 Documentation

Detailed analysis and findings are available in the `Docs/` folder:

- **Task 3**: Conceptual questions about support thresholds
- **Task 4**: Association rules analysis and metrics
- **Task 5**: Business interpretation and practical applications

## 📊 Visualizations

The project includes several visualizations in the `figures/` directory:
- Top frequent items bar charts
- Association rule network graphs
- Support vs. confidence scatter plots
- Itemset distribution analysis

## 🔍 Results

The analysis demonstrates that:
- Lower support thresholds (0.01) reveal more meaningful multi-item patterns
- Organic produce shows strong co-purchase associations
- Lift metric is crucial for identifying truly meaningful relationships
- Association rules can drive significant business value in e-commerce

## 📄 License

This project is part of an academic assignment for educational purposes.

## 👤 Author

**Parsa Haghighatgoo**

## 🙏 Acknowledgments

- Dataset provided by Instacart
- Course: E-Commerce (EC-HW3)
- Institution: CSE Program, Term 9

## 📞 Contact

For questions or feedback, please open an issue in the repository.

---

**Note**: This project is for educational purposes and demonstrates the application of association rule mining techniques in e-commerce analytics.
