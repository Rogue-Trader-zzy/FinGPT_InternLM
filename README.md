# FinGPT_InternLM
# 智能金融客服（使用大模型构建金融专业助手）

## 它能做什么？

### 金融咨询
● 该模组可以在中国金融语境下，与用户展开关于金融话题的多轮对话，或是为用户解释金融专业的相关知识。如智能金融技术知识回答，情感分析，命名实体识别和关系抽取
● 用到的技术：RAG, 微调
● 用到的数据：网上公开中文数据集和hugging face英文数据集翻译成中文

### 金融知识检索问答
● 该模组可以基于金融领域知识回答专业问题。
● 用到的技术：RAG
● 用到的数据：网上金融技术文档，课程PPT和手动整理的爬虫和可视化技术文档

## 用到的技术（InternLM训练营有教程）
### RAG（Retrieval Augmented Generation，增强检索生成）
先将金融知识等材料文本向量化处理存储至本地作为数据库，用户进行提问时，将问题向量化，然后算相似度找到最接近的文本材料作为Prompt（提示）来让基础大模型对问题和材料做一个总结性的回答。
● 优点：回答效果较好，准确。
● 缺点：每篇材料不能过长，与基础模型的输入最大token限制有关，可以将材料按内容分块存储。
### Lora微调
LORA是一种低资源微调大模型方法，使用LORA，训练参数仅为整体参数的万分之一、GPU显存使用量减少2/3且不会引入额外的推理耗时。基础模型参数锁住不变，增加新参数，使用数据进行微调。

![image](https://github.com/Rogue-Trader-zzy/FinGPT_InternLM/assets/64819379/a670e074-8682-499c-b612-378562307afb)

## 整体过程
### 微调
具体参考文件夹下的步骤
### RAG
具体参考文件夹下的步骤
### 部署
具体参考文件夹下的步骤
### Agent调用
具体参考文件夹下的步骤
