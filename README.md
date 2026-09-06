# Halloween


目前主要学习和实践NLP方面，现在主要研究大模型和预训练模型在教育打分方面的研究AES、SAS

我比较感兴趣的方向是：

> **自然语言处理 × 大语言模型 × 教育人工智能**

希望未来能够继续深入学习人工智能相关知识，并将所学技术应用到实际问题中。

---

## 👨‍💻 关于我

* 🎓 专业方向：人工智能
* 🧠 主要研究兴趣：NLP、深度学习、agent
* 🔬 感兴趣的应用：智能教育、自动评分、文本理解、文本生成

# 🚀 个人项目与实践经历

## 1. CAFE:Leveraging Large Language Model-Generated Comments for Fine-grained
Interpretable Essay Scoring

我对**自动作文评分（Automated Essay Scoring，AES）**进行了实践和研究。
该项目关注如何利用**大语言模型（LLM）与预训练语言模型（PLM）相结合**，对学生作文进行自动评分，同时提升评分模型的**准确性、可解释性和稳定性**。
传统的 BERT 等编码器模型能够高效地学习作文文本表示，但通常主要依赖最终分数进行监督，缺少对“**为什么这个作文得到这个分数**”的显式建模。另一方面，直接使用 LLM 进行评分虽然能够提供丰富的评价知识，但容易受到提示词、作文长度和位置等因素影响，并且计算成本较高。
因此，该项目提出 **CAFE（Comment-Augmented Fine-grained Explainable Essay Scoring）**，利用 LLM 生成的**细粒度诊断性评价评论（Diagnostic Comments）**作为中间评分知识，并将这些评价信息与作文文本表示进行融合，从而实现更加准确且具有可解释性的自动作文评分。

### 主要技术

* BERT / Pre-trained Language Models
* Large Language Models（LLM）
* LLM-generated Comments
* Dual-channel Representation
* Silhouette Score
* t-SNE

论文实验发现，适当增加评价维度能够进一步提升模型性能，其中 **CAFE-6D** 在性能与可解释性之间取得了较好的平衡；相比不使用评论信息的 CAFE-0D，其平均 QWK 从 **0.712 提升至 0.815**。
此外，项目还通过 t-SNE 对模型学习到的作文表示进行可视化分析。实验表明，引入 LLM 生成的评价评论后，不同质量等级的作文在表示空间中能够形成更加清晰的分布，Silhouette Score 从 **0.0965 提升至 0.2174**。
在 ASAP-AES 和 PERSUADE 2.0 数据集上的实验表明，CAFE 能够持续超过具有代表性的 PLM 和 LLM 基线模型，在获得更高评分性能的同时，还能够提供**细粒度的评价信息和可解释信号**。
这个项目让我进一步认识到，**LLM 不一定需要直接作为最终评分器，也可以作为“评分知识提供者”**，将其丰富的评价能力转化为结构化的中间知识，再与传统的预训练语言模型结合，从而在**准确性、效率和可解释性**之间取得更好的平衡。

详细的内容请联系我

## 2. Rubric-Guided Fine-grained Interpretable Short Answer Scoring with LLM and BERT

我对**短答案自动评分（Short Answer Scoring，SAS）**进行了研究与实践。传统 SAS 方法通常可以抽象为：

```text
(Question, Reference Answer, Student Answer) → Encoder → Holistic Score
```

这类方法虽然能够直接学习“完整答案到总分”的映射，但本质上更接近**黑盒整体评分**。模型只能输出一个最终分数，却无法解释为什么是这个分数：学生答案中哪一步正确、哪一步错误、每一步被扣了多少分、错误属于概念错误还是计算错误。这种缺乏细粒度评分和可解释性的问题，是传统 BERT 类 SAS 方法的核心痛点。
因此，本项目提出一种**基于评分量规（Rubric）引导的细粒度可解释短答案自动评分方法**。该方法采用“双模型”策略
## 主要技术

- BERT / Pre-trained Language Models
- Large Language Models（LLM）
- Reference Rubric Construction
- Student Step Decomposition and Alignment
- Step-wise Explainable Evaluation
- Cross Attention-based Representation Fusion


整体流程严格遵循 **Rubric First, Student Answer Second** 的原则，即评分标准首先根据题目和参考答案建立，并且对于同一道题的所有学生答案保持一致。项目在 **ADS、ASAG、LE** 等多个短答案评分数据集上进行了处理与验证。






# 📚 专业知识与能力自我评估

## ✅ 已经掌握的知识

*RL、

---

# 🔍 自我评价

虽然目前已经掌握了一些人工智能和 NLP 方面的基础知识，但我认为自己的专业能力仍然存在很多不足。

例如：

* 科研论文阅读能力需要继续提高
* 实验设计和科研创新能力需要加强
* 对模型底层实现和高效训练技术了解还不够深入

因此，我目前更希望从“会使用模型”逐渐提升到：

> **理解模型 → 修改模型 → 设计模型 → 独立开展研究**

---

# 🎯 我感兴趣的技术方向

目前我最感兴趣的方向主要包括：

### 1. 自然语言处理

希望进一步学习文本理解、文本生成、语义表示等 NLP 技术。

### 2. 大语言模型

希望深入了解 LLM 的：

* 预训练
* 指令微调
* 参数高效微调
* 推理
* 对齐
* 评价

### 3. 可解释人工智能

希望研究模型为什么做出某个预测，以及如何让 AI 的结果更加透明、可靠。

---

# 📖 最希望学习的知识

接下来，我最希望进一步学习以下内容：


* RAG
* Agent
* GRPO
* Reward Model
* LLM Evaluation
* 高效 LLM 推理
* 可解释人工智能

同时，我也希望加强数学基础，包括：

* 概率论
* 线性代数
* 微积分
* 优化理论

为以后深入研究人工智能算法打下更扎实的基础。

---

# 🗺️ 未来一年发展规划

## 📌 第一阶段：夯实基础

第一年，我计划进一步完善自己的人工智能基础知识。

继续学习人工智能领域的相关知识，多看看paper，提示代码能力

---

## 📌 第二阶段：深入研究

第二年，我希望将学习重点逐渐转向**自然语言处理和大语言模型研究**。

继续产出一些科研结果

希望在这个阶段逐渐找到一个自己真正感兴趣的研究方向。

---

## 📌 第三阶段：明确发展方向

考研?考公?
目前可能选择继续深造读研究生吧

---



# 📫 联系我

如果你也对以下方向感兴趣，欢迎交流：

* 🤖 人工智能
* 🧠 自然语言处理
* 💬 大语言模型
* 🎓 教育人工智能
* 🔬 深度学习

欢迎访问我的 GitHub，一起学习和交流！

---

⭐ **感谢你访问我的 GitHub 个人主页！**

> Keep Learning · Keep Building · Keep Exploring
