# 🤖 Hugging Face AI 论文每日速递 (2026-03-30)

> **今日趋势概览**：视频生成技术迎来突破性进展，长视频生成与内存机制成为焦点；同时多模态模型规模持续扩大，1万亿参数模型首次亮相。

### 📂 核心论文纵览

| 论文标题 | 核心领域 | 核心问题 | TL;DR | Upvotes |
| :--- | :--- | :--- | :---: | :---: |
| [Out of Sight but Not Out of Mind: Hybrid Memory for Dynamic Video World Models](https://huggingface.co/papers/2603.25716) | Video Generation | 动态主体隐藏后消失问题 | 提出Hybrid Memory和HyDRA架构，解决动态主体在视线外的身份保持和运动连续性，在HM-World数据集上显著超越SOTA | 134 |
| [Intern-S1-Pro: Scientific Multimodal Foundation Model at Trillion Scale](https://huggingface.co/papers/2603.25040) | LLM/Science | 多领域科学推理能力 | 首个1万亿参数科学多模态基础模型，涵盖100+科学任务，在通用能力达开源顶尖水平，专业任务超越闭源模型 | 118 |
| [PixelSmile: Toward Fine-Grained Facial Expression Editing](https://huggingface.co/papers/2603.25728) | CV/Generative | 表情编辑语义重叠问题 | 提出Flex Facial Expression数据集和PixelSmile框架，通过对称联合训练实现表情解耦，达到精确线性控制 | 114 |
| [ShotStream: Streaming Multi-Shot Video Generation for Interactive Storytelling](https://huggingface.co/papers/2603.25746) | Video Generation | 多镜头视频生成交互性差 | 首创因果多镜头架构，支持流式提示实时交互，16 FPS单GPU生成，实现亚秒级延迟 | 110 |
| [RealRestorer: Towards Generalizable Real-World Image Restoration](https://huggingface.co/papers/2603.25502) | CV | 真实场景图像恢复泛化性 | 构建大规模9类真实退化数据集和RealIR-Bench，开源模型达到SOTA，缩小与闭源差距 | 50 |
| [Voxtral TTS](https://huggingface.co/papers/2603.25551) | Speech/Audio | 多语言语音克隆自然度 | 3秒参考音频即可克隆，混合架构结合自回归语义token和flow-matching声学token，68.4%胜率超越ElevenLabs | 49 |
| [PackForcing: Short Video Training Suffices for Long Video Sampling](https://huggingface.co/papers/2603.25730) | Video Generation | 长视频生成KV缓存爆炸 | 提出三区KV-cache策略和32x token压缩，4GB显存生成2分钟832x480@16fps视频，实现24x时间外推 | 39 |
| [Trace2Skill: Distill Trajectory-Local Lessons into Transferable Agent Skills](https://huggingface.co/papers/2603.25158) | LLM/Agent | 智能体技能手工编写瓶颈 | 从执行轨迹中并行提取经验，通过归纳推理整合为统一技能目录，35B模型提取的技能可提升122B模型57.65分 | 33 |
| [MACRO: Advancing Multi-Reference Image Generation](https://huggingface.co/papers/2603.25319) | CV/Generative | 多参考图像生成性能衰减 | 构建400K样本10参考的MacroData数据集和MacroBench基准，揭示跨参考协同训练优势 | 30 |
| [RealChart2Code: Advancing Chart-to-Code Generation](https://huggingface.co/papers/2603.25804) | VLM/Code | 复杂图表代码生成能力 | 推出2800+真实数据图表基准，首次评估从大规模原始数据生成和迭代代码优化，揭示VLMs与闭源模型差距 | 19 |
| [Natural-Language Agent Harnesses](https://huggingface.co/papers/2603.25723) | Agent | Agent harness设计可迁移性 | 将agent控制逻辑外化为可执行自然语言工件，提出智能运行时IHR执行 | 12 |
| [Less Gaussians, Texture More: 4K Feed-Forward Textured Splatting](https://huggingface.co/papers/2603.25745) | 3D/CV | 高分辨率3DGS二次方增长 | 提出LGTM框架，解耦几何复杂性与渲染分辨率，4K新视角合成无需逐场景优化 | 10 |
| [MuRF: Unlocking the Multi-Scale Potential of Vision Foundation Models](https://huggingface.co/papers/2603.25744) | CV | VFM推理固定单一尺度 | 提出多分辨率融合MuRF，无需训练提升视觉表征，应用于DINOv2等多模型 | 9 |
| [Revisiting On-Policy Distillation: Empirical Failure Modes and Simple Fixes](https://huggingface.co/papers/2603.25562) | LLM | OPD在长程任务中的脆弱性 | 识别token级OPD三大失败模式，提出top-K本地支持匹配，数学推理和智能体任务更稳定 | 5 |
| [Vega: Learning to Drive with Natural Language Instructions](https://huggingface.co/papers/2603.25741) | Autonomous Driving | 驾驶系统缺乏指令跟随能力 | 构建100K场景指令数据集InstructScene，统一VLM-World-Action模型，AR+Diffusion联合范式 | 4 |

### 💡 深度洞察

* **关联分析**：视频生成领域出现三篇高热度论文（#1, #4, #7），共同指向长视频生成的内存机制和时序一致性难题。Hybrid Memory和PackForcing分别从记忆保持和KV缓存压缩角度切入，形成互补方案。Intern-S1-Pro的1万亿参数路线与Trace2Skill的技能蒸馏形成"大模型+高效复用"的技术呼应。

* **行业影响**：PackForcing实现2分钟视频单GPU生成（16 FPS），将推动短视频创作工具的实时化；Voxtral TTS的3秒克隆能力使个性化语音交互门槛大幅降低；MACRO和RealChart2Code的 benchmark推出将加速多参考图像生成和可视化代码助手的产品化。

* **安全伦理**：Intern-S1-Pro作为万亿级科学模型，其科学领域自动化推理能力需关注滥用风险；视频生成技术的突破可能加剧深度伪造治理压力。

* **重点关注**：视频生成方向的三篇论文（Hybrid Memory, ShotStream, PackForcing）与生成类工作高度相关。Hybrid Memory解决动态主体一致性、PackForcing实现长时序外推，两者结合可能催生长视频可控生成的新范式。
