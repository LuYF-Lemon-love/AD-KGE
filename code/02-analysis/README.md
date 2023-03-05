# Knowledge Graph Embedding Based Analysis of DRKG

我们通过之前训练的 RotatE 模型来分析 DRKG. **由于 DRKG 结合了来自不同数据源的信息, 我们希望验证使用知识图嵌入技术可以生成有意义的实体和关系嵌入.**

## Analyze the Relation Embedding Similarity

- [01_relation_similarity_analysis.ipynb](01_relation_similarity_analysis.ipynb): 我们分析了关系嵌入相似性. 我们首先使用 t-SNE 将关系嵌入映射到 2D 空间, 以显示关系嵌入分布, 然后绘制不同关系类型之间的成对相似性(the pair-wise similarity).

## Analyze the Entity Embedding Similarity

- [Entity_similarity_analysis.ipynb](Entity_similarity_analysis.ipynb): 我们分析了实体嵌入相似性. 我们首先使用 PCA 和 t-SNE 将实体嵌入映射到 2D 空间, 以显示实体嵌入分布.

## Analyze Link Type Recommendation Similarity

- [Edge_similarity_based_on_link_recommendation_results.ipynb](Edge_similarity_based_on_link_recommendation_results.ipynb): 我们分析了不同关系类型之间的链接预测的相似程度. 对于种子 head node $n_i$, 我们用链接预测 score 找到关系 $r_j$ 下最可能成立的 top10 tail node, 接下来, 我们对关系 $r_{j'}$ 重复上述工作, 并计算关系 $r_j$ 和 $r_{j'}$ 的 top10 tail node 集合的 Jaccard 相似系数 (the Jaccard similarity coefficient).
