# AD 知识图谱补全结果分析

```python
# ad_completion_drugs
#
# created by LuYF-Lemon-love <luyanfeng_nlp@qq.com> on January 12, 2023
# updated by LuYF-Lemon-love <luyanfeng_nlp@qq.com> on January 16, 2023
#
# 该文档分析了使用 DRKG 的预训练模型 (TransE) 进行药物重定位 (Alzheimer's disease) 的结果.
#
# 需要的文件:
#          AD_drug_repurposing.html
#
# 需要的链接:
#          Drugbank: https://go.drugbank.com/drugs
#          pubmed: https://pubmed.ncbi.nlm.nih.gov/?term=
#
# [6-58]: 卢艳峰, [60-100]: 杨思瀚 .
```

## 知识图谱补全的原始结果

```shell
[6]	Compound::DB04540	-0.1250646710395813
[8]	Compound::DB01224	-0.13244186341762543
[9]	Compound::DB00295	-0.135432630777359
[11]	Compound::DB00515	-0.13710395991802216
[12]	Compound::DB09341	-0.14528262615203857
[13]	Compound::DB00143	-0.15114769339561462
[15]	Compound::DB04216	-0.15679287910461426
[16]	Compound::DB00907	-0.15733285248279572
[17]	Compound::DB06774	-0.15746210515499115
[20]	Compound::DB00171	-0.16215726733207703
[22]	Compound::DB00624	-0.17482610046863556
[25]	Compound::DB02527	-0.17842411994934082
[26]	Compound::DB00783	-0.18119443953037262
[28]	Compound::DB00997	-0.1844681352376938
[32]	Compound::DB00563	-0.1951167732477188
[33]	Compound::DB00363	-0.1968984454870224
[35]	Compound::DB00661	-0.19837667047977448
[36]	Compound::DB04630	-0.20102301239967346
[38]	Compound::DB04652	-0.20188367366790771
[39]	Compound::DB00502	-0.2024267166852951
[42]	Compound::DB00477	-0.20295020937919617
[44]	Compound::DB01233	-0.20525988936424255
[46]	Compound::DB01229	-0.20591938495635986
[48]	Compound::DB00755	-0.20846834778785706
[49]	Compound::DB00640	-0.20932379364967346
[53]	Compound::DB00959	-0.21291860938072205
[54]	Compound::DB00608	-0.21537159383296967
[55]	Compound::DB12153	-0.2154090851545334
[56]	Compound::DB01183	-0.21780017018318176
[57]	Compound::DB00396	-0.21828481554985046
[58]	Compound::DB00458	-0.21880093216896057
[60]	Compound::DB09270	-0.22092074155807495
[62]	Compound::DB01708	-0.22179758548736572
[63]	Compound::DB00829	-0.22483842074871063
[66]	Compound::DB02169	-0.2264346033334732
[68]	Compound::DB00252	-0.23021790385246277
[69]	Compound::DB00321	-0.23166626691818237
[71]	Compound::DB01151	-0.23306965827941895
[72]	Compound::DB00908	-0.23369351029396057
[73]	Compound::DB00675	-0.23408204317092896
[74]	Compound::DB01100	-0.234358012676239
[75]	Compound::DB07795	-0.2368522584438324
[76]	Compound::DB04690	-0.23722517490386963
[77]	Compound::DB00762	-0.2373962104320526
[80]	Compound::DB15127	-0.24568934738636017
[83]	Compound::DB00806	-0.2460213303565979
[84]	Compound::DB01380	-0.24961985647678375
[85]	Compound::DB01069	-0.251217246055603
[86]	Compound::DB00715	-0.2516964375972748
[88]	Compound::DB00297	-0.25253671407699585
[89]	Compound::DB01181	-0.25281310081481934
[91]	Compound::DB00541	-0.2555280029773712
[94]	Compound::DB00104	-0.25777652859687805
[95]	Compound::DB00451	-0.25897955894470215
[96]	Compound::DB00747	-0.25976595282554626
[97]	Compound::DB00813	-0.2615016996860504
[100]	Compound::DB12290	-0.2625877559185028
```

## 结果分析

