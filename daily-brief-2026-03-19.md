# 🤖 Hugging Face AI 论文每日速递 (2026-03-19)

> **今日趋势概览**：Agent持续学习成为焦点，社会交互能力测评升温，视觉-动作解耦推进机器人策略学习。

### 📂 核心论文纵览（按upvotes排序）

| 论文标题 | 核心领域 | 核心问题 | TL;DR (核心突破) | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [InCoder-32B: Code Foundation Model for Industrial Scenarios](https://huggingface.co/papers/2603.16790) | LLM / Code | 工业场景代码推理能力不足 | 首个32B工业代码基础模型，涵盖芯片设计、GPU内核优化等5大领域，128K上下文扩展，在工业任务建立最强开源基线 | 284 |
| [Demystifing Video Reasoning](https://huggingface.co/papers/2603.16870) | CV / Video | 视频模型推理机制不透明 | 发现推理沿扩散去噪步骤涌现（Chain-of-Steps），识别工作记忆、自我修正等 emergent behaviors | 153 |
| [SocialOmni: Benchmarking Audio-Visual Social Interactivity in Omni Models](https://huggingface.co/papers/2603.16859) | VLM / Benchmark | Omni模型社交交互能力评估空白 | 提出社交互动三维评估框架（说话者分离、打断时机、生成自然打断），揭示感知准确率与交互能力的显著脱钩 | 101 |
| [MetaClaw: Just Talk -- An Agent That Meta-Learns and Evolves in the Wild](https://huggingface.co/papers/2603.17187) | LLM / Agent | 部署Agent无法持续适应用户需求 | 持续元学习框架，联合演化基础策略与可复用技能库，技能驱动快速适配相对提升32%，Kimi-K2.5从21.4%升至40.6% | 90 |
| [MosaicMem: Hybrid Spatial Memory for Controllable Video World Models](https://huggingface.co/papers/2603.17117) | CV / Generative | 视频世界模型可控性不足 | 混合空间记忆模块，实现精确的空间可控视频生成，支持细粒度控制 | 69 |
| [WorldCam: Interactive Autoregressive 3D Gaming Worlds](https://huggingface.co/papers/2603.16871) | CV / Generative | 动作控制精度与长程3D一致性 | 相机姿态作为统一几何表示，Lie代数实现精确6-DoF控制，长程导航保持3D一致性 | 52 |
| [Online Experiential Learning for Language Models](https://huggingface.co/papers/2603.16856) | LLM / RL | 部署经验未被利用 | 在线体验学习框架，从交互轨迹提取知识，通过策略内蒸馏整合，形成迭代学习循环 | 45 |
| [Alignment Makes Language Models Normative, Not Descriptive](https://huggingface.co/papers/2603.17218) | LLM / Alignment | 对齐优化与行为预测的权衡 | 对120个Base-Aligned模型对比，Base模型在复杂策略游戏预测人类行为优10:1，Aligned模型在规则场景优，揭示规范性偏差 | 34 |
| [Complementary Reinforcement Learning](https://huggingface.co/papers/2603.17621) | RL | 强化学习样本效率 | 提出互补强化学习方法，提升样本效率与收敛速度 | 28 |
| [GigaWorld-Policy: An Efficient Action-Centered World--Action Model](https://huggingface.co/papers/2603.17240) | Robotics / RL | 世界-动作模型推理开销大 | 动作中心WAM解耦视觉与运动表示，推理速度比Motus快9倍，任务成功率提升7%，比pi-0.5提升95% | 18 |

### 💡 深度洞察 (编者观察)

* **关联分析**：MetaClaw与Online Experiential Learning都关注LLM Agent的持续适应能力，只是路径不同——前者通过技能库+元学习，后者通过部署经验提取。GigaWorld-Policy与WorldCam则展示视觉-动作解耦的不同应用：前者专注机器人策略，后者聚焦游戏世界生成。SocialOmni的"感知-交互脱钩"发现与Alignment论文的"规范性偏差"形成有趣呼应——模型在理解与行动之间存在本质张力。

* **行业影响**：MetaClaw已在OpenClaw平台20+渠道生产环境部署，标志着LLM Agent进入"边用边学"阶段。SocialOmni为Omni模型（语音+视觉+文本）提供了社交能力评估标准，利好多模态对话系统开发。GigaWorld-Policy的9倍推理加速和95%性能提升，为机器人实际部署扫清障碍。

* **安全伦理**：Alignment论文揭示对齐模型在战略推理上的退化——这意味着用RLHF优化的助手可能在博弈场景中表现反直觉。MetaClaw的持续学习需防止数据污染，引入版本控制隔离support/query数据。SocialOmni的音频视觉不一致测试也间接涉及deepfake检测场景。

* **重点关注**：视频推理机制（Chain-of-Steps）的发现对AI生成内容检测有直接意义——理解推理在去噪步骤涌现，可用于识别AI生成视频的内部特征。SocialOmni的benchmark也可扩展用于检测模型在社交交互中的异常行为。

---

> 📌 **保存建议**：将本文保存为 `daily-brief-2026-03-19.md`