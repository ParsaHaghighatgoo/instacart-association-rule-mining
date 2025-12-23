## Task 5 – Question 2: Conceptual Questions

### What is the role of *Lift* in association rule mining?

Lift is one of the most important evaluation metrics in association rule mining.  
It measures how much more frequently the antecedent and consequent occur together compared to what would be expected if they were statistically independent.

Formally, lift is defined as:

Lift(A → B) = Confidence(A → B) / Support(B)

Interpretation:
- **Lift > 1**: Positive association (items occur together more than expected)
- **Lift = 1**: No association (items are independent)
- **Lift < 1**: Negative association (items occur together less than expected)

Unlike confidence, lift accounts for the popularity of the consequent item.  
This makes lift especially valuable in e-commerce applications, where some products (e.g., bananas) are very popular and could otherwise produce misleading rules.

In practice, rules with high lift represent truly meaningful relationships and are ideal for recommendations and cross-selling strategies.

---

### Why is the Apriori algorithm important for e-commerce stores?

The Apriori algorithm is important for e-commerce stores because it enables the discovery of hidden purchasing patterns from large volumes of transactional data.

Key reasons include:

- **Understanding customer behavior:**  
  Apriori identifies which products are frequently purchased together, revealing natural buying habits.

- **Improving recommender systems:**  
  The extracted association rules can be directly used to recommend complementary products in real time.

- **Increasing sales through cross-selling:**  
  By identifying strong product associations, stores can design effective “frequently bought together” offers.

- **Data-driven decision making:**  
  Apriori provides an interpretable and rule-based approach that business teams can easily understand and act upon.

- **Scalability to large datasets:**  
  Apriori is designed to work efficiently on large transactional datasets, making it suitable for real-world e-commerce platforms.

Overall, Apriori helps transform raw purchase data into actionable business knowledge that improves customer experience and increases revenue.
