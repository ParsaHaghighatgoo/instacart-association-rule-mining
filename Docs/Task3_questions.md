## Task 3 – Conceptual Questions

### 1. What should be the final value of `min_support`?

Based on the experimental results, a minimum support value of **0.01** is the most appropriate choice for this dataset.

When `min_support = 0.01`, the Apriori algorithm identifies a larger number of frequent itemsets, including multi-item combinations. These itemsets capture meaningful co-occurrence patterns between products, which are essential for market basket analysis and recommender systems.

In contrast, using a higher support threshold such as `min_support = 0.05` results in only a small number of single-item itemsets and removes all multi-item patterns. This significantly reduces the analytical value of the results.

Therefore, **`min_support = 0.01`** provides a better balance between pattern richness and computational efficiency.

---

### 2. Why does increasing `min_support` reduce the number of itemsets?

Increasing the minimum support threshold imposes a stricter requirement on how frequently an itemset must appear in transactions to be considered frequent.

Larger itemsets naturally occur less often than smaller ones. As a result, when the support threshold increases, multi-item combinations are filtered out first. Only the most frequently occurring individual items remain.

This leads to:
- Fewer frequent itemsets overall
- Smaller maximum itemset sizes
- Loss of potentially interesting co-purchase patterns

In summary, higher `min_support` values simplify the results but reduce the ability to discover meaningful associations between products.
