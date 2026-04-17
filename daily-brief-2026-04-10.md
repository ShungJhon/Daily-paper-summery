# 🤖 Hugging Face AI 论文每日速递 (2026-04-10)

> **今日趋势概览**：AI Agent 与具身智能成为核心焦点，LLM 推理训练、多模态理解、Web 自动化和高效推理并行发展，涌现多个高质量基准数据集与新训练范式。

### 📂 核心论文纵览（按 Upvotes 排序）

| 论文标题 | 核心领域 | 核心问题 | TL;DR | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [Rethinking Generalization in Reasoning SFT](https://huggingface.co/papers/2604.06628) | LLM/SFT | 推理 SFT 的跨领域泛化条件 | 提出条件性泛化分析框架，发现"先降后升"的dip-and-recovery模式，强模型能习得可迁移推理策略 | 292 |
| [SkillClaw](https://huggingface.co/papers/2604.08377) | Agent | 跨用户技能演化 | 提出多用户智能体生态的集体技能演化框架，通过自主 evolver 聚合轨迹并更新技能库，实现跨用户知识迁移 | 259 |
| [ClawBench](https://huggingface.co/papers/2604.08523) | Agent/Web | AI 能否完成日常网络任务 | 构建153个跨144平台的真实网络任务基准，最强模型仅33.3%成功率 | 242 |
| [HY-Embodied-0.5](https://huggingface.co/papers/2604.07430) | Embodied/VLM | 具身智能的核心能力 | 推出 MoT 架构的2B/32B模型，融合空间时序感知与具身推理，在22个基准上达SOTA | 152 |
| [When Numbers Speak](https://huggingface.co/papers/2604.08546) | Video/Gen | Text-to-video 数量对齐 | 提出 NUMINA 框架，通过注意力头识别可计数的潜在布局，计数精度提升7.4% | 109 |
| [MegaStyle](https://huggingface.co/papers/2604.08364) | Style Transfer | 大规模风格数据集构建 | 提出可扩展的风格数据 curation  pipeline，170K风格prompt+400K内容prompt构建1.4M数据集 | 92 |
| [LPM 1.0](https://huggingface.co/papers/2604.07823) | Video/Gen | 角色表演视频生成 | 17B Diffusion Transformer 实现实时、无限长度的对话角色表演，解决表现力-实时性-身份一致性三角难题 | 55 |
| [OpenVLThinkerV2](https://huggingface.co/papers/2604.08539) | Multimodal/RL | 开源多模态模型的 GRPO 训练 | 提出 Gaussian GRPO (G²RPO)，通过分布匹配确保任务间梯度公平，增强感知-推理平衡 | 44 |
| [DMax](https://huggingface.co/papers/2604.08302) | Efficient/LLM | 扩散语言模型的并行解码 | 提出渐进式自精化框架，将TPF从2.04提升至5.47，同时保持准确率 | 43 |
| [KnowU-Bench](https://huggingface.co/papers/2604.08455) | Agent/Mobile | 个性化移动 agent 评估 | 构建42通用+86个性化+64主动任务的移动agent基准，揭示偏好的获取和干预校准是核心瓶颈 | 40 |
| [Externalization in LLM Agents](https://huggingface.co/papers/2604.08224) | Agent/Theory | Agent 外部化架构演进 | 系统回顾从权重到上下文到 harness 的转变，memory/skills/protocols 是三种外部化形式 | 40 |
| [Act Wisely](https://huggingface.co/papers/2604.08545) | Agent/Tool | Agent 元认知工具使用 | 提出 HDPO 框架解耦准确率与效率优化通道，实现"先解题后优化"认知课程 | 37 |
| [MolmoWeb](https://huggingface.co/papers/2604.08516) | Agent/Web | 开放视觉 Web Agent | 构建100K+合成轨迹+30K+人类演示的开源网络agent，8B版本超越封闭前沿模型 | 35 |
| [OpenSpatial](https://huggingface.co/papers/2604.07296) | Spatial/Reasoning | 空间智能数据引擎 | 提出3D边界框原语构建5大空间任务数据层次，3M数据集带来19%相对性能提升 | 33 |
| [OmniJigsaw](https://huggingface.co/papers/2604.08209) | Multimodal/RL | 全模态联合推理 | 提出时序重排代理任务的自我监督框架，通过跨模态集成策略增强视频-音频理解 | 21 |
| [FIT](https://huggingface.co/papers/2604.08526) | CV/VTON | 合身虚拟试穿 | 构建1.13M含精确身体-服���尺寸的虚拟试穿数据集，解决"不合身"情况 | 19 |
| [Graph of Skills](https://huggingface.co/papers/2604.05333) | Agent/Skills | 大规模技能库检索 | 提出技能图结构检索，输入token减少37.8%同时平均reward提升43.6% | 19 |
| [Agent-as-Annotators](https://huggingface.co/papers/2604.07776) | Agent/Web |Web Agent 能力蒸馏 | 用前沿模型作为教师生成轨迹微调9B学生，在WebArena达41.5%超越闭源模型 | 17 |
| [SIM1](https://huggingface.co/papers/2604.08544) | Robotics/Deformable | 可变形物体操纵 | 提出物理对齐的模拟器，合成数据训练策略达真实部署90%零样本成功率 | 13 |
| [Flux Attention](https://huggingface.co/papers/2604.07394) | Efficient/LLM | 高效 LLM 推理 | 提出层级别路由的动态注意力，预填充阶段加速2.8倍，解码阶段加速2.0倍 | 13 |

### 💡 深度洞察 (编者观察)

* **关联分析**：SkillClaw 与 Graph of Skills 两条路径分别从技能演化与技能检索入手解决大规模技能库问题；ClawBench 和 KnowU-Bench 分别从通用任务和个性化任务两个维度评估 Agent 能力，形成互补；多个工作（DMax、Flux Attention）聚焦长上下文推理效率，方法论上从并行解码到动态稀疏注意力各有千秋。

* **行业影响**：HY-Embodied-0.5 和 SIM1 代表具身智能的物理世界落地进展；LPM 1.0 推动数字人/虚拟主播进入实时交互时代；ClawBench 揭示当前前沿模型在真实网络任务上33%的瓶颈，为 Agent 产品化指明方向。

* **安全伦理**：Rethinking Generalization in Reasoning SFT 揭示推理提升与安全下降的非对称性，需要在训练中显式考虑安全对齐成本。

* **重点关注**：今日无 AIGC 检测相关论文。多篇论文聚焦 Agent 工具使用优化（Act Wisely、SkillClaw），反映学界对 Agent 可靠性的高度关注。

---

*数据来源：https://huggingface.co/papers/date/2026-04-10*