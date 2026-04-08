# 🤖 Hugging Face AI 论文每日速递 (2026-04-06)

> **今日趋势概览**：Agent 能力评估成为焦点，企业自动化和视频理解领域涌现新基准，安全与隐私研究持续升温。

### 📂 核心论文纵览

| 论文标题 | 核心领域 | 核心问题 | TL;DR | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [Self-Distilled RLVR](https://huggingface.co/papers/2604.03128) | RL / LLM | On-policy distillation 在 RL 中的应用 | 提出 Self-Distillation 作为 RLVR 辅助方法，推理时性能显著提升 | 98 |
| [Terminal Agents Suffice for Enterprise Automation](https://huggingface.co/papers/2604.00073) | Agent / Enterprise | 企业自动化可行性 | 证明终端 Agent 足以执行有意义的企业任务 | 84 |
| [MiroEval: Benchmarking Multimodal Deep Research Agents](https://huggingface.co/papers/2603.28407) | Agent / Benchmark | 深度研究 Agent 评估 | 同时评估过程与结果的新基准，填补现有评估空白 | 64 |
| [ViGoR-Bench: Visual Generative Models Zero-Shot Reasoning](https://huggingface.co/papers/2603.25823) | CV / VLM | 视觉生成模型的推理能力 | 揭示 AIGC 模型"逻辑荒漠"问题，评估零样本推理能力 | 42 |
| [Vision2Web: Visual Website Development Benchmark](https://huggingface.co/papers/2603.26648) | CV / Agent | 视觉网站开发 | 提出带 Agent 验证的层级基准 | 40 |
| [QuitoBench: Time Series Forecasting Benchmark](https://huggingface.co/papers/2603.26017) | Time Series | 时序预测基准 | 高质量开放时序预测基准，解决数据稀缺问题 | 30 |
| [Reasoning Shift: How Context Shortens LLM Reasoning](https://huggingface.co/papers/2604.01161) | LLM / Reasoning | 上下文对推理的影响 | 发现上下文会悄然缩短 LLM 推理深度 | 28 |
| [Embarrassingly Simple Self-Distillation Improves Code Generation](https://huggingface.co/papers/2604.01193) | LLM / Code | 代码生成自蒸馏 | 无需 verifier/teacher/RL，极简自蒸馏提升代码生成 | 27 |
| [HippoCamp: Contextual Agents on Personal Computers](https://huggingface.co/papers/2604.01221) | Agent | PC 上下文 Agent | 评估多模态文件管理能力的新基准 | 26 |
| [GaussianGPT: Autoregressive 3D Gaussian Scene Generation](https://huggingface.co/papers/2603.26661) | Generative AI / 3D | 3D 场景生成 | 探索扩散/flow-matching 之外的自回归替代方案 | 21 |
| [Brevity Constraints Reverse Performance Hierarchies](https://huggingface.co/papers/2604.00025) | LLM | 简洁约束的影响 | 7.7% 基准问题上，大模型被小模型超越 28.4% | 19 |
| [PerceptionComp: Video Reasoning Benchmark](https://huggingface.co/papers/2603.26653) | CV / Video | 视频感知推理 | 需多时刻信息融合的复杂推理基准 | 16 |
| [Proactive Agent Research Environment](https://huggingface.co/papers/2604.00842) | Agent | 主动助手评估 | 模拟主动用户评估 Proactive Assistant | 10 |
| [Do Phone-Use Agents Respect Your Privacy?](https://huggingface.co/papers/2604.00986) | Agent / Privacy | 手机 Agent 隐私 | 评估手机 Agent 在移动任务中的隐私保护 | 7 |
| [A Survey of On-Policy Distillation for LLM](https://huggingface.co/papers/2604.00626) | Survey / LLM | LLM 蒸馏综述 | 全面综述 on-policy distillation 范式 | 7 |

### 💡 深度洞察

* **关联分析**：今日论文形成两条主线：1) **Agent 基准爆发** —— MiroEval、Vision2Web、HippoCamp、Proactive Agent Research Environment 集中发布，评估维度从单一任务走向过程与结果并重；2) **自蒸馏深化** —— Self-Distilled RLVR 和 Embarrassingly Simple Self-Distillation 表明无需外部信号即可提升 LLM 能力。

* **行业影响**：Terminal Agents 在企业自动化的研究证明 AI Agent 已具备实用价值。MiroEval 等新基准将推动深度研究 Agent 的标准化评估。

* **安全伦理**：Do Phone-Use Agents Respect Your Privacy 关注手机 Agent 隐私问题 —— 随着 Agent 获得更多系统权限，隐私保护成为关键挑战。

* **重点关注**：ViGoR-Bench 揭示 AIGC 模型的"逻辑荒漠"问题 —— 与 AIGC 检测直接相关，需持续跟踪。

---
*数据来源：https://huggingface.co/papers/date/2026-04-06*
