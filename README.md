# AD-KGE

## 介绍

利用知识图谱嵌入模型研究阿尔茨海默病的药物重定位.

## 数据

原始的 DRKG 知识图谱 ( 链接:https://pan.baidu.com/s/1KRSHPjdCXf8y-0PfIEoPcg 提取码:war6 )

## 配置环境

```shell
$ git clone git@github.com:LuYF-Lemon-love/AD-KGE.git
$ cd AD-KGE/
$ conda env create -f environment.yaml
$ pip install -r requirements.txt
```

## 文件

- [code](./code/): 代码目录.

   - [01-model](code/01-model/): 训练模型.
      
      - [01_split_dataset.ipynb](code/01-model/01_split_dataset.ipynb): 该脚本展示了如何划分 DRKG 数据集 (训练集、验证集、测试集). 需要的原始的知识图谱 (链接：https://pan.baidu.com/s/19kPh0kLL2X4HL30yjlm_vA 提取码：r4k5 )
      
      - [02_Train_TransE_l1.ipynb](code/01-model/02_Train_TransE_l1.ipynb): 这个 notebook 展示了如何在 DRKG 上训练模型 (TransE_l1), 并利用网格搜索寻找到最优参数.
      
      - [03_Train_TransE_l2.ipynb](code/01-model/03_Train_TransE_l2.ipynb): 该脚本展示了如何在 DRKG 上训练模型 (TransE_l2), 并利用网格搜索寻找到最优参数.
      
      - [04_Train_TransR.ipynb](code/01-model/04_Train_TransR.ipynb): 该脚本展示了如何在 DRKG 上训练模型 (TransR), 并利用网格搜索寻找到最优参数.
      
      - [05_Train_RESCAL.ipynb](code/01-model/05_Train_RESCAL.ipynb): 该脚本展示了如何在 DRKG 上训练模型 (RESCAL), 并利用网格搜索寻找到最优参数.
      
      - [06_Train_DistMult.ipynb](code/01-model/06_Train_DistMult.ipynb): 该脚本展示了如何在 DRKG 上训练模型 (DistMult), 并利用网格搜索寻找到最优参数.
      
      - [07_Train_ComplEx.ipynb](code/01-model/07_Train_ComplEx.ipynb): 该脚本展示了如何在 DRKG 上训练模型 (ComplEx), 并利用网格搜索寻找到最优参数.
      
      - [08_Train_RotatE.ipynb](code/01-model/08_Train_RotatE.ipynb): 该脚本展示了如何在 DRKG 上训练模型 (RotatE), 并利用网格搜索寻找到最优参数.
      
      - [09_Train_final_model_TransE_l1.ipynb](code/01-model/09_Train_final_model_TransE_l1.ipynb): 该脚本展示了如何在 DRKG 上训练最终模型 (TransE_l1).
      
      - [10_Train_final_model_TransE_l2.ipynb](code/01-model/10_Train_final_model_TransE_l2.ipynb): 该脚本展示了如何在 DRKG 上训练最终模型 (TransE_l2).
      
      - [11_Train_final_model_ComplEx.ipynb](code/01-model/11_Train_final_model_ComplEx.ipynb): 该脚本展示了如何在 DRKG 上训练最终模型 (ComplEx).
      
      - [12_Train_final_model_RotatE.ipynb](code/01-model/12_Train_final_model_RotatE.ipynb): 该脚本展示了如何在 DRKG 上训练最终模型 (RotatE).
   
   - [02-analysis](code/02-analysis/): 知识图谱嵌入向量分析.
  
      - [01_relation_similarity_analysis.ipynb](code/02-analysis/01_relation_similarity_analysis.ipynb): 该脚本展示了如何分析训练的关系嵌入.
      
      - [01_relation_similarity_analysis_supplement.ipynb](code/02-analysis/01_relation_similarity_analysis_supplement.ipynb): 上面分析关系嵌入脚本的补充.

      - [02_entity_similarity_analysis.ipynb](code/02-analysis/02_entity_similarity_analysis.ipynb): 该脚本展示了如何分析训练的实体嵌入.

      - [03_TransE_l1_edge_similarity_based_on_link_recommendation_results.ipynb](code/02-analysis/03_TransE_l1_edge_similarity_based_on_link_recommendation_results.ipynb): 该脚本展示了如何分析 TransE_l1 的关系类型推荐相似性 (Link Type Recommendation Similarity).
      
      - [04_TransE_l2_edge_similarity_based_on_link_recommendation_results.ipynb](code/02-analysis/04_TransE_l2_edge_similarity_based_on_link_recommendation_results.ipynb): 该脚本展示了如何分析 TransE_l2 的关系类型推荐相似性 (Link Type Recommendation Similarity).
      
      - [05_ComplEx_edge_similarity_based_on_link_recommendation_results.ipynb](code/02-analysis/05_ComplEx_edge_similarity_based_on_link_recommendation_results.ipynb): 该脚本展示了如何分析 ComplEx 的关系类型推荐相似性 (Link Type Recommendation Similarity).
      
      - [06_RotatE_edge_similarity_based_on_link_recommendation_results.ipynb](code/02-analysis/06_RotatE_edge_similarity_based_on_link_recommendation_results.ipynb): 该脚本展示了如何分析 RotatE 的关系类型推荐相似性 (Link Type Recommendation Similarity).
      
      - [result](code/02-analysis/result/): 保存上面脚本的结果.
   
   - [03-repurpose](code/03-repurpose/): 药物重定位.

      - [prerequisites](code/03-repurpose/prerequisites/): 先决条件.
         
         - [disease.tsv](code/03-repurpose/prerequisites/disease.tsv): 是 **drkg** 的疾病实体文件, 总共 **5103** 个实体. 每一行是**疾病实体名**, **疾病英文名**, **疾病中文名**. 例如: 第一行中的 **Disease::DOID:0050156**, **idiopathic pulmonary fibrosis**, **特发性肺纤维化**, 其中**疾病实体名**由**实体类型** (Disease) 和**源数据库的 ID** 组成. 参考于原始 DRKG 知识图谱的 **entity2src.tsv**.
         
         - [relation.tsv](code/03-repurpose/prerequisites/relation.tsv): 是 **drkg** 的关系文件, 总共 **107** 个关系. 从第二行起, 每一行是关系的**英文名**和**中文名**. 例如: 第二行中的 **DGIDB::ACTIVATOR::Gene:Compound**, **激活剂**, 其中**英文关系名**由**源数据库名**, **关系**, **头尾实体**组成. 参考于原始 DRKG 知识图谱的 **relation_glossary.tsv**.
      
         - [infer_drug.tsv](code/03-repurpose/prerequisites/infer_drug.tsv): Drugbank 中的 FDA 批准的药物清单 (排除分子量 < 250 的药物), 来源于原始 DRKG 知识图谱.
         
         - [raw_ad_triples.ipynb](code/03-repurpose/prerequisites/raw_ad_triples.ipynb) 该脚本展示了如何提取 DRKG 中药物治疗 Alzheimer's disease 的三元组. 需要的原始的知识图谱 (链接：https://pan.baidu.com/s/19kPh0kLL2X4HL30yjlm_vA 提取码：r4k5 )
         
            - [drug_treat_ad.tsv](code/03-repurpose/prerequisites/drug_treat_ad.tsv): DRKG 中药物治疗 AD 的三元组集合. 利用 [raw_ad_triples.ipynb](code/03-repurpose/prerequisites/raw_ad_triples.ipynb) 脚本生成.
            
            - [ad_drugs.txt](code/03-repurpose/prerequisites/ad_drugs.txt): [drug_treat_ad.tsv](code/03-repurpose/prerequisites/drug_treat_ad.tsv) 中的药物集合. 利用 [raw_ad_triples.ipynb](code/03-repurpose/prerequisites/raw_ad_triples.ipynb) 脚本生成.

      - 最终训练的模型 (TransE_l1, TransE_l2, ComplEx, RotatE): 链接：https://pan.baidu.com/s/1-9o2ELys5T3rqC9UEKgkXg?pwd=jigj 提取码：jigj .
   
      - [01_TransE_l1_AD_drug_repurposing.ipynb](code/03-repurpose/01_TransE_l1_AD_drug_repurposing.ipynb): 该脚本展示了如何使用我们的预训练模型 ([09_Train_final_model_TransE_l1.ipynb](code/01-model/09_Train_final_model_TransE_l1.ipynb)) 进行药物重定位 (Alzheimer's disease), 其中 topk = 50.
   
      - [02_TransE_l2_AD_drug_repurposing.ipynb](code/03-repurpose/02_TransE_l2_AD_drug_repurposing.ipynb): 该脚本展示了如何使用我们的预训练模型 ([10_Train_final_model_TransE_l2.ipynb](code/01-model/10_Train_final_model_TransE_l2.ipynb)) 进行药物重定位 (Alzheimer's disease), 其中 topk = 50.
   
      - [03_ComplEx_AD_drug_repurposing.ipynb](code/03-repurpose/03_ComplEx_AD_drug_repurposing.ipynb): 该脚本展示了如何使用我们的预训练模型 ([11_Train_final_model_ComplEx.ipynb](code/01-model/11_Train_final_model_ComplEx.ipynb)) 进行药物重定位 (Alzheimer's disease), 其中 topk = 100.
      
      - [04_RotatE_AD_drug_repurposing.ipynb](code/03-repurpose/04_RotatE_AD_drug_repurposing.ipynb): 该脚本展示了如何使用我们的预训练模型 ([12_Train_final_model_RotatE.ipynb](code/01-model/12_Train_final_model_RotatE.ipynb)) 进行药物重定位 (Alzheimer's disease), 其中 topk = 50.
      
      - [result](code/03-repurpose/results/): 保存上面脚本的结果.
      
      - [05_calculate_overlap.ipynb](code/03-repurpose/05_calculate_overlap.ipynb): 该脚本计算了四个个预训练模型 (transE_l1, transE_l2, ComplEx, rotatE) 药物重定位 (Alzheimer's disease) 结果重叠情况.

## Reference

[1] Drug Repurposing Knowledge Graph (DRKG), link: https://github.com/gnn4dr/DRKG .

[2] OpenKE: An Open Toolkit for Knowledge Embedding, link: https://github.com/thunlp/OpenKE .
