# 🤖 Hugging Face AI 论文每日速递 (2026-04-01)

> **今日趋势概览**：多模态Agent与搜索增强生成成为主流研究方向，同时轻量化设备端模型取得突破性进展。

### 📂 核心论文纵览

| 论文标题 | 核心领域 | 核心问题 | TL;DR | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [Towards a Medical AI Scientist](https://arxiv.org/abs/2603.28589) | LLM/AI Science | 医学研究自动化 | 提出首个临床医学AI科学家框架，通过Clinician-Engineer协同推理机制生成可追溯的研究想法，生成手稿达到MICCAI级别质量 | 81 |
| [Gen-Searcher: Reinforcing Agentic Search for Image Generation](https://arxiv.org/abs/2603.28767) | Multimodal/Agent | 知识密集型图像生成 | 首个训练搜索增强图像生成Agent的工作，构建多跳推理+外部知识检索流水线，在KnowGen上提升Qwen-Image约16点 | 51 |
| [Unify-Agent: A Unified Multimodal Agent for World-Grounded Image Synthesis](https://arxiv.org/abs/2603.29620) | Multimodal/Agent | 世界知识对齐的图像生成 | 将图像生成重构为Agentic Pipeline，包含提示理解、多模态证据搜索、基础重标注和最终合成，在FactIP基准上显著提升 | 33 |
| [GEditBench v2: A Human-Aligned Benchmark for General Image Editing](https://arxiv.org/abs/2603.28547) | CV/Image Editing | 图像编辑评估 | 提出1200个真实用户查询和PVC-Judge开源评估模型，在视觉一致性评估上超越GPT-5.1 | 31 |
| [CutClaw: Agentic Hours-Long Video Editing via Music Synchronization](https://arxiv.org/abs/2603.29664) | Video/Agent | 长时间视频智能剪辑 | 首个多Agent系统实现小时级原始素材自动剪辑为音乐同步短视频，使用分层多模态分解和Playwriter Agent编排叙事 | 30 |
| [Video Generation Models as World Models: Efficient Paradigms, Architectures and Algorithms](https://arxiv.org/abs/2603.28489) | Video/World Model | 视频生成作为世界模拟器 | 系统性综述高效视频生成框架，从高效建模范式、网络架构、推理算法三维度分析，论证效率是成为通用世界模拟器的前提 | 25 |
| [On-the-fly Repulsion in the Contextual Space for Rich Diversity in Diffusion Transformers](https://arxiv.org/abs/2603.28762) | Generative AI/T2I | Diffusion Transformer多样性 | 提出在Contextual Space中应用即时排斥力增加生成多样性，无需额外优化且在Turbo模型上同样有效 | 22 |
| [Terminal Agents Suffice for Enterprise Automation](https://arxiv.org/abs/2604.00073) | Agent/Automation | 企业自动化架构选择 | 论证配备终端和文件系统的简单编码Agent即可胜任企业任务，性能匹敌复杂MCP/Web Agent架构 | 19 |
| [MonitorBench: A Comprehensive Benchmark for Chain-of-Thought Monitorability](https://arxiv.org/abs/2603.28590) | LLM/Interpretability | CoT可监测性评估 | 提出1514个测试实例评估CoT与最终输出的因果关联性，发现模型能力越强可监测性越低，压力测试下可下降30% | 17 |
| [ResAdapt: Adaptive Resolution for Efficient Multimodal Reasoning](https://arxiv.org/abs/2603.28610) | MLLM/Efficiency | 多模态推理效率 | 学习每个帧应分配多少视觉预算，支持相同预算下16倍帧数提升，推理密集型基准提升超15% | 16 |
| [DreamLite: A Lightweight On-Device Unified Model for Image Generation and Editing](https://arxiv.org/abs/2603.28713) | On-device AI | 设备端统一生成模型 | 首个支持生成和编辑的统一端侧模型(0.39B)，在小米14手机1秒内完成1024x1024图像生成/编辑 | 15 |
| [Think Anywhere in Code Generation](https://arxiv.org/abs/2603.29957) | LLM/Code | 代码生成的思考位置 | 提出Think-Anywhere机制让LLM在代码生成任意位置按需调用思考，在四个主流代码基准达到SOTA | 14 |
| [Extend3D: Town-Scale 3D Generation](https://arxiv.org/abs/2603.29387) | 3D Generation | 城镇级3D场景生成 | 训练无关 pipeline，通过扩展latent空间和patch-wise生成实现单图像城镇级3D场景重建 | 14 |
| [FlowPIE: Test-Time Scientific Idea Evolution with Flow-Guided Literature Exploration](https://arxiv.org/abs/2603.29557) | AI Science | 科学想法生成 | 使用Flow-guided MCTS和测试时想法演化实现科学创意生成，显著提升想法的新颖性、可行性和多样性 | 11 |
| [HandX: Scaling Bimanual Motion and Interaction Generation](https://arxiv.org/abs/2603.28766) | Motion/Interaction | 双手运动生成 | 提出统一双手运动基础模型和数据框架，收集高质量双手交互运动捕捉数据，观察到明显的Scaling趋势 | 11 |

### 💡 深度洞察 (编者观察)

* **关联分析**：Gen-Searcher和Unify-Agent采用相似的技术路径——搜索增强+Agentic Pipeline来解决知识密集型图像生成问题。两者都强调外部知识 grounding的重要性，标志着图像生成从纯生成向检索增强生成(RAG)范式的转变。

* **行业影响**：
  - DreamLite等轻量化模型的突破意味着端侧AI应用即将进入实用阶段，1秒内完成生成/编辑对移动端意义重大
  - CutClaw展示的Agentic视频编辑工作流将大幅降低内容创作门槛
  - Terminal Agents的实证研究提示简单接口+强基座模型足以满足企业自动化需求，复杂中间层可能并非必需

* **安全伦理**：
  - MonitorBench揭示CoT可监测性问题：模型越强反而越难通过思考过程预测其行为，这对AI安全性有重要启示
  - 搜索增强图像生成可能引入知识版权和事实准确性风险

* **重点关注**：AI生成内容检测方向暂无新进展，但多篇论文(Gen-Searcher, Unify-Agent, FlowPIE)涉及外部知识检索与生成结合，这类技术可能被滥用于生成虚假"有据可查"的内容，值得跟踪。
