# 🤖 Hugging Face AI 论文每日速递 (2026-04-13 ~ 2026-04-14)

> **今日趋势概览**：多模态与 LLM Agent 并行爆发，制造业视觉评估、视觉语言模型隐私、推理奖励模型成为新焦点。

### 📂 核心论文纵览（按 Upvotes 排序）

| 论文标题 | 核心领域 | 核心问题 | TL;DR | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [FORGE: Fine-grained Multimodal Evaluation for Manufacturing](https://huggingface.co/papers/2604.07413) | CV/MLLM | 制造业场景缺乏高质量多模态评估基准 | 提出 FORGE 基准，涵盖 6 类任务，首次系统性评估 MLLM 在工业自动化的能力 | 87 |
| [Attention Sink in Transformers: A Survey](https://huggingface.co/papers/2604.10098) | LLM | Transformer 长序列生成时注意力分散问题 | 全面调研 Attention Sink 机制，探讨其在稳定生成、长度外推方面的作用 | 55 |
| [EXAONE 4.5 Technical Report](https://huggingface.co/papers/2604.08644) | VLM | 开源 VLM 性能不足 | LG 发布首个开放权重视觉语言模型，集成 MoE 架构，超越 Llava | 51 |
| [Strips as Tokens: Artist Mesh Generation](https://huggingface.co/papers/2604.09132) | 3D Gen | 3D 网格生成中 token 顺序问题 | 提出 UV 分割 token 排序方案，提升艺术家级别网格生成质量 | 44 |
| [Pseudo-Unification: Entropy Probing](https://huggingface.co/papers/2604.10949) | Multimodal | 统一多模态模型信息分离不足 | 通过熵探测揭示 UMM 中文本与视觉信息的伪融合现象 | 36 |
| [CocoaBench: Evaluating Unified Digital Agents](https://huggingface.co/papers/2604.11201) | Agent | 缺乏真实环境评估基准 | 发布首个数字 Agent 野外评估基准，覆盖软件工程、深度研究等场景 | 29 |
| [Multi-User Large Language Model Agents](https://huggingface.co/papers/2604.08567) | Agent | 多用户场景下 Agent 决策冲突 | 提出多用户协作框架，首次系统性研究 LLM Agent 在多用户环境的表现 | 22 |
| [ELT: Elastic Looped Transformers](https://huggingface.co/papers/2604.09168) | Visual Gen | 视觉生成参数效率低 | 提出循环 Transformer 架构，参数效率大幅提升 | 17 |
| [Tracing the Roots: Data Origin Tracking](https://huggingface.co/papers/2604.10480) | LLM/Post-training | 后训练数据来源不透明 | 提出多 Agent 框架追溯数据来源，揭示数据污染问题 | 14 |
| [Solving Physics Olympiad via RL](https://huggingface.co/papers/2604.11805) | RL/LLM | 物理推理数据稀缺 | 基于 PhysBench 数据集，用 RL 训练 LLM 解决物理奥赛题 | 13 |
| [Backdoor Attacks on Decentralised Post-Training](https://huggingface.co/papers/2604.02372) | Security | 分布式训练后门风险 | 揭示去中心化后训练中的后门攻击风险，提出防御策略 | 10 |
| [Mobile GUI Agent Privacy Personalization](https://huggingface.co/papers/2604.11259) | Privacy | 移动端 Agent 隐私泄露 | 通过轨迹推断实现隐私个性化保护 | 9 |
| [Efficient RL Training for LLMs](https://huggingface.co/papers/2604.08706) | RL/LLM | 经验回放效率低 | 提出高效经验回放方法，提升 RL 训练 LLM 的效率 | 9 |
| [VisionFoundry: Teaching VLMs Visual Perception](https://huggingface.co/papers/2604.09531) | VLM | VLM 空间理解弱 | 用合成数据训练 VLM 视觉感知能力 | 8 |
| [Envisioning the Future, One Step at a Time](https://huggingface.co/papers/2604.09527) | World Model | 长时序预测不确定性 | 提出逐步预测框架，增强复杂场景的时间推理能力 | 7 |

### 💡 深度洞察

* **关联分析**：本周多篇论文聚焦 **Agent 评估框架**（CocoaBench）和 **后训练数据追溯**（Tracing the Roots），反映出业界对 LLM 后训练阶段透明性的高度关注。同时 Attention Sink 论文表明长序列生成仍是核心难题。

* **行业影响**：EXAONE 4.5 的发布标志着开源 VLM 竞争加剧，制造业（FORGE）、物理奥赛（Physics Olympiad）等垂直领域出现专用评估基准，暗示 AI 应用正在向行业深度定制方向发展。

* **安全伦理**：Backdoor Attacks 和 Mobile GUI Agent Privacy 论文揭示分布式训练和移动端部署的安全风险，建议关注去中心化训练的可信度验证机制。

* **重点关注**：**AIGC 检测相关内容未出现在本期榜单**，但 `Tracing the Roots` 涉及数据来源追溯，可能与检测溯源技术存在关联。

---
*数据来源：https://huggingface.co/papers/date/2026-04-14, https://huggingface.co/papers/date/2026-04-13*