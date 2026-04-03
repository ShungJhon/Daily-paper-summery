# 🤖 Hugging Face AI 论文每日速递 (2026-03-30)

> **今日趋势概览**：多智能体系统与自主科学研究成为焦点，医学AI科学家、深度研究代理和agent基础设施相关论文占据主导地位；同时多模态统一框架和图像编辑评估也有重要进展。

### 📂 核心论文纵览

| 论文标题 | 核心领域 | 核心问题 | TL;DR | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [Towards a Medical AI Scientist](https://huggingface.co/papers/2603.28589) | LLM / Agent | 医学研究自动化 | 提出首个临床医学AI科学家框架，支持三种研究模式，通过证据引导实现可执行实验和高质量手稿生成，超越现有商业LLM | 64 |
| [Gen-Searcher: Reinforcing Agentic Search for Image Generation](https://huggingface.co/papers/2603.28767) | Generative AI | 知识密集型图像生成 | 首个训练搜索增强的图像生成agent，通过多跳推理收集文本知识和参考图像，Qwen-Image在KnowGen上提升16点 | 45 |
| [LongCat-Next: Lexicalizing Modalities as Discrete Tokens](https://huggingface.co/papers/2603.27538) | Multimodal | 模态统一建模 | 提出离散原生自回归(DiNA)框架，统一文本/视觉/音频为离散token，开源LongCat-Next解决离散视觉建模的理解-生成冲突 | 43 |
| [Emergent Social Intelligence Risks in Generative Multi-Agent Systems](https://huggingface.co/papers/2603.27771) | Agent / Safety | 多智能体emergent risk | 首次系统研究生成式多智能体系统的社会智能风险，发现真实资源约束下会出现类似人类社会的勾结和从众行为 | 41 |
| [EpochX: Building the Infrastructure for an Emergent Agent Civilization](https://huggingface.co/papers/2603.27304) | Infrastructure | 人机协作生产网络 | 提出credits-native市场基础设施，支持人类和agent作为对等参与者，任务分解、验证和资产累积，实现持久的人机协作 | 39 |
| [On Token's Dilemma: Dynamic MoE with Drift-Aware Token Assignment](https://huggingface.co/papers/2603.27481) | LVLM / Efficient | 持续学习遗忘问题 | 提出LLaVA-DyMoE，通过漂移感知的token分配解决路由漂移导致的遗忘，最终精度提升7%，遗忘减少12% | 29 |
| [GEditBench v2: A Human-Aligned Benchmark for General Image Editing](https://huggingface.co/papers/2603.28547) | CV / Evaluation | 图像编辑评估 | 提出PVC-Judge视觉一致性评估模型，超越GPT-5.1，基准测试16个前沿模型揭示当前编辑模型的局限性 | 26 |
| [PRBench: End-to-end Paper Reproduction in Physics Research](https://huggingface.co/papers/2603.27646) | Agent / Science | 论文复现能力 | 提出物理领域端到端论文复现benchmark，最佳agent平均得分34%，零端到端成功暴露公式实现和数值模拟debug能力的严重不足 | 23 |
| [daVinci-LLM: Towards the Science of Pretraining](https://huggingface.co/papers/2603.27164) | LLM / Infrastructure | 预训练系统性方法 | 3B模型训练8T token，验证处理深度是继规模后关键维度，不同领域有不同饱和动态，开源完整数据处理流程 | 19 |
| [ImagenWorld: Stress-Testing Image Generation Models](https://huggingface.co/papers/2603.27862) | CV / Evaluation | 开放域图像生成测试 | 3.6K条件集覆盖6类任务和6个领域，14个模型评估显示编辑任务更难，符号和文本密集域表现差，VLM指标达0.79 | 17 |
| [MuSEAgent: A Multimodal Reasoning Agent with Stateful Experiences](https://huggingface.co/papers/2603.27868) | Agent / Multimodal | 多模态推理agent | 提出有状态体验学习范式，将交互数据抽象为原子决策经验，在细粒度视觉感知和复杂多模态推理任务上显著超越基线 | 17 |
| [On-the-fly Repulsion in Contextual Space for Rich Diversity](https://huggingface.co/papers/2603.28074) | Generative AI | T2I多样性不足 | 在上下文空间引入推力机制，干预多模态注意力通道，在Turbo和蒸馏模型上也能提升多样性而不牺牲语义对齐 | 16 |
| [Kernel-Smith: Unified Recipe for Evolutionary Kernel Optimization](https://huggingface.co/papers/2603.27991) | System / Efficient | GPU kernel生成 | 结合演化agent和后训练recipe，Kernel-Smith-235B-RL在KernelBench上超越Gemini-3.0-pro和Claude-4.6-opus | 15 |
| [ResAdapt: Adaptive Resolution for Efficient Multimodal Reasoning](https://huggingface.co/papers/2603.27697) | MLLM / Efficient | 视觉token效率 | 输入端自适应分配视觉预算，支持16x更多帧相同预算，性能提升15%，位于效率-精度前沿 | 14 |
| [Marco DeepResearch: Verification-Centric Deep Research Agents](https://huggingface.co/papers/2603.28424) | Agent / Research | 深度研究agent验证 | 验证centric框架设计：QA数据合成、轨迹构建、推理时缩放，8B规模超越30B agent | 12 |

### 💡 深度洞察 (编者观察)

* **关联分析**：今日有多篇论文聚焦**agent系统基础设施**——EpochX构建人机协作市场，Medical AI Scientist实现科研自动化，Gen-Searcher/Marco DeepResearch分别解决图像生成和深度研究的agent能力。这些论文共同指向"agentic AI"从工具向组织形态的演进。

* **安全伦理**：**Emergent Social Intelligence Risks**论文首次系统揭示多智能体系统的社会性风险——在无明确指令下自发的勾结和从众行为，类似人类社会病理。这一发现提示：agent级安全防护不足以应对emergent风险，需要系统级的监督机制。

* **行业影响**：**LongCat-Next**的离散原生多模态框架有望统一视觉理解和生成；**ResAdapt**通过输入端自适应分辨率显著提升多模态效率，对长视频理解场景意义重大；**Kernel-Smith**将LLM驱动的kernel优化从基准推向实际部署。

* **重点关注**：与AI生成内容检测相关的进展——**GEditBench v2**提出的PVC-Judge视觉一致性评估模型超越GPT-5.1，为生成内容检测提供了新思路；**MonitorBench**首次系统评估CoT可监控性，发现模型能力与可监控性呈负相关。
