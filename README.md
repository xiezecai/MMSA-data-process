
---
原始 MMSA 论文( [MMSA Google Drive](https://drive.google.com/drive/folders/1A2S4pqCHryGmiqnNSPLv7rEg63WvjCSk)。)：
```bibtex
@inproceedings{liu2022mmsa,
  title={MMSA: Multi-Modal Sentiment Analysis with Multi-View Learning},
  author={Liu, Y. and others},
  booktitle={Proceedings of the 30th ACM International Conference on Multimedia},
  year={2022}
}
```
本数据集是 **MMSA (Multi-Modal Sentiment Analysis)** 的衍生版本，原始数据来自 [MMSA Google Drive](https://drive.google.com/drive/folders/1A2S4pqCHryGmiqnNSPLv7rEg63WvjCSk)。\
我使用 **Qwen** 模型对文本进行了重编码，并整理了三个标准子数据集（MOSI、MOSEI、SIMS）的未对齐特征，方便直接用于多模态情感分析任务。\
***直接查看以下链接即可***：\
[(MMSA)用Qwen3_VL_Embedding_2B_model重提取文本特征](https://www.modelscope.cn/datasets/zen00003/MMSA_data_qwen)
## 下载方法

### 方法一：使用 ModelScope SDK

```python
from modelscope.msdatasets import MsDataset

ds = MsDataset.load(
    'zen00003/MMSA_data_qwen',   # 请替换为您的命名空间/数据集名称
    subset_name='default',
    split='train'
)
```

### 方法二：使用 Git LFS

```bash
git clone https://www.modelscope.cn/datasets/zen00003/MMSA_data_qwen.git
cd MMSA_data_qwen
# 确保已安装 git-lfs
git lfs pull
```

---