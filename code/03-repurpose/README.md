# AD 知识图谱补全结果分析

```python
# created by LuYF-Lemon-love <luyanfeng_nlp@qq.com> on January 12, 2023
# updated by LuYF-Lemon-love <luyanfeng_nlp@qq.com> on March 5, 2023
#
# 该文档分析了两个预训练模型 (TransE 和 RotatE) 药物重定位 (Alzheimer's disease) 重叠的药物.
#
# 需要的文件:
#          03_calculate_overlap.ipynb
#
# 需要的链接:
#          Drugbank: https://go.drugbank.com/drugs
#          pubmed: https://pubmed.ncbi.nlm.nih.gov/?term=
```

## 知识图谱补全的原始结果

每一行分别是每一个药物在 RotatE 预测结果的 rank 和药物的实体名.

```shell
[9]	Compound::DB00143
[11]	Compound::DB00502
[13]	Compound::DB06774
[16]	Compound::DB04216
[17]	Compound::DB00783
[18]	Compound::DB09341
[21]	Compound::DB00640
[31]	Compound::DB00907
[39]	Compound::DB01229
[41]	Compound::DB04540
```

## 结果分析

- [9] [DB00143](https://go.drugbank.com/drugs/DB00143): **Glutathione**(谷胱甘肽), A tripeptide with many roles in cells. It conjugates to drugs to make them more soluble for excretion, is a cofactor for some enzymes, is involved in protein disulfide bond rearrangement and reduces peroxides.(在细胞中具有多种作用的三肽。它与药物缀合，使药物更易溶解于排泄物，是某些酶的辅因子，参与蛋白质二硫键重排并减少过氧化物。)

   - The beneficial effect of many nutrients on the course of AD has been demonstrated. These include: glutathione, polyphenols, curcumin, coenzyme Q10, vitamins B6, B12, folic acid, unsaturated fatty acids, lecithin, UA, caffeine and some probiotic bacteria[1].

- [11] [DB00502](https://go.drugbank.com/drugs/DB00502): **Haloperidol** is an antipsychotic agent used to treat schizophrenia and other psychoses, as well as symptoms of agitation, irritability, and delirium.(**氟哌啶醇**是一种抗精神病药，用于治疗精神分裂症和其他精神病，以及焦虑、易怒和谵妄症状.)

   - Haloperidol inactivates AMPK and reduces tau phosphorylation in a tau mouse model of Alzheimer's disease[2].

- [13] [DB06774](https://go.drugbank.com/drugs/DB06774): **Capsaicin** is a topical analgesic agent used for the symptomatic relief of neuropathic pain associated with post-herpetic neuralgia, as well as other muscle and joint pain.(**辣椒素**是一种局部镇痛剂，用于缓解疱疹后神经痛以及其他肌肉和关节疼痛相关的神经性疼痛。)

   - In Alzheimer's disease, capsaicin reduces neurodegeneration and memory impairment[3].

- [16] [DB04216](https://go.drugbank.com/drugs/DB04216): **Quercetin** is a natural flavonoid found in foods and natural supplement products.(**槲皮素**是一种天然类黄酮，存在于食品和天然补充剂产品中。)

   - Quercetin has demonstrated antioxidant, anti-inflammatory, hypoglycemic, and hypolipidemic activities, suggesting therapeutic potential against type 2 diabetes mellitus (T2DM) and Alzheimer's disease (AD)[4].

- [17] [DB00783](https://go.drugbank.com/drugs/DB00783): **Estradiol** is an estrogenic steroid used to treat vasomotor symptoms of vulvar and vaginal atrophy in menopause, hypoestrogenism, prevention of postmenopausal osteoporosis, treatment of breast cancer, and advanced androgen-dependent carcinoma of the prostate.(雌二醇是一种雌激素类固醇，用于治疗更年期外阴和阴道萎缩的血管舒缩症状、雌激素减少、预防绝经后骨质疏松症、治疗乳腺癌和晚期雄激素依赖性前列腺癌。)

   - Mounting evidence indicates that the neurosteroid estradiol (17β-estradiol) plays a supporting role in neurogenesis, neuronal activity, and synaptic plasticity of AD. This effect may provide preventive and/or therapeutic approaches for AD[5].

- [18] [DB09341](https://go.drugbank.com/drugs/DB09341): **Glucose** is a form of glucose used for caloric supply and the replenishment of fluid in total parenteral nutrition and other therapies as well as for the treatment of hypoglycemic episodes.(**葡萄糖**是一种葡萄糖，用于全胃肠外营养和其他疗法中的热量供应和补充液体，以及治疗低血糖发作。)
   
   - Specifically, decreased O-GlcNAcylation levels by glucose deficiency alter mitochondrial functions and together contribute to Alzheimer's disease pathogenesis[6].

- [21] [DB00640](https://go.drugbank.com/drugs/DB00640): Adenosine is a medication used in myocardial perfusion scintigraphy and to treat supraventricular tachycardia.(腺苷是一种用于心肌灌注显像和治疗室上性心动过速的药物。)

   - Emerging evidence suggests adenosine G protein-coupled receptors (GPCRs) are promising therapeutic targets for Alzheimer's disease[7]. 

- [31] [DB00907](https://go.drugbank.com/drugs/DB00907): **Cocaine** is an ester local anesthetic used during diagnostic procedures and surgeries in or through the nasal cavities.(**可卡因**是一种酯类局部麻醉剂，用于鼻腔内或通过鼻腔的诊断程序和手术。) 

   - None.

- [39] [DB01229](https://go.drugbank.com/drugs/DB01229): **Paclitaxel** is a taxoid chemotherapeutic agent used as first-line and subsequent therapy for the treatment of advanced carcinoma of the ovary, and other various cancers including breast and lung cancer.(**紫杉醇**是一种紫杉醇类化疗药物，用作治疗晚期卵巢癌和其他各种癌症（包括乳腺癌和肺癌）的一线和后续治疗。)

   - In addition to NSAIDs, an anticancer drug, paclitaxel, has considerable potential as an AD treatment[8].

- [41] [DB04540](https://go.drugbank.com/drugs/DB04540): **Cholesterol**(胆固醇), The principal sterol of all higher animals, distributed in body tissues, especially the brain and spinal cord, and in animal fats and oils.(所有高等动物的主要固醇，分布于身体组织，特别是大脑和脊髓，以及动物脂肪和油中。)

   - None.

## Reference

- [1] Sliwinska S,Jeziorek M.The role of nutrition in Alzheimer's disease[J].Roczniki Panstwowego Zakladu Higieny,2021,72(1):29-39. https://doi.org/10.32394/rpzh.2021.0154.

- [2] Koppel J,Jimenez H,Adrien L,et al.Haloperidol inactivates AMPK and reduces tau phosphorylation in a tau mouse model of Alzheimer's disease[J].Alzheimer's & dementia,2016,2(2):121-130. https://doi.org/10.1016/j.trci.2016.05.003.

- [3] Pasierski M,Szulczyk B.Beneficial effects of capsaicin in disorders of the central nervous system[J].Molecules,2022,27(8):2484. https://doi.org/10.3390/molecules27082484.

- [4] Zu GX,Sun KY,Li L,et al.Mechanism of quercetin therapeutic targets for Alzheimer disease and type 2 diabetes mellitus[J].Scientific reports,2021,11(1):22959. https://doi.org/10.1038/s41598-021-02248-5.

- [5] Sahab-Negah S,Hajali V,Moradi HR,et al.The impact of estradiol on neurogenesis and cognitive functions in Alzheimer's disease[J]. Cellular and molecular neurobiology,2020,40(3):283-299. https://doi.org/10.1007/s10571-019-00733-0.

- [6] Huang CW,Rust NC,Wu HF,et al.Altered O-GlcNAcylation and mitochondrial dysfunction, a molecular link between brain glucose dysregulation and sporadic Alzheimer's disease[J].Neural regeneration research,2023,18(4):779-783. https://doi.org/10.4103/1673-5374.354515.

- [7] Trinh PNH,Baltos JA,Hellyer SD,et al.Adenosine receptor signalling in Alzheimer's disease[J].Purinergic signal,2022,18(3):359-381. https://doi.org/10.1007/s11302-022-09883-1.

- [8] Lehrer S,Rheinstein PH.Transspinal delivery of drugs by transdermal patch back-of-neck for Alzheimer's disease: a new route of administration[J]. Discovery Medicine,2019,27(146):37-43.