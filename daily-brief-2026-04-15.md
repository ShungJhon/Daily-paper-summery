# 🤖 Hugging Face AI 论文每日速递 (2026-04-15)

> **今日趋势概览**：强化学习推理与On-Policy Distillation成为焦点，多模态Agent安全引发关注，Habitat-GS推动具身智能模拟器升级。

### 📂 核心论文纵览

| 论文标题 | 核心领域 | 核心问题 | TL;DR | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [KnowRL: Boosting LLM Reasoning via Reinforcement Learning with Minimal-Sufficient Knowledge Guidance](https://huggingface.co/papers/2604.12627) | LLM + RL | 强化学习推理的奖励稀疏问题 | 提出KnowRL，通过最小充分知识引导减少冗余，将推理任务奖励稀疏度从严重降至可解，显著提升RLVR效果。 | 82 |
| [Rethinking On-Policy Distillation of Large Language Models: Phenomenology, Mechanism, and Recipe](https://huggingface.co/papers/2604.13016) | LLM | 蒸馏效果不稳定的根本原因 | 发现OPD成功两条件：师生思维模式兼容 + 学生保留探索空间，揭示蒸馏失败本质并给出recipe。 | 59 |
| [SPPO: Sequence-Level PPO for Long-Horizon Reasoning Tasks](https://huggingface.co/papers/2604.08865) | LLM + RL | Token级PPO的时间信用分配不稳定 | 提出序列级PPO，在长CoT推理任务上减少时序信用分配不稳定性，降低显存成本。 | 25 |
| [Towards Long-horizon Agentic Multimodal Search](https://huggingface.co/papers/2604.12890) | Agent + 多模态 | 多模态搜索的上下文爆炸问题 | 提出方法管理异构信息与高Token成本，在长视野搜索中保持关键视觉信号。 | 15 |
| [Many-Tier Instruction Hierarchy in LLM Agents](https://huggingface.co/papers/2604.09443) | Agent | 多源指令冲突时的特权级别 | 提出多层级指令层级框架，处理系统消息/用户提示/工具输出等多来源指令冲突。 | 13 |
| [The Blind Spot of Agent Safety: How Benign User Instructions Expose Critical Vulnerabilities in Computer-Use Agents](https://huggingface.co/papers/2604.10577) | Agent安全 | 良性用户指令下的隐藏危害 | 揭示Computer-Use Agent的新安全问题：完全良性的指令也可能导致危害，填补安全评估空白。 | 12 |
| [Habitat-GS: A High-Fidelity Navigation Simulator with Dynamic Gaussian Splatting](https://huggingface.co/papers/2604.12626) | 具身智能 | 模拟器视觉保真度不足 | 引入动态Gaussian Splatting，提升视觉保真度并支持动态人类avatar。 | 12 |
| [Self-Adversarial One Step Generation via Condition Shifting](https://huggingface.co/papers/2604.12322) | 图像生成 | 一步生成的保真度/速度/效率权衡 | 通过Condition Shifting实现自对抗一步生成，平衡质量、速度和训练效率。 | 12 |
| [LARY: A Latent Action Representation Yielding Benchmark](https://huggingface.co/papers/2604.11689) | VLA | 视觉信号转潜在动作的泛化挑战 | 提出潜在动作表示的基准测试，评估VLA从人类视频学习泛化能力。 | 7 |
| [You Only Judge Once: Multi-response Reward Modeling](https://huggingface.co/papers/2604.10966) | 奖励模型 | 单次前向传播评分多响应 | 一次性评估所有候选响应，提升多响应奖励建模效率。 | 6 |
| [Generative Refinement Networks for Visual Synthesis](https://huggingface.co/papers/2604.13030) | 图像生成 | 扩散模型的计算效率问题 | 引入生成式优化网络，自适应计算复杂度以提升效率。 | 5 |
| [Masked by Consensus: Disentangling Privileged Knowledge in LLM Correctness](https://huggingface.co/papers/2604.12373) | LLM评估 | 模型内部正确性判断的特权知识 | 探究LLM是否拥有关于答案正确性的特权知识（内部状态）。 | 4 |
| [Do Thought Streams Matter? Evaluating Reasoning in Gemini Vision-Language Models](https://huggingface.co/papers/2604.11177) | VLM评估 | Gemini思维流对视频理解的影响 | 评估思维流是否随思考量增加而提升视频场景理解。 | 4 |
| [Lightning OPD: Efficient Post-Training for Large Reasoning Models](https://huggingface.co/papers/2604.13010) | LLM | OPD需要实时教师推理的高开销 | 离线OPD预计算教师log-probabilities，大幅降低基础设施开销。 | 4 |
| [Accelerating Speculative Decoding with Block Diffusion Draft Trees](https://huggingface.co/papers/2604.12989) | 推理加速 | 投机解码的Token生成效率 | 块扩散draft生成整块token，一次前向pass超越AR drafters。 | 4 |

### 💡 深度洞察

* **关联分析**：本周多篇论文聚焦LLM后训练方法——KnowRL(RLVR)、Rethinking OPD(Lightning OPD)形成完整技术链条：KnowRL解决奖励稀疏 → OPD反思揭示条件机制 → Lightning OPD实现离线高效训练。

* **行业影响**：Computer-Use Agent安全论文(篇6)揭示"良性指令危害"新范式，对实际部署AI助手有重要警示作用。Habitat-GS将推动具身智能训练数据质量升级。

* **安全伦理**：Agent Safety论文指出当前评估遗漏了关键场景——当用户指令完全善意但任务本质有害时，Agent仍会执行。这对AI安全评估体系有重要补充。

* **重点关注**：推荐篇1(KnowRL)和篇2(Rethinking OPD)——前者给出RLVR瓶颈的系统解法，后者澄清了蒸馏本质，两者结合是当前LLM后训练的关键突破。

---
*数据来源：https://huggingface.co/papers/date/2026-04-15*