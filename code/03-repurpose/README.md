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

   - The beneficial effect of many nutrients on the course of AD has been demonstrated. These include: **glutathione**, polyphenols, curcumin, coenzyme Q10, vitamins B6, B12, folic acid, unsaturated fatty acids, lecithin, UA, caffeine and some probiotic bacteria.(许多营养素对AD过程的有益作用已经被证明。其中包括：**谷胱甘肽**、多酚、姜黄素、辅酶Q10、维生素B6、B12、叶酸、不饱和脂肪酸、卵磷脂、尿酸、咖啡因和一些益生菌。)
   
   - Śliwińska S, Jeziorek M. The role of nutrition in Alzheimer's disease. Rocz Panstw Zakl Hig. 2021;72(1):29-39. doi: 10.32394/rpzh.2021.0154. PMID: 33882663. link: https://pubmed.ncbi.nlm.nih.gov/33882663/ .

- [11] [DB00502](https://go.drugbank.com/drugs/DB00502): **Haloperidol** is an antipsychotic agent used to treat schizophrenia and other psychoses, as well as symptoms of agitation, irritability, and delirium.(**氟哌啶醇**是一种抗精神病药，用于治疗精神分裂症和其他精神病，以及焦虑、易怒和谵妄症状.)

   - The goal of this study was to compare the efficacy and side effects of two doses of haloperidol and placebo in the treatment of psychosis and disruptive behaviors in patients with Alzheimer's disease. The results indicated a favorable therapeutic profile for **haloperidol** in doses of 2-3 mg/day, although a subgroup developed moderate to severe extrapyramidal signs. (本研究的目的是比较两剂氟哌啶醇和安慰剂治疗阿尔茨海默病患者精神病和破坏行为的疗效和副作用。结果表明，尽管一个亚组出现了中度至重度锥体外系症状，但剂量为2-3 mg/天的**氟哌啶醇**治疗效果良好。)
   
   - Devanand DP, Marder K, Michaels KS, Sackeim HA, Bell K, Sullivan MA, Cooper TB, Pelton GH, Mayeux R. A randomized, placebo-controlled dose-comparison trial of haloperidol for psychosis and disruptive behaviors in Alzheimer's disease. Am J Psychiatry. 1998 Nov;155(11):1512-20. doi: 10.1176/ajp.155.11.1512. PMID: 9812111. link: https://pubmed.ncbi.nlm.nih.gov/9812111/ .

- [13] [DB06774](https://go.drugbank.com/drugs/DB06774): **Capsaicin** is a topical analgesic agent used for the symptomatic relief of neuropathic pain associated with post-herpetic neuralgia, as well as other muscle and joint pain.(**辣椒素**是一种局部镇痛剂，用于缓解疱疹后神经痛以及其他肌肉和关节疼痛相关的神经性疼痛。)

   - Many recent publications show the positive effects of capsaicin in animal models of brain disorders. In Alzheimer's disease, **capsaicin** reduces neurodegeneration and memory impairment.(最近的许多出版物显示辣椒素在脑疾病动物模型中的积极作用。在阿尔茨海默病中，**辣椒素**可以减少神经退化和记忆障碍。)
   
   - Pasierski M, Szulczyk B. Beneficial Effects of Capsaicin in Disorders of the Central Nervous System. Molecules. 2022 Apr 12;27(8):2484. doi: 10.3390/molecules27082484. PMID: 35458680; PMCID: PMC9029810. link: https://pubmed.ncbi.nlm.nih.gov/35458680/ .

- [16] [DB04216](https://go.drugbank.com/drugs/DB04216): **Quercetin** is a natural flavonoid found in foods and natural supplement products.(**槲皮素**是一种天然类黄酮，存在于食品和天然补充剂产品中。)

   - **Quercetin** has demonstrated antioxidant, anti-inflammatory, hypoglycemic, and hypolipidemic activities, suggesting therapeutic potential against type 2 diabetes mellitus (T2DM) and Alzheimer's disease (AD).(**槲皮素**已显示出抗氧化、抗炎、降血糖和降血脂活性，表明其对2型糖尿病（T2DM）和阿尔茨海默病（AD）具有治疗潜力。) 
   
   - Zu G, Sun K, Li L, Zu X, Han T, Huang H. Mechanism of quercetin therapeutic targets for Alzheimer disease and type 2 diabetes mellitus. Sci Rep. 2021 Nov 25;11(1):22959. doi: 10.1038/s41598-021-02248-5. PMID: 34824300; PMCID: PMC8617296. link: https://pubmed.ncbi.nlm.nih.gov/34824300/ .

- [17] [DB00783](https://go.drugbank.com/drugs/DB00783): **Estradiol** is an estrogenic steroid used to treat vasomotor symptoms of vulvar and vaginal atrophy in menopause, hypoestrogenism, prevention of postmenopausal osteoporosis, treatment of breast cancer, and advanced androgen-dependent carcinoma of the prostate.(雌二醇是一种雌激素类固醇，用于治疗更年期外阴和阴道萎缩的血管舒缩症状、雌激素减少、预防绝经后骨质疏松症、治疗乳腺癌和晚期雄激素依赖性前列腺癌。)

   - Mounting evidence indicates that the neurosteroid estradiol (**17β-estradiol**) plays a supporting role in neurogenesis, neuronal activity, and synaptic plasticity of AD. This effect may provide preventive and/or therapeutic approaches for AD.(越来越多的证据表明，神经甾体雌二醇（**17β-雌二醇**）在AD的神经发生、神经元活动和突触可塑性中起着支持作用。这种作用可能为AD提供预防和/或治疗途径。)
   
   - Sahab-Negah S, Hajali V, Moradi HR, Gorji A. The Impact of Estradiol on Neurogenesis and Cognitive Functions in Alzheimer's Disease. Cell Mol Neurobiol. 2020 Apr;40(3):283-299. doi: 10.1007/s10571-019-00733-0. Epub 2019 Sep 9. PMID: 31502112. link: https://pubmed.ncbi.nlm.nih.gov/31502112/ .

- [18] [DB09341](https://go.drugbank.com/drugs/DB09341): **Glucose** is a form of glucose used for caloric supply and the replenishment of fluid in total parenteral nutrition and other therapies as well as for the treatment of hypoglycemic episodes.(**葡萄糖**是一种葡萄糖，用于全胃肠外营养和其他疗法中的热量供应和补充液体，以及治疗低血糖发作。)
   
   - poorly controlled blood sugar may increase the risk of developing Alzheimer's. Furthermore, insulin-related therapeutic strategies are suggested to succeed in the development of therapies for AD by slowing down their progressive nature or even halting their future complications.(血糖控制不佳可能会增加患老年痴呆症的风险。此外，**胰岛素相关的治疗策略被建议通过减缓AD的进展性甚至停止其未来的并发症来成功开发AD治疗方法。**)
   
   - Nguyen TT, Ta QTH, Nguyen TKO, Nguyen TTD, Giau VV. Type 3 Diabetes and Its Role Implications in Alzheimer's Disease. Int J Mol Sci. 2020 Apr 30;21(9):3165. doi: 10.3390/ijms21093165. PMID: 32365816; PMCID: PMC7246646. link: https://pubmed.ncbi.nlm.nih.gov/32365816/ .

- [21] [DB00640](https://go.drugbank.com/drugs/DB00640): Adenosine is a medication used in myocardial perfusion scintigraphy and to treat supraventricular tachycardia.(腺苷是一种用于心肌灌注显像和治疗室上性心动过速的药物。)

   - 并没有发现有研究表明 Adenosine 能够治疗 AD.

- [31] [DB00907](https://go.drugbank.com/drugs/DB00907): **Cocaine** is an ester local anesthetic used during diagnostic procedures and surgeries in or through the nasal cavities.(**可卡因**是一种酯类局部麻醉剂，用于鼻腔内或通过鼻腔的诊断程序和手术。) 

   - The accumulation of amyloid-beta (Aβ) and oxidative stress damage in the brain are recognized as early features of Alzheimer's disease (AD). **The cocaine- and amphetamine-regulated transcript** (CART) peptide may possibly play an antioxidative role in neurons.Our results therefore indicate that CART peptide could serve as an antioxidant in early therapy for AD. (β淀粉样蛋白（Aβ）的积累和大脑中的氧化应激损伤被认为是阿尔茨海默病（AD）的早期特征。**可卡因和苯丙胺调节转录物**（CART）肽可能在神经元中**发挥抗氧化作用**。因此，我们的结果表明CART肽可以作为AD早期治疗的抗氧化剂。)
   
   - Jiao W, Wang Y, Kong L, Ou-Yang T, Meng Q, Fu Q, Hu Z. CART peptide activates the Nrf2/HO-1 antioxidant pathway and protects hippocampal neurons in a rat model of Alzheimer's disease. Biochem Biophys Res Commun. 2018 Jul 2;501(4):1016-1022. doi: 10.1016/j.bbrc.2018.05.101. Epub 2018 May 18. PMID: 29777699. link: https://pubmed.ncbi.nlm.nih.gov/29777699/ .

- [39] [DB01229](https://go.drugbank.com/drugs/DB01229): **Paclitaxel** is a taxoid chemotherapeutic agent used as first-line and subsequent therapy for the treatment of advanced carcinoma of the ovary, and other various cancers including breast and lung cancer.(**紫杉醇**是一种紫杉醇类化疗药物，用作治疗晚期卵巢癌和其他各种癌症（包括乳腺癌和肺癌）的一线和后续治疗。)

   - In addition to NSAIDs, an anticancer drug, **paclitaxel**, has considerable potential as an AD treatment.(除了非甾体抗炎药外，**紫杉醇**是一种抗癌药物，具有相当大的治疗AD的潜力。)
   
   - Lehrer S, Rheinstein PH. Transspinal delivery of drugs by transdermal patch back-of-neck for Alzheimer's disease: a new route of administration. Discov Med. 2019 Jan;27(146):37-43. PMID: 30721650. link: https://pubmed.ncbi.nlm.nih.gov/30721650/ .

- [41] [DB04540](https://go.drugbank.com/drugs/DB04540): **Cholesterol**(胆固醇), The principal sterol of all higher animals, distributed in body tissues, especially the brain and spinal cord, and in animal fats and oils.(所有高等动物的主要固醇，分布于身体组织，特别是大脑和脊髓，以及动物脂肪和油中。)

   - **Cholesterol Metabolism** Is **a Druggable Axis** that Independently Regulates Tau and Amyloid-β in iPSC-Derived Alzheimer's Disease Neurons. (**胆固醇代谢**是独立调节iPSC衍生阿尔茨海默病神经元中Tau和淀粉样蛋白-β的**可药用轴**)
   
   - van der Kant R, Langness VF, Herrera CM, Williams DA, Fong LK, Leestemaker Y, Steenvoorden E, Rynearson KD, Brouwers JF, Helms JB, Ovaa H, Giera M, Wagner SL, Bang AG, Goldstein LSB. Cholesterol Metabolism Is a Druggable Axis that Independently Regulates Tau and Amyloid-β in iPSC-Derived Alzheimer's Disease Neurons. Cell Stem Cell. 2019 Mar 7;24(3):363-375.e9. doi: 10.1016/j.stem.2018.12.013. Epub 2019 Jan 24. PMID: 30686764; PMCID: PMC6414424. link: https://pubmed.ncbi.nlm.nih.gov/30686764/ .