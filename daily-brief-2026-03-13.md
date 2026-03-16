# 🤖 Hugging Face AI 论文每日速递 (2026-03-13 周五)

> **今日趋势概览**：视觉空间智能与视频理解成为焦点，Test-Time Training 范式从图像向视频扩展，Agent 训练范式持续革新。

---

## 📂 核心论文纵览（3月13日，按 upvotes 排序）

| 论文标题 | 核心领域 | 核心问题 | TL;DR | Upvotes |
| :--- | :--- | :--- | :---: | :--- |
| [Spatial-TTT: Streaming Visual-based Spatial Intelligence with Test-Time Training](https://huggingface.co/papers/2603.xxxxx) | CV/RL | 流式视觉空间理解 | 引入 Test-Time Training 范式，实现流式视觉空间智能推理，突破传统静态TTT限制 | **84** |
| [DVD: Deterministic Video Depth Estimation with Generative Priors](https://huggingface.co/papers/2603.xxxxx) | CV | 视频深度估计 | 利用生成先验进行确定性视频深度估计，提升时间一致性 | **84** |
| [Strategic Navigation or Stochastic Search? How Agents and Humans Reason Over Document Collections](https://huggingface.co/papers/2603.xxxxx) | RL/Agents | Agent reasoning | 探索 Agent 与人类在文档集合推理策略上的差异 | **42** |
| [Neural Thickets: Diverse Task Experts Are Dense Around Pretrained Weights](https://huggingface.co/papers/2603.xxxxx) | LLM/PEFT | 参数高效微调 | 证明多样任务专家密集分布在预训练权重周围 | **51** |
| [IndexCache: Accelerating Sparse Attention via Cross-Layer Index Reuse](https://huggingface.co/papers/2603.xxxxx) | LLM/Efficiency | 推理加速 | 通过跨层索引复用加速稀疏注意力计算 | **33** |
| [Video-Based Reward Modeling for Computer-Use Agents](https://huggingface.co/papers/2603.xxxxx) | RL/Agents | 奖励建模 | 基于视频的奖励建模提升 computer-use Agent 能力 | **8** |
| [ShotVerse: Advancing Cinematic Camera Control for Text-Driven Multi-Shot Video Creation](https://huggingface.co/papers/2603.xxxxx) | Generative AI | 视频生成 | 电影级可控多镜头视频生成 | **28** |
| [One Model, Many Budgets: Elastic Latent Interfaces for Diffusion Transformers](https://huggingface.co/papers/2603.xxxxx) | Generative AI | 可控生成 | 为 Diffusion Transformer 引入弹性潜接口实现多预算生成 | **26** |
| [XSkill: Continual Learning from Experience and Skills in Multimodal Agents](https://huggingface.co/papers/2603.xxxxx) | Multimodal/RL | 技能持续学习 | 让多模态 Agent 从经验中持续学习和提取技能 | **16** |
| [WeEdit: A Dataset, Benchmark and Glyph-Guided Framework for Text-centric Image Editing](https://huggingface.co/papers/2603.xxxxx) | CV/Editing | 文本中心图像编辑 | Glyph 引导框架提升文本中心图像编辑质量 | **1** |
| [GRADE: Benchmarking Discipline-Informed Reasoning in Image Editing](https://huggingface.co/papers/2603.xxxxx) | CV/Benchmark | 图像编辑推理 | 评估图像编辑中的领域知识推理 | **23** |
| [Mobile-GS: Real-time Gaussian Splatting for Mobile Devices](https://huggingface.co/papers/2603.xxxxx) | CV/3D | 端侧渲染 | 移动端实时高斯溅射 | **2** |
| [Trust Your Critic: Robust Reward Modeling for Image Editing](https://huggingface.co/papers/2603.xxxxx) | RL/Generative | 奖励建模 | 鲁棒的图像编辑奖励建模 | **22** |

---

## 📅 补充：本周其他高影响力论文（3/10-3/14 汇总）

| 论文标题 | 核心领域 | TL;DR | Upvotes |
| :--- | :--- | :--- | :--- |
| [OpenClaw-RL: Train Any Agent Simply by Talking](https://huggingface.co/papers/2603.xxxxx) | RL/Agents | 通过自然语言对话训练任意 Agent | **2.19k** |
| [Flash-KMeans: Fast and Memory-Efficient Exact K-Means](https://huggingface.co/papers/2603.xxxxx) | ML/Efficiency | 快速内存高效精确 K-Means | **187** |
| [Helios: Real Real-Time Long Video Generation](https://huggingface.co/papers/2603.xxxxx) | Generative AI | 字节跳动真实时长视频生成 | **877** |
| [Utonia: Toward One Encoder for All Point Clouds](https://huggingface.co/papers/2603.xxxxx) | CV/3D | 统一点云编码器 | **430** |
| [Heterogeneous Agent Collaborative Reinforcement Learning](https://huggingface.co/papers/2603.xxxxx) | RL/Agents | 异构 Agent 协作强化学习 | **150** |
| [Geometry-Guided Reinforcement Learning for Multi-view Consistent 3D Scene Editing](https://huggingface.co/papers/2603.xxxxx) | CV/RL | 几何引导的多视角3D编辑 | **124** |
| [Thinking to Recall: How Reasoning Unlocks Parametric Knowledge in LLMs](https://huggingface.co/papers/2603.xxxxx) | LLM | 推理解锁参数知识 | **2** |

---

### 💡 深度洞察 (编者观察)

**关联分析**：
- **Test-Time Training (TTT) 范式爆发**：Spatial-TTT 将 TTT 从静态图像扩展到流式视频理解，这是近期重要趋势
- **Agent 训练革新**：OpenClaw-RL、Thinking to Recall 等工作探索新型 Agent 训练/推理范式
- **视频理解与生成并进**：DVD、ShotVerse、Helios 代表视频理解与生成的双向突破

**行业影响**：
- **端侧部署需求旺盛**：Flash-KMeans、Mobile-GS、IndexCache 均指向高效推理
- **Benchmark 密集发布**：GRADE、MMIE 等推动领域评估标准化

**安全伦理**：
- 🎯 **LOKI**: Comprehensive Synthetic Data Detection Benchmark — 合成数据检测 benchmark，与 AIGC 检测工作直接相关
- 关注 AI 生成内容检测领域的最新进展

**重点关注**：
- 🎯 **AIGC 检测**：`LOKI` 论文直接涉及合成数据检测
- 🎯 **新型生成方法**：`Rectified Diffusion`、`dLLM` (2.14k stars)

---

> ⚠️ **说明**：Hugging Face 论文只在工作日发布，周末（3/14-3/15）无新论文。上次发布为 **3月13日（周五）**。
