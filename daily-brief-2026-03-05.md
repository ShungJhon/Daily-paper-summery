# 🤖 Hugging Face AI 论文每日速递 (2026-03-05)

> **今日趋势概览**：视频生成与多模态理解成为今日焦点，ByteDance 和 Microsoft 分别带来了突破性的实时视频生成和推理模型。

### 📂 核心论文纵览

| 论文标题 | 核心领域 | TL;DR (一句话核心突破) | Upvotes |
| :--- | :--- | :--- | :---: |
| [Helios: Real Real-Time Long Video Generation Model](https://huggingface.co/papers/2603.04379) | Generative AI / Video | 首个14B参数视频生成模型，在单张H100 GPU上达到19.5 FPS，支持分钟级长视频生成，无需传统加速技术。 | 105 |
| [T2S-Bench & Structure-of-Thought](https://huggingface.co/papers/2603.03790) | NLP / LLM | 提出Structure of Thought提示技术，引导模型构建中间文本结构，在8个任务上平均提升5.7%。 | 92 |
| [Heterogeneous Agent Collaborative RL (HACRL)](https://huggingface.co/papers/2603.02604) | RL | 异构智能体在训练时共享验证过的rollout进行协作优化，推理时独立运行，GSPO平均提升3.3%。 | 92 |
| [Proact-VL](https://huggingface.co/papers/2603.03447) | CV / Multimodal | 微软发布实时交互式AI伴侣框架，针对游戏场景实现低延迟响应和强视频理解能力。 | 22 |
| [Phi-4-reasoning-vision-15B Technical Report](https://huggingface.co/papers/2603.03975) | Multimodal LLM | 微软发布紧凑开源多模态推理模型，通过直接回答与Chain-of-Thought混合方法达到竞争性能。 | 11 |
| [ArtHOI](https://huggingface.co/papers/2603.04338) | CV / 4D | 通过单目视频先验进行4D重建，使用光流进行部件分割，实现物理可信的几何一致交互。 | 19 |
| [CubeComposer](https://huggingface.co/papers/2603.04291) | Generative AI / Video | 腾讯提出时空自回归扩散模型，通过立方图表示生成高分辨率360°全景视频。 | 9 |
| [Memex](https://huggingface.co/papers/2603.04257) | LLM / Agent | 大语言模型智能体的记忆机制，通过结构化摘要维护紧凑上下文，全交互细节存储于外部数据库。 | 8 |
| [RIVER Bench](https://huggingface.co/papers/2603.03985) | CV / Video | 实时视频交互基准，评估MLLM的回顾性记忆、实时感知和主动预测能力。 | 4 |
| [V1 Verification](https://huggingface.co/papers/2603.04304) | LLM / Reasoning | 测试时扩展方法，通过成对自验证框架提升代码生成和数学推理基准的性能。 | 5 |
| [MIBURI](https://huggingface.co/papers/2603.03282) | CV / Animation | 在线因果框架生成与实时对话同步的全身手势和面部表情。 | 1 |
| [AgilePruner](https://huggingface.co/papers/2603.01236) | CV / VLM | 视觉token剪枝方法研究，注意力和多样性方法各有适用场景。 | 6 |
| [MUSE](https://huggingface.co/papers/2603.02482) | Safety / Multimodal | 多模态安全评估开源平台，评估跨模态攻击和LLM判断。 | 2 |
| [SpeciaRL](https://huggingface.co/papers/2603.03197) | RL / VLM | 通过强化学习提升大规模多模态模型在细粒度图像分类中的特异性。 | 1 |
| [GroupEnsemble](https://huggingface.co/papers/2603.01847) | CV / Detection | 单次前向传播实现DETR模型的不确定性估计。 | 1 |
| [Video Storytelling](https://huggingface.co/papers/2603.03646) | Generative AI / Video | 长视频故事合成框架，保证背景一致性和多主体转换。 | 4 |
| [SWE-CI](https://huggingface.co/papers/2603.03823) | Software Engineering | 代码生成智能体的仓库级基准，评估长期软件演化。 | 3 |
| [EmbodiedSplat](https://huggingface.co/papers/2603.04254) | CV / 3D | 结合在线3D Gaussian Splatting与CLIP实现实时3D场景理解。 | 1 |
| [BeamPERL](https://huggingface.co/papers/2603.04124) | RL / Physics | 紧凑语言模型的物理推理奖励强化学习。 | 1 |
| [HDINO](https://huggingface.co/papers/2603.02924) | CV / Detection | 高效开放词汇目标检测器。 | 0 |

### 💡 深度洞察 (编者观察)

* **关联分析**：今日论文呈现两大技术主线：
  1. **视频生成领域** - 从 Helios 的实时长视频到 CubeComposer 的 360° 视频，再到 Video Storytelling，都在聚焦突破生成时长和质量瓶颈
  2. **多模态推理** - 从 Phi-4-reasoning 到 RIVER Bench，探索 LLM 在实时场景下的理解与推理能力
  
  Microsoft 同时发布了 Proact-VL 和 Phi-4-reasoning-vision-15B，体现了其在多模态领域的全面布局。ByteDance (Helios) 和 Tencent (CubeComposer) 在视频生成领域展开竞争。

* **行业影响**：
  - Helios 的出现标志着视频生成从"能生成"向"实时生成"的质变
  - HACRL 和 Memex 为 AI Agent 的长期任务执行提供了新范式
  - MIBURI 和 ArtHOI 推动虚拟数字人技术进步

* **安全伦理**：
  - MUSE 平台关注多模态模型安全评估
  - 视频生成技术快速进步带来深度伪造风险
  - AI Agent 记忆机制（Memex）带来隐私保护新挑战

---
*📌 提示：可将本文保存为 `daily-brief-2026-03-05.md`*