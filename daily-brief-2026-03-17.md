# 🤖 Hugging Face AI 论文每日速递 (2026-03-17)

> **今日趋势概览**：Agent与多模态理解成为焦点，搜索智能体和世界模拟模型获得最高关注，同时LLM推理效率优化持续推进。

### 📂 核心论文纵览

| 论文标题 | 核心领域 | 核心问题 | TL;DR | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [AI Can Learn Scientific Taste](https://huggingface.co/papers/2603.14473) | LLM/Science | LLM能否像科学家一样阅读论文 | 提出SGI-Bench基准，评估LLM跨10个科学领域的科学推理能力 | 216 |
| [OpenSeeker: Democratizing Frontier Search Agents](https://huggingface.co/papers/2603.15594) | RL/Agent | 如何开源前沿搜索智能体 | 全开源训练数据的搜索智能体框架 | 125 |
| [EnterpriseOps-Gym](https://huggingface.co/papers/2603.13594) | Agent | 企业场景的智能体规划 | 提供企业环境中的有状态智能体规划基准 | 117 |
| [Grounding World Simulation Models](https://huggingface.co/papers/2603.15583) | CV/Simulation | 真实世界模拟 | 将世界模拟模型锚定到真实城市环境 | 96 |
| [HSImul3R](https://huggingface.co/papers/2603.15612) | CV/3D | 人体场景交互3D重建 | 物理驱动的双向优化框架，生成simulation-ready的HSI重建 | 92 |
| [Attention Residuals](https://huggingface.co/papers/2603.15031) | LLM/Architecture | Transformer效率 | 揭示注意力残差机制，提出新架构改进方向 | 57 |
| [Mixture-of-Depths Attention](https://huggingface.co/papers/2603.15619) | LLM/Architecture | 动态计算分配 | 混合深度注意力实现动态计算资源分配 | 48 |
| [Effective Distillation to Hybrid xLSTM](https://huggingface.co/papers/2603.15590) | LLM/Architecture | 模型压缩 | 有效蒸馏至混合xLSTM架构 | 30 |
| [Anatomy of a Lie](https://huggingface.co/papers/2603.15557) | VLM/Safety | VLM幻觉检测 | 多阶段诊断框架追溯VLM幻觉来源 | 24 |
| [ViFeEdit](https://huggingface.co/papers/2603.15478) | CV/Video | 视频编辑 | 无需调优器的视频Diffusion Transformer编辑 | 21 |
| [Safe and Scalable Web Agent Learning](https://huggingface.co/papers/2603.10505) | RL/Agent | Web智能体安全 | 通过重建网站实现安全可扩展的Web智能体学习 | 18 |
| [POLCA](https://huggingface.co/papers/2603.14769) | LLM/Optimization | 生成式优化 | 随机生成式优化方法 | 16 |
| [TERMINATOR](https://huggingface.co/papers/2603.12529) | LLM/Reasoning | CoT早停 | 学习CoT推理中的最优退出点 | 13 |
| [WebVR](https://huggingface.co/papers/2603.13391) | VLM/Benchmark | 网页重建 | 基于人类对齐视觉Rubric的VLM网页重建基准 | 12 |
| [Training-free Detection of Generated Videos](https://huggingface.co/papers/2603.15026) | CV/Video | 生成视频检测 | 无需训练的空间-时间似然方法检测AI生成视频 | 7 |

### 💡 深度洞察

* **关联分析**：本月出现多个关于LLM推理效率的论文（Attention Residuals、Mixture-of-Depths、FineRMoE），表明计算效率优化成为重要研究方向。Anatomy of a Lie与多篇VLM论文形成呼应，VLM幻觉问题持续受到关注。

* **行业影响**：OpenSeeker和EnterpriseOps-Gym代表企业级Agent应用的最新进展，预计将推动自动化工作流程的落地。HSImul3R的物理仿真重建技术对机器人和VR应用有重要价值。

* **安全伦理**：Anatomy of a Lie提供VLM幻觉的系统性诊断框架，对提升多模态模型可靠性有重要意义。Safe and Scalable Web Agent Learning关注智能体学习过程中的安全性。

* **重点关注**：ViFeEdit和Training-free Detection of Generated Videos分别涉及生成内容检测的两端——生成与检测，这类研究与你当前工作高度相关，值得深入关注。

---
📌 **保存建议**：可将内容保存为 `daily-brief-2026-03-17.md`