- [6] [DB04540](https://go.drugbank.com/drugs/DB04540): **Cholesterol**(胆固醇), The principal sterol of all higher animals, distributed in body tissues, especially the brain and spinal cord, and in animal fats and oils.(所有高等动物的主要固醇，分布于身体组织，特别是大脑和脊髓，以及动物脂肪和油中。)

   - **Cholesterol Metabolism** Is **a Druggable Axis** that Independently Regulates Tau and Amyloid-β in iPSC-Derived Alzheimer's Disease Neurons. (**胆固醇代谢**是独立调节iPSC衍生阿尔茨海默病神经元中Tau和淀粉样蛋白-β的**可药用轴**)
   
   - van der Kant R, Langness VF, Herrera CM, Williams DA, Fong LK, Leestemaker Y, Steenvoorden E, Rynearson KD, Brouwers JF, Helms JB, Ovaa H, Giera M, Wagner SL, Bang AG, Goldstein LSB. Cholesterol Metabolism Is a Druggable Axis that Independently Regulates Tau and Amyloid-β in iPSC-Derived Alzheimer's Disease Neurons. Cell Stem Cell. 2019 Mar 7;24(3):363-375.e9. doi: 10.1016/j.stem.2018.12.013. Epub 2019 Jan 24. PMID: 30686764; PMCID: PMC6414424. link: https://pubmed.ncbi.nlm.nih.gov/30686764/ .

- [8] [DB01224](https://go.drugbank.com/drugs/DB01224): **Quetiapine** is a psychotropic agent used for the management of bipolar disorder, schizophrenia, and major depressive disorder.(**奎硫平**是一种精神药物，用于治疗双相情感障碍、精神分裂症和重度抑郁症。)

   - **Quetiapine** combined with sodium valproate is an effective and more suitable drug treatment for Alzheimer's disease.(**奎硫平**联合丙戊酸钠是治疗阿尔茨海默病的有效且更合适的药物。)
   
   - Zhang Z, Xu J, Xu P, Liu W, He X, Fu K. Quetiapine Combined with Sodium Valproate in Patients with Alzheimer's Disease with Mental and Behavioral Symptoms Efficacy Observation. J Healthc Eng. 2022 Jan 17;2022:1278092. doi: 10.1155/2022/1278092. PMID: 35083020; PMCID: PMC8786510. link: https://pubmed.ncbi.nlm.nih.gov/35083020/ .

- [9] [DB00295](https://go.drugbank.com/drugs/DB00295): Morphine is an opioid agonist used for the relief of moderate to severe acute and chronic pain.(吗啡是一种阿片类激动剂，用于缓解中重度急性和慢性疼痛。)

   - 并没有发现有研究表明 Morphine 能够治疗 AD.

- [11] [DB00515](https://go.drugbank.com/drugs/DB00515): **Cisplatin** is a platinum based chemotherapy agent used to treat various sarcomas, carcinomas, lymphomas, and germ cell tumors.(**顺铂**是一种铂基化疗剂，用于治疗各种肉瘤、癌、淋巴瘤和生殖细胞肿瘤。)

   - **Cisplatin** inhibits the formation of a reactive intermediate during copper-catalyzed oxidation of amyloid β peptide. These findings may lead to the design of better platinum complexes to treat oxidative stress in Alzheimer's disease and other related neurological disorders.(**顺铂抑制铜催化氧化淀粉样β肽过程中活性中间体的形成**, 这些发现可能导致设计更好的铂配合物来治疗阿尔茨海默病和其他相关神经疾病中的氧化应激。)
   
   - Walke GR, Rapole S, Kulkarni PP. Cisplatin inhibits the formation of a reactive intermediate during copper-catalyzed oxidation of amyloid β peptide. Inorg Chem. 2014 Oct 6;53(19):10003-5. doi: 10.1021/ic5007764. Epub 2014 Sep 19. PMID: 25237806. link: https://pubmed.ncbi.nlm.nih.gov/25237806/ .

- [12] [DB09341](https://go.drugbank.com/drugs/DB09341): **Glucose** is a form of glucose used for caloric supply and the replenishment of fluid in total parenteral nutrition and other therapies as well as for the treatment of hypoglycemic episodes.(**葡萄糖**是一种葡萄糖，用于全胃肠外营养和其他疗法中的热量供应和补充液体，以及治疗低血糖发作。)
   
   - poorly controlled blood sugar may increase the risk of developing Alzheimer's. Furthermore, insulin-related therapeutic strategies are suggested to succeed in the development of therapies for AD by slowing down their progressive nature or even halting their future complications.(血糖控制不佳可能会增加患老年痴呆症的风险。此外，**胰岛素相关的治疗策略被建议通过减缓AD的进展性甚至停止其未来的并发症来成功开发AD治疗方法。**)
   
   - Nguyen TT, Ta QTH, Nguyen TKO, Nguyen TTD, Giau VV. Type 3 Diabetes and Its Role Implications in Alzheimer's Disease. Int J Mol Sci. 2020 Apr 30;21(9):3165. doi: 10.3390/ijms21093165. PMID: 32365816; PMCID: PMC7246646. link: https://pubmed.ncbi.nlm.nih.gov/32365816/ .

- [13] [DB00143](https://go.drugbank.com/drugs/DB00143): **Glutathione**(谷胱甘肽), A tripeptide with many roles in cells. It conjugates to drugs to make them more soluble for excretion, is a cofactor for some enzymes, is involved in protein disulfide bond rearrangement and reduces peroxides.(在细胞中具有多种作用的三肽。它与药物缀合，使药物更易溶解于排泄物，是某些酶的辅因子，参与蛋白质二硫键重排并减少过氧化物。)

   - The beneficial effect of many nutrients on the course of AD has been demonstrated. These include: **glutathione**, polyphenols, curcumin, coenzyme Q10, vitamins B6, B12, folic acid, unsaturated fatty acids, lecithin, UA, caffeine and some probiotic bacteria.(许多营养素对AD过程的有益作用已经被证明。其中包括：**谷胱甘肽**、多酚、姜黄素、辅酶Q10、维生素B6、B12、叶酸、不饱和脂肪酸、卵磷脂、尿酸、咖啡因和一些益生菌。)
   
   - Śliwińska S, Jeziorek M. The role of nutrition in Alzheimer's disease. Rocz Panstw Zakl Hig. 2021;72(1):29-39. doi: 10.32394/rpzh.2021.0154. PMID: 33882663. link: https://pubmed.ncbi.nlm.nih.gov/33882663/ .

- [15] [DB04216](https://go.drugbank.com/drugs/DB04216): **Quercetin** is a natural flavonoid found in foods and natural supplement products.(**槲皮素**是一种天然类黄酮，存在于食品和天然补充剂产品中。)

   - **Quercetin** has demonstrated antioxidant, anti-inflammatory, hypoglycemic, and hypolipidemic activities, suggesting therapeutic potential against type 2 diabetes mellitus (T2DM) and Alzheimer's disease (AD).(**槲皮素**已显示出抗氧化、抗炎、降血糖和降血脂活性，表明其对2型糖尿病（T2DM）和阿尔茨海默病（AD）具有治疗潜力。) 
   
   - Zu G, Sun K, Li L, Zu X, Han T, Huang H. Mechanism of quercetin therapeutic targets for Alzheimer disease and type 2 diabetes mellitus. Sci Rep. 2021 Nov 25;11(1):22959. doi: 10.1038/s41598-021-02248-5. PMID: 34824300; PMCID: PMC8617296. link: https://pubmed.ncbi.nlm.nih.gov/34824300/ .

- [16] [DB00907](https://go.drugbank.com/drugs/DB00907): **Cocaine** is an ester local anesthetic used during diagnostic procedures and surgeries in or through the nasal cavities.(**可卡因**是一种酯类局部麻醉剂，用于鼻腔内或通过鼻腔的诊断程序和手术。) 

   - The accumulation of amyloid-beta (Aβ) and oxidative stress damage in the brain are recognized as early features of Alzheimer's disease (AD). **The cocaine- and amphetamine-regulated transcript** (CART) peptide may possibly play an antioxidative role in neurons.Our results therefore indicate that CART peptide could serve as an antioxidant in early therapy for AD. (β淀粉样蛋白（Aβ）的积累和大脑中的氧化应激损伤被认为是阿尔茨海默病（AD）的早期特征。**可卡因和苯丙胺调节转录物**（CART）肽可能在神经元中**发挥抗氧化作用**。因此，我们的结果表明CART肽可以作为AD早期治疗的抗氧化剂。)
   
   - Jiao W, Wang Y, Kong L, Ou-Yang T, Meng Q, Fu Q, Hu Z. CART peptide activates the Nrf2/HO-1 antioxidant pathway and protects hippocampal neurons in a rat model of Alzheimer's disease. Biochem Biophys Res Commun. 2018 Jul 2;501(4):1016-1022. doi: 10.1016/j.bbrc.2018.05.101. Epub 2018 May 18. PMID: 29777699. link: https://pubmed.ncbi.nlm.nih.gov/29777699/ .

- [17] [DB06774](https://go.drugbank.com/drugs/DB06774): **Capsaicin** is a topical analgesic agent used for the symptomatic relief of neuropathic pain associated with post-herpetic neuralgia, as well as other muscle and joint pain.(**辣椒素**是一种局部镇痛剂，用于缓解疱疹后神经痛以及其他肌肉和关节疼痛相关的神经性疼痛。)

   - Many recent publications show the positive effects of capsaicin in animal models of brain disorders. In Alzheimer's disease, **capsaicin** reduces neurodegeneration and memory impairment.(最近的许多出版物显示辣椒素在脑疾病动物模型中的积极作用。在阿尔茨海默病中，**辣椒素**可以减少神经退化和记忆障碍。)
   
   - Pasierski M, Szulczyk B. Beneficial Effects of Capsaicin in Disorders of the Central Nervous System. Molecules. 2022 Apr 12;27(8):2484. doi: 10.3390/molecules27082484. PMID: 35458680; PMCID: PMC9029810. link: https://pubmed.ncbi.nlm.nih.gov/35458680/ .

- [20] [DB00171](https://go.drugbank.com/drugs/DB00171): **ATP**, An adenine nucleotide containing three phosphate groups esterified to the sugar moiety. In addition to its crucial roles in metabolism adenosine triphosphate is a neurotransmitter.(一种腺嘌呤核苷酸，含有三个与糖部分酯化的磷酸基团。除了在新陈代谢中的关键作用外，三磷酸腺苷还是一种神经递质。)

   - Microglial cells consume adenosine triphosphate (ATP) during phagocytosis to clear neurotoxic β-amyloid in Alzheimer's disease (AD).(**小胶质细胞在吞噬过程中消耗三磷酸腺苷（ATP）**，以清除阿尔茨海默病（AD）中的神经毒性β-淀粉样蛋白。) 
   
   - Leng L, Yuan Z, Pan R, Su X, Wang H, Xue J, Zhuang K, Gao J, Chen Z, Lin H, Xie W, Li H, Chen Z, Ren K, Zhang X, Wang W, Jin ZB, Wu S, Wang X, Yuan Z, Xu H, Chow HM, Zhang J. Microglial hexokinase 2 deficiency increases ATP generation through lipid metabolism leading to β-amyloid clearance. Nat Metab. 2022 Oct;4(10):1287-1305. doi: 10.1038/s42255-022-00643-4. Epub 2022 Oct 6. Erratum in: Nat Metab. 2022 Oct 14;: PMID: 36203054. link: https://pubmed.ncbi.nlm.nih.gov/36203054/ .

- [22] [DB00624](https://go.drugbank.com/drugs/DB00624): **Testosterone** is a hormone used to treat hypogonadism, breast carcinoma in women, or the vasomotor symptoms of menopause.(**睾酮**是一种用于治疗性腺功能减退、女性乳腺癌或更年期血管舒缩症状的激素。)

   - Animal models demonstrated that **testosterone** (T) exerted a neuroprotective effect reducing the production of amyloid-beta (Aβ), improving synaptic signaling, and counteracting neuronal death.(动物模型表明，**睾酮**（T）具有神经保护作用，减少淀粉样蛋白β（aβ）的产生，改善突触信号，并对抗神经元死亡。)
   
   - Bianchi VE. Impact of Testosterone on Alzheimer's Disease. World J Mens Health. 2022 Apr;40(2):243-256. doi: 10.5534/wjmh.210175. Epub 2022 Jan 2. PMID: 35021306; PMCID: PMC8987133. link: https://pubmed.ncbi.nlm.nih.gov/35021306/ .

- [25] [DB02527](https://go.drugbank.com/drugs/DB02527): **Cyclic adenosine monophosphate**(环磷酸腺苷), Cyclic adenosine monophosphate (cAMP, cyclic AMP or 3'-5'-cyclic adenosine monophosphate) is a molecule that is important in many biological processes; it is derived from adenosine triphosphate (ATP).(环磷酸腺苷（cAMP、环AMP或3'-5'-环磷酸腺苷）是一种在许多生物过程中很重要的分子；它来源于三磷酸腺苷（ATP）。)

   - Preclinical studies, clinical trials, and reviews suggest increasing **3',5'-cyclic adenosine monophosphate** (cAMP) and **3',5'-cyclic guanosine monophosphate** (cGMP) with phosphodiesterase inhibitors is disease-modifying in Alzheimer's disease (AD).(临床前研究、临床试验和综述表明，使用磷酸二酯酶抑制剂增加**3'，5'-环磷酸腺苷**（cAMP）和**3'，5'-环磷酸鸟苷**（cGMP）可改善阿尔茨海默病（AD）的病情。)
   
   - Sanders O, Rajagopal L. Phosphodiesterase Inhibitors for Alzheimer's Disease: A Systematic Review of Clinical Trials and Epidemiology with a Mechanistic Rationale. J Alzheimers Dis Rep. 2020 Jun 16;4(1):185-215. doi: 10.3233/ADR-200191. PMID: 32715279; PMCID: PMC7369141. link: https://pubmed.ncbi.nlm.nih.gov/32715279/ .

- [26] [DB00783](https://go.drugbank.com/drugs/DB00783): **Estradiol** is an estrogenic steroid used to treat vasomotor symptoms of vulvar and vaginal atrophy in menopause, hypoestrogenism, prevention of postmenopausal osteoporosis, treatment of breast cancer, and advanced androgen-dependent carcinoma of the prostate.(雌二醇是一种雌激素类固醇，用于治疗更年期外阴和阴道萎缩的血管舒缩症状、雌激素减少、预防绝经后骨质疏松症、治疗乳腺癌和晚期雄激素依赖性前列腺癌。)

   - Mounting evidence indicates that the neurosteroid estradiol (**17β-estradiol**) plays a supporting role in neurogenesis, neuronal activity, and synaptic plasticity of AD. This effect may provide preventive and/or therapeutic approaches for AD.(越来越多的证据表明，神经甾体雌二醇（**17β-雌二醇**）在AD的神经发生、神经元活动和突触可塑性中起着支持作用。这种作用可能为AD提供预防和/或治疗途径。)
   
   - Sahab-Negah S, Hajali V, Moradi HR, Gorji A. The Impact of Estradiol on Neurogenesis and Cognitive Functions in Alzheimer's Disease. Cell Mol Neurobiol. 2020 Apr;40(3):283-299. doi: 10.1007/s10571-019-00733-0. Epub 2019 Sep 9. PMID: 31502112. link: https://pubmed.ncbi.nlm.nih.gov/31502112/ .

- [28] [DB00997](https://go.drugbank.com/drugs/DB00997): Doxorubicin is a medication used to treat various cancers and Kaposi's Sarcoma.(阿霉素是一种用于治疗各种癌症和卡波西肉瘤的药物。)

   - 并没有发现有研究表明 Doxorubicin 能够治疗 AD.

- [32] [DB00563](https://go.drugbank.com/drugs/DB00563): **Methotrexate** is an antineoplastic agent used the treatment of a wide variety of cancers as well as severe psoriasis, severe rheumatoid arthritis, and juvenile rheumatoid arthritis.(**甲氨蝶呤**是一种抗肿瘤药物，用于治疗多种癌症以及严重的牛皮癣、严重的类风湿性关节炎和幼年类风湿性关节炎。)

   - In addition, the issue of the potential benefits of **methotrexate** in the development of neurological disorders in Alzheimer's disease or myasthenia gravis will be discussed.(此外，还将讨论**甲氨蝶呤**在阿尔茨海默病或重症肌无力的神经紊乱发展中的潜在益处的问题。)
   
   - Koźmiński P, Halik PK, Chesori R, Gniazdowska E. Overview of Dual-Acting Drug Methotrexate in Different Neurological Diseases, Autoimmune Pathologies and Cancers. Int J Mol Sci. 2020 May 14;21(10):3483. doi: 10.3390/ijms21103483. PMID: 32423175; PMCID: PMC7279024. link: https://pubmed.ncbi.nlm.nih.gov/32423175/ .

- [33] [DB00363](https://go.drugbank.com/drugs/DB00363): **Clozapine** is an antipsychotic drug used in treatment resistant schizophrenia and to decrease suicide risk in schizophrenic patients.(**氯氮平**是一种抗精神病药物，用于治疗抗精神分裂症和降低精神分裂症患者的自杀风险。)

   - This study suggests that as one of candidate for multi-target approach of AD treatment, **clozapine** is proposed as a therapeutic drug for treatment of AD patients.(这项研究表明，作为多靶点治疗AD的候选方法之一，**氯氮平**被提议作为治疗AD患者的治疗药物。)
   
   - Choi Y, Jeong HJ, Liu QF, Oh ST, Koo BS, Kim Y, Chung IW, Kim YS, Jeon S. Clozapine Improves Memory Impairment and Reduces Aβ Level in the Tg-APPswe/PS1dE9 Mouse Model of Alzheimer's Disease. Mol Neurobiol. 2017 Jan;54(1):450-460. doi: 10.1007/s12035-015-9636-x. Epub 2016 Jan 7. PMID: 26742522. link: https://pubmed.ncbi.nlm.nih.gov/26742522/ .

- [35] [DB00661](https://go.drugbank.com/drugs/DB00661): **Verapamil** is a non-dihydropyridine calcium channel blocker used in the treatment of angina, arrhythmia, and hypertension.

   - Thus, the present study demonstrates the neuroprotective effect of **verapamil** against the pathogenesis of AD such as oxidative stress, mitochondrial dysfunction and cognitive decline.(因此，本研究证明了**维拉帕米**对AD发病机制的神经保护作用，如氧化应激、线粒体功能障碍和认知功能下降。)
   
   - Ponne S, Kumar CR, Boopathy R. Verapamil attenuates scopolamine induced cognitive deficits by averting oxidative stress and mitochondrial injury - A potential therapeutic agent for Alzheimer's Disease. Metab Brain Dis. 2020 Mar;35(3):503-515. doi: 10.1007/s11011-019-00498-x. Epub 2019 Nov 5. PMID: 31691145. link: https://pubmed.ncbi.nlm.nih.gov/31691145/ .

- [36] [DB04630](https://go.drugbank.com/drugs/DB04630): Aldosterone(醛固酮), A hormone secreted by the adrenal cortex that regulates electrolyte and water balance by increasing the renal retention of sodium and the excretion of potassium.(肾上腺皮质分泌的一种激素，通过增加肾内钠的潴留和钾的排泄来调节电解质和水平衡。)

   - 并没有发现有研究表明 Aldosterone 能够治疗 AD.

- [38] [DB04652](https://go.drugbank.com/drugs/DB04652): Corticosterone(皮质酮), An adrenocortical steroid that has modest but significant activities as a mineralocorticoid and a glucocorticoid. (From Goodman and Gilman's The Pharmacological Basis of Therapeutics, 8th ed, p1437)(一种肾上腺皮质激素，作为盐皮质激素和糖皮质激素具有适度但显著的活性。（摘自古德曼和吉尔曼的《治疗学的药理学基础》，第8版，第437页）)

   - 并没有发现有研究表明 Corticosterone 能够治疗 AD.

- [39] [DB00502](https://go.drugbank.com/drugs/DB00502): **Haloperidol** is an antipsychotic agent used to treat schizophrenia and other psychoses, as well as symptoms of agitation, irritability, and delirium.(**氟哌啶醇**是一种抗精神病药，用于治疗精神分裂症和其他精神病，以及焦虑、易怒和谵妄症状.)

   - The goal of this study was to compare the efficacy and side effects of two doses of haloperidol and placebo in the treatment of psychosis and disruptive behaviors in patients with Alzheimer's disease. The results indicated a favorable therapeutic profile for **haloperidol** in doses of 2-3 mg/day, although a subgroup developed moderate to severe extrapyramidal signs. (本研究的目的是比较两剂氟哌啶醇和安慰剂治疗阿尔茨海默病患者精神病和破坏行为的疗效和副作用。结果表明，尽管一个亚组出现了中度至重度锥体外系症状，但剂量为2-3 mg/天的**氟哌啶醇**治疗效果良好。)
   
   - Devanand DP, Marder K, Michaels KS, Sackeim HA, Bell K, Sullivan MA, Cooper TB, Pelton GH, Mayeux R. A randomized, placebo-controlled dose-comparison trial of haloperidol for psychosis and disruptive behaviors in Alzheimer's disease. Am J Psychiatry. 1998 Nov;155(11):1512-20. doi: 10.1176/ajp.155.11.1512. PMID: 9812111. link: https://pubmed.ncbi.nlm.nih.gov/9812111/ .

- [42] [DB00477](https://go.drugbank.com/drugs/DB00477): **Chlorpromazine** is a phenothiazine antipsychotic used to treat nausea, vomiting, preoperative anxiety, schizophrenia, bipolar disorder, and severe behavioral problems in children.(**氯丙嗪**是一种吩噻嗪类抗精神病药，用于治疗儿童恶心、呕吐、术前焦虑、精神分裂症、双相情感障碍和严重的行为问题。)

   - The clinical applications of antipsychotics for symptoms unrelated to schizophrenia, such as behavioral and psychological symptoms, in patients with Alzheimer's disease, and the likelihood of doctors prescribing antipsychotics for elderly people are increasing.(**抗精神病药物在阿尔茨海默病患者中用于治疗与精神分裂症无关的症状**，如行为和心理症状，医生为老年人开抗精神病药的可能性正在增加。)
   
   - Obara K, Matsuoka Y, Iwata N, Abe Y, Ikegami Y, Shioda N, Hattori Y, Hamamatsu S, Yoshioka K, Yamaki F, Matsuo K, Yoshio T, Tanaka Y. Inhibitory Effects of Antipsychotics on the Contractile Response to Acetylcholine in Rat Urinary Bladder Smooth Muscles. Biol Pharm Bull. 2021;44(8):1140-1150. doi: 10.1248/bpb.b21-00363. PMID: 34334499. link: https://pubmed.ncbi.nlm.nih.gov/34334499/ .

- [44] [DB01233](https://go.drugbank.com/drugs/DB01233): Metoclopramide is an antiemetic agent and dopamine D2 antagonist used in the treatment of gastroesophageal reflux disease, prevention of nausea and vomiting, and to stimulate gastric emptying.(甲氧氯普胺是一种止吐剂和多巴胺D2拮抗剂，用于治疗胃食管反流病、预防恶心和呕吐以及刺激胃排空。)

   - 并没有发现有研究表明 Metoclopramide 能够治疗 AD.

- [46] [DB01229](https://go.drugbank.com/drugs/DB01229): **Paclitaxel** is a taxoid chemotherapeutic agent used as first-line and subsequent therapy for the treatment of advanced carcinoma of the ovary, and other various cancers including breast and lung cancer.(**紫杉醇**是一种紫杉醇类化疗药物，用作治疗晚期卵巢癌和其他各种癌症（包括乳腺癌和肺癌）的一线和后续治疗。)

   - In addition to NSAIDs, an anticancer drug, **paclitaxel**, has considerable potential as an AD treatment.(除了非甾体抗炎药外，**紫杉醇**是一种抗癌药物，具有相当大的治疗AD的潜力。)
   
   - Lehrer S, Rheinstein PH. Transspinal delivery of drugs by transdermal patch back-of-neck for Alzheimer's disease: a new route of administration. Discov Med. 2019 Jan;27(146):37-43. PMID: 30721650. link: https://pubmed.ncbi.nlm.nih.gov/30721650/ .

- [48] [DB00755](https://go.drugbank.com/drugs/DB00755): **Tretinoin** is a vitamin A derivative used to treat acne vulgaris, certain types of promyelocytic leukemia, and fine wrinkles.(**维甲酸**是一种维生素a衍生物，用于治疗寻常痤疮、某些类型的早幼粒细胞白血病和细皱纹。)

   - **Retinoic acid** is a potent cell differentiating factor, which through its nuclear receptors affects a vast range of promoter sites in brain neuronal and glial cells in every step of embryonic and postnatal life. Its capacities, facilitating maturation of neurotransmitter phenotype in different groups of neurons, pave the way for its application as a potential therapeutic agent in neurodegenerative diseases including Alzheimer's disease.(**维甲酸**是一种有效的细胞分化因子，在胚胎和出生后的每一步，它通过其核受体影响脑神经元和神经胶质细胞中的大量启动子位点。它的能力，促进不同神经元群神经递质表型的成熟，为其作为神经退行性疾病（包括阿尔茨海默病）潜在治疗剂的应用铺平了道路。)
   
   - Szutowicz A, Bielarczyk H, Jankowska-Kulawy A, Ronowska A, Pawełczyk T. Retinoic acid as a therapeutic option in Alzheimer's disease: a focus on cholinergic restoration. Expert Rev Neurother. 2015 Mar;15(3):239-49. doi: 10.1586/14737175.2015.1008456. Epub 2015 Feb 15. PMID: 25683350. link: https://pubmed.ncbi.nlm.nih.gov/25683350/ .

- [49] [DB00640](https://go.drugbank.com/drugs/DB00640): Adenosine is a medication used in myocardial perfusion scintigraphy and to treat supraventricular tachycardia.(腺苷是一种用于心肌灌注显像和治疗室上性心动过速的药物。)

   - 并没有发现有研究表明 Adenosine 能够治疗 AD.

- [53] [DB00959](https://go.drugbank.com/drugs/DB00959): Methylprednisolone is a corticosteroid used to treat inflammation or immune reactions across a variety of organ systems, endocrine conditions, and neoplastic diseases.(甲基泼尼松龙是一种皮质类固醇，用于治疗各种器官系统、内分泌疾病和肿瘤疾病的炎症或免疫反应。)

   - 并没有发现有研究表明 Methylprednisolone 能够治疗 AD.

- [54] [DB00608](https://go.drugbank.com/drugs/DB00608): Chloroquine is an antimalarial drug used to treat susceptible infections with P. vivax, P. malariae, P. ovale, and P. falciparum. It is also used for second line treatment for rheumatoid arthritis.(氯喹是一种抗疟药物，用于治疗间日疟原虫、疟疾疟原虫、卵圆疟原虫和恶性疟原虫的易感感染。它也用于类风湿关节炎的二线治疗。)

   - 并没有发现有研究表明 Chloroquine 能够治疗 AD.

- [55] [DB12153](https://go.drugbank.com/drugs/DB12153): **Citicoline** is an endogenous intermediate in the formation of phosphatidylcholine from choline which is thought to have neuroprotective effects.(**胞磷胆碱**是胆碱形成磷脂酰胆碱的内源性中间体，被认为具有神经保护作用。)

   - Then, we added citicoline to memantine in the CITIMEM study, and finally, we demonstrated benefits in terms of delay in cognitive worsening with the triple therapy (**citicoline** + AchEIs + memantine). Other authors also reinforced our hypothesis through two further studies. Open, prospective studies are advised to confirm the utility of combination therapy with citicoline for the treatment of AD and MD. (然后，在CITIMEM研究中，我们将胞磷胆碱添加到美金刚中，最后，我们证明了三联疗法（**胞磷胆碱**+乙酰胆碱+美金刚）在延缓认知恶化方面的益处。其他作者也通过两项进一步的研究加强了我们的假设。建议进行开放性前瞻性研究，以确认胞磷胆碱联合治疗AD和MD的效用。)
   
   - Gareri P, Veronese N, Cotroneo AM. An Overview of Combination Treatment with Citicoline in Dementia. Rev Recent Clin Trials. 2022;17(1):4-8. doi: 10.2174/1574887117666211221170344. PMID: 34939548. link: https://pubmed.ncbi.nlm.nih.gov/34939548/ .

- [56] [DB01183](https://go.drugbank.com/drugs/DB01183): Naloxone is an opioid receptor antagonist used to rapidly reverse an opioid overdose. Also included in some drug formulations as an abuse deterrent to prevent injection.(纳洛酮是一种阿片受体拮抗剂，用于快速逆转阿片类药物过量。也包括在一些药物配方中，作为防止注射的滥用威慑。)

   - 并没有发现有研究表明 Naloxone 能够治疗 AD.

- [57] [DB00396](https://go.drugbank.com/drugs/DB00396): **Progesterone** is a hormone used for a variety of functions, including contraception, control of abnormal uterine bleeding, maintenance of pregnancy, and prevention of endometrial hyperplasia.(孕激素是一种用于多种功能的激素，包括避孕、控制异常子宫出血、维持妊娠和预防子宫内膜增生。)

   - Alzheimer's disease (AD) is closely related to abnormal glucose metabolism in the central nervous system. **Progesterone** has been shown to have obvious neuroprotective effects in the pathogenesis of AD, but the specific mechanism has not been fully elucidated. These results confirm that progesterone significantly improves the glucose metabolism of neurons.(阿尔茨海默病（AD）与中枢神经系统葡萄糖代谢异常密切相关。**黄体酮**在AD发病机制中具有明显的神经保护作用，但其具体机制尚未完全阐明。这些结果证实，黄体酮显著改善了神经元的葡萄糖代谢.)
   
   - Wu H, Wu ZG, Shi WJ, Gao H, Wu HH, Bian F, Jia PP, Hou YN. Effects of progesterone on glucose uptake in neurons of Alzheimer's disease animals and cell models. Life Sci. 2019 Dec 1;238:116979. doi: 10.1016/j.lfs.2019.116979. Epub 2019 Oct 21. PMID: 31647947. link: https://pubmed.ncbi.nlm.nih.gov/31647947/ .

- [58] [DB00458](https://go.drugbank.com/drugs/DB00458): **Imipramine** is a tricyclic antidepressant indicated for the treatment of depression and to reduce childhood enuresis.(**丙咪嗪**是一种三环类抗抑郁药，用于治疗抑郁症和减少儿童遗尿。)

   - So, **imipramine** prevents memory impairment through its intrinsic property to inhibit TNF-alpha and Abeta accumulation and may represent a potential candidate for AD treatment.(因此，丙咪嗪通过其抑制TNF-α和Abeta积累的内在特性防止记忆损伤，可能是AD治疗的潜在候选药物。)
   
   - Chavant F, Deguil J, Pain S, Ingrand I, Milin S, Fauconneau B, Pérault-Pochat MC, Lafay-Chebassier C. Imipramine, in part through tumor necrosis factor alpha inhibition, prevents cognitive decline and beta-amyloid accumulation in a mouse model of Alzheimer's disease. J Pharmacol Exp Ther. 2010 Feb;332(2):505-14. doi: 10.1124/jpet.109.162164. Epub 2009 Nov 4. PMID: 19889791. link: https://pubmed.ncbi.nlm.nih.gov/19889791/ .

- [60] [DB09270](https://go.drugbank.com/drugs/DB09270): **Ubidecarenone** is a cofactor found in various dietary supplements. Ubidecarenone, also called **coenzyme Q10**, is a 1,4-benzoquinone. From its name (Q10), the Q refers to the constitutive quinone group, and 10 is related to the number of isoprenyl subunits in its tail.(Ubidecarenone是多种膳食补充剂中的辅因子。Ubidecarenone，也称为**辅酶Q10**，是一种1,4-苯醌。从其名称（Q10）来看，Q指的是组成性醌基团，10与其尾部的异戊二烯亚基的数量有关。)

   - The beneficial effect of many nutrients on the course of AD has been demonstrated. These include: glutathione, polyphenols, curcumin, **coenzyme Q10**, vitamins B6, B12, folic acid, unsaturated fatty acids, lecithin, UA, caffeine and some probiotic bacteria.(许多营养素对阿尔兹海默症病程的有益作用已被证明。这些包括：谷胱甘肽、多酚、姜黄素、**辅酶 Q10**、维生素 B6、B12、叶酸、不饱和脂肪酸、卵磷脂、UA、咖啡因和一些益生菌。)
   
   - Śliwińska S, Jeziorek M. The role of nutrition in Alzheimer's disease. Rocz Panstw Zakl Hig. 2021;72(1):29-39. doi: 10.32394/rpzh.2021.0154. PMID: 33882663. link:https://pubmed.ncbi.nlm.nih.gov/33882663/ .

- [62] [DB01708](https://go.drugbank.com/drugs/DB01708): **Prasterone** is a steroid formulated as a vaginal insert indicated for the treatment of moderate to severe dyspareunia associated with menopausal vulvar and vaginal atrophy. Prasterone, also known as **dehydroepiandrosterone** (DHEA) is a major C19 steroid produced by the adrenal cortex. It is also produced in small quantities in the testis and the ovary.(Prasterone 是一种作为阴道插入物配制的类固醇，用于治疗与更年期外阴和阴道萎缩相关的中度至重度性交困难。普拉酮，也称为**脱氢表雄酮**（DHEA）是由肾上腺皮质产生的主要C19类固醇。它也在睾丸和卵巢中少量产生。)

   - Neurodegenerative diseases, such as multiple sclerosis (MS), Alzheimer's disease (AD), Parkinson's disease (PD) and traumatic brain injury (TBI), display inflammatory activation of microglia and astrocytes. Intriguingly, the central nervous system (CNS) is a highly steroidogenic environment synthesizing steroids de novo, as well as metabolizing steroids deriving from the circulation. Neurosteroid synthesis can be substantially affected by neuroinflammation, while, in turn, several steroids, such as 17β-estradiol, **dehydroepiandrosterone** (DHEA) and allopregnanolone, can regulate neuroinflammatory responses.(神经退行性疾病，如多发性硬化症（MS），阿尔茨海默病（AD），帕金森病（PD）和创伤性脑损伤（TBI），显示出小胶质细胞和星形胶质细胞的炎症激活。有趣的是，中枢神经系统（CNS）是一个高度类固醇生成的环境，从头合成类固醇，以及代谢来自循环的类固醇。神经类固醇的合成可以受到神经炎症的严重影响，而反过来，几种类固醇，如17β-雌二醇，**脱氢表雄酮**（DHEA）和异孕酮，可以调节神经炎症反应。)
   
   - Yilmaz C, Karali K, Fodelianaki G, Gravanis A, Chavakis T, Charalampopoulos I, Alexaki VI. Neurosteroids as regulators of neuroinflammation. Front Neuroendocrinol. 2019 Oct;55:100788. doi: 10.1016/j.yfrne.2019.100788. Epub 2019 Sep 9. PMID: 31513776.link:https://pubmed.ncbi.nlm.nih.gov/31513776/ .

- [63] [DB00829](https://go.drugbank.com/drugs/DB00829): **Diazepam** is a long-acting benzodiazepine with rapid onset commonly used to treat panic disorders, severe anxiety, alcohol withdrawal, and seizures.(**地西泮**是一种起效快效的长效苯二氮卓类药物，通常用于治疗惊恐障碍、严重焦虑、酒精戒断和癫痫发作。)

   - One may suggest that at low and moderate doses diazepam is targeting non-specific, probably allosteric GABAA receptor sites, thus leading to stimulatory effects that can be beneficial for **diazepam** use in early pre-dementia stages of AD.(有人可能认为，在低剂量和中等剂量下，**地西泮**靶向非特异性的，可能是变构的GABAA受体位点，从而导致刺激作用，这可能有益于在AD早期痴呆前阶段使用地西泮。)
   
   - Pilipenko V, Narbute K, Pupure J, Rumaks J, Jansone B, Klusa V. Neuroprotective action of diazepam at very low and moderate doses in Alzheimer's disease model rats. Neuropharmacology. 2019 Jan;144:319-326. doi: 10.1016/j.neuropharm.2018.11.003. Epub 2018 Nov 5. PMID: 30408486. link:https://pubmed.ncbi.nlm.nih.gov/30408486/ .
 
- [66] [DB02169](https://go.drugbank.com/drugs/DB02169): 9,10-Deepithio-9,10-Didehydroacanthifolicin(9，10-脱硫代-9，10-二脱氢坎硫磷脂素), A specific inhibitor of phosphoserine/threonine protein phosphatase 1 and 2a. It is also a potent tumor promoter. (磷酸丝氨酸/苏氨酸蛋白磷酸酶 1 和 2a 的特异性抑制剂。它也是一种有效的肿瘤促进剂。)

   - 并没有研究表明 9,10-Deepithio-9,10-Didehydroacanthifolicin 能够治疗 AD. 

- [68] [DB00252](https://go.drugbank.com/drugs/DB00252): **Phenytoin** is an anticonvulsant drug used in the prophylaxis and control of various types of seizures.(**苯妥英钠**是一种抗惊厥药物，用于预防和控制各种类型的癫痫发作。)

   - among many drugs that have been shown to prevent hippocampal atrophy is phenytoin. It is time tested and proven anticonvulsant that can be used to prevent the development of atrophy and consequent development of AD. **Phenytoin** can thus be exploited for its dual effects i.e. reversal of hippocampal atrophy and anti-seizure effects. (在许多已被证明可以预防海马萎缩的药物中，苯妥英是苯妥英。它是经过时间考验和验证的抗惊厥药，可用于预防萎缩的发展和随后的AD发展。 因此，**苯妥英**因其双重作用而得到利用，即逆转海马萎缩和抗癫痫发作作用。)
   
   - Dhikav V. Can phenytoin prevent Alzheimer's disease? Med Hypotheses. 2006;67(4):725-8. doi: 10.1016/j.mehy.2006.04.038. Epub 2006 Jun 16. PMID: 16781825.link:https://pubmed.ncbi.nlm.nih.gov/16781825/


- [69] [DB00321](https://go.drugbank.com/drugs/DB00321): **Amitriptyline**(阿米替林),Amitriptyline hydrochloride, also known as Elavil, is a tricyclic antidepressant (TCA) with analgesic properties, widely used to treat depression and neuropathic pain . It was originally approved by the FDA in 1977 and manufactured by Sandoz .(盐酸阿米替林，又称Elavil，是一种具有镇痛特性的三环类抗抑郁药（TCA），广泛用于治疗抑郁症和神经性疼痛。它最初于1977年获得FDA批准，由Sandoz制造。)
   
   - These results indicate that **amitriptyline** has significant beneficial actions in aged and damaged AD brains and that it shows promise as a tolerable novel therapeutic for the treatment of AD.(这些结果表明，**阿米替林**对衰老和受损的AD大脑具有显着的有益作用，并且它有望成为治疗AD的可耐受新型疗法。)
   
   - Chadwick W, Mitchell N, Caroll J, Zhou Y, Park SS, Wang L, Becker KG, Zhang Y, Lehrmann E, Wood WH 3rd, Martin B, Maudsley S. Amitriptyline-mediated cognitive enhancement in aged 3×Tg Alzheimer's disease mice is associated with neurogenesis and neurotrophic activity. PLoS One. 2011;6(6):e21660. doi: 10.1371/journal.pone.0021660. Epub 2011 Jun 27. PMID: 21738757; PMCID: PMC3124550 . link:https://pubmed.ncbi.nlm.nih.gov/21738757/ .

- [71] [DB01151](https://go.drugbank.com/drugs/DB01151): **Desipramine**(地昔帕明), Desipramine hydrochloride is a dibenzazepine-derivative tricyclic antidepressant (TCA). TCAs are structurally similar to phenothiazines. They contain a tricyclic ring system with an alkyl amine substituent on the central ring.(**盐酸地昔帕明**是一种二苯并氮杂卓衍生物三环类抗抑郁药（TCA）。TCA在结构上与吩噻嗪类相似。它们包含一个三环环系统，中心环上有一个烷基胺取代基。)

   - It is noteworthy that approximately 40% of AD patients have depressive symptom. The close correlation between cognitive deficits and mental depression suggests a possibility that antidepression treatment might be beneficial to cognitive improvement in AD. The present study, by using tail-suspension test (TST), forced swimming, alternative electro-stimulus Y maze test and immunohistochemistry, examined the neuroprotective effects of **desipramine**,(值得注意的是，大约40%的AD患者有抑郁症状。认知缺陷与精神抑郁之间的密切相关性表明，抗抑郁治疗可能有益于AD的认知改善。本研究采用尾悬试验（TST）、强制游泳、替代电刺激Y迷宫试验和免疫组化等方法，考察了**地昔帕明**的神经保护作用)

   - Wang DD, Li J, Yu LP, Wu MN, Sun LN, Qi JS. Desipramine improves depression-like behavior and working memory by up-regulating p-CREB in Alzheimer's disease associated mice. J Integr Neurosci. 2016 Jun;15(2):247-60. doi: 10.1142/S021963521650014X. Epub 2016 Jun 23. PMID: 27338163.link:https://pubmed.ncbi.nlm.nih.gov/27338163/ .

- [72] [DB00908](https://go.drugbank.com/drugs/DB00908): **Quinidine** is a medication used to restore normal sinus rhythm, treat atrial fibrillation and flutter, and treat ventricular arrhythmias.(**奎尼丁**是一种用于恢复正常窦性心律、治疗心房颤动和扑动以及治疗室性心律失常的药物。)

   - Promising pharmaceuticals for neuropsychiatric symptoms of dementia include pimavanserin, brexpiprazole, escitalopram, dextromethorphan/**quinidine**, and lithium.(治疗痴呆神经精神症状的有前途的药物包括匹马色林、布瑞匹拉唑、艾司西酞普兰、右美沙芬/**奎尼丁**和锂。)

   - Aftab A, Lam JA, Liu F, Ghosh A, Sajatovic M. Recent developments in geriatric psychopharmacology. Expert Rev Clin Pharmacol. 2021 Mar;14(3):341-355. doi: 10.1080/17512433.2021.1882848. Epub 2021 Feb 5. PMID: 33499693.link:https://pubmed.ncbi.nlm.nih.gov/33499693/ .

- [73] [DB00675](https://go.drugbank.com/drugs/DB00675): Tamoxifen is a selective estrogen receptor modulator used to treat estrogen receptor positive breast cancer, reduce the risk of invasive breast cancer following surgery, or reduce the risk of breast cancer in high risk women.(他莫昔芬是一种选择性雌激素受体调节剂，用于治疗雌激素受体阳性乳腺癌，降低手术后侵袭性乳腺癌的风险，或降低高危女性患乳腺癌的危险。)
 
   - 并没有研究表明 Tamoxifen 能够治疗 AD.

- [74] [DB01100](https://go.drugbank.com/drugs/DB01100): **Pimozide** is an antipsychotic used to manage debilitating motor and phonic tics in patients with Tourette's Disorder.(
匹莫齐特是一种抗精神病药，用于治疗图雷特病患者的衰弱运动和发声抽搐。)

   - The aim of this study was to assess the potency of selected antipsychotic drugs (haloperidol (HAL), bromperidol (BRMP), benperidol (BNP), penfluridol (PNF), **pimozide** (PIM), quetiapine (QUET) and promazine (PROM)) on the main pathological hallmarks of Alzheimer's disease (AD). In the case of astrocytes, BNP, PNF, PIM and PROM showed antioxidant potential.(本研究的目的是评估选定的抗精神病药物（氟哌啶醇（HAL），溴哌啶醇（BRMP），苯哌啶醇（BNP），五氟利多（PNF），**匹莫齐特**（PIM），喹硫平（QUET）和丙嗪（PROM））对阿尔茨海默病（AD）的主要病理标志的效力。在星形胶质细胞的情况下，BNP，PNF，PIM和PROM显示出抗氧化潜力。)

   - Podsiedlik M, Markowicz-Piasecka M, Sikora J. The Influence of Selected Antipsychotic Drugs on Biochemical Aspects of Alzheimer's Disease. Int J Mol Sci. 2022 Apr 21;23(9):4621. doi: 10.3390/ijms23094621. PMID: 35563011; PMCID:PMC9102502.link:https://pubmed.ncbi.nlm.nih.gov/35563011/ .

- [75] [DB07795](https://go.drugbank.com/drugs/DB07795): **Fisetin**(漆黄素)

   - Among the most promising group of substances with potential activity against AD are the flavonoids, including myricetin, morin, rutin, quercetin, **fisetin**, kaempferol, apigenin and glycitein, which have been shown, in vitro, to possess antiamyloidogenic and fibril-destabilization activity, as well as being able to act as metal chelators and to suppressing oxidative stress.(具有潜在抗AD活性的一组最有希望的物质是类黄酮，包括杨梅素，桑黄素，芦丁，槲皮素，**漆黄素**，山奈酚，芹菜素和黄豆黄素，它们在体外已被证明具有抗淀粉样蛋白生成和原纤维不稳定活性，以及能够作为金属螯合剂和抑制氧化应激。)

   - Simunkova M, Alwasel SH, Alhazza IM, Jomova K, Kollar V, Rusko M, Valko M. Management of oxidative stress and other pathologies in Alzheimer's disease. Arch Toxicol. 2019 Sep;93(9):2491-2513. doi: 10.1007/s00204-019-02538-y. Epub2019Aug22.PMID:31440798.link:https://pubmed.ncbi.nlm.nih.gov/31440798/ .

- [76] [DB04690](https://go.drugbank.com/drugs/DB04690): **Camptothecin** is an alkaloid isolated from the stem wood of the Chinese tree, Camptotheca acuminata. This compound selectively inhibits the nuclear enzyme DNA topoisomerase, type I. Several semisynthetic analogs of camptothecin have demonstrated antitumor activity.(**喜树碱**是从中国树的茎木中分离出的生物碱，喜树。该化合物选择性地抑制核酶DNA拓扑异构酶I型。喜树碱的几种半合成类似物已显示出抗肿瘤活性。)
   
   - Among these compounds, **camptothecin** (CPT) and its analogs showed inhibitory effects on amyloid-β 1-42 (Aβ42) with the IC50 value in the nanomolar range in HEKsw cells and SHSY5Ysw cells. Taken together, our results indicate that CPT and its analogs would be a promising therapeutic candidates for AD. (在这些化合物中，**喜树碱**（CPT）及其类似物在HEKsw细胞和SHSY5Ysw细胞中显示出对淀粉样蛋白-β1-42（Aβ42）的抑制作用，IC50值在纳摩尔范围内。总之，我们的结果表明CPT及其类似物将是AD的有前途的治疗候选药物。)
   
   - Wang J, Shi ZQ, Zhang M, Xin GZ, Pang T, Zhou P, Chen J, Qi LW, Yang H, Xu X, Li P. Camptothecin and its analogs reduce amyloid-β production and amyloid-β42-induced IL-1β production. J Alzheimers Dis. 2015;43(2):465-77. doi: 10.3233/JAD-140078. PMID: 25096614. link: https://pubmed.ncbi.nlm.nih.gov/25096614/ .


- [77] [DB00762](https://go.drugbank.com/drugs/DB00762): Irinotecan is an antineoplastic enzyme inhibitor primarily used in the treatment of colorectal cancer. It is a derivative of camptothecin that inhibits the action of topoisomeras(伊立替康是一种抗肿瘤酶抑制剂，主要用于治疗结直肠癌。它是喜树碱的衍生物，可抑制拓扑异构酶的作用)

   - 并没有研究表明 Irinotecan 能够治疗 AD. 

- [80] [DB15127](https://go.drugbank.com/drugs/DB15127): **Hydrogen** is under investigation in clinical trial NCT02830854 (Molecular Hydrogen for Cognitive Function and Performance in Elderly).(**氢**正在临床试验NCT02830854（用于老年人认知功能和表现的分子氢）中进行研究。)

   - Recent studies in animal models of focal or global cerebral ischemia and cerebral ischemia in humans suggest that **hydrogen has pleiotropic neuroprotective properties**. One potential mechanism explaining some of the general health benefits of using hydrogen is that it may prevent aging-related changes in cellular proteins such as amyloid and tau protein. We also present evidence that, following ischemia, hydrogen improves cognitive and neurological deficits and prevents or delays the onset of neurodegenerative changes in the brain. The available evidence suggests that molecular hydrogen has neuroprotective properties and may be a new therapeutic agent in the treatment of neurodegenerative diseases such as neurodegeneration following cerebral ischemia with progressive dementia.(最近对人类局灶性或全局性脑缺血和脑缺血动物模型的研究表明，氢具有多效性**神经保护特性**。一种解释使用氢对健康有益的潜在机制是，它可以防止淀粉样蛋白和tau蛋白等细胞蛋白的衰老相关变化。我们还提出证据表明，在缺血后，氢可以改善认知和神经功能缺陷，防止或延缓大脑神经退行性改变的发生。现有证据表明，分子氢具有神经保护特性，可能是治疗神经退行性疾病的新的治疗剂，如脑缺血伴进行性痴呆后的神经变性。)
   
   - Pluta R, Januszewski S, Czuczwar SJ. Molecular Hydrogen Neuroprotection in Post-Ischemic Neurodegeneration in the Form of Alzheimer's Disease Proteinopathy: Underlying Mechanisms and Potential for Clinical Implementation-Fantasy or Reality? Int J Mol Sci. 2022 Jun 13;23(12):6591. doi: 10.3390/ijms23126591. PMID: 35743035; PMCID: PMC9224395. link: https://pubmed.ncbi.nlm.nih.gov/35743035/ .

- [83] [DB00806](https://go.drugbank.com/drugs/DB00806): Pentoxifylline is a methylxanthine derivative used to treat intermittent claudication caused by chronic occlusive arterial disease of the limbs. Pentoxifylline (PTX) is a synthetic dimethylxanthine derivative that modulates the rheological properties of blood and also has both anti-oxidant and anti-inflammatory properties(己酮可可碱是一种甲基黄嘌呤衍生物，用于治疗由慢性四肢闭塞性动脉疾病引起的间歇性跛行。己酮可可碱（PTX）是一种合成的二甲基黄嘌呤衍生物，可调节血液的流变特性，还具有抗氧化和抗炎特性)

   - 并没有研究表明 Pentoxifylline 能够治疗 AD.


- [84] [DB01380](https://go.drugbank.com/drugs/DB01380): Cortisone acetate is a steroid hormone used for the relief of the inflammatory and pruritic manifestations of corticosteroid-responsive dermatoses and endocrine disorders associated with inadequate production of steroid hormones.(醋酸可的松是一种类固醇激素，用于缓解皮质类固醇反应性皮肤病的炎症和瘙痒症状，以及与类固醇激素产生不足相关的内分泌紊乱。)

   - 并没有研究表明 Cortisone acetate 能够治疗 AD. 

- [85] [DB01069](https://go.drugbank.com/drugs/DB01069): Promethazine is a first-generation antihistamine used for the treatment of allergic conditions, nausea and vomiting, and motion sickness.(异丙嗪是第一代抗组胺药，用于治疗过敏性疾病、恶心呕吐和运动病。)

  - 并没有研究表明 Promethazine 能够治疗 AD.

- [86] [DB00715](ttps://go.drugbank.com/drugs/DB00715): **Paroxetine** is a selective serotonin reuptake inhibitor used to treat major depressive disorder, panic disorder, OCD, social phobia, generalized anxiety disorder, the vasomotor symptoms of menopause, and premenstrual dysphoric disorder.(**帕罗西汀**是一种选择性5-羟色胺再摄取抑制剂，用于治疗重度抑郁症、惊恐障碍、强迫症、社交恐惧症、广泛性焦虑症、更年期血管运动症状和经前焦虑障碍。)

  - Neuropsychiatric symptoms (NPS) such as depression, anxiety, apathy, and irritability occur in prodromal phases of clinical Alzheimer's disease (AD), which might be an increased risk for later developing AD. Our data indicate that prophylactic administration of **paroxetine** ameliorates the emotional dysfunction and memory deficit in AD mice. These neuroprotective effects are attributable to functional restoration of glutamate receptor (GluN2A) in AD mice. (神经精神症状（NPS），如抑郁、焦虑、冷漠和易怒，发生在临床阿尔茨海默病（AD）的前驱期，这可能会增加后期发展为AD的风险。我们的数据表明，预防性服用**帕罗西汀**可以改善AD小鼠的情绪障碍和记忆缺陷。这些神经保护作用可归因于AD小鼠谷氨酸受体（GluN2A）的功能恢复。)
  
  - Ai PH, Chen S, Liu XD, Zhu XN, Pan YB, Feng DF, Chen S, Xu NJ, Sun S. Paroxetine ameliorates prodromal emotional dysfunction and late-onset memory deficit in Alzheimer's disease mice. Transl Neurodegener. 2020 May 12;9(1):18. doi: 10.1186/s40035-020-00194-2. PMID: 32398165; PMCID: PMC7216685. link: https://pubmed.ncbi.nlm.nih.gov/32398165/ .


- [88] [DB00297](https://go.drugbank.com/drugs/DB00297): Bupivacaine is a widely used local anesthetic agent.(布比卡因是一种广泛使用的局部麻醉剂。)

  - 并没有研究表明 Bupivacaine 能够治疗 AD.

- [89] [DB01181](https://go.drugbank.com/drugs/DB01181): Ifosfamide is an alkylating and immunosuppressive agent used in chemotherapy for the treatment of cancers, including testicular cancer, ovarian cancer, cervical cancer, osteocarcinoma, bladder cancer, small cell lung cancer, and non-Hodgkin's lymphoma.(异环磷酰胺是一种烷化和免疫抑制剂，用于化疗，用于治疗癌症，包括睾丸癌、卵巢癌、宫颈癌、骨癌、膀胱癌、小细胞肺癌和非霍奇金淋巴瘤。)

   - 并没有研究表明 Ifosfamide 能够治疗 AD. 

- [91] [DB00541](https://go.drugbank.com/drugs/DB00541): Vincristine is a vinca alkaloid used to treat acute leukemia, malignant lymphoma, Hodgkin's disease, acute erythraemia, and acute panmyelosis.(长春新碱是一种长春花生物碱，用于治疗急性白血病、恶性淋巴瘤、霍奇金病、急性红斑和急性全骨髓病。)

   - 并没有研究表明 Vincristine 能够治疗 AD.

- [94] [DB00104](https://go.drugbank.com/drugs/DB00104): **Octreotide** is a peptide drug used to treat acromegaly as well as diarrhea associated with metastatic carcinoid tumors and vasoactive intestinal peptide secreting tumors.(**奥曲肽**是一种肽药物，用于治疗肢端肥大症以及与转移性类癌肿瘤和血管活性肠肽分泌肿瘤相关的腹泻。)

   - Both insulin alone and the somatostatin analogue **octreotide** alone facilitate memory in patients with Alzheimer's disease (AD). Since octreotide inhibits endogenous insulin secretion, the cognitive effects of insulin and octreotide may not be independent.(单独使用胰岛素和单独使用生长抑素类似物**奥曲肽**均可促进阿尔茨海默病（AD）患者的记忆。由于奥曲肽抑制内源性胰岛素分泌，胰岛素和奥曲肽的认知作用可能不是独立的。)
  
   - Watson GS, Baker LD, Cholerton BA, Rhoads KW, Merriam GR, Schellenberg GD, Asthana S, Cherrier M, Craft S. Effects of insulin and octreotide on memory and growth hormone in Alzheimer's disease. J Alzheimers Dis. 2009;18(3):595-602. doi: 10.3233/JAD-2009-1165. PMID: 19625744; PMCID: PMC2842464. link: https://pubmed.ncbi.nlm.nih.gov/19625744/ .

- [95] [DB00451](https://go.drugbank.com/drugs/DB00451): **Levothyroxine** is a synthetic T4 hormone used to treat hypothyroidism that can be used along with surgery and radioiodine therapy to manage thyrotropin-dependent well-differentiated thyroid cancer.(**左旋甲状腺素**是一种合成的 T4 激素，用于治疗甲状腺功能减退症，可与手术和放射性碘治疗一起用于治疗促甲状腺激素依赖性高分化甲状腺癌。)

   - In this study, the effect of **levothyroxine** (L-T4) on tracheal responsiveness, lung inflammation, oxidative stress and pathological features in a rat model of Alzheimer's disease (AD), was evaluated.Alzheimer's disease may cause lung inflammation and treatment with low dose of T4 improved MDA level and lung inflammation.(在这项研究中，评估了左旋甲状腺素（L-T4）对阿尔茨海默病（AD）大鼠模型中气管反应性，肺部炎症，氧化应激和病理特征的影响。阿尔茨海默病可能导致肺部炎症，**低剂量T4治疗可改善MDA水平和肺部炎症。**)

   - Bavarsad K, Saadat S, Mohammadian Roshan N, Hadjzadeh MA, Boskabady MH. Effects of levothyroxine on lung inflammation, oxidative stress and pathology in a rat model of Alzheimer's disease. Respir Physiol Neurobiol. 2020 Jun;277:103437. doi: 10.1016/j.resp.2020.103437. Epub 2020 Apr5.PMID:32259689. link: https://pubmed.ncbi.nlm.nih.gov/32259689/ .

- [96] [DB00747](https://go.drugbank.com/drugs/DB00747): Scopolamine is a belladonna alkaloid with anticholinergic effects indicated for the treatment of nausea and vomiting associated with motion sickness and postoperative nausea and vomiting (PONV).(东莨菪碱是一种颠茄生物碱，具有抗胆碱能作用，用于治疗与晕动病和术后恶心呕吐相关的恶心和呕吐 （PONV）.)

   - 并没有研究表明 Scopolamine 能够治疗 AD.


- [97] [DB00813](https://go.drugbank.com/drugs/DB00813): Fentanyl is an opioid analgesic used in anesthesia, for breakthrough cancer pain, or round the clock pain management.(芬太尼是一种阿片类镇痛药，用于麻醉、突破性癌症疼痛或全天候疼痛管理。)

   - 并没有研究表明 Fentanyl 能够治疗 AD.


- [100] [DB12290](https://go.drugbank.com/drugs/DB12290): **Puerarin** has been investigated for the treatment of Alcohol Abuse.(**葛根素**已被研究用于治疗酒精滥用。)

   - It has been widely used in the treatment of cardiovascular and cerebrovascular diseases, diabetes and diabetic complications, osteonecrosis, Parkinson's disease, **Alzheimer's disease**, endometriosis, and cancer.(已广泛应用于心脑血管疾病、糖尿病及糖尿病并发症、骨坏死、帕金森病、**阿尔茨海默病**、子宫内膜异位症、癌症等的治疗。)

   - Zhou YX, Zhang H, Peng C. **Puerarin**: a review of pharmacological effects. Phytother Res. 2014 Jul;28(7):961-75. doi: 10.1002/ptr.5083. Epub 2013 Dec 13. PMID: 24339367. link: https://pubmed.ncbi.nlm.nih.gov/24339367/ .

