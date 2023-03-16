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
#          Web of Science: https://www.webofknowledge.com/
```

## 4 种模型药物重定位结果重叠情况

### TransE_l1_top50 and TransE_l2_top50

```shell
Compound::DB00477
Compound::DB00295
Compound::DB09341
Compound::DB00143
Compound::DB04216
Compound::DB00907
Compound::DB00783
Compound::DB00661
Compound::DB04540
Compound::DB00363
Compound::DB00624
```

### TransE_l1_top50 and ComplEx_top100

```shell
Compound::DB00563
Compound::DB00661
Compound::DB00363
```

### TransE_l1_top50 and RotatE_top50

```shell
Compound::DB06774
Compound::DB09341
Compound::DB00143
Compound::DB04216
Compound::DB00783
Compound::DB04540
Compound::DB00907
```

### TransE_l2_top50 and ComplEx_top100

```shell
Compound::DB00959
Compound::DB00661
Compound::DB00363
```

### TransE_l2_top50 and RotatE_top50

```shell
Compound::DB09341
Compound::DB00143
Compound::DB04216
Compound::DB00783
Compound::DB04540
Compound::DB00907
Compound::DB00502
Compound::DB01229
```

### ComplEx_top100 and RotatE_top50

```shell
Compound::DB01016
Compound::DB00715
```

### TransE_l1_top50 and TransE_l2_top50 and ComplEx_top100

```shell
Compound::DB00363
Compound::DB00661
```

### TransE_l1_top50 and TransE_l2_top50 and RotatE_top50

```shell
Compound::DB09341
Compound::DB00143
Compound::DB04216
Compound::DB00783
Compound::DB04540
Compound::DB00907
```

### TransE_l1_top50 and ComplEx_top100 and RotatE_top50

```shell
None
```

### TransE_l2_top50 and ComplEx_top100 and RotatE_top50

```shell
None
```

## 结果分析

- [DB00477](https://go.drugbank.com/drugs/DB00477): Chlorpromazine is a phenothiazine antipsychotic used to treat nausea, vomiting, preoperative anxiety, schizophrenia, bipolar disorder, and severe behavioral problems in children.

   - None.

- [DB00295](https://go.drugbank.com/drugs/DB00295): Morphine is an opioid agonist used for the relief of moderate to severe acute and chronic pain.

   - None.

- [DB09341](https://go.drugbank.com/drugs/DB09341): Glucose is a form of glucose used for caloric supply and the replenishment of fluid in total parenteral nutrition and other therapies as well as for the treatment of hypoglycemic episodes.
   
   - Specifically, decreased O-GlcNAcylation levels by glucose deficiency alter mitochondrial functions and together contribute to Alzheimer's disease pathogenesis.
   - Huang CW,Rust NC,Wu HF,et al.Altered O-GlcNAcylation and mitochondrial dysfunction, a molecular link between brain glucose dysregulation and sporadic Alzheimer's disease[J].Neural regeneration research,2023,18(4):779-783. https://doi.org/10.4103/1673-5374.354515.

- [DB00143](https://go.drugbank.com/drugs/DB00143): Glutathione, A tripeptide with many roles in cells. It conjugates to drugs to make them more soluble for excretion, is a cofactor for some enzymes, is involved in protein disulfide bond rearrangement and reduces peroxides.

   - The beneficial effect of many nutrients on the course of AD has been demonstrated. These include: glutathione, polyphenols, curcumin, coenzyme Q10, vitamins B6, B12, folic acid, unsaturated fatty acids, lecithin, UA, caffeine and some probiotic bacteria.
   - Sliwinska S,Jeziorek M.The role of nutrition in Alzheimer's disease[J].Roczniki Panstwowego Zakladu Higieny,2021,72(1):29-39. https://doi.org/10.32394/rpzh.2021.0154.

- [DB04216](https://go.drugbank.com/drugs/DB04216): Quercetin is a natural flavonoid found in foods and natural supplement products.

   - Quercetin has demonstrated antioxidant, anti-inflammatory, hypoglycemic, and hypolipidemic activities, suggesting therapeutic potential against type 2 diabetes mellitus (T2DM) and Alzheimer's disease (AD).
   - Zu GX,Sun KY,Li L,et al.Mechanism of quercetin therapeutic targets for Alzheimer disease and type 2 diabetes mellitus[J].Scientific reports,2021,11(1):22959. https://doi.org/10.1038/s41598-021-02248-5.

- [DB00907](https://go.drugbank.com/drugs/DB00907): Cocaine is an ester local anesthetic used during diagnostic procedures and surgeries in or through the nasal cavities.

   - None.

- [DB00783](https://go.drugbank.com/drugs/DB00783): Estradiol is an estrogenic steroid used to treat vasomotor symptoms of vulvar and vaginal atrophy in menopause, hypoestrogenism, prevention of postmenopausal osteoporosis, treatment of breast cancer, and advanced androgen-dependent carcinoma of the prostate.

   - Mounting evidence indicates that the neurosteroid estradiol (17β-estradiol) plays a supporting role in neurogenesis, neuronal activity, and synaptic plasticity of AD. This effect may provide preventive and/or therapeutic approaches for AD.
   - Sahab-Negah S,Hajali V,Moradi HR,et al.The impact of estradiol on neurogenesis and cognitive functions in Alzheimer's disease[J]. Cellular and molecular neurobiology,2020,40(3):283-299. https://doi.org/10.1007/s10571-019-00733-0.

- [DB00661](https://go.drugbank.com/drugs/DB00661): Verapamil is a non-dihydropyridine calcium channel blocker used in the treatment of angina, arrhythmia, and hypertension.

   - Verapamil Prevents Development of Cognitive Impairment in an Aged Mouse Model of Sporadic Alzheimer’s Disease.
   - Ahmed HA,Ismael S,Mirzahosseini G,et al.Verapamil Prevents Development of Cognitive Impairment in an Aged Mouse Model of Sporadic Alzheimer’s Disease[J]. Molecular Neurobiology,2021,58(7):3374–3387. https://doi.org/10.1007/s12035-021-02350-9.

- [DB04540](https://go.drugbank.com/drugs/DB04540): Cholesterol, The principal sterol of all higher animals, distributed in body tissues, especially the brain and spinal cord, and in animal fats and oils.

   - None.

- [DB00363](https://go.drugbank.com/drugs/DB00363): Clozapine is an atypical or second-generation antipsychotic drug used in treatment-resistant schizophrenia and to decrease suicide risk in schizophrenic patients.

   - Clozapine Improves Memory Impairment and Reduces A beta Level in the Tg-APPswe/PS1dE9 Mouse Model of Alzheimer's Disease.
   - Choi Y,Jeong HJ,Liu QF,et al.Clozapine Improves Memory Impairment and Reduces Aβ Level in the Tg-APPswe/PS1dE9 Mouse Model of Alzheimer’s Disease[J]. Molecular Neurobiology,2017,54(1):450–460. https://doi.org/10.1007/s12035-015-9636-x.

- [DB00624](https://go.drugbank.com/drugs/DB00624): Testosterone is a hormone used to treat hypogonadism, breast carcinoma in women, or the vasomotor symptoms of menopause.

   - Animal models demonstrated that testosterone (T) exerted a neuroprotective effect reducing the production of amyloid-beta (Aβ), improving synaptic signaling, and counteracting neuronal death.
   - Bianchi VE.Impact of Testosterone on Alzheimer's Disease[J]. World Journal of Nens Health,2022,40(2):243-256. https://doi.org/10.5534/wjmh.210175.

- [DB00563](https://go.drugbank.com/drugs/DB00563): Methotrexate is an antineoplastic agent used the treatment of a wide variety of cancers as well as severe psoriasis, severe rheumatoid arthritis, and juvenile rheumatoid arthritis.

   - anti-inflammatory methotrexate treatment reduced the incidence of Alzheimer's disease in high-risk individuals.
   - Lindbohm JV,Mars N,Sipilae, PN,et al.Immune system-wide Mendelian randomization and triangulation analyses support autoimmunity as a modifiable component in dementia-causing diseases[J].nature aging,2022,2(10):956–972. https://doi.org/10.1038/s43587-022-00293-x.

- [DB06774](https://go.drugbank.com/drugs/DB06774): Capsaicin is a topical analgesic agent used for the symptomatic relief of neuropathic pain associated with post-herpetic neuralgia, as well as other muscle and joint pain.

   - In Alzheimer's disease, capsaicin reduces neurodegeneration and memory impairment.
   - Pasierski M,Szulczyk B.Beneficial effects of capsaicin in disorders of the central nervous system[J].Molecules,2022,27(8):2484. https://doi.org/10.3390/molecules27082484.

- [DB00959](https://go.drugbank.com/drugs/DB00959): Methylprednisolone is a corticosteroid used to treat inflammation or immune reactions across a variety of organ systems, endocrine conditions, and neoplastic diseases.

   - None.

- - [DB00502](https://go.drugbank.com/drugs/DB00502): Haloperidol is an antipsychotic agent used to treat schizophrenia and other psychoses, as well as symptoms of agitation, irritability, and delirium.

   - Haloperidol inactivates AMPK and reduces tau phosphorylation in a tau mouse model of Alzheimer's disease[2].
   - Koppel J,Jimenez H,Adrien L,et al.Haloperidol inactivates AMPK and reduces tau phosphorylation in a tau mouse model of Alzheimer's disease[J].Alzheimer's & dementia,2016,2(2):121-130. https://doi.org/10.1016/j.trci.2016.05.003.

- [DB01229](https://go.drugbank.com/drugs/DB01229): Paclitaxel is a taxoid chemotherapeutic agent used as first-line and subsequent therapy for the treatment of advanced carcinoma of the ovary, and other various cancers including breast and lung cancer.

   - In addition to NSAIDs, an anticancer drug, paclitaxel, has considerable potential as an AD treatment.
   - Lehrer S,Rheinstein PH.Transspinal delivery of drugs by transdermal patch back-of-neck for Alzheimer's disease: a new route of administration[J]. Discovery Medicine,2019,27(146):37-43.

- [DB01016](https://go.drugbank.com/drugs/DB01016): Glyburide is a sulfonylurea used in the treatment of non insulin dependent diabetes mellitus.

   - Our findings suggest that a pharmacologic approach to inhibit galanin in the brain, either by glibenclamide or pioglitazone might dramatically improve symptoms in Alzheimer's disease.
   - Baraka A,ElGhotny S.Study of the effect of inhibiting galanin in Alzheimer's disease induced in rats[J].European Journal of Pharmacology,2010,641(2):123-127. https://doi.org/10.1016/j.ejphar.2010.05.030.

- [DB00715](https://go.drugbank.com/drugs/DB00715): Paroxetine is a selective serotonin reuptake inhibitor used to treat major depressive disorder, panic disorder, OCD, social phobia, generalized anxiety disorder, the vasomotor symptoms of menopause, and premenstrual dysphoric disorder.

   - Paroxetine ameliorates prodromal emotional dysfunction and late-onset memory deficit in Alzheimer's disease mice.
   - Ai PH,Chen S,Liu XD,et al.Paroxetine ameliorates prodromal emotional dysfunction and late-onset memory deficit in Alzheimer's disease mice[J].Translational Neurodegeneration,2020,9(1):18. https://doi.org/10.1186/s40035-020-00194-2.

- [DB00515](https://go.drugbank.com/drugs/DB00515): Cisplatin is a platinum based chemotherapy agent used to treat various sarcomas, carcinomas, lymphomas, and germ cell tumors.

   - Cisplatin Inhibits the Formation of a Reactive Intermediate during Copper-Catalyzed Oxidation of Amyloid beta Peptide.
   - Walke GR,Rapole S,Kulkarni PP.Cisplatin inhibits the formation of a reactive intermediate during copper-catalyzed oxidation of amyloid β peptide[J].Inorganic Chemistry,2014,53(19):10003-10005. https://doi.org/10.1021/ic5007764.