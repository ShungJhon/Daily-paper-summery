# 🤖 Hugging Face AI 论文每日速递 (2026-03-18)

> **今日趋势概览**：视频理解与3D生成模型持续升温，工业场景代码模型崛起，边缘端轻量级推理成为新焦点。

### 📂 核心论文纵览（按upvotes排序）

| 论文标题 | 核心领域 | 核心问题 | TL;DR (核心突破) | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [InCoder-32B: Code Foundation Model for Industrial Scenarios](https://huggingface.co/papers/2603.16790) | LLM / Code | 工业场景代码推理能力不足 | 首个32B工业代码基础模型，统一芯片设计、GPU内核优化、嵌入式系统等5大领域，通过128K上下文扩展和执行验证，在工业任务上建立最强开源基线 | 140 |
| [Kinema4D: Kinematic 4D World Modeling for Spatiotemporal Embodied Simulation](https://huggingface.co/papers/2603.16669) | CV / Embodied AI | 机器人-环境交互模拟 | 4D生成式机器人模拟器，将机器人运动学控制与环境反应生成分离，支持物理合理、几何一致的跨实体交互，首次展示零样本迁移能力 | 64 |
| [Demystifing Video Reasoning](https://huggingface.co/papers/2603.16870) | CV / Video | 视频模型推理机制不透明 | 发现视频推理主要沿扩散去噪步骤而非帧序列展开，提出Chain-of-Steps机制，识别出工作记忆、自我修正、感知先于行动等 emergent behaviors | 56 |
| [WorldCam: Interactive Autoregressive 3D Gaming Worlds](https://huggingface.co/papers/2603.16871) | CV / Generative AI | 动作控制精度与长程3D一致性 | 将相机姿态作为统一几何表示，通过物理连续动作空间和Lie代数实现精确6-DoF控制，长程导航时利用全局姿态索引检索历史观测保证3D一致性 | 48 |
| [TRUST-SQL: Tool-Integrated Multi-Turn RL for Text-to-SQL](https://huggingface.co/papers/2603.16448) | NLP / RL | 未知Schema下的Text-to-SQL | 将任务建模为POMDP，采用四阶段协议和Dual-Track GRPO策略，通过token级masked advantages解决信用分配问题，在无预加载元数据下超越基线30.6% | 43 |
| [Online Experiential Learning for Language Models](https://huggingface.co/papers/2603.16856) | LLM / RL | 部署经验未被利用 | 提出在线体验学习框架，从交互轨迹中提取可迁移知识，通过策略内上下文蒸馏整合到模型参数，形成迭代在线学习循环，提升任务准确率和token效率 | 36 |
| [Unified Spatio-Temporal Token Scoring for Efficient Video VLMs](https://huggingface.co/papers/2603.18004) | VLM / Efficient | 视频VLM计算效率 | STTS模块在ViT和LLM全程剪枝50%视觉token，训练推理效率提升62%，性能仅下降0.7%，平衡SOTA效率-精度 tradeoff | 0 |
| [Efficient Reasoning on the Edge](https://huggingface.co/papers/2603.16867) | LLM / Edge | 边缘设备部署LLM推理 | 结合LoRA适配器、监督微调和RL预算强制，轻量级方法在小模型中启用推理能力，通过并行测试时扩展和动态适配器切换实现移动端可行推理 | 13 |

### 💡 深度洞察 (编者观察)

* **关联分析**：视频理解领域出现两条主线——一是通过Token Pruning（STTS）提升效率，二是深入理解推理机制（Demystifying Video Reasoning、Kinema4D）。两者共同指向视频VLM的可解释性和效率优化。代码模型方面，InCoder-32B专注工业场景的垂直领域优化，而TRUST-SQL则展示RL在结构化任务（SQL）上的突破。

* **行业影响**：WorldCam和Kinema4D将生成式AI引入游戏和机器人模拟，意味着内容创作与物理仿真边界进一步模糊。InCoder-32B有望在芯片设计、编译器优化等硬核工业场景落地。边缘推理突破（Efficient Reasoning on the Edge）将使LLM推理走向手机、车载等终端设备。

* **安全伦理**：Demystifying Video Reasoning揭示Diffusion Transformer内部的功能专业化（早期层编码感知结构、中间层执行推理），这一发现可能被用于更高效地检测AI生成视频_content。但本次论文中未涉及明确的AI安全风险评估。

* **重点关注**：视频推理机制的新发现（Chain-of-Steps vs Chain-of-Frames）对你当前的工作具有直接参考价值——理解推理在去噪步骤中涌现意味着视频生成模型可作为新型智能 substrate。STTS的Token剪枝方法也值得借鉴，用于优化多模态模型的推理效率。

---

> 📌 **保存建议**：将本文保存为 `daily-brief-2026-03-18.md`