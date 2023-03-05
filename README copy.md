# susu-drkg

## 介绍

整理好的 drkg 知识图谱.

原始的 drkg 数据库 ( 链接:https://pan.baidu.com/s/1KRSHPjdCXf8y-0PfIEoPcg 提取码:war6 )

## 文件

- [relation.tsv](./relation.tsv): 是 **drkg** 的关系文件, 总共 **107** 个关系. 从第二行起, 每一行是关系的**英文名**和**中文名**. 例如: 第二行中的 **DGIDB::ACTIVATOR::Gene:Compound**, **激活剂**, 其中**英文关系名**由**源数据库名**, **关系**, **头尾实体**组成. 参考于 **relation_glossary.tsv**.

- [disease.tsv](./disease.tsv): 是 **drkg** 的疾病实体文件, 总共 **5103** 个实体. 每一行是**疾病实体名**, **疾病英文名**, **疾病中文名**. 例如: 第一行中的 **Disease::DOID:0050156**, **idiopathic pulmonary fibrosis**, **特发性肺纤维化**, 其中**疾病实体名**由**实体类型** (Disease) 和**源数据库的 ID** 组成. 参考于 **entity2src.tsv**.

- [intermediate_dir](./intermediate_dir/): 临时数据目录.
   
   - [01_raw_disease.tsv](./intermediate_dir/01_raw_disease.tsv): **drkg** 原始的**疾病实体文件**, 来自于 **entity2src.tsv**.
   
   - [02_manual_disease.tsv](./intermediate_dir/02_manual_disease.tsv): 基于 [01_raw_disease.tsv](./intermediate_dir/01_raw_disease.tsv) 修改, 手动获取前 **215** 个疾病实体的英文名和中文名. 源数据库链接: https://disease-ontology.org/ 和 https://www.ncbi.nlm.nih.gov/mesh/?term= .
   
   - [03_mesh_spider_disease.tsv](./intermediate_dir/03_mesh_spider_disease.tsv): 基于 [02_manual_disease.tsv](./intermediate_dir/02_manual_disease.tsv) 修改, 通过 [MeSH RDF API](https://id.nlm.nih.gov/mesh/swagger/ui) 获得剩余 ID 为 **MESH ID** 的疾病英文名 (前 **4998**).
   
   - [04_omim_disease.tsv](./intermediate_dir/04_omim_disease.tsv): 基于  [03_mesh_spider_disease.tsv](./intermediate_dir/03_mesh_spider_disease.tsv) 修改, 手动获取 ID 为 **OMIM ID** 的**疾病中英文名** (**4999** - **5076**), 进一步写入了 **新型冠状病毒肺炎** 的**中英文疾病名**, 并手动翻译了第 **216** - **242** 的**疾病中文名**. 源数据库链接: https://www.ncbi.nlm.nih.gov/omim/ .
   
   - [05_baidufanyi_spider_disease.tsv](./intermediate_dir/05_baidufanyi_spider_disease.tsv): 基于 [04_omim_disease.tsv](./intermediate_dir/04_omim_disease.tsv) 修改, 通过[百度翻译通用翻译API](https://api.fanyi.baidu.com/doc/21) 获得了剩余疾病的**中文名**. 与 [disease.tsv](./disease.tsv) 内容相同.

- [script](./script/): 脚本目录.

   - [01_mesh_id2name.ipynb](./script/01_mesh_id2name.ipynb): 通过 [MeSH RDF API](https://id.nlm.nih.gov/mesh/swagger/ui) 获得剩余 ID 为 **MESH ID** 的疾病英文名 (前 **4998** 个) 的脚本.
   
   - [02_baidufanyi.ipynb](./script/02_baidufanyi.ipynb): 通过[百度翻译通用翻译API](https://api.fanyi.baidu.com/doc/21) 获得了剩余疾病的**中文名**的脚本.
   
   - [03_read_data.ipynb](./script/03_read_data.ipynb): 读取 [relation.tsv](./relation.tsv) 和 [disease.tsv](./disease.tsv) 的脚本.

- [report](./report/): 汇报文件目录.

- [ad_drug_repurpose](./ad_drug_repurpose/): ad 药物重定位.
   
   - [AD_drug_repurposing.ipynb](./ad_drug_repurpose/AD_drug_repurposing.ipynb): 该脚本展示了如何使用 DRKG 的预训练模型 (TransE) 进行药物重定位 (Alzheimer's disease). 需要的预训练模型 (链接：https://pan.baidu.com/s/1MiRNpE9iZTiuqe_aKN9gvg 提取码：lnkt )
   
   - [infer_drug.tsv](./ad_drug_repurpose/infer_drug.tsv): Drugbank 中的 FDA 批准的药物清单 (排除分子量 < 250 的药物).
   
   - [raw_ad_triples.ipynb](./ad_drug_repurpose/raw_ad_triples.ipynb) 该脚本展示了如何提取 DRKG 中药物治疗 Alzheimer's disease 的三元组. 需要的原始的知识图谱 (链接：https://pan.baidu.com/s/19kPh0kLL2X4HL30yjlm_vA 提取码：r4k5 )
   
   - [drug_treat_ad.tsv](./ad_drug_repurpose/drug_treat_ad.tsv): DRKG 中药物治疗 AD 的三元组集合. 利用 [raw_ad_triples.ipynb](./ad_drug_repurpose/raw_ad_triples.ipynb) 脚本生成.
   
   - [ad_drugs.txt](./ad_drug_repurpose/ad_drugs.txt): [drug_treat_ad.tsv](./ad_drug_repurpose/drug_treat_ad.tsv) 中的药物集合. 利用 [raw_ad_triples.ipynb](./ad_drug_repurpose/raw_ad_triples.ipynb) 脚本生成.
   
   - [AD_completion_drugs.md](./ad_drug_repurpose/AD_completion_drugs.md): [AD_drug_repurposing.ipynb](./ad_drug_repurpose/AD_drug_repurposing.ipynb) 的结果分析.

- [drug_repurposing_papers](drug_repurposing_papers/): 药物重定位学习笔记.

- [embedding_analysis](./embedding_analysis/): 知识图谱嵌入向量分析.

   - [Train_embeddings.ipynb](./embedding_analysis/Train_embeddings.ipynb): 该脚本展示了如何在 DRKG 上训练 TransE. 需要的原始的知识图谱 (链接：https://pan.baidu.com/s/19kPh0kLL2X4HL30yjlm_vA 提取码：r4k5 )

   - [Relation_similarity_analysis.ipynb](./embedding_analysis/Relation_similarity_analysis.ipynb): 该脚本展示了如何分析训练的关系嵌入.

   - [Entity_similarity_analysis.ipynb](./embedding_analysis/Entity_similarity_analysis.ipynb): 该脚本展示了如何分析训练的实体嵌入.

   - [Edge_similarity_based_on_link_recommendation_results.ipynb](./embedding_analysis/Edge_similarity_based_on_link_recommendation_results.ipynb): 该脚本展示了如何分析链接类型推荐的相似性 (link type recommendation similarity).

   - [result](./embedding_analysis/result/): 上面脚本保存的结果.

- [paper01-dgl-ke](./paper01-dgl-ke/): 药大学报论文对应的代码.

   - [01-model](./paper01-dgl-ke/01-model/): 训练模型.
      
      - [Train_embeddings.ipynb](./paper01-dgl-ke/01-model/Train_embeddings.ipynb): 该脚本展示了如何在 DRKG 上训练 TransE. 需要的原始的知识图谱 (链接：https://pan.baidu.com/s/19kPh0kLL2X4HL30yjlm_vA 提取码：r4k5 ) 

   - [02-analysis](./paper01-dgl-ke/02-analysis/): 知识图谱嵌入向量分析.
  
      - [Relation_similarity_analysis.ipynb](./paper01-dgl-ke/02-analysis/Relation_similarity_analysis.ipynb): 该脚本展示了如何分析训练的关系嵌入.

      - [Entity_similarity_analysis.ipynb](./paper01-dgl-ke/02-analysis/Entity_similarity_analysis.ipynb): 该脚本展示了如何分析训练的实体嵌入.

      - [Edge_similarity_based_on_link_recommendation_results.ipynb](./paper01-dgl-ke/02-analysis/Edge_similarity_based_on_link_recommendation_results.ipynb): 该脚本展示了如何分析链接类型推荐的相似性 (link type recommendation similarity).
      
      - [result](./paper01-dgl-ke/02-analysis/result/): 上面脚本保存的结果.
   
   - [03-repurpose](./paper01-dgl-ke/03-repurpose/): 药物重定位.

      - [AD_drug_repurposing.ipynb](./paper01-dgl-ke/03-repurpose/AD_drug_repurposing.ipynb): 该脚本展示了如何使用 DRKG 的预训练模型 (TransE) 进行药物重定位 (Alzheimer's disease). 需要的预训练模型 (链接：https://pan.baidu.com/s/1MiRNpE9iZTiuqe_aKN9gvg 提取码：lnkt )
         
         - [disease.tsv](./paper01-dgl-ke/03-repurpose/prerequisites/disease.tsv): 是 **drkg** 的疾病实体文件, 总共 **5103** 个实体. 每一行是**疾病实体名**, **疾病英文名**, **疾病中文名**. 例如: 第一行中的 **Disease::DOID:0050156**, **idiopathic pulmonary fibrosis**, **特发性肺纤维化**, 其中**疾病实体名**由**实体类型** (Disease) 和**源数据库的 ID** 组成. 参考于 **entity2src.tsv**.
         
         - [relation.tsv](./paper01-dgl-ke/03-repurpose/prerequisites/relation.tsv): 是 **drkg** 的关系文件, 总共 **107** 个关系. 从第二行起, 每一行是关系的**英文名**和**中文名**. 例如: 第二行中的 **DGIDB::ACTIVATOR::Gene:Compound**, **激活剂**, 其中**英文关系名**由**源数据库名**, **关系**, **头尾实体**组成. 参考于 **relation_glossary.tsv**.
      
         - [infer_drug.tsv](./paper01-dgl-ke/03-repurpose/prerequisites/infer_drug.tsv): Drugbank 中的 FDA 批准的药物清单 (排除分子量 < 250 的药物).
         
         - [raw_ad_triples.ipynb](./paper01-dgl-ke/03-repurpose/prerequisites/raw_ad_triples.ipynb) 该脚本展示了如何提取 DRKG 中药物治疗 Alzheimer's disease 的三元组. 需要的原始的知识图谱 (链接：https://pan.baidu.com/s/19kPh0kLL2X4HL30yjlm_vA 提取码：r4k5 )
         
            - [drug_treat_ad.tsv](./paper01-dgl-ke/03-repurpose/prerequisites/drug_treat_ad.tsv): DRKG 中药物治疗 AD 的三元组集合. 利用 [raw_ad_triples.ipynb](./paper01-dgl-ke/03-repurpose/prerequisites/raw_ad_triples.ipynb) 脚本生成.
            
            - [ad_drugs.txt](./paper01-dgl-ke/03-repurpose/prerequisites/ad_drugs.txt): [drug_treat_ad.tsv](./paper01-dgl-ke/03-repurpose/prerequisites/drug_treat_ad.tsv) 中的药物集合. 利用 [raw_ad_triples.ipynb](./paper01-dgl-ke/03-repurpose/prerequisites/raw_ad_triples.ipynb) 脚本生成.

      - [AD_completion_drugs.md](./paper01-dgl-ke/03-repurpose/AD_completion_drugs.md): [AD_drug_repurposing.ipynb](./paper01-dgl-ke/03-repurpose/AD_drug_repurposing.ipynb) 的结果分析.

## Reference

[1] Drug Repurposing Knowledge Graph (DRKG), link: https://github.com/gnn4dr/DRKG .