## Task 4 – Association Rules Analysis

### Support
Support measures how frequently an itemset appears in the dataset. In association rules, it represents the proportion of transactions that contain both the antecedent and the consequent.

Rules with very low support may not be reliable, while rules with higher support indicate commonly occurring product combinations.

---

### Confidence
Confidence represents the conditional probability that the consequent is purchased given that the antecedent is purchased.

A high confidence value means that when customers buy the antecedent product, they are likely to also buy the consequent product. However, confidence alone does not account for the overall popularity of the consequent.

---

### Lift
Lift measures how much more often the antecedent and consequent occur together compared to what would be expected if they were independent.

- Lift > 1 indicates a positive association
- Lift = 1 indicates independence
- Lift < 1 indicates a negative association

Lift is the most important metric for evaluating association rules because it accounts for item popularity and reveals truly meaningful relationships.

---

### Top Rules by Lift
The strongest association rules in this analysis are observed between organic fruit products, such as organic raspberries and organic strawberries. These high-lift rules indicate strong co-purchase behavior and are ideal candidates for recommendation and cross-selling strategies.
