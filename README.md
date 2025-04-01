<!--
 * @Author: PengJie pengjieb@mail.ustc.edu.cn
 * @Date: 2025-04-01 17:00:26
 * @LastEditors: PengJie pengjieb@mail.ustc.edu.cn
 * @LastEditTime: 2025-04-01 18:04:46
 * @FilePath: /amc_rebuttal/README.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->

<img src="img/more_token_fusion-modality_gradient_conflict.png" alt="My Image" width="1000">

Figure 1. The gradient conflict between different modalities in the MIMIC-IV dataset. The `AMC w/ MoE` is the proposed AMC method, and `AMC w/o MoE` replaces the MoE to its dense counterpart. 


<img src="img/more_token_fusion-modality_quality.png" alt="My Image" width="1000">

Figure 2. The case study about the modality data quality identified by our proposed modality importance. The image in the left side obtain the lowest modality importance, and the right side image obtain the highest modality importance.


| **MIMIC-IV** | Code | Note | Lab || **ADNI** | Genomic | Image | Biospecimen | Clinical |
|---|:---:|:---:|:---:|-|---|:---:|:---:|:---:|:---:|
| Acc | **67.95** | 67.58 | 64.77 |-| Acc | 52.94 | 53.21 | 50.4 | **53.50** |
| Precision | 55.44 | 55.82 | **59.18** |-| Precision | 53.23 | **55.91** | 49.1 | 53.30 |
| Recall | 55.88 | 56.51 | **62.50** |-| Recall | 53.55 | **54.7**0 | 32.6 | 52.43 |
| F1 | 55.60 | 56.02 | **58.67** |-| F1 | 52.30 | **54.12** | 39.1 | 47.32 |

Table 1. The single modality performance with the same backbone in MIMIC-IV and ADNI datasets. Here we use the F1 score to indicate the modality importance (Higher is better).