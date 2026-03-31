# 🤖 Hugging Face AI 论文每日速递 (2026-03-26)

> **今日趋势概览**：视频理解与多模态Agent成为焦点，EVA实现planning-before-perception范式突破，CUA-Suite发布大规模计算机使用视频数据集推动Agent实用化。

---

### 📂 核心论文纵览

| 论文标题 | 核心领域 | 核心问题 | TL;DR (核心突破) | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [CUA-Suite: Massive Human-annotated Video Demonstrations for Computer-Use Agents](https://huggingface.co/papers/2603.XXXXX) | Agent/CV | 计算机使用Agent训练数据稀缺 | 发布约10,000任务、55小时、600万帧的视频数据集，包含连续30fps屏幕录制和动作标注，为计算机使用Agent提供关键训练资源。 | 69 |
| [EVA: Efficient Reinforcement Learning for End-to-End Video Agent](https://huggingface.co/papers/2603.22918) | CV/RL | 长视频理解token冗余与效率问题 | 提出planning-before-perception框架，通过迭代summary-plan-action-reflection实现query-driven视频理解，三阶段训练(SFT+KTO+GRPO)在6个基准上提升6-12%。 | 34 |
| [T-MAP: Red-Teaming LLM Agents with Trajectory-aware Evolutionary Search](https://huggingface.co/papers/2603.XXXXX) | RL/Agent | LLM Agent多步工具执行的安全漏洞 | 提出基于轨迹感知的进化搜索方法，利用执行轨迹引导对抗提示生成，在MCP环境中攻击实现率显著超越baseline，对GPT-5.2等前沿模型仍有效。 | 30 |
| [UI-Voyager: A Self-Evolving GUI Agent Learning via Failed Experience](https://huggingface.co/papers/2603.XXXXX) | Agent/CV | 移动GUI Agent从失败中学习效率低 | 提出两阶段自演进框架，第一阶段RFT实现数据和模型完全自主循环协同进化，第二阶段GRSD从成功轨迹构建密集监督信号，4B模型达81.0% Pass@1。 | 29 |
| [Why Does Self-Distillation (Sometimes) Degrade the Reasoning Capability of LLMs?](https://huggingface.co/papers/2603.XXXXX) | LLM | 自蒸馏导致数学推理能力下降 | 发现自蒸馏抑制了模型的不确定性表达(epistemic verbalization)，在Qwen3-8B等模型上性能下降达40%，暴露了优化推理行为的重要性。 | 27 |
| [GameplayQA: A Benchmarking Framework for Decision-Dense POV-Synced Multi-Video Understanding of 3D Virtual Agents](https://huggingface.co/papers/2603.XXXXX) | CV/Agent | 3D环境中多视频理解评估空白 | 提出决策密集型POV同步多视频理解基准，以1.22标签/秒密度注释游戏视频，包含2.4K诊断QA对，揭示前沿MLLM在时序理解和角色归属上的显著差距。 | 16 |
| [When Models Judge Themselves: Unsupervised Self-Evolution for Multimodal Reasoning](https://huggingface.co/papers/2603.XXXXX) | MLLM | 多模态推理依赖高质量标注数据 | 提出无监督自演进训练框架，利用模型自一致性信号和bounded Judge调制，在无标注数据上通过GRPO持续提升推理性能。 | 14 |
| [Understanding the Challenges in Iterative Generative Optimization with LLMs](https://huggingface.co/papers/2603.XXXXX) | LLM/Agent | 生成式优化工程化落地困难 | 调查了三个关键设计因素：起始工件、执行轨迹的信用视野、批量试验，发现这些决策决定了生成式优化的成败。 | 13 |
| [The Pulse of Motion: Measuring Physical Frame Rate from Visual Dynamics](https://huggingface.co/papers/2603.XXXXX) | CV/Video | AI生成视频的时间一致性 | 提出Visual Chronometer预测视频的物理帧率(PhyFPS)，发现当前视频生成模型存在严重的PhyFPS错位和时间不稳定问题。 | 10 |
| [SpectralSplats: Robust Differentiable Tracking via Spectral Moment Supervision](https://huggingface.co/papers/2603.XXXXX) | CV/3DGS | 3D Gaussian Splatting跟踪中的梯度消失 | 将优化目标从空间域转移到频域，通过频谱矩监督构建全局吸引域，即使在无像素重叠时也能获得有效梯度。 | 10 |

---

### 💡 深度洞察 (编者观察)

* **关联分析**：今日论文形成完整研究链——CUA-Suite提供训练数据基础(69 upvotes)，EVA实现高效视频理解(34 upvotes)，T-MAP保障安全(30 upvotes)，UI-Voyager实现持续进化(29 upvotes)，GameplayQA提供评估基准(16 upvotes)，覆盖从数据到安全到评估的全流程。

* **行业影响**：
  - CUA-Suite的55小时视频数据将显著推动Computer-Use Agent发展
  - EVA的planning-before-perception有望革新长视频问答、监控分析等应用
  - CarePilot将多Agent框架应用于医疗场景，实现15.26%性能提升
  - EnterpriseArena首次评估LLM在企业资源分配决策中的能力

* **安全伦理**：
  - T-MAP揭示了MCP生态中LLM Agent的新攻击面，对GPT-5.2等前沿模型仍有效
  - When Models Judge Thelves展示无监督自演进路径，减少对外部标注的依赖
  - Qworld提出问题特定评估标准，在HealthBench上覆盖89%专家标准

* **重点关注**：EVA框架将传统"先看后想"转变为"先想后看"，体现了Agent从被动识别到主动规划的范式转变，是视频理解领域的重要里程碑。自蒸馏研究揭示了不确定性表达对OOD泛化的关键作用，为推理优化提供新思路。

---

*注：本简报基于 Hugging Face Daily Papers 自动生成，数据来源：ChatPaper.ai。upvotes 截至发稿前。*
