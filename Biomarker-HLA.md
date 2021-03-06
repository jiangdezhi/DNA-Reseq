# HLA对肿瘤免疫治疗影响 2018.11.19
## 1.HLA体细胞突变
  - 1.1 实验目的
    - 分析TCGA中10种肿瘤类型共9176个肿瘤患者的体细胞突变与HLA的关系
  - 1.2 实验设计
    - 创建一个新的参数：PHBR(patient harmonic best rank)，体细胞突变产生的长度为8-11突变肽段与3种（至多共6个HLA-A/B/C)HLA-I型等位基因的多个亲和力之和
    - PHBR含义：表示患者HLA对该突变的整体抗原呈递水平。PHBR越高，HLA对该突变抗原呈递能力越差。注:**PHBR是根据HLA与突变肽段的亲和力从高到底进行排列，故Rank越大，亲和力越低。**
  - 1.3 HLA体细胞突变与免疫逃逸的关系
    - TCGA肿瘤患者中的群体突变频率越高（可认为是肿瘤高频突变基因），则该突变所产生的突变肽段被HLA抗原呈递能力越弱
    - 携带HLA体细胞突变患者相比于HLA野生型患者有着显著高的TMB(HLA呈递新生抗原的能力越弱，说明其介导的免疫监视功能也在削弱，使得携带突变的肿瘤克隆易于免疫逃逸）
  - 1.4 HLA体细胞突变如何影响免疫反应
    - 突变正好出现在HLA与抗原识别并结合的位点，导致不能结合或结合力变弱？
    - 突变正好出现在HLA与抗原识别并结合位点的附近，影响了肽段的空间结构，导致结合力偏弱？
  - 1.5 方法
    - HLA亲和性检测软件：NetMHCPan 3.0 - artificial neural networks
    - IC50
  

## 2.HLA拷贝数杂合缺失

## 3.遗传性HLA等位基因
