[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## Updated on 2025.01.31
> Usage instructions: [here](./docs/README.md#usage)

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href=#agent>agent</a></li>
    <li><a href=#llm>llm</a></li>
    <li><a href=#moe>moe</a></li>
    <li><a href=#ssms>SSMs</a></li>
    <li><a href=#communication-intelligence>Communication Intelligence</a></li>
    <li><a href=#rag>RAG</a></li>
    <li><a href=#text2sql>text2sql</a></li>
    <li><a href=#ppc>PPC</a></li>
  </ol>
</details>

## agent

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-01-29**|**Is Conversational XAI All You Need? Human-AI Decision Making With a Conversational XAI Assistant**|Gaole He et.al.|[2501.17546](http://arxiv.org/abs/2501.17546)|**[link](https://github.com/delftcrowd/iui2025_convxai)**|**可解释的人工智能（XAI）方法被提出以帮助解读和理解人工智能系统如何做出特定预测。受先前关于对话用户界面工作的启发，我们认为将现有的XAI方法与对话用户界面相结合可以增加用户参与度并提高用户对AI系统的理解。在本文中，我们探讨了对话式XAI界面对于用户理解AI系统、信任以及依赖AI系统的影响。与XAI仪表板相比，我们发现对话式XAI界面能够更好地让用户理解AI系统，并且用户信任度更高。然而，无论是使用XAI仪表板还是对话式XAI界面的用户都表现出对AI系统的明显过度依赖。由大型语言模型（LLM）代理支持的增强对话进一步放大了这种过度依赖。根据我们的研究结果，我们认为这种过度依赖的潜在原因是伴随两种XAI界面出现的解释深度错觉。我们的研究结果对于设计有效的对话式XAI界面以促进适当的依赖性和改善人机协作具有重要意义。代码可以在https://github.com/delftcrowd/IUI2025_ConvXAI找到。**|
|**2025-01-28**|**A sketch of an AI control safety case**|Tomek Korbak et.al.|[2501.17315](http://arxiv.org/abs/2501.17315)|null|随着大型语言模型（LLM）代理造成伤害的能力日益增强，人工智能开发者可能会越来越多地依赖监控等控制措施来证明它们是安全的。我们概述了开发者如何构建一个“控制安全案例”，这是一个结构化的论证，表明模型无法通过颠覆控制措施来导致不可接受的结果。作为案例研究，我们概述了一个论点，即假设部署在一家AI公司内部的LLM代理不会泄露敏感信息。该概述依赖于从“控制评估”中获得的证据，在这种评估中，红队故意设计模型以在一个代表实际部署环境的环境中泄露数据。然后，安全案例基于几个主张：(1) 红队充分激发了模型泄露数据的能力；(2) 控制措施在部署时至少保持同样的有效性；以及 (3) 开发者保守地推断模型性能以预测部署时数据泄露的概率。这个安全案例概述是朝着更具体论证的一个步骤，这些论证可以用来表明一个危险能力的LLM代理在部署时是安全的。|
|**2025-01-28**|**Large Language Model Critics for Execution-Free Evaluation of Code Changes**|Aashish Yadavally et.al.|[2501.16655](http://arxiv.org/abs/2501.16655)|**[link](https://github.com/amazon-science/code-agent-eval)**|**大型语言模型（LLM）为通过多步骤的基于LLM的工作流自动化软件工程任务（如修复bug、添加功能等）提供了一种有前景的方法。然而，现有的评估此类工作流的指标，主要是构建状态偶尔加上日志分析，过于稀疏且有限，无法提供评估代码变更质量所需的信息。在这项工作中，我们设计了基于LLM的评价器，以导出针对仓库级别代码变更的结构良好且严格的中间/步骤级、无需执行的评估代理。重要的是，我们假设可以访问问题的黄金测试补丁（即参考感知），以此来评估生成补丁的语义和可执行性。利用黄金测试补丁作为参考，我们预测所有编辑位置的可执行性的F1得分为91.6%，通过聚合这些预测，我们可以预测SWE-bench中84.8%实例的构建状态。特别是，这种专注于执行的LLM评价器比其他无参考和参考感知的LLM评价器高出38.9%到72.5%。此外，我们展示了这种参考感知框架在比较不同代理工作流生成的补丁时的有用性。最后，我们将该项目开发的库开源，以便进一步用于其他代理工作流或其他基准测试。源代码可在https://github.com/amazon-science/code-agent-eval获取。**|
|**2025-01-27**|**Will Systems of LLM Agents Cooperate: An Investigation into a Social Dilemma**|Richard Willis et.al.|[2501.16173](http://arxiv.org/abs/2501.16173)|null|随着自主代理的日益普及，理解它们在策略互动中的集体行为变得至关重要。本研究探讨了大型语言模型（LLM）代理系统在社会困境中出现的合作倾向。与以往研究中LLM输出个体行动不同，我们促使最先进的LLM为迭代囚徒困境生成完整的策略。利用进化博弈论，我们模拟了具有不同策略倾向（攻击性、合作性或中立性）的代理人群体，并观察其进化动态。我们的发现揭示了不同的LLM表现出影响攻击性和合作性策略相对成功度的独特偏差。这项研究提供了关于部署基于LLM的自主代理系统的潜在长期行为的见解，并强调了仔细考虑其所处的战略环境的重要性。|
|**2025-01-27**|**LLM-attacker: Enhancing Closed-loop Adversarial Scenario Generation for Autonomous Driving with Large Language Models**|Yuewen Mei et.al.|[2501.15850](http://arxiv.org/abs/2501.15850)|null|确保和提高自动驾驶系统（ADS）的安全性，特别是在安全关键事件中，对于高度自动化车辆的部署至关重要。为了解决罕见事件的问题，开发了对抗性场景生成方法，其中通过操纵交通参与者的行为主动引发安全关键事件。然而，现有方法仍面临两个局限性。首先，对抗参与者的识别直接影响生成的有效性。然而，现实世界场景的复杂性，包括众多参与者和多样化的行为，使得识别变得困难。其次，生成的安全关键场景在持续改进ADS性能方面的潜力尚未得到充分探索。为解决这些问题，我们提出了LLM-attacker：一种利用大型语言模型（LLMs）的闭环对抗场景生成框架。具体而言，设计并协调多个LLM代理以识别最优攻击者。然后，优化这些攻击者的轨迹以生成对抗性场景。这些场景基于ADS的表现进行迭代细化，形成反馈循环以改进ADS。实验结果表明，LLM-attacker可以比其他方法生成更危险的场景，并且使用它训练的ADS碰撞率仅为正常场景训练的一半。这表明LLM-attacker能够测试和增强ADS的安全性和鲁棒性。视频演示请参见：https://drive.google.com/file/d/1Zv4V3iG7825oyiKbUwS2Y-rR0DQIE1ZA/view。|
|**2025-01-25**|**Are Human Interactions Replicable by Generative Agents? A Case Study on Pronoun Usage in Hierarchical Interactions**|Naihao Deng et.al.|[2501.15283](http://arxiv.org/abs/2501.15283)|null|随着大型语言模型（LLM）能力的不断提升，研究人员越来越多地将其用于社会模拟。在本文中，我们研究了LLM代理之间的互动是否类似于人类的互动。具体来说，我们关注领导者与非领导者之间代词使用的差异，考察这些模拟是否会引导LLM在互动过程中展现出类似人类的代词使用模式。我们的评估揭示了基于LLM的模拟与人类代词使用之间的显著差异，即使是在基于提示或专门设计的代理中，也未能展示出类似人类的代词使用模式。此外，我们还发现，即便LLM理解人类的代词使用模式，在实际互动过程中它们仍无法展现出来。本研究强调了基于LLM代理的社会模拟的局限性，并敦促从业者在决策过程中谨慎使用此类社会模拟。|
|**2025-01-24**|**Serving Long-Context LLMs at the Mobile Edge: Test-Time Reinforcement Learning-based Model Caching and Inference Offloading**|Minrui Xu et.al.|[2501.14205](http://arxiv.org/abs/2501.14205)|null|大型语言模型（LLM）可以在未见过的任务上执行零样本学习，并在复杂的推理任务上进行少样本学习。然而，资源有限的移动边缘网络难以支持在多轮用户交互过程中为LLM代理提供长上下文的LLM服务。与无状态计算卸载和静态服务卸载不同，在边缘计算中优化LLM服务具有挑战性，因为LLM从上下文中持续学习，这增加了准确性、延迟和资源消耗的动态变化。在本文中，我们提出了一种联合模型缓存和推理卸载框架，该框架利用测试时深度强化学习（T2DRL）来优化长上下文LLM服务的部署和执行策略。在此框架下，我们分析了性能收敛并设计了一个考虑LLM中上下文窗口利用率的优化问题。此外，T2DRL算法能够在训练阶段和测试阶段都进行学习，以主动管理缓存模型和服务请求，并适应执行过程中的上下文变化和使用模式。为了进一步提高资源分配效率，我们提出了一种双重荷兰拍卖（DDA）机制，该机制能够动态匹配供需，同时最大化社会福利。最后，实验结果表明，与基线相比，T2DRL算法至少可以降低30%的系统成本，同时保证LLM代理在实际感知和推理任务中的性能。|
|**2025-01-24**|**AI Chatbots as Professional Service Agents: Developing a Professional Identity**|Wenwen Li et.al.|[2501.14179](http://arxiv.org/abs/2501.14179)|null|随着大型语言模型（LLM）应用的迅速扩展，基于LLM的AI聊天机器人从仅仅作为通用查询工具的角色正在向担任专业服务代理的角色转变。然而，当前的研究往往忽视了专业服务代理的一个关键方面：即以与其职业身份一致的方式进行沟通。这一点在医疗保健领域尤为重要，在该领域中，与患者的有效沟通对于实现专业目标（如通过鼓励健康行为来促进患者福祉）至关重要。为了解决这一问题，我们提出了LAPI（具有专业身份的LLM基础代理），这是一种针对医疗服务中的问答服务设计的专业服务代理的新框架，确保其与特定的专业身份相一致。我们的方法包括一个理论指导的任务规划过程，将复杂的专业任务分解成与专业目标对齐的可管理子任务，以及一种旨在生成专业且伦理上正确的、不确定性低的回答的实用熵方法。在各种LLM上的实验表明，所提出的方法在流畅性、自然度、同情心、以患者为中心及ROUGE-L得分等关键指标上优于基线方法，包括少量示例提示和思维链提示。此外，消融研究强调了每个组件对整个方法有效性的贡献。|
|**2025-01-23**|**AgentRec: Agent Recommendation Using Sentence Embeddings Aligned to Human Feedback**|Joshua Park et.al.|[2501.13333](http://arxiv.org/abs/2501.13333)|**[link](https://github.com/joshprk/agentrec)**|**多智能体系统必须决定哪个智能体最适合执行给定的任务。我们提出了一种新的架构，通过扩展Sentence-BERT（SBERT）编码器模型来推荐在自然语言提示下应由哪个大语言模型智能体执行任务。在测试数据上，我们能够达到92.2%的top-1准确率，并且每次分类耗时不到300毫秒。与传统的分类方法相比，我们的架构计算成本低廉、适应新类别、可解释性强，并且可以通过强化学习使用任意度量进行控制。通过将自然语言提示编码为句子嵌入，我们的模型捕捉了推荐智能体相关的语义内容。然后通过微调最小化属于同一智能体的句子嵌入之间的距离，并通过从人类反馈中进行强化学习使其与人类价值观对齐。这使得可以根据最近邻测量嵌入之间的余弦相似性来对自然语言提示进行分类。这项工作是通过生成一个用于智能体推荐的合成数据集实现的，我们已将该数据集和AgentRec推荐系统的代码开源至https://github.com/joshprk/agentrec。**|
|**2025-01-23**|**Hypothesis Generation for Materials Discovery and Design Using Goal-Driven and Constraint-Guided LLM Agents**|Shrinidhi Kumbhar et.al.|[2501.13299](http://arxiv.org/abs/2501.13299)|null|材料的发现与设计对于通过开发特定应用材料来推动各行各业技术进步至关重要。近期研究利用大型语言模型（LLM）加速这一进程。我们探讨了LLM生成可行假设的潜力，这些假设一旦得到验证，可以加快材料发现的速度。与材料科学专家合作，我们从最近的期刊出版物中整理了一个新颖的数据集，其中包含实现实际应用目标的真实世界目标、约束条件和方法。使用该数据集，我们测试了基于LLM的代理生成在特定约束条件下达成给定目标的假设的能力。为了评估这些假设的相关性和质量，我们提出了一种新的可扩展评估指标，模拟材料科学家用来批判性评估假设的过程。我们整理的数据集、提出的方法和评估框架旨在促进未来利用LLM加速材料发现与设计的研究。|
|**2025-01-21**|**LLM-Agents Driven Automated Simulation Testing and Analysis of small Uncrewed Aerial Systems**|Venkata Sai Aswath Duvvuru et.al.|[2501.11864](http://arxiv.org/abs/2501.11864)|null|
|**2025-01-20**|**Agent-R: Training Language Model Agents to Reflect via Iterative Self-Training**|Siyu Yuan et.al.|[2501.11425](http://arxiv.org/abs/2501.11425)|**[link](https://github.com/bytedance/agent-r)**|
|**2025-01-20**|**Towards Advancing Code Generation with Large Language Models: A Research Roadmap**|Haolin Jin et.al.|[2501.11354](http://arxiv.org/abs/2501.11354)|null|
|**2025-01-20**|**Large Language Model Agents for Radio Map Generation and Wireless Network Planning**|Hongye Quan et.al.|[2501.11283](http://arxiv.org/abs/2501.11283)|null|
|**2025-01-20**|**PlotEdit: Natural Language-Driven Accessible Chart Editing in PDFs via Multimodal LLM Agents**|Kanika Goswami et.al.|[2501.11233](http://arxiv.org/abs/2501.11233)|null|
|**2025-01-18**|**Learn-by-interact: A Data-Centric Framework for Self-Adaptive Agents in Realistic Environments**|Hongjin Su et.al.|[2501.10893](http://arxiv.org/abs/2501.10893)|null|
|**2025-01-18**|**ML-SceGen: A Multi-level Scenario Generation Framework**|Yicheng Xiao et.al.|[2501.10782](http://arxiv.org/abs/2501.10782)|null|
|**2025-01-17**|**PaSa: An LLM Agent for Comprehensive Academic Paper Search**|Yichen He et.al.|[2501.10120](http://arxiv.org/abs/2501.10120)|**[link](https://github.com/bytedance/pasa)**|
|**2025-01-17**|**A Survey on LLM Test-Time Compute via Search: Tasks, LLM Profiling, Search Algorithms, and Relevant Frameworks**|Xinzhe Li et.al.|[2501.10069](http://arxiv.org/abs/2501.10069)|null|
|**2025-01-15**|**Leveraging LLM Agents for Translating Network Configurations**|Yunze Wei et.al.|[2501.08760](http://arxiv.org/abs/2501.08760)|null|
|**2025-01-14**|**Addressing the sustainable AI trilemma: a case study on LLM agents and RAG**|Hui Wu et.al.|[2501.08262](http://arxiv.org/abs/2501.08262)|null|
|**2025-01-14**|**Flow: A Modular Approach to Automated Agentic Workflow Generation**|Boye Niu et.al.|[2501.07834](http://arxiv.org/abs/2501.07834)|null|
|**2025-01-13**|**SST-EM: Advanced Metrics for Evaluating Semantic, Spatial and Temporal Aspects in Video Editing**|Varun Biyyala et.al.|[2501.07554](http://arxiv.org/abs/2501.07554)|**[link](https://github.com/custommetrics-sst/sst_customevaluationmetrics)**|
|**2025-01-13**|**Lifelong Learning of Large Language Model based Agents: A Roadmap**|Junhao Zheng et.al.|[2501.07278](http://arxiv.org/abs/2501.07278)|**[link](https://github.com/qianlima-lab/awesome-lifelong-llm-agent)**|
|**2025-01-12**|**AIOpsLab: A Holistic Framework to Evaluate AI Agents for Enabling Autonomous Clouds**|Yinfang Chen et.al.|[2501.06706](http://arxiv.org/abs/2501.06706)|null|
|**2025-01-12**|**DVM: Towards Controllable LLM Agents in Social Deduction Games**|Zheng Zhang et.al.|[2501.06695](http://arxiv.org/abs/2501.06695)|null|
|**2025-01-10**|**OpenFOAMGPT: a RAG-Augmented LLM Agent for OpenFOAM-Based Computational Fluid Dynamics**|Sandeep Pandey et.al.|[2501.06327](http://arxiv.org/abs/2501.06327)|null|
|**2025-01-10**|**Multi-Agent Collaboration Mechanisms: A Survey of LLMs**|Khanh-Tung Tran et.al.|[2501.06322](http://arxiv.org/abs/2501.06322)|null|
|**2025-01-09**|**Emergence of human-like polarization among large language model agents**|Jinghua Piao et.al.|[2501.05171](http://arxiv.org/abs/2501.05171)|null|
|**2025-01-09**|**LearningFlow: Automated Policy Learning Workflow for Urban Driving with Large Language Models**|Zengqi Peng et.al.|[2501.05057](http://arxiv.org/abs/2501.05057)|null|
|**2025-01-08**|**Agent Laboratory: Using LLM Agents as Research Assistants**|Samuel Schmidgall et.al.|[2501.04227](http://arxiv.org/abs/2501.04227)|null|
|**2025-01-02**|**Toward Inclusive Educational AI: Auditing Frontier LLMs through a Multiplexity Lens**|Abdullah Mushtaq et.al.|[2501.03259](http://arxiv.org/abs/2501.03259)|null|
|**2025-01-10**|**MoColl: Agent-Based Specific and General Model Collaboration for Image Captioning**|Pu Yang et.al.|[2501.01834](http://arxiv.org/abs/2501.01834)|null|
|**2025-01-03**|**SDPO: Segment-Level Direct Preference Optimization for Social Agents**|Aobo Kong et.al.|[2501.01821](http://arxiv.org/abs/2501.01821)|**[link](https://github.com/alibabaresearch/damo-convai)**|
|**2025-01-03**|**AgentRefine: Enhancing Agent Generalization through Refinement Tuning**|Dayuan Fu et.al.|[2501.01702](http://arxiv.org/abs/2501.01702)|null|
|**2025-01-02**|**BoxingGym: Benchmarking Progress in Automated Experimental Design and Model Discovery**|Kanishk Gandhi et.al.|[2501.01540](http://arxiv.org/abs/2501.01540)|**[link](https://github.com/kanishkg/boxing-gym)**|
|**2025-01-02**|**Harnessing Multi-Agent LLMs for Complex Engineering Problem-Solving: A Framework for Senior Design Projects**|Abdullah Mushtaq et.al.|[2501.01205](http://arxiv.org/abs/2501.01205)|null|
|**2025-01-01**|**Agentic Systems: A Guide to Transforming Industries with Vertical AI Agents**|Fouad Bousetouane et.al.|[2501.00881](http://arxiv.org/abs/2501.00881)|null|
|**2024-12-31**|**Enabling New HDLs with Agents**|Mark Zakharov et.al.|[2501.00642](http://arxiv.org/abs/2501.00642)|null|
|**2024-12-31**|**Embodied VideoAgent: Persistent Memory from Egocentric Videos and Embodied Sensors Enables Dynamic Scene Understanding**|Yue Fan et.al.|[2501.00358](http://arxiv.org/abs/2501.00358)|null|
|**2024-12-31**|**MAIN-RAG: Multi-Agent Filtering Retrieval-Augmented Generation**|Chia-Yuan Chang et.al.|[2501.00332](http://arxiv.org/abs/2501.00332)|null|
|**2024-12-30**|**AI Agent for Education: von Neumann Multi-Agent System Framework**|Yuan-Hao Jiang et.al.|[2501.00083](http://arxiv.org/abs/2501.00083)|null|
|**2024-12-30**|**Aviary: training language agents on challenging scientific tasks**|Siddharth Narayanan et.al.|[2412.21154](http://arxiv.org/abs/2412.21154)|null|
|**2024-12-30**|**Exploring and Controlling Diversity in LLM-Agent Conversation**|KuanChao Chu et.al.|[2412.21102](http://arxiv.org/abs/2412.21102)|null|
|**2024-12-30**|**Plancraft: an evaluation dataset for planning with LLM agents**|Gautier Dagan et.al.|[2412.21033](http://arxiv.org/abs/2412.21033)|**[link](https://github.com/gautierdag/plancraft)**|
|**2024-12-29**|**Planning, Living and Judging: A Multi-agent LLM-based Framework for Cyclical Urban Planning**|Hang Ni et.al.|[2412.20505](http://arxiv.org/abs/2412.20505)|null|
|**2024-12-28**|**FaGeL: Fabric LLMs Agent empowered Embodied Intelligence Evolution with Autonomous Human-Machine Collaboration**|Jia Liu et.al.|[2412.20297](http://arxiv.org/abs/2412.20297)|null|
|**2024-12-28**|**OneKE: A Dockerized Schema-Guided LLM Agent-based Knowledge Extraction System**|Yujie Luo et.al.|[2412.20005](http://arxiv.org/abs/2412.20005)|**[link](https://github.com/zjunlp/oneke)**|
|**2024-12-24**|**Explainable Multi-Modal Data Exploration in Natural Language via LLM Agent**|Farhad Nooralahzadeh et.al.|[2412.18428](http://arxiv.org/abs/2412.18428)|**[link](https://github.com/yizhang-unifr/xmode)**|
|**2024-12-25**|**Defining and Detecting the Defects of the Large Language Model-based Autonomous Agents**|Kaiwen Ning et.al.|[2412.18371](http://arxiv.org/abs/2412.18371)|**[link](https://github.com/KevinHeiwa/Agentable)**|
|**2024-12-24**|**Multi-Agents Based on Large Language Models for Knowledge-based Visual Question Answering**|Zhongjian Hu et.al.|[2412.18351](http://arxiv.org/abs/2412.18351)|null|
|**2024-12-24**|**INVESTORBENCH: A Benchmark for Financial Decision-Making Tasks with LLM-based Agent**|Haohang Li et.al.|[2412.18174](http://arxiv.org/abs/2412.18174)|null|
|**2024-12-23**|**Large Language Model Safety: A Holistic Survey**|Dan Shi et.al.|[2412.17686](http://arxiv.org/abs/2412.17686)|**[link](https://github.com/tjunlp-lab/awesome-llm-safety-papers)**|
|**2024-12-23**|**LegalAgentBench: Evaluating LLM Agents in Legal Domain**|Haitao Li et.al.|[2412.17259](http://arxiv.org/abs/2412.17259)|**[link](https://github.com/cshaitao/legalagentbench)**|
|**2024-12-22**|**LLM Agent for Fire Dynamics Simulations**|Leidong Xu et.al.|[2412.17146](http://arxiv.org/abs/2412.17146)|null|
|**2024-12-21**|**The Task Shield: Enforcing Task Alignment to Defend Against Indirect Prompt Injection in LLM Agents**|Feiran Jia et.al.|[2412.16682](http://arxiv.org/abs/2412.16682)|null|
|**2024-12-19**|**Tree-of-Code: A Tree-Structured Exploring Framework for End-to-End Code Generation and Execution in Complex Task Handling**|Ziyi Ni et.al.|[2412.15305](http://arxiv.org/abs/2412.15305)|null|
|**2024-12-17**|**Memory-Augmented Agent Training for Business Document Understanding**|Jiale Liu et.al.|[2412.15274](http://arxiv.org/abs/2412.15274)|null|
|**2024-12-17**|**On the Structural Memory of LLM Agents**|Ruihong Zeng et.al.|[2412.15266](http://arxiv.org/abs/2412.15266)|**[link](https://github.com/zengrh3/StructuralMemory)**|
|**2024-12-19**|**On Verbalized Confidence Scores for LLMs**|Daniel Yang et.al.|[2412.14737](http://arxiv.org/abs/2412.14737)|**[link](https://github.com/danielyxyang/llm-verbalized-uq)**|
|**2024-12-19**|**Agent-SafetyBench: Evaluating the Safety of LLM Agents**|Zhexin Zhang et.al.|[2412.14470](http://arxiv.org/abs/2412.14470)|**[link](https://github.com/thu-coai/agent-safetybench)**|
|**2024-12-18**|**A Survey on Large Language Model-based Agents for Statistics and Data Science**|Maojun Sun et.al.|[2412.14222](http://arxiv.org/abs/2412.14222)|null|
|**2024-12-18**|**Tree-of-Code: A Hybrid Approach for Robust Complex Task Planning and Execution**|Ziyi Ni et.al.|[2412.14212](http://arxiv.org/abs/2412.14212)|null|
|**2024-12-18**|**TheAgentCompany: Benchmarking LLM Agents on Consequential Real World Tasks**|Frank F. Xu et.al.|[2412.14161](http://arxiv.org/abs/2412.14161)|**[link](https://github.com/theagentcompany/experiments)**|
|**2024-12-18**|**Exploring Multi-Modal Integration with Tool-Augmented LLM Agents for Precise Causal Discovery**|ChengAo Shen et.al.|[2412.13667](http://arxiv.org/abs/2412.13667)|null|
|**2024-12-18**|**SafeAgentBench: A Benchmark for Safe Task Planning of Embodied LLM Agents**|Sheng Yin et.al.|[2412.13178](http://arxiv.org/abs/2412.13178)|**[link](https://github.com/shengyin1224/safeagentbench)**|
|**2024-12-17**|**RareAgents: Autonomous Multi-disciplinary Team for Rare Disease Diagnosis and Treatment**|Xuanzhong Chen et.al.|[2412.12475](http://arxiv.org/abs/2412.12475)|null|
|**2024-12-16**|**Codenames as a Benchmark for Large Language Models**|Matthew Stephenson et.al.|[2412.11373](http://arxiv.org/abs/2412.11373)|null|
|**2024-12-14**|**Towards Action Hijacking of Large Language Model-based Agent**|Yuyang Zhang et.al.|[2412.10807](http://arxiv.org/abs/2412.10807)|null|
|**2024-12-13**|**Cultural Evolution of Cooperation among LLM Agents**|Aron Vallinder et.al.|[2412.10270](http://arxiv.org/abs/2412.10270)|null|
|**2024-12-13**|**ROUTE: Robust Multitask Tuning and Collaboration for Text-to-SQL**|Yang Qin et.al.|[2412.10138](http://arxiv.org/abs/2412.10138)|**[link](https://github.com/alibaba/route)**|
|**2024-12-13**|**You Name It, I Run It: An LLM Agent to Execute Tests of Arbitrary Projects**|Islem Bouzenia et.al.|[2412.10133](http://arxiv.org/abs/2412.10133)|null|
|**2024-12-12**|**Can Modern LLMs Act as Agent Cores in Radiology~Environments?**|Qiaoyu Zheng et.al.|[2412.09529](http://arxiv.org/abs/2412.09529)|**[link](https://github.com/magic-ai4med/radabench)**|
|**2024-12-11**|**ChatDyn: Language-Driven Multi-Actor Dynamics Generation in Street Scenes**|Yuxi Wei et.al.|[2412.08685](http://arxiv.org/abs/2412.08685)|null|
|**2024-12-11**|**TapeAgents: a Holistic Framework for Agent Development and Optimization**|Dzmitry Bahdanau et.al.|[2412.08445](http://arxiv.org/abs/2412.08445)|null|
|**2024-12-11**|**Federated In-Context LLM Agent Learning**|Panlong Wu et.al.|[2412.08054](http://arxiv.org/abs/2412.08054)|null|
|**2024-12-11**|**MAGIC: Mastering Physical Adversarial Generation in Context through Collaborative LLM Agents**|Yun Xing et.al.|[2412.08014](http://arxiv.org/abs/2412.08014)|null|
|**2024-12-10**|**Agents for self-driving laboratories applied to quantum computing**|Shuxiang Cao et.al.|[2412.07978](http://arxiv.org/abs/2412.07978)|null|
|**2024-12-10**|**MAGE: A Multi-Agent Engine for Automated RTL Code Generation**|Yujie Zhao et.al.|[2412.07822](http://arxiv.org/abs/2412.07822)|**[link](https://github.com/stable-lab/MAGE-A-Multi-Agent-Engine-for-Automated-RTL-Code-Generation)**|
|**2024-12-11**|**Searching for Structure: Investigating Emergent Communication with Large Language Models**|Tom Kouwenhoven et.al.|[2412.07646](http://arxiv.org/abs/2412.07646)|null|
|**2024-12-06**|**Enhancing LLMs for Impression Generation in Radiology Reports through a Multi-Agent System**|Fang Zeng et.al.|[2412.06828](http://arxiv.org/abs/2412.06828)|null|
|**2024-12-09**|**AutoDCWorkflow: LLM-based Data Cleaning Workflow Auto-Generation and Benchmark**|Lan Li et.al.|[2412.06724](http://arxiv.org/abs/2412.06724)|**[link](https://github.com/LanLi2017/LLM4DC)**|
|**2024-12-09**|**Toward LLM-Agent-Based Modeling of Transportation Systems: A Conceptual Framework**|Tianming Liu et.al.|[2412.06681](http://arxiv.org/abs/2412.06681)|null|
|**2024-12-09**|**Simulating Human-like Daily Activities with Desire-driven Autonomy**|Yiding Wang et.al.|[2412.06435](http://arxiv.org/abs/2412.06435)|null|
|**2024-12-09**|**StarWhisper Telescope: Agent-Based Observation Assistant System to Approach AI Astrophysicist**|Cunshi Wang et.al.|[2412.06412](http://arxiv.org/abs/2412.06412)|null|
|**2024-12-09**|**Beyond pip install: Evaluating LLM Agents for the Automated Installation of Python Projects**|Louis Milliken et.al.|[2412.06294](http://arxiv.org/abs/2412.06294)|**[link](https://github.com/coinse/installamatic)**|
|**2024-12-08**|**Cooperative SQL Generation for Segmented Databases By Using Multi-functional LLM Agents**|Zhiguang Wu et.al.|[2412.05850](http://arxiv.org/abs/2412.05850)|null|
|**2024-12-06**|**Sense and Sensitivity: Evaluating the simulation of social dynamics via Large Language Models**|Da Ju et.al.|[2412.05093](http://arxiv.org/abs/2412.05093)|null|
|**2024-12-05**|**Practical Considerations for Agentic LLM Systems**|Chris Sypherd et.al.|[2412.04093](http://arxiv.org/abs/2412.04093)|null|
|**2024-12-05**|**LossAgent: Towards Any Optimization Objectives for Image Processing with LLM Agents**|Bingchen Li et.al.|[2412.04090](http://arxiv.org/abs/2412.04090)|null|
|**2024-12-05**|**MISR: Measuring Instrumental Self-Reasoning in Frontier Models**|Kai Fronsdal et.al.|[2412.03904](http://arxiv.org/abs/2412.03904)|**[link](https://github.com/kaifronsdal/self-reasoning-evals)**|
|**2024-12-05**|**Educational-Psychological Dialogue Robot Based on Multi-Agent Collaboration**|Shiwen Ni et.al.|[2412.03847](http://arxiv.org/abs/2412.03847)|null|
|**2024-12-04**|**From Individual to Society: A Survey on Social Simulation Driven by Large Language Model-based Agents**|Xinyi Mou et.al.|[2412.03563](http://arxiv.org/abs/2412.03563)|**[link](https://github.com/fudandisc/socialagent)**|
|**2024-12-03**|**Hacking CTFs with Plain Agents**|Rustem Turtayev et.al.|[2412.02776](http://arxiv.org/abs/2412.02776)|**[link](https://github.com/palisaderesearch/intercode)**|
|**2024-12-04**|**DataLab: A Unified Platform for LLM-Powered Business Intelligence**|Luoxuan Weng et.al.|[2412.02205](http://arxiv.org/abs/2412.02205)|null|
|**2024-12-02**|**HackSynth: LLM Agent and Evaluation Framework for Autonomous Penetration Testing**|Lajos Muzsai et.al.|[2412.01778](http://arxiv.org/abs/2412.01778)|**[link](https://github.com/aielte-research/HackSynth)**|
|**2024-12-02**|**Medchain: Bridging the Gap Between LLM Agents and Clinical Practice through Interactive Sequential Benchmarking**|Jie Liu et.al.|[2412.01605](http://arxiv.org/abs/2412.01605)|null|
|**2024-12-02**|**Can Large Language Models Serve as Evaluators for Code Summarization?**|Yang Wu et.al.|[2412.01333](http://arxiv.org/abs/2412.01333)|**[link](https://github.com/CGCL-codes/naturalcc)**|
|**2024-12-02**|**RL2: Reinforce Large Language Model to Assist Safe Reinforcement Learning for Energy Management of Active Distribution Networks**|Xu Yang et.al.|[2412.01303](http://arxiv.org/abs/2412.01303)|null|
|**2024-12-02**|**SAUP: Situation Awareness Uncertainty Propagation on LLM Agent**|Qiwei Zhao et.al.|[2412.01033](http://arxiv.org/abs/2412.01033)|null|
|**2024-11-28**|**SceneTAP: Scene-Coherent Typographic Adversarial Planner against Vision-Language Models in Real-World Environments**|Yue Cao et.al.|[2412.00114](http://arxiv.org/abs/2412.00114)|null|
|**2024-11-29**|**Training Agents with Weakly Supervised Feedback from Large Language Models**|Dihong Gong et.al.|[2411.19547](http://arxiv.org/abs/2411.19547)|null|
|**2024-11-28**|**Using a Feedback Loop for LLM-based Infrastructure as Code Generation**|Mayur Amarnath Palavalli et.al.|[2411.19043](http://arxiv.org/abs/2411.19043)|**[link](https://github.com/Mayur-Palavalli/LLM-IaC-generation)**|
|**2024-12-02**|**MATATA: a weak-supervised MAthematical Tool-Assisted reasoning for Tabular Applications**|Vishnou Vinayagame et.al.|[2411.18915](http://arxiv.org/abs/2411.18915)|null|
|**2024-11-28**|**Wearable intelligent throat enables natural speech in stroke patients with dysarthria**|Chenyu Tang et.al.|[2411.18266](http://arxiv.org/abs/2411.18266)|null|
|**2024-11-26**|**MALMM: Multi-Agent Large Language Models for Zero-Shot Robotics Manipulation**|Harsh Singh et.al.|[2411.17636](http://arxiv.org/abs/2411.17636)|null|
|**2024-11-26**|**LLM-Based Offline Learning for Embodied Agents via Consistency-Guided Reward Ensemble**|Yujeong Lee et.al.|[2411.17135](http://arxiv.org/abs/2411.17135)|null|
|**2024-11-23**|**Two Heads Are Better Than One: Collaborative LLM Embodied Agents for Human-Robot Interaction**|Mitchell Rosser et.al.|[2411.16723](http://arxiv.org/abs/2411.16723)|null|
|**2024-11-25**|**Agent-Based Modelling Meets Generative AI in Social Network Simulations**|Antonino Ferraro et.al.|[2411.16031](http://arxiv.org/abs/2411.16031)|null|
|**2024-11-24**|**From Laws to Motivation: Guiding Exploration through Law-Based Reasoning and Rewards**|Ziyu Chen et.al.|[2411.15891](http://arxiv.org/abs/2411.15891)|null|
|**2024-11-23**|**The Decoy Dilemma in Online Medical Information Evaluation: A Comparative Study of Credibility Assessments by LLM and Human Judges**|Jiqun Liu et.al.|[2411.15396](http://arxiv.org/abs/2411.15396)|null|
|**2024-11-27**|**XGrammar: Flexible and Efficient Structured Generation Engine for Large Language Models**|Yixin Dong et.al.|[2411.15100](http://arxiv.org/abs/2411.15100)|null|
|**2024-11-22**|**ScribeAgent: Towards Specialized Web Agents Using Production-Scale Workflow Data**|Junhong Shen et.al.|[2411.15004](http://arxiv.org/abs/2411.15004)|**[link](https://github.com/colonylabs/ScribeAgent)**|
|**2024-11-21**|**Star-Agents: Automatic Data Optimization with LLM Agents for Instruction Tuning**|Hang Zhou et.al.|[2411.14497](http://arxiv.org/abs/2411.14497)|**[link](https://github.com/CANGLETIAN/Star-Agents)**|
|**2024-11-20**|**Mediating Modes of Thought: LLM's for design scripting**|Moritz Rietschel et.al.|[2411.14485](http://arxiv.org/abs/2411.14485)|null|
|**2024-11-21**|**Physics-Informed LLM-Agent for Automated Modulation Design in Power Electronics Systems**|Junhua Liu et.al.|[2411.14214](http://arxiv.org/abs/2411.14214)|null|
|**2024-11-21**|**Multi-LLM-Agent Systems: Techniques and Business Perspectives**|Yingxuan Yang et.al.|[2411.14033](http://arxiv.org/abs/2411.14033)|null|
|**2024-11-21**|**Towards Full Delegation: Designing Ideal Agentic Behaviors for Travel Planning**|Song Jiang et.al.|[2411.13904](http://arxiv.org/abs/2411.13904)|null|
|**2024-11-21**|**Next-Generation Phishing: How LLM Agents Empower Cyber Attackers**|Khalifa Afane et.al.|[2411.13874](http://arxiv.org/abs/2411.13874)|null|
|**2024-11-21**|**An Evaluation-Driven Approach to Designing LLM Agents: Process and Architecture**|Boming Xia et.al.|[2411.13768](http://arxiv.org/abs/2411.13768)|null|
|**2024-11-20**|**Metacognition for Unknown Situations and Environments (MUSE)**|Rodolfo Valiente et.al.|[2411.13537](http://arxiv.org/abs/2411.13537)|null|
|**2024-11-19**|**Human-In-the-Loop Software Development Agents**|Wannita Takerngsaksiri et.al.|[2411.12924](http://arxiv.org/abs/2411.12924)|null|
|**2024-11-19**|**Probing the Capacity of Language Model Agents to Operationalize Disparate Experiential Context Despite Distraction**|Sonny George et.al.|[2411.12828](http://arxiv.org/abs/2411.12828)|**[link](https://github.com/sonnygeorge/oedd)**|
|**2024-11-19**|**A More Advanced Group Polarization Measurement Approach Based on LLM-Based Agents and Graphs**|Zixin Liu et.al.|[2411.12196](http://arxiv.org/abs/2411.12196)|null|
|**2024-11-19**|**Generative World Explorer**|Taiming Lu et.al.|[2411.11844](http://arxiv.org/abs/2411.11844)|null|
|**2024-11-18**|**LLM-IE: A Python Package for Generative Information Extraction with Large Language Models**|Enshuo Hsu et.al.|[2411.11779](http://arxiv.org/abs/2411.11779)|null|
|**2024-11-18**|**OASIS: Open Agents Social Interaction Simulations on One Million Agents**|Ziyi Yang et.al.|[2411.11581](http://arxiv.org/abs/2411.11581)|**[link](https://github.com/camel-ai/oasis)**|
|**2024-11-16**|**IntentGPT: Few-shot Intent Discovery with Large Language Models**|Juan A. Rodriguez et.al.|[2411.10670](http://arxiv.org/abs/2411.10670)|null|
|**2024-11-15**|**Evaluating Creativity and Deception in Large Language Models: A Simulation Framework for Multi-Agent Balderdash**|Parsa Hejabi et.al.|[2411.10422](http://arxiv.org/abs/2411.10422)|**[link](https://github.com/parsahejabi/simulation-framework-for-multi-agent-balderdash)**|
|**2024-11-15**|**An Empirical Study on LLM-based Agents for Automated Bug Fixing**|Xiangxin Meng et.al.|[2411.10213](http://arxiv.org/abs/2411.10213)|null|
|**2024-11-15**|**Agentic LLMs in the Supply Chain: Towards Autonomous Multi-Agent Consensus-Seeking**|Valeria Jannelli et.al.|[2411.10184](http://arxiv.org/abs/2411.10184)|null|
|**2024-11-14**|**Navigating the Risks: A Survey of Security, Privacy, and Ethics Threats in LLM-Based Agents**|Yuyou Gan et.al.|[2411.09523](http://arxiv.org/abs/2411.09523)|null|
|**2024-11-18**|**Towards Evaluating Large Language Models for Graph Query Generation**|Siraj Munir et.al.|[2411.08449](http://arxiv.org/abs/2411.08449)|null|
|**2024-11-13**|**Collaborative Participatory Research with LLM Agents in South Asia: An Empirically-Grounded Methodological Initiative and Agenda from Field Evidence in Sri Lanka**|Xinjie Zhao et.al.|[2411.08294](http://arxiv.org/abs/2411.08294)|null|
|**2024-11-11**|**Tooling or Not Tooling? The Impact of Tools on Language Agents for Chemistry Problem Solving**|Botao Yu et.al.|[2411.07228](http://arxiv.org/abs/2411.07228)|null|
|**2024-11-10**|**Hermes: A Large Language Model Framework on the Journey to Autonomous Networks**|Fadhel Ayed et.al.|[2411.06490](http://arxiv.org/abs/2411.06490)|null|
|**2024-11-12**|**Game-theoretic LLM: Agent Workflow for Negotiation Games**|Wenyue Hua et.al.|[2411.05990](http://arxiv.org/abs/2411.05990)|**[link](https://github.com/wenyueh/game_theory)**|
|**2024-11-08**|**LightVA: Lightweight Visual Analytics with LLM Agent-Based Task Planning and Execution**|Yuheng Zhao et.al.|[2411.05651](http://arxiv.org/abs/2411.05651)|null|
|**2024-11-08**|**Enhancing Cluster Resilience: LLM-agent Based Autonomous Intelligent Cluster Diagnosis System and Evaluation Framework**|Honghao Shi et.al.|[2411.05349](http://arxiv.org/abs/2411.05349)|null|
|**2024-11-07**|**Alopex: A Computational Framework for Enabling On-Device Function Calls with LLMs**|Yide Ran et.al.|[2411.05209](http://arxiv.org/abs/2411.05209)|null|
|**2024-11-07**|**PentestAgent: Incorporating LLM Agents to Automated Penetration Testing**|Xiangmin Shen et.al.|[2411.05185](http://arxiv.org/abs/2411.05185)|null|
|**2024-11-12**|**CodeTree: Agent-guided Tree Search for Code Generation with Large Language Models**|Jierui Li et.al.|[2411.04329](http://arxiv.org/abs/2411.04329)|null|
|**2024-11-06**|**From Novice to Expert: LLM Agent Policy Optimization via Step-wise Reinforcement Learning**|Zhirui Deng et.al.|[2411.03817](http://arxiv.org/abs/2411.03817)|null|
|**2024-11-05**|**AI Metropolis: Scaling Large Language Model-based Multi-Agent Simulation with Out-of-order Execution**|Zhiqiang Xie et.al.|[2411.03519](http://arxiv.org/abs/2411.03519)|null|
|**2024-11-03**|**Fixing Security Vulnerabilities with AI in OSS-Fuzz**|Yuntong Zhang et.al.|[2411.03346](http://arxiv.org/abs/2411.03346)|null|
|**2024-11-05**|**SMoA: Improving Multi-agent Large Language Models with Sparse Mixture-of-Agents**|Dawei Li et.al.|[2411.03284](http://arxiv.org/abs/2411.03284)|**[link](https://github.com/david-li0406/smoa)**|
|**2024-11-05**|**Spontaneous Emergence of Agent Individuality through Social Interactions in LLM-Based Communities**|Ryosuke Takata et.al.|[2411.03252](http://arxiv.org/abs/2411.03252)|null|
|**2024-11-04**|**CRMArena: Understanding the Capacity of LLM Agents to Perform Professional CRM Tasks in Realistic Environments**|Kung-Hsiang Huang et.al.|[2411.02305](http://arxiv.org/abs/2411.02305)|**[link](https://github.com/salesforceairesearch/crmarena)**|
|**2024-11-04**|**DynaSaur: Large Language Agents Beyond Predefined Actions**|Dang Nguyen et.al.|[2411.01747](http://arxiv.org/abs/2411.01747)|null|
|**2024-11-03**|**EcoAct: Economic Agent Determines When to Register What Action**|Shaokun Zhang et.al.|[2411.01643](http://arxiv.org/abs/2411.01643)|null|
|**2024-11-02**|**AutoPT: How Far Are We from the End2End Automated Web Penetration Testing?**|Benlong Wu et.al.|[2411.01236](http://arxiv.org/abs/2411.01236)|**[link](https://github.com/Dizzy-K/AutoPT)**|
|**2024-11-02**|**A Large-scale Time-aware Agents Simulation for Influencer Selection in Digital Advertising Campaigns**|Xiaoqing Zhang et.al.|[2411.01143](http://arxiv.org/abs/2411.01143)|null|
|**2024-05-16**|**When LLMs step into the 3D World: A Survey and Meta-Analysis of 3D Tasks via Multi-modal Large Language Models**|Xianzheng Ma et.al.|[2405.10255](http://arxiv.org/abs/2405.10255)|**[link](https://github.com/activevisionlab/awesome-llm-3d)**|

<p align=right>(<a href=#updated-on-20250131>back to top</a>)</p>

## llm

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-01-29**|**Learning Beyond the Surface: How Far Can Continual Pre-Training with LoRA Enhance LLMs' Domain-Specific Insight Learning?**|Pouya Pezeshkpour et.al.|[2501.17840](http://arxiv.org/abs/2501.17840)|**[link](https://github.com/megagonlabs/insight_miner)**|**大型语言模型（LLMs）在各种任务中表现出色，但它们从特定领域数据集中提取和内化更深层次见解的能力仍有待探索。在这项研究中，我们探讨了持续预训练如何增强LLMs在三种不同形式的见解学习中的能力：陈述性、统计性和概率性见解。我们专注于医学和金融这两个关键领域，使用LoRA对两个现有数据集上的LLMs进行训练。为了评估每种类型的见解，我们创建了基准来衡量持续预训练在帮助模型超越表面知识方面的效果。我们还评估了文档修改对捕捉见解的影响。结果显示，虽然在原始文档上进行持续预训练的效果有限，但通过修改文档仅保留关键信息，可以显著提高LLMs的学习见解能力。**|
|**2025-01-29**|**BreezyVoice: Adapting TTS for Taiwanese Mandarin with Enhanced Polyphone Disambiguation -- Challenges and Insights**|Chan-Jan Hsu et.al.|[2501.17790](http://arxiv.org/abs/2501.17790)|null|我们推出了BreezyVoice，这是一个专门针对台湾普通话的文本转语音（TTS）系统，特别强调其在处理语言中多音字辨析的独特挑战时所具备的音素控制能力。基于CosyVoice，我们整合了 $S^{3}$ 分词器、大型语言模型（LLM）、最优传输条件流匹配模型（OT-CFM）以及从字符到音素的预测模型，以生成接近真人发声的逼真语音。评估结果显示，BreezyVoice无论是在一般情境还是语码转换场景下都表现出色，突显了其在生成高保真语音方面的稳健性和有效性。此外，我们还解决了长尾说话者建模和多音字辨析中的泛化难题。我们的方法显著提升了性能，并为神经编码TTS系统的工作原理提供了宝贵的见解。|
|**2025-01-29**|**2SSP: A Two-Stage Framework for Structured Pruning of LLMs**|Fabrizio Sandri et.al.|[2501.17771](http://arxiv.org/abs/2501.17771)|null|我们提出了一种新的两阶段结构化剪枝框架（2SSP），用于大型语言模型（LLMs）的剪枝，该框架结合了宽度剪枝和深度剪枝两种不同的剪枝策略。第一阶段（宽度剪枝）通过移除整个神经元及其对应的行和列来保持每个Transformer块中前馈网络中间状态的连接性。这是基于一个衡量每个神经元对输出幅度影响的重要度得分来完成的。第二阶段（深度剪枝）则通过迭代过程移除对给定兴趣指标（在本例中为困惑度）影响最小的注意力子模块。我们还提出了一种新机制，以根据所需的全局稀疏度平衡两个阶段的稀疏率。我们在四个大型语言模型家族上测试了2SSP，并使用三种稀疏率（25%、37.5% 和 50%），测量了三个语言建模数据集上的结果困惑度以及六个下游任务的表现。我们的方法在三个语言建模和六个下游任务上始终优于五种最先进的竞争对手，且在剪枝时间上最高可达到两个数量级的提升。代码可在 https://github.com/FabrizioSandri/2SSP 获取。|
|**2025-01-29**|**Hybrid Graphs for Table-and-Text based Question Answering using LLMs**|Ankush Agarwal et.al.|[2501.17767](http://arxiv.org/abs/2501.17767)|null|回答需要在结构化（表格）和非结构化（原始文本）数据源之间进行推理和聚合的问题存在重大挑战。当前的方法依赖于微调和高质量的人工整理的数据，这很难获得。最近的大规模语言模型（LLMs）在单源文本数据的多跳问答（QA）中，在零样本设置下展示了有希望的结果，但对多源表-文问答的研究仍然有限。在本文中，我们提出了一种新的基于混合图的方法用于表-文问答，该方法利用大规模语言模型而无需微调。我们的方法从文本和表格数据构建了一个统一的混合图，并根据输入问题修剪信息，为大规模语言模型提供简洁的相关上下文。我们在具有挑战性的Hybrid-QA和OTT-QA数据集上使用最先进的大规模语言模型，包括GPT-3.5、GPT-4和LLaMA-3评估了我们的方法。我们的方法在这两个数据集上实现了最佳的零样本性能，在Hybrid-QA上的准确匹配得分提高了10%，在OTT-QA上提高了5.4%。此外，与原始上下文相比，我们的方法减少了高达53%的token使用量。|
|**2025-01-29**|**Early External Safety Testing of OpenAI's o3-mini: Insights from the Pre-Deployment Evaluation**|Aitor Arrieta et.al.|[2501.17749](http://arxiv.org/abs/2501.17749)|null|大型语言模型（LLM）已经成为我们日常生活的重要组成部分。然而，它们也带来了一些风险，包括可能侵犯个人隐私、延续偏见和传播错误信息。这些风险凸显了需要强大的安全机制、伦理准则和全面测试以确保其负责任的部署。LLM的安全性是一个关键属性，在模型向普通用户开放之前必须经过彻底测试。本文报告了蒙德拉贡大学和塞维利亚大学的研究人员对OpenAI的新o3-mini LLM进行外部安全测试的经验，这是OpenAI早期安全测试计划的一部分。特别是，我们使用我们的工具ASTRAL自动且系统地生成最新的不安全测试输入（即提示），帮助我们测试和评估LLM的不同安全类别。我们在一个早期版本的o3-mini上自动生成并执行了总共10,080个不安全的测试输入。在手动验证被ASTRAL分类为不安全的测试用例后，我们发现了总共87个实际的不安全LLM行为实例。我们强调了在OpenAI最新LLM预部署外部测试阶段发现的关键见解和发现。|
|**2025-01-29**|**Using Code Generation to Solve Open Instances of Combinatorial Design Problems**|Christopher D. Rosin et.al.|[2501.17725](http://arxiv.org/abs/2501.17725)|**[link](https://github.com/constructive-codes/cpro1)**|**《组合设计手册》收录了许多类型的组合设计，以及尚未确定存在性的一些开放实例。我们开发了一种构造性协议CPro1，该协议利用大型语言模型（LLM）生成代码来构建组合设计并解决其中一些开放实例。该协议从特定类型设计的定义开始，并使用一个能够可靠确认提议设计是否有效的验证器。LLM选择策略并将其编码实现，而框架则提供自动超参数调优和基于验证器的执行反馈。虽然大多数生成的代码会失败，但通过生成大量候选方案，该协议自动化探索了多种标准方法（如模拟退火、遗传算法）及其变体（如成本函数），以找到成功的方法。在16种不同类型的设计上进行测试后，CPro1为其中6种设计构建了解决方案：对称和斜称权矩阵、等距排列数组、装箱数组、平衡三进制设计和佛罗伦萨矩形。**|
|**2025-01-29**|**RICoTA: Red-teaming of In-the-wild Conversation with Test Attempts**|Eujeong Choi et.al.|[2501.17715](http://arxiv.org/abs/2501.17715)|**[link](https://github.com/boychaboy/ricota)**|**随着用户与对话代理（CAs）的互动在高度受限的大语言模型（LLMs）时代不断发展，当用户试图突破预设边界以探索和建立与这些系统的关系时，对于未经授权的访问或操纵行为的担忧日益增加，这种现象通常被称为“越狱”。此外，具有高度类人特性的CAs使用户倾向于发起亲密性互动或尝试驯服聊天机器人。为了捕捉并反映这些实际发生的互动到聊天机器人的设计中，我们提出了RICoTA，一个韩语红队测试数据集，包含609个挑战LLMs的提示，这些提示基于用户制作的真实对话，记录了越狱尝试。我们利用了一个类似韩国Reddit社区上用户自发发布的、对社交聊天机器人有特定测试和游戏意图的对话。通过这些提示，我们旨在评估LLMs识别对话类型及用户测试目的的能力，并为减轻越狱风险提供聊天机器人设计上的启示。我们的数据集将通过GitHub公开发布。**|
|**2025-01-29**|**Planning with Vision-Language Models and a Use Case in Robot-Assisted Teaching**|Xuzhe Dang et.al.|[2501.17665](http://arxiv.org/abs/2501.17665)|null|自动化生成规划领域定义语言（PDDL）与大型语言模型（LLM）结合为人工智能规划开辟了新的研究方向，特别是在处理复杂的现实世界任务时。本文介绍了一种名为Image2PDDL的新框架，该框架利用视觉-语言模型（VLMs）将初始状态的图像和目标状态的描述自动转换为PDDL问题。通过提供PDDL领域文件以及视觉输入，Image2PDDL解决了感知理解与符号规划之间的关键衔接问题，减少了创建结构化问题实例所需的专业知识，并提高了跨不同复杂度任务的可扩展性。我们在包括标准规划领域如积木世界和滑动拼图等在内的多个领域上对该框架进行了评估，使用了包含多种难度级别的数据集。性能评估基于语法正确性和内容正确性两个方面：前者确保生成的PDDL问题在语法和可执行性上无误；后者则验证生成的问题中状态表示的准确性。实验结果表明，所提出的方法在各种复杂度的任务上均表现出色，显示出其在更广泛的人工智能规划应用中的潜力。我们将讨论一个潜在的应用案例，即辅助自闭症谱系障碍学生学习的机器人教学。|
|**2025-01-29**|**In-Context Meta LoRA Generation**|Yihua Shao et.al.|[2501.17635](http://arxiv.org/abs/2501.17635)|null|低秩适应（LoRA）在任务特定的微调方面展示了显著的能力。然而，在涉及多个任务的情况下，为每个任务训练单独的LoRA模型会导致存储和推理方面的效率低下。此外，现有的参数生成方法无法捕捉这些任务之间的相关性，使得多任务LoRA参数生成具有挑战性。为了解决这些限制，我们提出了上下文元LoRA（ICM-LoRA），这是一种有效实现大规模语言模型（LLMs）任务特定定制的新方法。具体来说，我们使用所有任务的训练数据来训练一个定制的生成器——条件变分自编码器（CVAE）。CVAE以任务描述作为输入，输出任务感知的LoRA权重。然后将这些LoRA权重与LLMs合并，创建无需额外微调的任务专用模型。此外，我们利用上下文元学习来增强知识和任务映射，以捕捉任务与参数分布之间的关系。因此，我们的方法能够更准确地为各种任务生成LoRA参数。ICM-LoRA比当前的参数重建方法实现了更精确的LoRA参数重建，并且对于实施任务特定的LoRA参数增强非常有用。同时，我们的方法仅占用283MB的存储空间，仅为原始LoRA所需存储空间的1%。|
|**2025-01-29**|**The Imitation Game According To Turing**|Sharon Temtsin et.al.|[2501.17629](http://arxiv.org/abs/2501.17629)|null|当前关于人工智能对人类社会的利弊的炒作和焦虑不仅源于公众越来越多地使用生成式AI和其他AI工具，还源于普及者和科学家们对该技术所作的声明。特别是，最近的研究声称大型语言模型（LLMs）能够通过图灵测试——自1950年代以来AI的一个目标——因此可以“思考”。有人预测这将对社会产生大规模影响。然而，经过详细审查，这些研究都没有忠实遵循图灵最初的指示。因此，我们进行了一项严格遵循图灵指示的三玩家模仿游戏测试，以GPT-4-Turbo为对象。在图灵指示模糊或缺失的地方，我们按照既定的科学标准进行了实验。例如，我们进行了一场不限制时间长度的计算机模仿人类游戏（CIHG），并作为基准进行了男性模仿女性游戏（MIWG）。除了一个参与者外，其他所有参与者都正确识别出了LLM，表明当今最先进的LLM之一无法通过严格的图灵测试。我们得出结论，近期对这类模型的夸张声明是无根据的，并不值得对会思考的机器的社会影响感到乐观或担忧。|
|**2025-01-28**|**FactCG: Enhancing Fact Checkers with Graph-Based Multi-Hop Data**|Deren Lei et.al.|[2501.17144](http://arxiv.org/abs/2501.17144)|**[link](https://github.com/derenlei/factcg)**|
|**2025-01-28**|**ASTRAL: Automated Safety Testing of Large Language Models**|Miriam Ugarte et.al.|[2501.17132](http://arxiv.org/abs/2501.17132)|null|
|**2025-01-28**|**Optimizing Large Language Model Training Using FP4 Quantization**|Ruizhe Wang et.al.|[2501.17116](http://arxiv.org/abs/2501.17116)|null|
|**2025-01-28**|**Unlocking Transparent Alignment Through Enhanced Inverse Constitutional AI for Principle Extraction**|Carl-Leander Henneking et.al.|[2501.17112](http://arxiv.org/abs/2501.17112)|null|
|**2025-01-28**|**Token-by-Token Regeneration and Domain Biases: A Benchmark of LLMs on Advanced Mathematical Problem-Solving**|Evgenii Evstafev et.al.|[2501.17084](http://arxiv.org/abs/2501.17084)|null|
|**2025-01-28**|**Enhanced Retrieval of Long Documents: Leveraging Fine-Grained Block Representations with Large Language Models**|Minghan Li et.al.|[2501.17039](http://arxiv.org/abs/2501.17039)|null|
|**2025-01-28**|**Challenges in Ensuring AI Safety in DeepSeek-R1 Models: The Shortcomings of Reinforcement Learning Strategies**|Manojkumar Parmar et.al.|[2501.17030](http://arxiv.org/abs/2501.17030)|null|
|**2025-01-28**|**Automated Refactoring of Non-Idiomatic Python Code: A Differentiated Replication with LLMs**|Alessandro Midolo et.al.|[2501.17024](http://arxiv.org/abs/2501.17024)|null|
|**2025-01-28**|**Large Language Models for Code Generation: The Practitioners Perspective**|Zeeshan Rasheed et.al.|[2501.16998](http://arxiv.org/abs/2501.16998)|null|
|**2025-01-28**|**Over-Tokenized Transformer: Vocabulary is Generally Worth Scaling**|Hongzhi Huang et.al.|[2501.16975](http://arxiv.org/abs/2501.16975)|null|
|**2025-01-27**|**Evaluating The Performance of Using Large Language Models to Automate Summarization of CT Simulation Orders in Radiation Oncology**|Meiyun Cao et.al.|[2501.16309](http://arxiv.org/abs/2501.16309)|null|
|**2025-01-27**|**RAPID: Retrieval-Augmented Parallel Inference Drafting for Text-Based Video Event Retrieval**|Long Nguyen et.al.|[2501.16303](http://arxiv.org/abs/2501.16303)|null|
|**2025-01-27**|**Matryoshka Re-Ranker: A Flexible Re-Ranking Architecture With Configurable Depth and Width**|Zheng Liu et.al.|[2501.16302](http://arxiv.org/abs/2501.16302)|null|
|**2025-01-27**|**Large Models in Dialogue for Active Perception and Anomaly Detection**|Tzoulio Chamiti et.al.|[2501.16300](http://arxiv.org/abs/2501.16300)|**[link](https://github.com/Tzoulio/Large_Models_Dialogue_for_Active_Perception)**|
|**2025-01-27**|**Do LLMs Have Visualization Literacy? An Evaluation on Modified Visualizations to Test Generalization in Data Interpretation**|Jiayi Hong et.al.|[2501.16277](http://arxiv.org/abs/2501.16277)|**[link](https://github.com/vaderasu/llm4viz-experiments)**|
|**2025-01-27**|**URAG: Implementing a Unified Hybrid RAG for Precise Answers in University Admission Chatbots -- A Case Study at HCMUT**|Long Nguyen et.al.|[2501.16276](http://arxiv.org/abs/2501.16276)|null|
|**2025-01-27**|**A foundation model for human-AI collaboration in medical literature mining**|Zifeng Wang et.al.|[2501.16255](http://arxiv.org/abs/2501.16255)|null|
|**2025-01-27**|**Multi-Agent Geospatial Copilots for Remote Sensing Workflows**|Chaehong Lee et.al.|[2501.16254](http://arxiv.org/abs/2501.16254)|null|
|**2025-01-27**|**Zero-Shot Decision Tree Construction via Large Language Models**|Lucas Carrasco et.al.|[2501.16247](http://arxiv.org/abs/2501.16247)|null|
|**2025-01-27**|**Phase Transitions in Large Language Models and the $O(N)$ Model**|Youran Sun et.al.|[2501.16241](http://arxiv.org/abs/2501.16241)|null|
|**2025-01-24**|**HERMES: A Unified Self-Driving World Model for Simultaneous 3D Scene Understanding and Generation**|Xin Zhou et.al.|[2501.14729](http://arxiv.org/abs/2501.14729)|**[link](https://github.com/lmd0311/hermes)**|
|**2025-01-24**|**Do LLMs Provide Consistent Answers to Health-Related Questions across Languages?**|Ipek Baris Schlicht et.al.|[2501.14719](http://arxiv.org/abs/2501.14719)|null|
|**2025-01-24**|**Towards Better Understanding Table Instruction Tuning: Decoupling the Effects from Data versus Models**|Naihao Deng et.al.|[2501.14717](http://arxiv.org/abs/2501.14717)|null|
|**2025-01-24**|**FlexiGPT: Pruning and Extending Large Language Models with Low-Rank Weight Sharing**|James Seale Smith et.al.|[2501.14713](http://arxiv.org/abs/2501.14713)|null|
|**2025-01-24**|**The Karp Dataset**|Mason DiCicco et.al.|[2501.14705](http://arxiv.org/abs/2501.14705)|null|
|**2025-01-24**|**Rethinking Table Instruction Tuning**|Naihao Deng et.al.|[2501.14693](http://arxiv.org/abs/2501.14693)|null|
|**2025-01-24**|**An Empirical Study on LLM-based Classification of Requirements-related Provisions in Food-safety Regulations**|Shabnam Hassani et.al.|[2501.14683](http://arxiv.org/abs/2501.14683)|null|
|**2025-01-24**|**MedAgentBench: Dataset for Benchmarking LLMs as Agents in Medical Applications**|Yixing Jiang et.al.|[2501.14654](http://arxiv.org/abs/2501.14654)|**[link](https://github.com/stanfordmlgroup/medagentbench)**|
|**2025-01-24**|**Investigating the (De)Composition Capabilities of Large Language Models in Natural-to-Formal Language Conversion**|Ziyao Xu et.al.|[2501.14649](http://arxiv.org/abs/2501.14649)|**[link](https://github.com/xzy-xzy/dedc)**|
|**2025-01-24**|**Extracting Problem Structure with LLMs for Optimized SAT Local Search**|André Schilder et.al.|[2501.14630](http://arxiv.org/abs/2501.14630)|null|
|**2025-01-23**|**CRPO: Confidence-Reward Driven Preference Optimization for Machine Translation**|Guofeng Cui et.al.|[2501.13927](http://arxiv.org/abs/2501.13927)|null|
|**2025-01-23**|**Analysis of Indic Language Capabilities in LLMs**|Aatman Vaidya et.al.|[2501.13912](http://arxiv.org/abs/2501.13912)|null|
|**2025-01-23**|**Privacy-Preserving Personalized Federated Prompt Learning for Multimodal Large Language Models**|Linh Tran et.al.|[2501.13904](http://arxiv.org/abs/2501.13904)|null|
|**2025-01-23**|**Exploring Finetuned Audio-LLM on Heart Murmur Features**|Adrian Florea et.al.|[2501.13884](http://arxiv.org/abs/2501.13884)|null|
|**2025-01-23**|**The machine learning platform for developers of large systems**|Alexey Naikov et.al.|[2501.13881](http://arxiv.org/abs/2501.13881)|null|
|**2025-01-23**|**A RAG-Based Institutional Assistant**|Gustavo Kuratomi et.al.|[2501.13880](http://arxiv.org/abs/2501.13880)|null|
|**2025-01-23**|**On the Reasoning Capacity of AI Models and How to Quantify It**|Santosh Kumar Radha et.al.|[2501.13833](http://arxiv.org/abs/2501.13833)|null|
|**2025-01-23**|**Predicting Compact Phrasal Rewrites with Large Language Models for ASR Post Editing**|Hao Zhang et.al.|[2501.13831](http://arxiv.org/abs/2501.13831)|null|
|**2025-01-23**|**Hallucinations Can Improve Large Language Models in Drug Discovery**|Shuzhou Yuan et.al.|[2501.13824](http://arxiv.org/abs/2501.13824)|null|
|**2025-01-23**|**Large Language Model driven Policy Exploration for Recommender Systems**|Jie Wang et.al.|[2501.13816](http://arxiv.org/abs/2501.13816)|null|
|**2025-01-22**|**Refining Input Guardrails: Enhancing LLM-as-a-Judge Efficiency Through Chain-of-Thought Fine-Tuning and Alignment**|Melissa Kazemi Rad et.al.|[2501.13080](http://arxiv.org/abs/2501.13080)|null|
|**2025-01-22**|**Does Table Source Matter? Benchmarking and Improving Multimodal Scientific Table Understanding and Reasoning**|Bohao Yang et.al.|[2501.13042](http://arxiv.org/abs/2501.13042)|**[link](https://github.com/bernard-yang/mmsci_table)**|
|**2025-01-22**|**Pairwise RM: Perform Best-of-N Sampling with Knockout Tournament**|Yantao Liu et.al.|[2501.13007](http://arxiv.org/abs/2501.13007)|**[link](https://github.com/thu-keg/pairwiserm)**|
|**2025-01-22**|**Large Language Model-Based Semantic Communication System for Image Transmission**|Soheyb Ribouh et.al.|[2501.12988](http://arxiv.org/abs/2501.12988)|null|
|**2025-01-22**|**LLM4WM: Adapting LLM for Wireless Multi-Tasking**|Xuanyu Liu et.al.|[2501.12983](http://arxiv.org/abs/2501.12983)|null|
|**2025-01-22**|**OnionEval: An Unified Evaluation of Fact-conflicting Hallucination for Small-Large Language Models**|Chongren Sun et.al.|[2501.12975](http://arxiv.org/abs/2501.12975)|**[link](https://github.com/sunchongren/onioneval)**|
|**2025-01-22**|**Accessible Smart Contracts Verification: Synthesizing Formal Models with Tamed LLMs**|Jan Corazza et.al.|[2501.12972](http://arxiv.org/abs/2501.12972)|null|
|**2025-01-22**|**Efficient Prompt Compression with Evaluator Heads for Long-Context Transformer Inference**|Weizhi Fei et.al.|[2501.12959](http://arxiv.org/abs/2501.12959)|null|
|**2025-01-22**|**GANQ: GPU-Adaptive Non-Uniform Quantization for Large Language Models**|Pengxiang Zhao et.al.|[2501.12956](http://arxiv.org/abs/2501.12956)|null|
|**2025-01-22**|**Correctness Assessment of Code Generated by Large Language Models Using Internal Representations**|Tuan-Dung Bui et.al.|[2501.12934](http://arxiv.org/abs/2501.12934)|null|
|**2025-01-21**|**Is Long Context All You Need? Leveraging LLM's Extended Context for NL2SQL**|Yeounoh Chung et.al.|[2501.12372](http://arxiv.org/abs/2501.12372)|null|
|**2025-01-21**|**Automatic Labelling with Open-source LLMs using Dynamic Label Schema Integration**|Thomas Walshe et.al.|[2501.12332](http://arxiv.org/abs/2501.12332)|null|
|**2025-01-21**|**LLM-Assisted Knowledge Graph Completion for Curriculum and Domain Modelling in Personalized Higher Education Recommendations**|Hasan Abu-Rasheed et.al.|[2501.12300](http://arxiv.org/abs/2501.12300)|null|
|**2025-01-21**|**Condor: Enhance LLM Alignment with Knowledge-Driven Data Synthesis and Refinement**|Maosong Cao et.al.|[2501.12273](http://arxiv.org/abs/2501.12273)|**[link](https://github.com/internlm/condor)**|
|**2025-01-21**|**FOCUS: First Order Concentrated Updating Scheme**|Yizhou Liu et.al.|[2501.12243](http://arxiv.org/abs/2501.12243)|null|
|**2025-01-21**|**CDW-CoT: Clustered Distance-Weighted Chain-of-Thoughts Reasoning**|Yuanheng Fang et.al.|[2501.12226](http://arxiv.org/abs/2501.12226)|null|
|**2025-01-21**|**Leveraging Large Language Models for Realizing Truly Intelligent User Interfaces**|Allard Oelen et.al.|[2501.12221](http://arxiv.org/abs/2501.12221)|null|
|**2025-01-21**|**You Can't Eat Your Cake and Have It Too: The Performance Degradation of LLMs with Jailbreak Defense**|Wuyuao Mai et.al.|[2501.12210](http://arxiv.org/abs/2501.12210)|null|
|**2025-01-21**|**BiMarker: Enhancing Text Watermark Detection for Large Language Models with Bipolar Watermarks**|Zhuang Li et.al.|[2501.12174](http://arxiv.org/abs/2501.12174)|null|
|**2025-01-21**|**Contextualizing Recommendation Explanations with LLMs: A User Study**|Yuanjun Feng et.al.|[2501.12152](http://arxiv.org/abs/2501.12152)|null|
|**2025-01-17**|**Agent4Edu: Generating Learner Response Data by Generative Agents for Intelligent Education Systems**|Weibo Gao et.al.|[2501.10332](http://arxiv.org/abs/2501.10332)|null|
|**2025-01-17**|**Large language models for automated scholarly paper review: A survey**|Zhenzhen Zhuang et.al.|[2501.10326](http://arxiv.org/abs/2501.10326)|null|
|**2025-01-17**|**Addressing Popularity Bias in Third-Party Library Recommendations Using LLMs**|Claudio Di Sipio et.al.|[2501.10313](http://arxiv.org/abs/2501.10313)|null|
|**2025-01-17**|**Computational Protein Science in the Era of Large Language Models (LLMs)**|Wenqi Fan et.al.|[2501.10282](http://arxiv.org/abs/2501.10282)|null|
|**2025-01-17**|**Test Wars: A Comparative Study of SBST, Symbolic Execution, and LLM-Based Approaches to Unit Test Generation**|Azat Abdullin et.al.|[2501.10200](http://arxiv.org/abs/2501.10200)|null|
|**2025-01-17**|**Generative Artificial Intelligence: Implications for Biomedical and Health Professions Education**|William Hersh et.al.|[2501.10186](http://arxiv.org/abs/2501.10186)|null|
|**2025-01-17**|**Multi-stage Training of Bilingual Islamic LLM for Neural Passage Retrieval**|Vera Pavlova et.al.|[2501.10175](http://arxiv.org/abs/2501.10175)|null|
|**2025-01-17**|**Exploring the Impact of Generative Artificial Intelligence in Education: A Thematic Analysis**|Abhishek Kaushik et.al.|[2501.10134](http://arxiv.org/abs/2501.10134)|null|
|**2025-01-17**|**ComplexFuncBench: Exploring Multi-Step and Constrained Function Calling under Long-Context Scenario**|Lucen Zhong et.al.|[2501.10132](http://arxiv.org/abs/2501.10132)|**[link](https://github.com/thudm/complexfuncbench)**|
|**2025-01-17**|**LLM Reasoner and Automated Planner: A new NPC approach**|Israel Puerta-Merino et.al.|[2501.10106](http://arxiv.org/abs/2501.10106)|null|
|**2025-01-16**|**Distilling Multi-modal Large Language Models for Autonomous Driving**|Deepti Hegde et.al.|[2501.09757](http://arxiv.org/abs/2501.09757)|null|
|**2025-01-16**|**Lost in Translation, Found in Context: Sign Language Translation with Contextual Cues**|Youngjoon Jang et.al.|[2501.09754](http://arxiv.org/abs/2501.09754)|null|
|**2025-01-16**|**Enhancing Lexicon-Based Text Embeddings with Large Language Models**|Yibin Lei et.al.|[2501.09749](http://arxiv.org/abs/2501.09749)|null|
|**2025-01-16**|**Inference-Time Scaling for Diffusion Models beyond Scaling Denoising Steps**|Nanye Ma et.al.|[2501.09732](http://arxiv.org/abs/2501.09732)|null|
|**2025-01-16**|**CyberMentor: AI Powered Learning Tool Platform to Address Diverse Student Needs in Cybersecurity Education**|Tianyu Wang et.al.|[2501.09709](http://arxiv.org/abs/2501.09709)|**[link](https://github.com/tisage/cybermentor)**|
|**2025-01-16**|**Towards Large Reasoning Models: A Survey of Reinforced Reasoning with Large Language Models**|Fengli Xu et.al.|[2501.09686](http://arxiv.org/abs/2501.09686)|null|
|**2025-01-16**|**Robin: a Suite of Multi-Scale Vision-Language Models and the CHIRP Evaluation Benchmark**|Alexis Roger et.al.|[2501.09672](http://arxiv.org/abs/2501.09672)|null|
|**2025-01-16**|**A Survey of Research in Large Language Models for Electronic Design Automation**|Jingyu Pan et.al.|[2501.09655](http://arxiv.org/abs/2501.09655)|null|
|**2025-01-16**|**LLM-Based Routing in Mixture of Experts: A Novel Framework for Trading**|Kuan-Ming Liu et.al.|[2501.09636](http://arxiv.org/abs/2501.09636)|null|
|**2025-01-16**|**Empowering Large Language Models in Wireless Communication: A Novel Dataset and Fine-Tuning Framework**|Yushen Lin et.al.|[2501.09631](http://arxiv.org/abs/2501.09631)|null|
|**2025-01-15**|**Aegis2.0: A Diverse AI Safety Dataset and Risks Taxonomy for Alignment of LLM Guardrails**|Shaona Ghosh et.al.|[2501.09004](http://arxiv.org/abs/2501.09004)|null|
|**2025-01-15**|**Development and Validation of the Provider Documentation Summarization Quality Instrument for Large Language Models**|Emma Croxford et.al.|[2501.08977](http://arxiv.org/abs/2501.08977)|null|
|**2025-01-15**|**GenAI Content Detection Task 3: Cross-Domain Machine-Generated Text Detection Challenge**|Liam Dugan et.al.|[2501.08913](http://arxiv.org/abs/2501.08913)|**[link](https://github.com/liamdugan/raid)**|
|**2025-01-15**|**Leveraging Large Language Models as Knowledge-Driven Agents for Reliable Retrosynthesis Planning**|Qinyu Ma et.al.|[2501.08897](http://arxiv.org/abs/2501.08897)|**[link](https://github.com/qinyuma316/retrosynthesisagent)**|
|**2025-01-15**|**Enhanced Large Language Models for Effective Screening of Depression and Anxiety**|June M. Liu et.al.|[2501.08769](http://arxiv.org/abs/2501.08769)|null|
|**2025-01-15**|**Leveraging LLM Agents for Translating Network Configurations**|Yunze Wei et.al.|[2501.08760](http://arxiv.org/abs/2501.08760)|null|
|**2025-01-15**|**The Inherent Limits of Pretrained LLMs: The Unexpected Convergence of Instruction Tuning and In-Context Learning Capabilities**|Irina Bigoulaeva et.al.|[2501.08716](http://arxiv.org/abs/2501.08716)|**[link](https://github.com/ukplab/arxiv2025-inherent-limits-plms)**|
|**2025-01-15**|**Knowledge Graph-based Retrieval-Augmented Generation for Schema Matching**|Chuangtao Ma et.al.|[2501.08686](http://arxiv.org/abs/2501.08686)|**[link](https://github.com/machuangtao/kg-rag4sm)**|
|**2025-01-15**|**Augmenting Smart Contract Decompiler Output through Fine-grained Dependency Analysis and LLM-facilitated Semantic Recovery**|Zeqin Liao et.al.|[2501.08670](http://arxiv.org/abs/2501.08670)|null|
|**2025-01-15**|**MAGNET: Augmenting Generative Decoders with Representation Learning and Infilling Capabilities**|Savya Khosla et.al.|[2501.08648](http://arxiv.org/abs/2501.08648)|null|
|**2025-01-14**|**PokerBench: Training Large Language Models to become Professional Poker Players**|Richard Zhuang et.al.|[2501.08328](http://arxiv.org/abs/2501.08328)|**[link](https://github.com/pokerllm/pokerbench)**|
|**2025-01-14**|**ADAM-1: AI and Bioinformatics for Alzheimer's Detection and Microbiome-Clinical Data Integrations**|Ziyuan Huang et.al.|[2501.08324](http://arxiv.org/abs/2501.08324)|null|
|**2025-01-14**|**Exploring Robustness of Multilingual LLMs on Real-World Noisy Data**|Amirhossein Aliakbarzadeh et.al.|[2501.08322](http://arxiv.org/abs/2501.08322)|**[link](https://github.com/caisa-lab/llms-real-world-noise-robustness)**|
|**2025-01-14**|**Enhancing Automated Interpretability with Output-Centric Feature Descriptions**|Yoav Gur-Arieh et.al.|[2501.08319](http://arxiv.org/abs/2501.08319)|**[link](https://github.com/yoavgur/feature-descriptions)**|
|**2025-01-14**|**HALoGEN: Fantastic LLM Hallucinations and Where to Find Them**|Abhilasha Ravichander et.al.|[2501.08292](http://arxiv.org/abs/2501.08292)|null|
|**2025-01-14**|**Exploring Robustness of LLMs to Sociodemographically-Conditioned Paraphrasing**|Pulkit Arora et.al.|[2501.08276](http://arxiv.org/abs/2501.08276)|null|
|**2025-01-14**|**Addressing the sustainable AI trilemma: a case study on LLM agents and RAG**|Hui Wu et.al.|[2501.08262](http://arxiv.org/abs/2501.08262)|null|
|**2025-01-14**|**Text-Diffusion Red-Teaming of Large Language Models: Unveiling Harmful Behaviors with Proximity Constraints**|Jonathan Nöther et.al.|[2501.08246](http://arxiv.org/abs/2501.08246)|null|
|**2025-01-14**|**Investigating Energy Efficiency and Performance Trade-offs in LLM Inference Across Tasks and DVFS Settings**|Paul Joe Maliakel et.al.|[2501.08219](http://arxiv.org/abs/2501.08219)|null|
|**2025-01-14**|**ASTRID -- An Automated and Scalable TRIaD for the Evaluation of RAG-based Clinical Question Answering Systems**|Mohita Chowdhury et.al.|[2501.08208](http://arxiv.org/abs/2501.08208)|null|
|**2025-01-13**|**Imagine while Reasoning in Space: Multimodal Visualization-of-Thought**|Chengzu Li et.al.|[2501.07542](http://arxiv.org/abs/2501.07542)|null|
|**2025-01-13**|**Investigating Large Language Models in Inferring Personality Traits from User Conversations**|Jianfeng Zhu et.al.|[2501.07532](http://arxiv.org/abs/2501.07532)|null|
|**2025-01-13**|**RadAlign: Advancing Radiology Report Generation with Vision-Language Concept Alignment**|Difei Gu et.al.|[2501.07525](http://arxiv.org/abs/2501.07525)|**[link](https://github.com/difeigu/radalign)**|
|**2025-01-13**|**Parallel Key-Value Cache Fusion for Position Invariant RAG**|Philhoon Oh et.al.|[2501.07523](http://arxiv.org/abs/2501.07523)|null|
|**2025-01-13**|**Exploring and Mitigating Adversarial Manipulation of Voting-Based Leaderboards**|Yangsibo Huang et.al.|[2501.07493](http://arxiv.org/abs/2501.07493)|null|
|**2025-01-13**|**Understanding and Benchmarking Artificial Intelligence: OpenAI's o3 Is Not AGI**|Rolf Pfister et.al.|[2501.07458](http://arxiv.org/abs/2501.07458)|null|
|**2025-01-13**|**Enhancing LLM's Ability to Generate More Repository-Aware Unit Tests Through Precise Contextual Information Injection**|Xin Yin et.al.|[2501.07425](http://arxiv.org/abs/2501.07425)|null|
|**2025-01-13**|**Initial Findings on Sensor based Open Vocabulary Activity Recognition via Text Embedding Inversion**|Lala Shakti Swarup Ray et.al.|[2501.07408](http://arxiv.org/abs/2501.07408)|null|
|**2025-01-13**|**Emergent effects of scaling on the functional hierarchies within large language models**|Paul C. Bogdan et.al.|[2501.07359](http://arxiv.org/abs/2501.07359)|null|
|**2025-01-13**|**FinerWeb-10BT: Refining Web Data with LLM-Based Line-Level Filtering**|Erik Henriksson et.al.|[2501.07314](http://arxiv.org/abs/2501.07314)|**[link](https://github.com/turkunlp/finerweb-10bt)**|
|**2025-01-10**|**Supervision policies can shape long-term risk management in general-purpose AI models**|Manuel Cebrian et.al.|[2501.06137](http://arxiv.org/abs/2501.06137)|**[link](https://github.com/manuelcebrianramos/llm_supervision_policies)**|
|**2025-01-10**|**From Conversation to Automation: Leveraging Large Language Models to Analyze Strategies in Problem Solving Therapy**|Elham Aghakhani et.al.|[2501.06101](http://arxiv.org/abs/2501.06101)|null|
|**2025-01-10**|**Addressing speaker gender bias in large scale speech translation systems**|Shubham Bansal et.al.|[2501.05989](http://arxiv.org/abs/2501.05989)|null|
|**2025-01-10**|**Exploring LLMs for Automated Pre-Testing of Cross-Cultural Surveys**|Divya Mani Adhikari et.al.|[2501.05985](http://arxiv.org/abs/2501.05985)|null|
|**2025-01-10**|**Hermit Kingdom Through the Lens of Multiple Perspectives: A Case Study of LLM Hallucination on North Korea**|Eunjung Cho et.al.|[2501.05981](http://arxiv.org/abs/2501.05981)|null|
|**2025-01-10**|**Model Inversion in Split Learning for Personalized LLMs: New Insights from Information Bottleneck Theory**|Yunmeng Shu et.al.|[2501.05965](http://arxiv.org/abs/2501.05965)|null|
|**2025-01-10**|**LLMs Reproduce Stereotypes of Sexual and Gender Minorities**|Ruby Ostrow et.al.|[2501.05926](http://arxiv.org/abs/2501.05926)|null|
|**2025-01-10**|**Navigating Tomorrow: Reliably Assessing Large Language Models Performance on Future Event Prediction**|Petraq Nako et.al.|[2501.05925](http://arxiv.org/abs/2501.05925)|null|
|**2025-01-10**|**Prompt engineering and its implications on the energy consumption of Large Language Models**|Riccardo Rubei et.al.|[2501.05899](http://arxiv.org/abs/2501.05899)|**[link](https://github.com/riccardoRubei/Greens-2025-Replication-Package)**|
|**2025-01-10**|**Affordably Fine-tuned LLMs Provide Better Answers to Course-specific MCQs**|Bianca Raimondi et.al.|[2501.05891](http://arxiv.org/abs/2501.05891)|**[link](https://github.com/biancaraimondi/llama2_for_mcqs)**|
|**2025-01-09**|**ReFocus: Visual Editing as a Chain of Thought for Structured Image Understanding**|Xingyu Fu et.al.|[2501.05452](http://arxiv.org/abs/2501.05452)|null|
|**2025-01-09**|**A survey of textual cyber abuse detection using cutting-edge language models and large language models**|Jose A. Diaz-Garcia et.al.|[2501.05443](http://arxiv.org/abs/2501.05443)|null|
|**2025-01-09**|**FairCode: Evaluating Social Bias of LLMs in Code Generation**|Yongkang Du et.al.|[2501.05396](http://arxiv.org/abs/2501.05396)|**[link](https://github.com/yongkdu/faircode)**|
|**2025-01-09**|**Large Physics Models: Towards a collaborative approach with Large Language Models and Foundation Models**|Kristian G. Barman et.al.|[2501.05382](http://arxiv.org/abs/2501.05382)|null|
|**2025-01-09**|**Stream Aligner: Efficient Sentence-Level Alignment via Distribution Induction**|Hantao Lou et.al.|[2501.05336](http://arxiv.org/abs/2501.05336)|**[link](https://github.com/htlou/stream-aligner)**|
|**2025-01-09**|**"What's Happening"- A Human-centered Multimodal Interpreter Explaining the Actions of Autonomous Vehicles**|Xuewen Luo et.al.|[2501.05322](http://arxiv.org/abs/2501.05322)|null|
|**2025-01-09**|**RAG-WM: An Efficient Black-Box Watermarking Approach for Retrieval-Augmented Generation of Large Language Models**|Peizhuo Lv et.al.|[2501.05249](http://arxiv.org/abs/2501.05249)|null|
|**2025-01-09**|**Deriving Coding-Specific Sub-Models from LLMs using Resource-Efficient Pruning**|Laura Puccioni et.al.|[2501.05248](http://arxiv.org/abs/2501.05248)|null|
|**2025-01-09**|**Online Prompt and Solver Selection for Program Synthesis**|Yixuan Li et.al.|[2501.05247](http://arxiv.org/abs/2501.05247)|null|
|**2025-01-09**|**Optimizing Estonian TV Subtitles with Semi-supervised Learning and LLMs**|Artem Fedorchenko et.al.|[2501.05234](http://arxiv.org/abs/2501.05234)|null|
|**2025-01-08**|**Re-ranking the Context for Multimodal Retrieval Augmented Generation**|Matin Mortaheb et.al.|[2501.04695](http://arxiv.org/abs/2501.04695)|null|
|**2025-01-08**|**URSA: Understanding and Verifying Chain-of-thought Reasoning in Multimodal Mathematics**|Ruilin Luo et.al.|[2501.04686](http://arxiv.org/abs/2501.04686)|**[link](https://github.com/URSA-MATH/URSA-MATH)**|
|**2025-01-08**|**Enhancing Financial VQA in Vision Language Models using Intermediate Structured Representations**|Archita Srivastava et.al.|[2501.04675](http://arxiv.org/abs/2501.04675)|null|
|**2025-01-08**|**Multi-task retriever fine-tuning for domain-specific and efficient RAG**|Patrice Béchard et.al.|[2501.04652](http://arxiv.org/abs/2501.04652)|null|
|**2025-01-08**|**FlairGPT: Repurposing LLMs for Interior Designs**|Gabrielle Littlefair et.al.|[2501.04648](http://arxiv.org/abs/2501.04648)|null|
|**2025-01-08**|**Knowledge Retrieval Based on Generative AI**|Te-Lun Yang et.al.|[2501.04635](http://arxiv.org/abs/2501.04635)|null|
|**2025-01-08**|**The Impostor is Among Us: Can Large Language Models Capture the Complexity of Human Personas?**|Christopher Lazik et.al.|[2501.04543](http://arxiv.org/abs/2501.04543)|null|
|**2025-01-08**|**CGP-Tuning: Structure-Aware Soft Prompt Tuning for Code Vulnerability Detection**|Ruijun Feng et.al.|[2501.04510](http://arxiv.org/abs/2501.04510)|null|
|**2025-01-08**|**Integrating remote sensing data assimilation, deep learning and large language model for interactive wheat breeding yield prediction**|Guofeng Yang et.al.|[2501.04487](http://arxiv.org/abs/2501.04487)|null|
|**2025-01-08**|**When LLMs Struggle: Reference-less Translation Evaluation for Low-resource Languages**|Archchana Sindhujan et.al.|[2501.04473](http://arxiv.org/abs/2501.04473)|null|
|**2025-01-07**|**RAG-Check: Evaluating Multimodal Retrieval Augmented Generation Performance**|Matin Mortaheb et.al.|[2501.03995](http://arxiv.org/abs/2501.03995)|null|
|**2025-01-07**|**Influences on LLM Calibration: A Study of Response Agreement, Loss Functions, and Prompt Styles**|Yuxi Xia et.al.|[2501.03991](http://arxiv.org/abs/2501.03991)|null|
|**2025-01-07**|**(De)-Indexing and the Right to be Forgotten**|Salvatore Vilella et.al.|[2501.03989](http://arxiv.org/abs/2501.03989)|null|
|**2025-01-07**|**VLM-driven Behavior Tree for Context-aware Task Planning**|Naoki Wake et.al.|[2501.03968](http://arxiv.org/abs/2501.03968)|**[link](https://github.com/microsoft/scene-aware-robot-BT-planner)**|
|**2025-01-07**|**Localizing AI: Evaluating Open-Weight Language Models for Languages of Baltic States**|Jurgita Kapočiūtė-Dzikienė et.al.|[2501.03952](http://arxiv.org/abs/2501.03952)|null|
|**2025-01-07**|**Not all tokens are created equal: Perplexity Attention Weighted Networks for AI generated text detection**|Pablo Miralles-González et.al.|[2501.03940](http://arxiv.org/abs/2501.03940)|null|
|**2025-01-07**|**Exploring the Potential of Large Language Models in Public Transportation: San Antonio Case Study**|Ramya Jonnala et.al.|[2501.03904](http://arxiv.org/abs/2501.03904)|null|
|**2025-01-07**|**LLaVA-Mini: Efficient Image and Video Large Multimodal Models with One Vision Token**|Shaolei Zhang et.al.|[2501.03895](http://arxiv.org/abs/2501.03895)|**[link](https://github.com/ictnlp/llava-mini)**|
|**2025-01-07**|**AlphaPO -- Reward shape matters for LLM alignment**|Aman Gupta et.al.|[2501.03884](http://arxiv.org/abs/2501.03884)|null|
|**2025-01-07**|**CL3DOR: Contrastive Learning for 3D Large Multimodal Models via Odds Ratio on High-Resolution Point Clouds**|Keonwoo Kim et.al.|[2501.03879](http://arxiv.org/abs/2501.03879)|null|
|**2025-01-06**|**BoostStep: Boosting mathematical capability of Large Language Models via improved single-step reasoning**|Beichen Zhang et.al.|[2501.03226](http://arxiv.org/abs/2501.03226)|**[link](https://github.com/beichenzbc/booststep)**|
|**2025-01-06**|**Leveraging Explainable AI for LLM Text Attribution: Differentiating Human-Written and Multiple LLMs-Generated Text**|Ayat Najjar et.al.|[2501.03212](http://arxiv.org/abs/2501.03212)|null|
|**2025-01-06**|**Detecting AI-Generated Text in Educational Content: Leveraging Machine Learning and Explainable AI for Academic Integrity**|Ayat A. Najjar et.al.|[2501.03203](http://arxiv.org/abs/2501.03203)|null|
|**2025-01-06**|**Semantic Captioning: Benchmark Dataset and Graph-Aware Few-Shot In-Context Learning for SQL2Text**|Ali Al-Lawati et.al.|[2501.03166](http://arxiv.org/abs/2501.03166)|**[link](https://github.com/aliwister/ast-icl)**|
|**2025-01-06**|**Large language models for artificial general intelligence (AGI): A survey of foundational principles and approaches**|Alhassan Mumuni et.al.|[2501.03151](http://arxiv.org/abs/2501.03151)|null|
|**2025-01-06**|**VicSim: Enhancing Victim Simulation with Emotional and Linguistic Fidelity**|Yerong Li et.al.|[2501.03139](http://arxiv.org/abs/2501.03139)|null|
|**2025-01-06**|**CAT: Content-Adaptive Image Tokenization**|Junhong Shen et.al.|[2501.03120](http://arxiv.org/abs/2501.03120)|null|
|**2025-01-06**|**LangFair: A Python Package for Assessing Bias and Fairness in Large Language Model Use Cases**|Dylan Bouchard et.al.|[2501.03112](http://arxiv.org/abs/2501.03112)|**[link](https://github.com/cvs-health/langfair)**|
|**2025-01-06**|**Retrieval-Augmented TLAPS Proof Generation with Large Language Models**|Yuhao Zhou et.al.|[2501.03073](http://arxiv.org/abs/2501.03073)|null|
|**2025-01-06**|**ChronoSense: Exploring Temporal Understanding in Large Language Models with Time Intervals of Events**|Duygu Sezen Islakoglu et.al.|[2501.03040](http://arxiv.org/abs/2501.03040)|null|
|**2025-01-03**|**Cold-Start Recommendation towards the Era of Large Language Models (LLMs): A Comprehensive Survey and Roadmap**|Weizhi Zhang et.al.|[2501.01945](http://arxiv.org/abs/2501.01945)|**[link](https://github.com/yuanchenbei/awesome-cold-start-recommendation)**|
|**2025-01-03**|**Virgo: A Preliminary Exploration on Reproducing o1-like MLLM**|Yifan Du et.al.|[2501.01904](http://arxiv.org/abs/2501.01904)|**[link](https://github.com/rucaibox/virgo)**|
|**2025-01-03**|**Multi-Agent Conversational Online Learning for Adaptive LLM Response Identification**|Xiangxiang Dai et.al.|[2501.01849](http://arxiv.org/abs/2501.01849)|**[link](https://github.com/tarfersoul/maco)**|
|**2025-01-03**|**MoColl: Agent-Based Specific and General Model Collaboration for Image Captioning**|Pu Yang et.al.|[2501.01834](http://arxiv.org/abs/2501.01834)|null|
|**2025-01-03**|**Time Series Language Model for Descriptive Caption Generation**|Mohamed Trabelsi et.al.|[2501.01832](http://arxiv.org/abs/2501.01832)|null|
|**2025-01-03**|**Auto-RT: Automatic Jailbreak Strategy Exploration for Red-Teaming Large Language Models**|Yanjiang Liu et.al.|[2501.01830](http://arxiv.org/abs/2501.01830)|null|
|**2025-01-03**|**SDPO: Segment-Level Direct Preference Optimization for Social Agents**|Aobo Kong et.al.|[2501.01821](http://arxiv.org/abs/2501.01821)|**[link](https://github.com/alibabaresearch/damo-convai)**|
|**2025-01-03**|**Creating Artificial Students that Never Existed: Leveraging Large Language Models and CTGANs for Synthetic Data Generation**|Mohammad Khalil et.al.|[2501.01793](http://arxiv.org/abs/2501.01793)|**[link](https://github.com/mohdkhalil/repository-supplementary-for-lak-25-paper--creating-artificial-students-that-never-existed)**|
|**2025-01-03**|**Efficient LLM Inference with Activation Checkpointing and Hybrid Caching**|Sanghyeon Lee et.al.|[2501.01792](http://arxiv.org/abs/2501.01792)|null|
|**2025-01-03**|**SaLoRA: Safety-Alignment Preserved Low-Rank Adaptation**|Mingjie Li et.al.|[2501.01765](http://arxiv.org/abs/2501.01765)|null|
|**2025-01-02**|**Unifying Specialized Visual Encoders for Video Language Models**|Jihoon Chung et.al.|[2501.01426](http://arxiv.org/abs/2501.01426)|**[link](https://github.com/princetonvisualai/merv)**|
|**2025-01-02**|**Aligning Large Language Models for Faithful Integrity Against Opposing Argument**|Yong Zhao et.al.|[2501.01336](http://arxiv.org/abs/2501.01336)|**[link](https://github.com/zhaoy777/afice)**|
|**2025-01-02**|**CySecBench: Generative AI-based CyberSecurity-focused Prompt Dataset for Benchmarking Large Language Models**|Johan Wahréus et.al.|[2501.01335](http://arxiv.org/abs/2501.01335)|**[link](https://github.com/cysecbench/dataset)**|
|**2025-01-02**|**Decoding Knowledge in Large Language Models: A Framework for Categorization and Comprehension**|Yanbo Fang et.al.|[2501.01332](http://arxiv.org/abs/2501.01332)|null|
|**2025-01-02**|**The Prompt Alchemist: Automated LLM-Tailored Prompt Optimization for Test Case Generation**|Shuzheng Gao et.al.|[2501.01329](http://arxiv.org/abs/2501.01329)|null|
|**2025-01-02**|**Think More, Hallucinate Less: Mitigating Hallucinations via Dual Process of Fast and Slow Thinking**|Xiaoxue Cheng et.al.|[2501.01306](http://arxiv.org/abs/2501.01306)|null|
|**2025-01-02**|**Large Language Models for Mental Health Diagnostic Assessments: Exploring The Potential of Large Language Models for Assisting with Mental Health Diagnostic Assessments -- The Depression and Anxiety Case**|Kaushik Roy et.al.|[2501.01305](http://arxiv.org/abs/2501.01305)|null|
|**2025-01-02**|**Does a Large Language Model Really Speak in Human-Like Language?**|Mose Park et.al.|[2501.01273](http://arxiv.org/abs/2501.01273)|null|
|**2025-01-02**|**ProgCo: Program Helps Self-Correction of Large Language Models**|Xiaoshuai Song et.al.|[2501.01264](http://arxiv.org/abs/2501.01264)|null|
|**2025-01-02**|**CodeElo: Benchmarking Competition-level Code Generation of LLMs with Human-comparable Elo Ratings**|Shanghaoran Quan et.al.|[2501.01257](http://arxiv.org/abs/2501.01257)|null|
|**2024-12-30**|**Distributed Mixture-of-Agents for Edge Inference with Large Language Models**|Purbesh Mitra et.al.|[2412.21200](http://arxiv.org/abs/2412.21200)|**[link](https://github.com/purbeshmitra/distributed_moa)**|
|**2024-12-30**|**Facilitating large language model Russian adaptation with Learned Embedding Propagation**|Mikhail Tikhomirov et.al.|[2412.21140](http://arxiv.org/abs/2412.21140)|**[link](https://github.com/RefalMachine/llmtf_open)**|
|**2024-12-30**|**ExpShield: Safeguarding Web Text from Unauthorized Crawling and Language Modeling Exploitation**|Ruixuan Liu et.al.|[2412.21123](http://arxiv.org/abs/2412.21123)|null|
|**2024-12-30**|**Toward Intelligent and Secure Cloud: Large Language Model Empowered Proactive Defense**|Yuyang Zhou et.al.|[2412.21051](http://arxiv.org/abs/2412.21051)|**[link](https://github.com/SEU-ProactiveSecurity-Group/LLM-PD)**|
|**2024-12-30**|**TangoFlux: Super Fast and Faithful Text to Audio Generation with Flow Matching and Clap-Ranked Preference Optimization**|Chia-Yu Hung et.al.|[2412.21037](http://arxiv.org/abs/2412.21037)|**[link](https://github.com/declare-lab/TangoFlux)**|
|**2024-12-30**|**MapQaTor: A System for Efficient Annotation of Map Query Datasets**|Mahir Labib Dihan et.al.|[2412.21015](http://arxiv.org/abs/2412.21015)|**[link](https://github.com/MapQaTor/.github/tree/main/profile)**|
|**2024-12-31**|**Verbosity-Aware Rationale Reduction: Effective Reduction of Redundant Rationale via Principled Criteria**|Joonwon Jang et.al.|[2412.21006](http://arxiv.org/abs/2412.21006)|null|
|**2024-12-30**|**Plug-and-Play Training Framework for Preference Optimization**|Jingyuan Ma et.al.|[2412.20996](http://arxiv.org/abs/2412.20996)|null|
|**2024-12-30**|**KARPA: A Training-free Method of Adapting Knowledge Graph as References for Large Language Model's Reasoning Path Aggregation**|Siyuan Fang et.al.|[2412.20995](http://arxiv.org/abs/2412.20995)|null|
|**2024-12-30**|**Efficiently Serving LLM Reasoning Programs with Certaindex**|Yichao Fu et.al.|[2412.20993](http://arxiv.org/abs/2412.20993)|null|
|**2024-12-27**|**Can AI Help with Your Personal Finances?**|Oudom Hean et.al.|[2412.19784](http://arxiv.org/abs/2412.19784)|null|
|**2024-12-27**|**Fortran2CPP: Automating Fortran-to-C++ Migration using LLMs via Multi-Turn Dialogue and Dual-Agent Integration**|Le Chen et.al.|[2412.19770](http://arxiv.org/abs/2412.19770)|**[link](https://github.com/hpc-fortran2cpp/fortran2cpp)**|
|**2024-12-27**|**Can Large Language Models Adapt to Other Agents In-Context?**|Matthew Riemer et.al.|[2412.19726](http://arxiv.org/abs/2412.19726)|null|
|**2024-12-27**|**Toward Adaptive Reasoning in Large Language Models with Thought Rollback**|Sijia Chen et.al.|[2412.19707](http://arxiv.org/abs/2412.19707)|**[link](https://github.com/iQua/llmpebase)**|
|**2024-12-27**|**FreStega: A Plug-and-Play Method for Boosting Imperceptibility and Capacity in Generative Linguistic Steganography for Real-World Scenarios**|Kaiyi Pang et.al.|[2412.19652](http://arxiv.org/abs/2412.19652)|null|
|**2024-12-27**|**IMTP: Search-based Code Generation for In-memory Tensor Programs**|Yongwon Shin et.al.|[2412.19630](http://arxiv.org/abs/2412.19630)|null|
|**2024-12-27**|**Signatures of prediction during natural listening in MEG data?**|Sahel Azizpour et.al.|[2412.19622](http://arxiv.org/abs/2412.19622)|null|
|**2024-12-27**|**Gradient Weight-normalized Low-rank Projection for Efficient LLM Training**|Jia-Hong Huang et.al.|[2412.19616](http://arxiv.org/abs/2412.19616)|**[link](https://github.com/jhhuangkay/gradient-weight-normalized-low-rank-projection-for-efficient-llm-training)**|
|**2024-12-27**|**SocRATES: Towards Automated Scenario-based Testing of Social Navigation Algorithms**|Shashank Rao Marpally et.al.|[2412.19595](http://arxiv.org/abs/2412.19595)|null|
|**2024-12-27**|**Hindsight Planner: A Closed-Loop Few-Shot Planner for Embodied Instruction Following**|Yuxiao Yang et.al.|[2412.19562](http://arxiv.org/abs/2412.19562)|null|
|**2024-12-24**|**Decentralized Intelligence in GameFi: Embodied AI Agents and the Convergence of DeFi and Virtual Ecosystems**|Fernando Jia et.al.|[2412.18601](http://arxiv.org/abs/2412.18601)|**[link](https://github.com/FJDeFi/Decentralized-Intelligence-in-GameFi)**|
|**2024-12-24**|**A Paragraph is All It Takes: Rich Robot Behaviors from Interacting, Trusted LLMs**|OpenMind et.al.|[2412.18588](http://arxiv.org/abs/2412.18588)|null|
|**2024-12-24**|**Zero-resource Speech Translation and Recognition with LLMs**|Karel Mundnich et.al.|[2412.18566](http://arxiv.org/abs/2412.18566)|null|
|**2024-12-24**|**Distilling Fine-grained Sentiment Understanding from Large Language Models**|Yice Zhang et.al.|[2412.18552](http://arxiv.org/abs/2412.18552)|**[link](https://github.com/hitsz-hlt/fsa-distillation)**|
|**2024-12-24**|**Token-Budget-Aware LLM Reasoning**|Tingxu Han et.al.|[2412.18547](http://arxiv.org/abs/2412.18547)|**[link](https://github.com/geniushtx/tale)**|
|**2024-12-24**|**Harnessing Large Language Models for Knowledge Graph Question Answering via Adaptive Multi-Aspect Retrieval-Augmentation**|Derong Xu Xinhang Li et.al.|[2412.18537](http://arxiv.org/abs/2412.18537)|**[link](https://github.com/Applied-Machine-Learning-Lab/AMAR)**|
|**2024-12-24**|**Automated Code Review In Practice**|Umut Cihan et.al.|[2412.18531](http://arxiv.org/abs/2412.18531)|null|
|**2024-12-24**|**Large Language Model guided Deep Reinforcement Learning for Decision Making in Autonomous Driving**|Hao Pang et.al.|[2412.18511](http://arxiv.org/abs/2412.18511)|null|
|**2024-12-24**|**Think or Remember? Detecting and Directing LLMs Towards Memorization or Generalization**|Yi-Fu Fu et.al.|[2412.18497](http://arxiv.org/abs/2412.18497)|null|
|**2024-12-24**|**3DGraphLLM: Combining Semantic Graphs and Large Language Models for 3D Scene Understanding**|Tatiana Zemskova et.al.|[2412.18450](http://arxiv.org/abs/2412.18450)|**[link](https://github.com/cognitiveaisystems/3dgraphllm)**|
|**2024-12-23**|**ResearchTown: Simulator of Human Research Community**|Haofei Yu et.al.|[2412.17767](http://arxiv.org/abs/2412.17767)|**[link](https://github.com/ulab-uiuc/research-town)**|
|**2024-12-23**|**ADC: Enhancing Function Calling Via Adversarial Datasets and Code Line-Level Feedback**|Wei Zhang et.al.|[2412.17754](http://arxiv.org/abs/2412.17754)|null|
|**2024-12-23**|**Deliberation in Latent Space via Differentiable Cache Augmentation**|Luyang Liu et.al.|[2412.17747](http://arxiv.org/abs/2412.17747)|null|
|**2024-12-23**|**YuLan-Mini: An Open Data-efficient Language Model**|Yiwen Hu et.al.|[2412.17743](http://arxiv.org/abs/2412.17743)|**[link](https://github.com/ruc-gsai/yulan-mini)**|
|**2024-12-23**|**Reasoning to Attend: Try to Understand How <SEG> Token Works**|Rui Qian et.al.|[2412.17741](http://arxiv.org/abs/2412.17741)|**[link](https://github.com/rui-qian/read)**|
|**2024-12-23**|**Knowledge Editing through Chain-of-Thought**|Changyue Wang et.al.|[2412.17727](http://arxiv.org/abs/2412.17727)|**[link](https://github.com/bebr2/editcot)**|
|**2024-12-23**|**Large Language Model Safety: A Holistic Survey**|Dan Shi et.al.|[2412.17686](http://arxiv.org/abs/2412.17686)|**[link](https://github.com/tjunlp-lab/awesome-llm-safety-papers)**|
|**2024-12-23**|**Generating Completions for Fragmented Broca's Aphasic Sentences Using Large Language Models**|Sijbren van Vaals et.al.|[2412.17669](http://arxiv.org/abs/2412.17669)|**[link](https://github.com/sijbrenvv/completions_for_broca-s_aphasia)**|
|**2024-12-23**|**Detecting anxiety and depression in dialogues: a multi-label and explainable approach**|Francisco de Arriba-Pérez et.al.|[2412.17651](http://arxiv.org/abs/2412.17651)|null|
|**2024-12-23**|**Tracking the Feature Dynamics in LLM Training: A Mechanistic Study**|Yang Xu et.al.|[2412.17626](http://arxiv.org/abs/2412.17626)|null|
|**2024-12-20**|**HoVLE: Unleashing the Power of Monolithic Vision-Language Models with Holistic Vision-Language Embedding**|Chenxin Tao et.al.|[2412.16158](http://arxiv.org/abs/2412.16158)|null|
|**2024-12-20**|**Offline Reinforcement Learning for LLM Multi-Step Reasoning**|Huaijie Wang et.al.|[2412.16145](http://arxiv.org/abs/2412.16145)|**[link](https://github.com/jwhj/oreo)**|
|**2024-12-20**|**Can LLMs Obfuscate Code? A Systematic Analysis of Large Language Models into Assembly Code Obfuscation**|Seyedreza Mohseni et.al.|[2412.16135](http://arxiv.org/abs/2412.16135)|null|
|**2024-12-20**|**Data-Driven Mechanism Design: Jointly Eliciting Preferences and Information**|Dirk Bergemann et.al.|[2412.16132](http://arxiv.org/abs/2412.16132)|null|
|**2024-12-20**|**PromptOptMe: Error-Aware Prompt Compression for LLM-based MT Evaluation Metrics**|Daniil Larionov et.al.|[2412.16120](http://arxiv.org/abs/2412.16120)|null|
|**2024-12-20**|**Deciphering the Underserved: Benchmarking LLM OCR for Low-Resource Scripts**|Muhammad Abdullah Sohail et.al.|[2412.16119](http://arxiv.org/abs/2412.16119)|**[link](https://github.com/abdullahsohaill/cs6303-researchproject)**|
|**2024-12-20**|**PruneVid: Visual Token Pruning for Efficient Video Large Language Models**|Xiaohu Huang et.al.|[2412.16117](http://arxiv.org/abs/2412.16117)|**[link](https://github.com/visual-ai/prunevid)**|
|**2024-12-20**|**Logical Consistency of Large Language Models in Fact-checking**|Bishwamittra Ghosh et.al.|[2412.16100](http://arxiv.org/abs/2412.16100)|null|
|**2024-12-20**|**The Evolution of LLM Adoption in Industry Data Curation Practices**|Crystal Qian et.al.|[2412.16089](http://arxiv.org/abs/2412.16089)|null|
|**2024-12-20**|**The Only Way is Ethics: A Guide to Ethical Research with Large Language Models**|Eddie L. Ungless et.al.|[2412.16022](http://arxiv.org/abs/2412.16022)|**[link](https://github.com/mxeddie/ethics-whitepaper)**|
|**2024-12-19**|**MMLU-CF: A Contamination-free Multi-task Language Understanding Benchmark**|Qihao Zhao et.al.|[2412.15194](http://arxiv.org/abs/2412.15194)|**[link](https://github.com/microsoft/mmlu-cf)**|
|**2024-12-19**|**LlamaFusion: Adapting Pretrained Language Models for Multimodal Generation**|Weijia Shi et.al.|[2412.15188](http://arxiv.org/abs/2412.15188)|null|
|**2024-12-19**|**HPC-Coder-V2: Studying Code LLMs Across Low-Resource Parallel Languages**|Aman Chaturvedi et.al.|[2412.15178](http://arxiv.org/abs/2412.15178)|null|
|**2024-12-19**|**Critical-Questions-of-Thought: Steering LLM reasoning with Argumentative Querying**|Federico Castagna et.al.|[2412.15177](http://arxiv.org/abs/2412.15177)|**[link](https://github.com/fcast07/cqot)**|
|**2024-12-19**|**Rethinking Uncertainty Estimation in Natural Language Generation**|Lukas Aichberger et.al.|[2412.15176](http://arxiv.org/abs/2412.15176)|null|
|**2024-12-19**|**Language Models as Continuous Self-Evolving Data Engineers**|Peidong Wang et.al.|[2412.15151](http://arxiv.org/abs/2412.15151)|null|
|**2024-12-19**|**Adaptive Pruning for Large Language Models with Structural Importance Awareness**|Haotian Zheng et.al.|[2412.15127](http://arxiv.org/abs/2412.15127)|null|
|**2024-12-19**|**Qwen2.5 Technical Report**|Qwen et.al.|[2412.15115](http://arxiv.org/abs/2412.15115)|**[link](https://github.com/qwenlm/qwen2.5)**|
|**2024-12-19**|**Associative memory inspires improvements for in-context learning using a novel attention residual stream architecture**|Thomas F Burns et.al.|[2412.15113](http://arxiv.org/abs/2412.15113)|**[link](https://github.com/tfburns/amicl-and-residual-attention-streams)**|
|**2024-12-19**|**Review-Then-Refine: A Dynamic Framework for Multi-Hop Question Answering with Temporal Adaptability**|Xiangsen Chen et.al.|[2412.15101](http://arxiv.org/abs/2412.15101)|null|
|**2024-12-18**|**TheAgentCompany: Benchmarking LLM Agents on Consequential Real World Tasks**|Frank F. Xu et.al.|[2412.14161](http://arxiv.org/abs/2412.14161)|**[link](https://github.com/theagentcompany/experiments)**|
|**2024-12-18**|**Advanced Reasoning and Transformation Engine for Multi-Step Insight Synthesis in Data Analytics with Large Language Models**|Atin Sakkeer Hussain et.al.|[2412.14146](http://arxiv.org/abs/2412.14146)|null|
|**2024-12-18**|**LLMs can realize combinatorial creativity: generating creative ideas via LLMs for scientific research**|Tianyang Gu et.al.|[2412.14141](http://arxiv.org/abs/2412.14141)|null|
|**2024-12-18**|**Design choices made by LLM-based test generators prevent them from finding bugs**|Noble Saji Mathews et.al.|[2412.14137](http://arxiv.org/abs/2412.14137)|null|
|**2024-12-18**|**Rango: Adaptive Retrieval-Augmented Proving for Automated Software Verification**|Kyle Thompson et.al.|[2412.14063](http://arxiv.org/abs/2412.14063)|**[link](https://github.com/rkthomps/coq-modeling)**|
|**2024-12-18**|**Understanding and Evaluating Trust in Generative AI and Large Language Models for Spreadsheets**|Simon Thorne et.al.|[2412.14062](http://arxiv.org/abs/2412.14062)|null|
|**2024-12-18**|**A Review of Multimodal Explainable Artificial Intelligence: Past, Present and Future**|Shilin Sun et.al.|[2412.14056](http://arxiv.org/abs/2412.14056)|**[link](https://github.com/shilinsun/mxai_review)**|
|**2024-12-18**|**Digestion Algorithm in Hierarchical Symbolic Forests: A Fast Text Normalization Algorithm and Semantic Parsing Framework for Specific Scenarios and Lightweight Deployment**|Kevin You et.al.|[2412.14054](http://arxiv.org/abs/2412.14054)|null|
|**2024-12-18**|**Cross-Lingual Transfer of Debiasing and Detoxification in Multilingual LLMs: An Extensive Investigation**|Vera Neplenbroek et.al.|[2412.14050](http://arxiv.org/abs/2412.14050)|**[link](https://github.com/veranep/crosslingualdetoxdebias)**|
|**2024-12-18**|**CAD-Recode: Reverse Engineering CAD Code from Point Clouds**|Danila Rukhovich et.al.|[2412.14042](http://arxiv.org/abs/2412.14042)|**[link](https://github.com/filaPro/cad-recode)**|
|**2024-12-17**|**SafeAgentBench: A Benchmark for Safe Task Planning of Embodied LLM Agents**|Sheng Yin et.al.|[2412.13178](http://arxiv.org/abs/2412.13178)|**[link](https://github.com/shengyin1224/safeagentbench)**|
|**2024-12-17**|**DnDScore: Decontextualization and Decomposition for Factuality Verification in Long-Form Text Generation**|Miriam Wanner et.al.|[2412.13175](http://arxiv.org/abs/2412.13175)|null|
|**2024-12-17**|**Algorithmic Fidelity of Large Language Models in Generating Synthetic German Public Opinions: A Case Study**|Bolei Ma et.al.|[2412.13169](http://arxiv.org/abs/2412.13169)|**[link](https://github.com/soda-lmu/llm-opinion-german)**|
|**2024-12-17**|**C-FedRAG: A Confidential Federated Retrieval-Augmented Generation System**|Parker Addison et.al.|[2412.13163](http://arxiv.org/abs/2412.13163)|null|
|**2024-12-17**|**Are Your LLMs Capable of Stable Reasoning?**|Junnan Liu et.al.|[2412.13147](http://arxiv.org/abs/2412.13147)|**[link](https://github.com/open-compass/gpassk)**|
|**2024-12-17**|**AIR-Bench: Automated Heterogeneous Information Retrieval Benchmark**|Jianlyu Chen et.al.|[2412.13102](http://arxiv.org/abs/2412.13102)|**[link](https://github.com/air-bench/air-bench)**|
|**2024-12-17**|**OmniEval: An Omnidirectional and Automatic RAG Evaluation Benchmark in Financial Domain**|Shuting Wang et.al.|[2412.13018](http://arxiv.org/abs/2412.13018)|**[link](https://github.com/ruc-nlpir/omnieval)**|
|**2024-12-17**|**The Emergence of Strategic Reasoning of Large Language Models**|Dongwoo Lee et.al.|[2412.13013](http://arxiv.org/abs/2412.13013)|null|
|**2024-12-17**|**Unlocking LLMs: Addressing Scarce Data and Bias Challenges in Mental Health**|Vivek Kumar et.al.|[2412.12981](http://arxiv.org/abs/2412.12981)|**[link](https://github.com/vsrana-ai/IC-AnnoMI)**|
|**2024-12-17**|**Adaptations of AI models for querying the LandMatrix database in natural language**|Fatiha Ait Kbir et.al.|[2412.12961](http://arxiv.org/abs/2412.12961)|**[link](https://github.com/tetis-nlp/landmatrix-graphql-python)**|
|**2024-12-16**|**SepLLM: Accelerate Large Language Models by Compressing One Segment into One Separator**|Guoxuan Chen et.al.|[2412.12094](http://arxiv.org/abs/2412.12094)|**[link](https://github.com/HKUDS/SepLLM)**|
|**2024-12-16**|**Making FETCH! Happen: Finding Emergent Dog Whistles Through Common Habitats**|Kuleen Sasse et.al.|[2412.12072](http://arxiv.org/abs/2412.12072)|**[link](https://github.com/kuleens/fetch-dog-whistle)**|
|**2024-12-16**|**Can LLM Prompting Serve as a Proxy for Static Analysis in Vulnerability Detection**|Ira Ceka et.al.|[2412.12039](http://arxiv.org/abs/2412.12039)|null|
|**2024-12-16**|**The Open Source Advantage in Large Language Models (LLMs)**|Jiya Manchanda et.al.|[2412.12004](http://arxiv.org/abs/2412.12004)|null|
|**2024-12-16**|**LLM-RG4: Flexible and Factual Radiology Report Generation across Diverse Input Contexts**|Zhuhao Wang et.al.|[2412.12001](http://arxiv.org/abs/2412.12001)|**[link](https://github.com/zh-wang-med/llm-rg4)**|
|**2024-12-16**|**Combining Large Language Models with Tutoring System Intelligence: A Case Study in Caregiver Homework Support**|Devika Venugopalan et.al.|[2412.11995](http://arxiv.org/abs/2412.11995)|**[link](https://github.com/devika-prog/caregiver-conversational-support-tool)**|
|**2024-12-16**|**ExecRepoBench: Multi-level Executable Code Completion Evaluation**|Jian Yang et.al.|[2412.11990](http://arxiv.org/abs/2412.11990)|null|
|**2024-12-16**|**SciFaultyQA: Benchmarking LLMs on Faulty Science Question Detection with a GAN-Inspired Approach to Synthetic Dataset Generation**|Debarshi Kundu et.al.|[2412.11988](http://arxiv.org/abs/2412.11988)|**[link](https://github.com/debarshikundupsu/scifaultyqa)**|
|**2024-12-16**|**Cost-Effective Label-free Node Classification with LLMs**|Taiyan Zhang et.al.|[2412.11983](http://arxiv.org/abs/2412.11983)|null|
|**2024-12-16**|**DARWIN 1.5: Large Language Models as Materials Science Adapted Learners**|Tong Xie et.al.|[2412.11970](http://arxiv.org/abs/2412.11970)|**[link](https://github.com/masterai-eam/darwin)**|
|**2024-12-13**|**UniMed-CLIP: Towards a Unified Image-Text Pretraining Paradigm for Diverse Medical Imaging Modalities**|Muhammad Uzair Khattak et.al.|[2412.10372](http://arxiv.org/abs/2412.10372)|**[link](https://github.com/mbzuai-oryx/unimed-clip)**|
|**2024-12-13**|**Iris: Breaking GUI Complexity with Adaptive Focus and Self-Refining**|Zhiqi Ge et.al.|[2412.10342](http://arxiv.org/abs/2412.10342)|null|
|**2024-12-13**|**AdvPrefix: An Objective for Nuanced LLM Jailbreaks**|Sicheng Zhu et.al.|[2412.10321](http://arxiv.org/abs/2412.10321)|**[link](https://github.com/facebookresearch/jailbreak-objectives)**|
|**2024-12-13**|**One world, one opinion? The superstar effect in LLM responses**|Sofie Goethals et.al.|[2412.10281](http://arxiv.org/abs/2412.10281)|null|
|**2024-12-13**|**Benchmarking Linguistic Diversity of Large Language Models**|Yanzhu Guo et.al.|[2412.10271](http://arxiv.org/abs/2412.10271)|**[link](https://github.com/yanzhuguo/llm-diversity)**|
|**2024-12-13**|**Cultural Evolution of Cooperation among LLM Agents**|Aron Vallinder et.al.|[2412.10270](http://arxiv.org/abs/2412.10270)|null|
|**2024-12-13**|**Does Multiple Choice Have a Future in the Age of Generative AI? A Posttest-only RCT**|Danielle R. Thomas et.al.|[2412.10267](http://arxiv.org/abs/2412.10267)|**[link](https://github.com/cmu-plus/lak2025-advocacy)**|
|**2024-12-13**|**Reasoner Outperforms: Generative Stance Detection with Rationalization for Social Media**|Jiaqing Yuan et.al.|[2412.10266](http://arxiv.org/abs/2412.10266)|null|
|**2024-12-13**|**Targeted Angular Reversal of Weights (TARS) for Knowledge Removal in Large Language Models**|Harry J. Davies et.al.|[2412.10257](http://arxiv.org/abs/2412.10257)|null|
|**2024-12-13**|**Detecting LLM Hallucination Through Layer-wise Information Deficiency: Analysis of Unanswerable Questions and Ambiguous Prompts**|Hazel Kim et.al.|[2412.10246](http://arxiv.org/abs/2412.10246)|null|
|**2024-12-12**|**SynerGen-VL: Towards Synergistic Image Understanding and Generation with Vision Experts and Token Folding**|Hao Li et.al.|[2412.09604](http://arxiv.org/abs/2412.09604)|null|
|**2024-12-12**|**DiverseAgentEntropy: Quantifying Black-Box LLM Uncertainty through Diverse Perspectives and Multi-Agent Interaction**|Yu Feng et.al.|[2412.09572](http://arxiv.org/abs/2412.09572)|null|
|**2024-12-12**|**Does Representation Matter? Exploring Intermediate Layers in Large Language Models**|Oscar Skean et.al.|[2412.09563](http://arxiv.org/abs/2412.09563)|null|
|**2024-12-12**|**Foundational Large Language Models for Materials Research**|Vaibhav Mishra et.al.|[2412.09560](http://arxiv.org/abs/2412.09560)|**[link](https://github.com/M3RG-IITD/llamat)**|
|**2024-12-12**|**Can Modern LLMs Act as Agent Cores in Radiology~Environments?**|Qiaoyu Zheng et.al.|[2412.09529](http://arxiv.org/abs/2412.09529)|**[link](https://github.com/magic-ai4med/radabench)**|
|**2024-12-12**|**The Impact of Copyrighted Material on Large Language Models: A Norwegian Perspective**|Javier de la Rosa et.al.|[2412.09460](http://arxiv.org/abs/2412.09460)|null|
|**2024-12-12**|**From Intention To Implementation: Automating Biomedical Research via LLMs**|Yi Luo et.al.|[2412.09429](http://arxiv.org/abs/2412.09429)|null|
|**2024-12-12**|**Unifying AI Tutor Evaluation: An Evaluation Taxonomy for Pedagogical Ability Assessment of LLM-Powered AI Tutors**|Kaushal Kumar Maurya et.al.|[2412.09416](http://arxiv.org/abs/2412.09416)|**[link](https://github.com/kaushal0494/UnifyingAITutorEvaluation)**|
|**2024-12-12**|**AI Predicts AGI: Leveraging AGI Forecasting and Peer Review to Explore LLMs' Complex Reasoning Capabilities**|Fabrizio Davide et.al.|[2412.09385](http://arxiv.org/abs/2412.09385)|null|
|**2024-12-12**|**Delving into Youth Perspectives on In-game Gambling-like Elements: A Proof-of-Concept Study Utilising Large Language Models for Analysing User-Generated Text Data**|Thomas Krause et.al.|[2412.09345](http://arxiv.org/abs/2412.09345)|null|
|**2024-12-11**|**Generative Semantic Communication: Architectures, Technologies, and Applications**|Jinke Ren et.al.|[2412.08642](http://arxiv.org/abs/2412.08642)|null|
|**2024-12-11**|**Fast Prompt Alignment for Text-to-Image Generation**|Khalil Mrini et.al.|[2412.08639](http://arxiv.org/abs/2412.08639)|**[link](https://github.com/tiktok/fast_prompt_alignment)**|
|**2024-12-11**|**Synthetic Vision: Training Vision-Language Models to Understand Physics**|Vahid Balazadeh et.al.|[2412.08619](http://arxiv.org/abs/2412.08619)|null|
|**2024-12-11**|**Exploiting the Index Gradients for Optimization-Based Jailbreaking on Large Language Models**|Jiahui Li et.al.|[2412.08615](http://arxiv.org/abs/2412.08615)|**[link](https://github.com/jiah-li/magic)**|
|**2024-12-11**|**Preference Discerning with LLM-Enhanced Generative Retrieval**|Fabian Paischer et.al.|[2412.08604](http://arxiv.org/abs/2412.08604)|null|
|**2024-12-11**|**Leveraging Graph-RAG and Prompt Engineering to Enhance LLM-Based Automated Requirement Traceability and Compliance Checks**|Arsalan Masoudifard et.al.|[2412.08593](http://arxiv.org/abs/2412.08593)|null|
|**2024-12-11**|**Advancing Single- and Multi-task Text Classification through Large Language Model Fine-tuning**|Hang Zhao et.al.|[2412.08587](http://arxiv.org/abs/2412.08587)|null|
|**2024-12-11**|**TURBOATTENTION: Efficient Attention Approximation For High Throughputs LLMs**|Hao Kang et.al.|[2412.08585](http://arxiv.org/abs/2412.08585)|null|
|**2024-12-11**|**MaestroMotif: Skill Design from Artificial Intelligence Feedback**|Martin Klissarov et.al.|[2412.08542](http://arxiv.org/abs/2412.08542)|null|
|**2024-12-11**|**EMS: Adaptive Evict-then-Merge Strategy for Head-wise KV Cache Compression Based on Global-Local Importance**|Yingxin Li et.al.|[2412.08521](http://arxiv.org/abs/2412.08521)|null|
|**2024-12-10**|**Zero-Shot ATC Coding with Large Language Models for Clinical Assessments**|Zijian Chen et.al.|[2412.07743](http://arxiv.org/abs/2412.07743)|null|
|**2024-12-10**|**Granite Guardian**|Inkit Padhi et.al.|[2412.07724](http://arxiv.org/abs/2412.07724)|**[link](https://github.com/ibm-granite/granite-guardian)**|
|**2024-12-10**|**Privacy-Preserving Customer Support: A Framework for Secure and Scalable Interactions**|Anant Prakash Awasthi et.al.|[2412.07687](http://arxiv.org/abs/2412.07687)|null|
|**2024-12-10**|**TRIM: Token Reduction and Inference Modeling for Cost-Effective Language Generation**|Alfredo Garrachón Ruiz et.al.|[2412.07682](http://arxiv.org/abs/2412.07682)|null|
|**2024-12-10**|**Ask Humans or AI? Exploring Their Roles in Visualization Troubleshooting**|Shuyu Shen et.al.|[2412.07673](http://arxiv.org/abs/2412.07673)|**[link](https://github.com/HKUSTDial/vistroubleshooting.github.io)**|
|**2024-12-10**|**FlexLLM: Exploring LLM Customization for Moving Target Defense on Black-Box LLMs Against Jailbreak Attacks**|Bocheng Chen et.al.|[2412.07672](http://arxiv.org/abs/2412.07672)|null|
|**2024-12-10**|**Automating Business Intelligence Requirements with Generative AI and Semantic Search**|Nimrod Busany et.al.|[2412.07668](http://arxiv.org/abs/2412.07668)|null|
|**2024-12-10**|**Searching for Structure: Investigating Emergent Communication with Large Language Models**|Tom Kouwenhoven et.al.|[2412.07646](http://arxiv.org/abs/2412.07646)|null|
|**2024-12-10**|**TrojanWhisper: Evaluating Pre-trained LLMs to Detect and Localize Hardware Trojans**|Md Omar Faruque et.al.|[2412.07636](http://arxiv.org/abs/2412.07636)|null|
|**2024-12-10**|**ChocoLlama: Lessons Learned From Teaching Llamas Dutch**|Matthieu Meeus et.al.|[2412.07633](http://arxiv.org/abs/2412.07633)|null|
|**2024-12-09**|**Training Large Language Models to Reason in a Continuous Latent Space**|Shibo Hao et.al.|[2412.06769](http://arxiv.org/abs/2412.06769)|null|
|**2024-12-09**|**Why Do Developers Engage with ChatGPT in Issue-Tracker? Investigating Usage and Reliance on ChatGPT-Generated Code**|Joy Krishan Das et.al.|[2412.06757](http://arxiv.org/abs/2412.06757)|null|
|**2024-12-09**|**JAPAGEN: Efficient Few/Zero-shot Learning via Japanese Training Dataset Generation with LLM**|Takuro Fujii et.al.|[2412.06738](http://arxiv.org/abs/2412.06738)|**[link](https://github.com/retrieva/japagen)**|
|**2024-12-09**|**AutoDCWorkflow: LLM-based Data Cleaning Workflow Auto-Generation and Benchmark**|Lan Li et.al.|[2412.06724](http://arxiv.org/abs/2412.06724)|**[link](https://github.com/LanLi2017/LLM4DC)**|
|**2024-12-09**|**OmniEvalKit: A Modular, Lightweight Toolbox for Evaluating Large Language Model and its Omni-Extensions**|Yi-Kai Zhang et.al.|[2412.06693](http://arxiv.org/abs/2412.06693)|null|
|**2024-12-09**|**Exploring Critical Testing Scenarios for Decision-Making Policies: An LLM Approach**|Weichao Xu et.al.|[2412.06684](http://arxiv.org/abs/2412.06684)|null|
|**2024-12-09**|**Toward LLM-Agent-Based Modeling of Transportation Systems: A Conceptual Framework**|Tianming Liu et.al.|[2412.06681](http://arxiv.org/abs/2412.06681)|null|
|**2024-12-09**|**Chatbots im Schulunterricht: Wir testen das Fobizz-Tool zur automatischen Bewertung von Hausaufgaben**|Rainer Mühlhoff et.al.|[2412.06651](http://arxiv.org/abs/2412.06651)|null|
|**2024-12-09**|**Anchoring Bias in Large Language Models: An Experimental Study**|Jiaxu Lou et.al.|[2412.06593](http://arxiv.org/abs/2412.06593)|null|
|**2024-12-09**|**Data Quality Enhancement on the Basis of Diversity with Large Language Models for Text Classification: Uncovered, Difficult, and Noisy**|Min Zeng et.al.|[2412.06575](http://arxiv.org/abs/2412.06575)|null|
|**2024-12-06**|**APOLLO: SGD-like Memory, AdamW-level Performance**|Hanqing Zhu et.al.|[2412.05270](http://arxiv.org/abs/2412.05270)|**[link](https://github.com/zhuhanqing/APOLLO)**|
|**2024-12-06**|**CompCap: Improving Multimodal Large Language Models with Composite Captions**|Xiaohui Chen et.al.|[2412.05243](http://arxiv.org/abs/2412.05243)|null|
|**2024-12-06**|**BEExformer: A Fast Inferencing Transformer Architecture via Binarization with Multiple Early Exits**|Wazib Ansar et.al.|[2412.05225](http://arxiv.org/abs/2412.05225)|null|
|**2024-12-06**|**100% Hallucination Elimination Using Acurai**|Michael C. Wood et.al.|[2412.05223](http://arxiv.org/abs/2412.05223)|**[link](https://github.com/AcuChat/acurai-RAGTruth-conflict-resolution)**|
|**2024-12-06**|**A Survey of Large Language Model-Based Generative AI for Text-to-SQL: Benchmarks, Applications, Use Cases, and Challenges**|Aditi Singh et.al.|[2412.05208](http://arxiv.org/abs/2412.05208)|null|
|**2024-12-06**|**Are Frontier Large Language Models Suitable for Q&A in Science Centres?**|Jacob Watson et.al.|[2412.05200](http://arxiv.org/abs/2412.05200)|null|
|**2024-12-06**|**SurgBox: Agent-Driven Operating Room Sandbox with Surgery Copilot**|Jinlin Wu et.al.|[2412.05187](http://arxiv.org/abs/2412.05187)|**[link](https://github.com/franciszchen/surgbox)**|
|**2024-12-06**|**LinVT: Empower Your Image-level Large Language Model to Understand Videos**|Lishuai Gao et.al.|[2412.05185](http://arxiv.org/abs/2412.05185)|**[link](https://github.com/gls0425/linvt)**|
|**2024-12-06**|**QueEn: A Large Language Model for Quechua-English Translation**|Junhao Chen et.al.|[2412.05184](http://arxiv.org/abs/2412.05184)|null|
|**2024-12-06**|**A text-to-tabular approach to generate synthetic patient data using LLMs**|Margaux Tornqvist et.al.|[2412.05153](http://arxiv.org/abs/2412.05153)|**[link](https://github.com/quinten-health-os/synth-data-gen-from-text)**|
|**2024-12-05**|**Divot: Diffusion Powers Video Tokenizer for Comprehension and Generation**|Yuying Ge et.al.|[2412.04432](http://arxiv.org/abs/2412.04432)|**[link](https://github.com/tencentarc/divot)**|
|**2024-12-05**|**Targeting the Core: A Simple and Effective Method to Attack RAG-based Agents via Direct LLM Manipulation**|Xuying Li et.al.|[2412.04415](http://arxiv.org/abs/2412.04415)|null|
|**2024-12-05**|**Retrieval-Augmented Machine Translation with Unstructured Knowledge**|Jiaan Wang et.al.|[2412.04342](http://arxiv.org/abs/2412.04342)|**[link](https://github.com/krystalan/RAGtrans)**|
|**2024-12-05**|**Liquid: Language Models are Scalable Multi-modal Generators**|Junfeng Wu et.al.|[2412.04332](http://arxiv.org/abs/2412.04332)|**[link](https://github.com/foundationvision/liquid)**|
|**2024-12-05**|**The Hyperfitting Phenomenon: Sharpening and Stabilizing LLMs for Open-Ended Text Generation**|Fredrik Carlsson et.al.|[2412.04318](http://arxiv.org/abs/2412.04318)|null|
|**2024-12-05**|**Densing Law of LLMs**|Chaojun Xiao et.al.|[2412.04315](http://arxiv.org/abs/2412.04315)|null|
|**2024-12-05**|**ALMA: Alignment with Minimal Annotation**|Michihiro Yasunaga et.al.|[2412.04305](http://arxiv.org/abs/2412.04305)|null|
|**2024-12-05**|**Evolutionary Pre-Prompt Optimization for Mathematical Reasoning**|Mathurin Videau et.al.|[2412.04291](http://arxiv.org/abs/2412.04291)|null|
|**2024-12-05**|**Arabic Stable LM: Adapting Stable LM 2 1.6B to Arabic**|Zaid Alyafeai et.al.|[2412.04277](http://arxiv.org/abs/2412.04277)|null|
|**2024-12-05**|**PoTable: Programming Standardly on Table-based Reasoning Like a Human Analyst**|Qingyang Mao et.al.|[2412.04272](http://arxiv.org/abs/2412.04272)|null|
|**2024-12-04**|**From Individual to Society: A Survey on Social Simulation Driven by Large Language Model-based Agents**|Xinyi Mou et.al.|[2412.03563](http://arxiv.org/abs/2412.03563)|**[link](https://github.com/fudandisc/socialagent)**|
|**2024-12-04**|**Evaluating Gender Bias Transfer between Pre-trained and Prompt-Adapted Language Models**|Natalie Mackraz et.al.|[2412.03537](http://arxiv.org/abs/2412.03537)|null|
|**2024-12-04**|**A Review on Scientific Knowledge Extraction using Large Language Models in Biomedical Sciences**|Gabriel Lino Garcia et.al.|[2412.03531](http://arxiv.org/abs/2412.03531)|null|
|**2024-12-04**|**You're (Not) My Type -- Can LLMs Generate Feedback of Specific Types for Introductory Programming Tasks?**|Dominic Lohr et.al.|[2412.03516](http://arxiv.org/abs/2412.03516)|null|
|**2024-12-04**|**Training-Free Mitigation of Language Reasoning Degradation After Multimodal Instruction Tuning**|Neale Ratzlaff et.al.|[2412.03467](http://arxiv.org/abs/2412.03467)|null|
|**2024-12-04**|**From Words to Workflows: Automating Business Processes**|Laura Minkova et.al.|[2412.03446](http://arxiv.org/abs/2412.03446)|null|
|**2024-12-04**|**RedStone: Curating General, Code, Math, and QA Data for Large Language Models**|Yaoyao Chang et.al.|[2412.03398](http://arxiv.org/abs/2412.03398)|null|
|**2024-12-04**|**WiS Platform: Enhancing Evaluation of LLM-Based Multi-Agent Systems Through Game-Based Analysis**|Chengwei Hu et.al.|[2412.03359](http://arxiv.org/abs/2412.03359)|null|
|**2024-12-04**|**Improving Linguistic Diversity of Large Language Models with Possibility Exploration Fine-Tuning**|Long Mai et.al.|[2412.03343](http://arxiv.org/abs/2412.03343)|**[link](https://github.com/mailong25/peft_diversity)**|
|**2024-12-04**|**AI-Driven Day-to-Day Route Choice**|Leizhen Wang et.al.|[2412.03338](http://arxiv.org/abs/2412.03338)|**[link](https://github.com/georgewanglz2019/LLMTraveler)**|
|**2024-12-03**|**T-REG: Preference Optimization with Token-Level Reward Regularization**|Wenxuan Zhou et.al.|[2412.02685](http://arxiv.org/abs/2412.02685)|null|
|**2024-12-03**|**Mind the Gap: Examining the Self-Improvement Capabilities of Large Language Models**|Yuda Song et.al.|[2412.02674](http://arxiv.org/abs/2412.02674)|null|
|**2024-12-03**|**LLM-Enhanced Path Planning: Safe and Efficient Autonomous Navigation with Instructional Inputs**|Pranav Doma et.al.|[2412.02655](http://arxiv.org/abs/2412.02655)|null|
|**2024-12-03**|**Time-Reversal Provides Unsupervised Feedback to LLMs**|Yerram Varun et.al.|[2412.02626](http://arxiv.org/abs/2412.02626)|null|
|**2024-12-03**|**CEGI: Measuring the trade-off between efficiency and carbon emissions for SLMs and VLMs**|Abhas Kumar et.al.|[2412.02602](http://arxiv.org/abs/2412.02602)|null|
|**2024-12-03**|**PrefixLLM: LLM-aided Prefix Circuit Design**|Weihua Xiao et.al.|[2412.02594](http://arxiv.org/abs/2412.02594)|null|
|**2024-12-03**|**OCR Hinders RAG: Evaluating the Cascading Impact of OCR on Retrieval-Augmented Generation**|Junyuan Zhang et.al.|[2412.02592](http://arxiv.org/abs/2412.02592)|**[link](https://github.com/opendatalab/OHR-Bench)**|
|**2024-12-03**|**Semantic Tokens in Retrieval Augmented Generation**|Joel Suro et.al.|[2412.02563](http://arxiv.org/abs/2412.02563)|null|
|**2024-12-03**|**Patent-CR: A Dataset for Patent Claim Revision**|Lekang Jiang et.al.|[2412.02549](http://arxiv.org/abs/2412.02549)|null|
|**2024-12-03**|**LLMForecaster: Improving Seasonal Event Forecasts with Unstructured Textual Data**|Hanyu Zhang et.al.|[2412.02525](http://arxiv.org/abs/2412.02525)|null|
|**2024-12-02**|**Critical Tokens Matter: Token-Level Contrastive Estimation Enhances LLM's Reasoning Capability**|Zicheng Lin et.al.|[2411.19943](http://arxiv.org/abs/2411.19943)|null|
|**2024-11-29**|**SIMS: Simulating Human-Scene Interactions with Real World Script Planning**|Wenjia Wang et.al.|[2411.19921](http://arxiv.org/abs/2411.19921)|null|
|**2024-11-29**|**PDDLFuse: A Tool for Generating Diverse Planning Domains**|Vedant Khandelwal et.al.|[2411.19886](http://arxiv.org/abs/2411.19886)|null|
|**2024-12-02**|**LUMIA: Linear probing for Unimodal and MultiModal Membership Inference Attacks leveraging internal LLM states**|Luis Ibanez-Lissen et.al.|[2411.19876](http://arxiv.org/abs/2411.19876)|null|
|**2024-11-29**|**AIDetx: a compression-based method for identification of machine-learning generated text**|Leonardo Almeida et.al.|[2411.19869](http://arxiv.org/abs/2411.19869)|**[link](https://github.com/aidetx/aidetx)**|
|**2024-11-29**|**Reverse Thinking Makes LLMs Stronger Reasoners**|Justin Chih-Yao Chen et.al.|[2411.19865](http://arxiv.org/abs/2411.19865)|null|
|**2024-11-29**|**Cross-Domain Recommendation Meets Large Language Models**|Ajay Krishna Vajjala et.al.|[2411.19862](http://arxiv.org/abs/2411.19862)|**[link](https://github.com/ajaykv1/CDR_Meets_LLMs)**|
|**2024-11-29**|**Sensitive Content Classification in Social Media: A Holistic Resource and Evaluation**|Dimosthenis Antypas et.al.|[2411.19832](http://arxiv.org/abs/2411.19832)|null|
|**2024-11-29**|**Advanced System Integration: Analyzing OpenAPI Chunking for Retrieval-Augmented Generation**|Robin D. Pesl et.al.|[2411.19804](http://arxiv.org/abs/2411.19804)|null|
|**2024-11-29**|**INCLUDE: Evaluating Multilingual Language Understanding with Regional Knowledge**|Angelika Romanou et.al.|[2411.19799](http://arxiv.org/abs/2411.19799)|null|
|**2024-11-27**|**Automated Literature Review Using NLP Techniques and LLM-Based Retrieval-Augmented Generation**|Nurshat Fateh Ali et.al.|[2411.18583](http://arxiv.org/abs/2411.18583)|null|
|**2024-11-27**|**Challenges in Adapting Multilingual LLMs to Low-Resource Languages using LoRA PEFT Tuning**|Omkar Khade et.al.|[2411.18571](http://arxiv.org/abs/2411.18571)|null|
|**2024-11-27**|**A Pipeline of Neural-Symbolic Integration to Enhance Spatial Reasoning in Large Language Models**|Rong Wang et.al.|[2411.18564](http://arxiv.org/abs/2411.18564)|null|
|**2024-11-27**|**LLM-ABBA: Understand time series via symbolic approximation**|Erin Carson et.al.|[2411.18506](http://arxiv.org/abs/2411.18506)|null|
|**2024-11-27**|**Beyond Examples: High-level Automated Reasoning Paradigm in In-Context Learning via MCTS**|Jinyang Wu et.al.|[2411.18478](http://arxiv.org/abs/2411.18478)|null|
|**2024-11-27**|**Is my Meeting Summary Good? Estimating Quality with a Multi-LLM Evaluator**|Frederic Kirstein et.al.|[2411.18444](http://arxiv.org/abs/2411.18444)|null|
|**2024-11-27**|**FastSwitch: Optimizing Context Switching Efficiency in Fairness-aware Large Language Model Serving**|Ao Shen et.al.|[2411.18424](http://arxiv.org/abs/2411.18424)|null|
|**2024-11-27**|**ChatGPT as speechwriter for the French presidents**|Dominique Labbé et.al.|[2411.18382](http://arxiv.org/abs/2411.18382)|null|
|**2024-11-27**|**GPT as ghostwriter at the White House**|Jacques Savoy et.al.|[2411.18365](http://arxiv.org/abs/2411.18365)|null|
|**2024-11-27**|**Can LLMs assist with Ambiguity? A Quantitative Evaluation of various Large Language Models on Word Sense Disambiguation**|T. G. D. K. Sumanathilaka et.al.|[2411.18337](http://arxiv.org/abs/2411.18337)|null|
|**2024-11-26**|**Adaptive Deployment of Untrusted LLMs Reduces Distributed Threats**|Jiaxin Wen et.al.|[2411.17693](http://arxiv.org/abs/2411.17693)|null|
|**2024-11-26**|**Low-Bit Quantization Favors Undertrained LLMs: Scaling Laws for Quantized LLMs with 100T Training Tokens**|Xu Ouyang et.al.|[2411.17691](http://arxiv.org/abs/2411.17691)|null|
|**2024-11-26**|**Enhancing Character-Level Understanding in LLMs through Token Internal Structure Learning**|Zhu Xu et.al.|[2411.17679](http://arxiv.org/abs/2411.17679)|**[link](https://github.com/FloatFrank/TIPA)**|
|**2024-11-26**|**SketchAgent: Language-Driven Sequential Sketch Generation**|Yael Vinker et.al.|[2411.17673](http://arxiv.org/abs/2411.17673)|null|
|**2024-11-26**|**Synthetic Data Generation with LLM for Improved Depression Prediction**|Andrea Kang et.al.|[2411.17672](http://arxiv.org/abs/2411.17672)|null|
|**2024-11-26**|**Toward High-Performance LLM Serving: A Simulation-Based Approach for Identifying Optimal Parallelism**|Yi-Chien Lin et.al.|[2411.17651](http://arxiv.org/abs/2411.17651)|null|
|**2024-11-26**|**On Limitations of LLM as Annotator for Low Resource Languages**|Suramya Jadhav et.al.|[2411.17637](http://arxiv.org/abs/2411.17637)|null|
|**2024-11-26**|**MALMM: Multi-Agent Large Language Models for Zero-Shot Robotics Manipulation**|Harsh Singh et.al.|[2411.17636](http://arxiv.org/abs/2411.17636)|null|
|**2024-11-26**|**Data-driven development of cycle prediction models for lithium metal batteries using multi modal mining**|Jaewoong Lee et.al.|[2411.17625](http://arxiv.org/abs/2411.17625)|null|
|**2024-11-26**|**Scaling Speech-Text Pre-training with Synthetic Interleaved Data**|Aohan Zeng et.al.|[2411.17607](http://arxiv.org/abs/2411.17607)|null|
|**2024-11-25**|**Do Large Language Models Perform Latent Multi-Hop Reasoning without Exploiting Shortcuts?**|Sohee Yang et.al.|[2411.16679](http://arxiv.org/abs/2411.16679)|null|
|**2024-11-25**|**DreamRunner: Fine-Grained Storytelling Video Generation with Retrieval-Augmented Motion Adaptation**|Zun Wang et.al.|[2411.16657](http://arxiv.org/abs/2411.16657)|null|
|**2024-11-25**|**Self-Generated Critiques Boost Reward Modeling for Language Models**|Yue Yu et.al.|[2411.16646](http://arxiv.org/abs/2411.16646)|null|
|**2024-11-25**|**Chat2SVG: Vector Graphics Generation with Large Language Models and Image Diffusion Models**|Ronghuan Wu et.al.|[2411.16602](http://arxiv.org/abs/2411.16602)|null|
|**2024-11-25**|**From Generation to Judgment: Opportunities and Challenges of LLM-as-a-judge**|Dawei Li et.al.|[2411.16594](http://arxiv.org/abs/2411.16594)|**[link](https://github.com/llm-as-a-judge/awesome-llm-as-a-judge)**|
|**2024-11-25**|**Large Language Model-based Decision-making for COLREGs and the Control of Autonomous Surface Vehicles**|Klinsmann Agyei et.al.|[2411.16587](http://arxiv.org/abs/2411.16587)|**[link](https://github.com/Psarhadi/Autonomous_ship_planning_collision_avoidance_control)**|
|**2024-11-25**|**Enhancing LLM Reasoning via Critique Models with Test-Time and Training-Time Supervision**|Zhiheng Xi et.al.|[2411.16579](http://arxiv.org/abs/2411.16579)|null|
|**2024-11-25**|**EnStack: An Ensemble Stacking Framework of Large Language Models for Enhanced Vulnerability Detection in Source Code**|Shahriyar Zaman Ridoy et.al.|[2411.16561](http://arxiv.org/abs/2411.16561)|null|
|**2024-11-25**|**Generating Out-Of-Distribution Scenarios Using Language Models**|Erfan Aasi et.al.|[2411.16554](http://arxiv.org/abs/2411.16554)|null|
|**2024-11-25**|**Profiling Bias in LLMs: Stereotype Dimensions in Contextual Word Embeddings**|Carolin M. Schuster et.al.|[2411.16527](http://arxiv.org/abs/2411.16527)|null|
|**2024-11-22**|**Measuring Bullshit in the Language Games played by ChatGPT**|Alessandro Trevisan et.al.|[2411.15129](http://arxiv.org/abs/2411.15129)|null|
|**2024-11-22**|**AttriBoT: A Bag of Tricks for Efficiently Approximating Leave-One-Out Context Attribution**|Fengyuan Liu et.al.|[2411.15102](http://arxiv.org/abs/2411.15102)|**[link](https://github.com/r-three/AttriBoT)**|
|**2024-11-22**|**One to rule them all: natural language to bind communication, perception and action**|Simone Colombani et.al.|[2411.15033](http://arxiv.org/abs/2411.15033)|null|
|**2024-11-22**|**FTA generation using GenAI with an Autonomy sensor Usecase**|Sneha Sudhir Shetiya et.al.|[2411.15007](http://arxiv.org/abs/2411.15007)|null|
|**2024-11-22**|**ScribeAgent: Towards Specialized Web Agents Using Production-Scale Workflow Data**|Junhong Shen et.al.|[2411.15004](http://arxiv.org/abs/2411.15004)|**[link](https://github.com/colonylabs/ScribeAgent)**|
|**2024-11-22**|**Generative AI may backfire for counterspeech**|Dominik Bär et.al.|[2411.14986](http://arxiv.org/abs/2411.14986)|null|
|**2024-11-22**|**SwissADT: An Audio Description Translation System for Swiss Languages**|Lukas Fischer et.al.|[2411.14967](http://arxiv.org/abs/2411.14967)|null|
|**2024-11-22**|**GOT4Rec: Graph of Thoughts for Sequential Recommendation**|Zewen Long et.al.|[2411.14922](http://arxiv.org/abs/2411.14922)|null|
|**2024-11-22**|**Task-Aware Robotic Grasping by evaluating Quality Diversity Solutions through Foundation Models**|Aurel X. Appius et.al.|[2411.14917](http://arxiv.org/abs/2411.14917)|null|
|**2024-11-22**|**A Reproducibility and Generalizability Study of Large Language Models for Query Generation**|Moritz Staudinger et.al.|[2411.14914](http://arxiv.org/abs/2411.14914)|null|
|**2024-11-21**|**Insight-V: Exploring Long-Chain Visual Reasoning with Multimodal Large Language Models**|Yuhao Dong et.al.|[2411.14432](http://arxiv.org/abs/2411.14432)|**[link](https://github.com/dongyh20/insight-v)**|
|**2024-11-21**|**Lightweight Safety Guardrails Using Fine-tuned BERT Embeddings**|Aaron Zheng et.al.|[2411.14398](http://arxiv.org/abs/2411.14398)|null|
|**2024-11-21**|**UnifiedCrawl: Aggregated Common Crawl for Affordable Adaptation of LLMs on Low-Resource Languages**|Bethel Melesse Tessema et.al.|[2411.14343](http://arxiv.org/abs/2411.14343)|**[link](https://github.com/bethelmelesse/unifiedcrawl)**|
|**2024-11-21**|**Automated Generation of Code Debugging Exercises**|Victor-Alexandru Pădurean et.al.|[2411.14303](http://arxiv.org/abs/2411.14303)|null|
|**2024-11-21**|**Auto-SPICE: Leveraging LLMs for Dataset Creation via Automated SPICE Netlist Extraction from Analog Circuit Diagrams**|Jitendra Bhandari et.al.|[2411.14299](http://arxiv.org/abs/2411.14299)|**[link](https://github.com/jitendra-bhandari/auto-spice)**|
|**2024-11-21**|**Efficient Aspect-Based Summarization of Climate Change Reports with Small Language Models**|Iacopo Ghinassi et.al.|[2411.14272](http://arxiv.org/abs/2411.14272)|**[link](https://github.com/ighina/llmclimate2024)**|
|**2024-11-21**|**Knowledge Graphs, Large Language Models, and Hallucinations: An NLP Perspective**|Ernests Lavrinovics et.al.|[2411.14258](http://arxiv.org/abs/2411.14258)|null|
|**2024-11-21**|**Generalizing End-To-End Autonomous Driving In Real-World Environments Using Zero-Shot LLMs**|Zeyu Dong et.al.|[2411.14256](http://arxiv.org/abs/2411.14256)|null|
|**2024-11-21**|**Intent-Aware Dialogue Generation and Multi-Task Contrastive Learning for Multi-Turn Intent Classification**|Junhua Liu et.al.|[2411.14252](http://arxiv.org/abs/2411.14252)|null|
|**2024-11-21**|**Natural Language Reinforcement Learning**|Xidong Feng et.al.|[2411.14251](http://arxiv.org/abs/2411.14251)|**[link](https://github.com/waterhorse1/natural-language-rl)**|
|**2024-11-20**|**SpecTool: A Benchmark for Characterizing Errors in Tool-Use LLMs**|Shirley Kokane et.al.|[2411.13547](http://arxiv.org/abs/2411.13547)|null|
|**2024-11-20**|**BALROG: Benchmarking Agentic LLM and VLM Reasoning On Games**|Davide Paglieri et.al.|[2411.13543](http://arxiv.org/abs/2411.13543)|null|
|**2024-11-20**|**Metacognition for Unknown Situations and Environments (MUSE)**|Rodolfo Valiente et.al.|[2411.13537](http://arxiv.org/abs/2411.13537)|null|
|**2024-11-20**|**Disentangling Memory and Reasoning Ability in Large Language Models**|Mingyu Jin et.al.|[2411.13504](http://arxiv.org/abs/2411.13504)|**[link](https://github.com/mingyuj666/disentangling-memory-and-reasoning)**|
|**2024-11-20**|**Utilizing Large Language Models to Synthesize Product Desirability Datasets**|John D. Hastings et.al.|[2411.13485](http://arxiv.org/abs/2411.13485)|null|
|**2024-11-20**|**PatentEdits: Framing Patent Novelty as Textual Entailment**|Ryan Lee et.al.|[2411.13477](http://arxiv.org/abs/2411.13477)|null|
|**2024-11-20**|**When Precision Meets Position: BFloat16 Breaks Down RoPE in Long-Context Training**|Haonan Wang et.al.|[2411.13476](http://arxiv.org/abs/2411.13476)|**[link](https://github.com/haonan3/anchorcontext)**|
|**2024-11-20**|**SoK: A Systems Perspective on Compound AI Threats and Countermeasures**|Sarbartha Banerjee et.al.|[2411.13459](http://arxiv.org/abs/2411.13459)|null|
|**2024-11-20**|**WaterPark: A Robustness Assessment of Language Model Watermarking**|Jiacheng Liang et.al.|[2411.13425](http://arxiv.org/abs/2411.13425)|**[link](https://github.com/JACKPURCELL/sok-llm-watermark)**|
|**2024-11-20**|**Unleashing the Power of Large Language Models for Group POI Recommendations**|Jing Long et.al.|[2411.13415](http://arxiv.org/abs/2411.13415)|null|
|**2024-11-19**|**ACING: Actor-Critic for Instruction Learning in Black-Box Large Language Models**|Salma Kharrat et.al.|[2411.12736](http://arxiv.org/abs/2411.12736)|**[link](https://github.com/salmakh1/ACING)**|
|**2024-11-19**|**When Backdoors Speak: Understanding LLM Backdoor Attacks Through Model-Generated Explanations**|Huaizhi Ge et.al.|[2411.12701](http://arxiv.org/abs/2411.12701)|null|
|**2024-11-19**|**DLBacktrace: A Model Agnostic Explainability for any Deep Learning Models**|Vinay Kumar Sankarapu et.al.|[2411.12643](http://arxiv.org/abs/2411.12643)|**[link](https://github.com/aryaxai/dlbacktrace)**|
|**2024-11-19**|**Improving Controllability and Editability for Pretrained Text-to-Music Generation Models**|Yixiao Zhang et.al.|[2411.12641](http://arxiv.org/abs/2411.12641)|null|
|**2024-11-19**|**AdaCM $^2$ : On Understanding Extremely Long-Term Video with Adaptive Cross-Modality Memory Reduction**|Yuanbin Man et.al.|[2411.12593](http://arxiv.org/abs/2411.12593)|null|
|**2024-11-19**|**Large Language Models for Combinatorial Optimization of Design Structure Matrix**|Shuo Jiang et.al.|[2411.12571](http://arxiv.org/abs/2411.12571)|null|
|**2024-11-19**|**Enhancing Reasoning Capabilities of LLMs via Principled Synthetic Logic Corpus**|Terufumi Morishita et.al.|[2411.12498](http://arxiv.org/abs/2411.12498)|**[link](https://github.com/hitachi-nlp/fld)**|
|**2024-11-19**|**AI Flow at the Network Edge**|Jiawei Shao et.al.|[2411.12469](http://arxiv.org/abs/2411.12469)|null|
|**2024-11-19**|**Guide-to-Explain for Controllable Summarization**|Sangwon Ryu et.al.|[2411.12460](http://arxiv.org/abs/2411.12460)|null|
|**2024-11-19**|**\textsc{Neon}: News Entity-Interaction Extraction for Enhanced Question Answering**|Sneha Singhania et.al.|[2411.12449](http://arxiv.org/abs/2411.12449)|null|
|**2024-11-18**|**Tackling prediction tasks in relational databases with LLMs**|Marek Wydmuch et.al.|[2411.11829](http://arxiv.org/abs/2411.11829)|null|
|**2024-11-18**|**Exploring adversarial robustness of JPEG AI: methodology, comparison and new methods**|Egor Kovalev et.al.|[2411.11795](http://arxiv.org/abs/2411.11795)|null|
|**2024-11-18**|**LLM-IE: A Python Package for Generative Information Extraction with Large Language Models**|Enshuo Hsu et.al.|[2411.11779](http://arxiv.org/abs/2411.11779)|null|
|**2024-11-18**|**sMoRe: Enhancing Object Manipulation and Organization in Mixed Reality Spaces with LLMs and Generative AI**|Yunhao Xing et.al.|[2411.11752](http://arxiv.org/abs/2411.11752)|null|
|**2024-11-18**|**BitMoD: Bit-serial Mixture-of-Datatype LLM Acceleration**|Yuzong Chen et.al.|[2411.11745](http://arxiv.org/abs/2411.11745)|**[link](https://github.com/yc2367/bitmod-hpca-25)**|
|**2024-11-18**|**Moral Persuasion in Large Language Models: Evaluating Susceptibility and Ethical Alignment**|Allison Huang et.al.|[2411.11731](http://arxiv.org/abs/2411.11731)|**[link](https://github.com/acyhuang/moral-persuasion)**|
|**2024-11-18**|**Semantic-Geometric-Physical-Driven Robot Manipulation Skill Transfer via Skill Library and Tactile Representation**|Mingchao Qi et.al.|[2411.11714](http://arxiv.org/abs/2411.11714)|**[link](https://github.com/mingchaoqi/skill_transfer)**|
|**2024-11-18**|**FedCoLLM: A Parameter-Efficient Federated Co-tuning Framework for Large and Small Language Models**|Tao Fan et.al.|[2411.11707](http://arxiv.org/abs/2411.11707)|null|
|**2024-11-18**|**Technical Report: Enhancing LLM Reasoning with Reward-guided Tree Search**|Jinhao Jiang et.al.|[2411.11694](http://arxiv.org/abs/2411.11694)|null|
|**2024-11-18**|**TrojanRobot: Backdoor Attacks Against Robotic Manipulation in the Physical World**|Xianlong Wang et.al.|[2411.11683](http://arxiv.org/abs/2411.11683)|null|
|**2024-11-15**|**Evaluating Creativity and Deception in Large Language Models: A Simulation Framework for Multi-Agent Balderdash**|Parsa Hejabi et.al.|[2411.10422](http://arxiv.org/abs/2411.10422)|**[link](https://github.com/parsahejabi/simulation-framework-for-multi-agent-balderdash)**|
|**2024-11-15**|**Bias Unveiled: Investigating Social Bias in LLM-Generated Code**|Lin Ling et.al.|[2411.10351](http://arxiv.org/abs/2411.10351)|null|
|**2024-11-15**|**Static network structure cannot stabilize cooperation among Large Language Model agents**|Jin Han et.al.|[2411.10294](http://arxiv.org/abs/2411.10294)|null|
|**2024-11-15**|**Scaling Law for Post-training after Model Pruning**|Xiaodong Chen et.al.|[2411.10272](http://arxiv.org/abs/2411.10272)|null|
|**2024-11-15**|**An Empirical Study on LLM-based Agents for Automated Bug Fixing**|Xiangxin Meng et.al.|[2411.10213](http://arxiv.org/abs/2411.10213)|null|
|**2024-11-15**|**Agentic LLMs in the Supply Chain: Towards Autonomous Multi-Agent Consensus-Seeking**|Valeria Jannelli et.al.|[2411.10184](http://arxiv.org/abs/2411.10184)|null|
|**2024-11-15**|**Evaluating the role of `Constitutions' for learning from AI feedback**|Saskia Redgate et.al.|[2411.10168](http://arxiv.org/abs/2411.10168)|null|
|**2024-11-15**|**Compound-QA: A Benchmark for Evaluating LLMs on Compound Questions**|Yutao Hou et.al.|[2411.10163](http://arxiv.org/abs/2411.10163)|null|
|**2024-11-15**|**An Effective Framework to Help Large Language Models Handle Numeric-involved Long-context Tasks**|Yijiong Yu et.al.|[2411.10145](http://arxiv.org/abs/2411.10145)|null|
|**2024-11-15**|**Legal Evalutions and Challenges of Large Language Models**|Jiaqi Wang et.al.|[2411.10137](http://arxiv.org/abs/2411.10137)|null|
|**2024-11-14**|**Squeezed Attention: Accelerating Long Context Length LLM Inference**|Coleman Hooper et.al.|[2411.09688](http://arxiv.org/abs/2411.09688)|**[link](https://github.com/SqueezeAILab/SqueezedAttention)**|
|**2024-11-14**|**Local deployment of large-scale music AI models on commodity hardware**|Xun Zhou et.al.|[2411.09625](http://arxiv.org/abs/2411.09625)|null|
|**2024-11-14**|**PTR: Precision-Driven Tool Recommendation for Large Language Models**|Hang Gao et.al.|[2411.09613](http://arxiv.org/abs/2411.09613)|null|
|**2024-11-14**|**LLaMA-Mesh: Unifying 3D Mesh Generation with Language Models**|Zhengyi Wang et.al.|[2411.09595](http://arxiv.org/abs/2411.09595)|null|
|**2024-11-14**|**Adopting RAG for LLM-Aided Future Vehicle Design**|Vahid Zolfaghari et.al.|[2411.09590](http://arxiv.org/abs/2411.09590)|null|
|**2024-11-14**|**Software Performance Engineering for Foundation Model-Powered Software (FMware)**|Haoxiang Zhang et.al.|[2411.09580](http://arxiv.org/abs/2411.09580)|null|
|**2024-11-14**|**A Practical Guide to Fine-tuning Language Models with Limited Data**|Márton Szép et.al.|[2411.09539](http://arxiv.org/abs/2411.09539)|null|
|**2024-11-14**|**Navigating the Risks: A Survey of Security, Privacy, and Ethics Threats in LLM-Based Agents**|Yuyou Gan et.al.|[2411.09523](http://arxiv.org/abs/2411.09523)|null|
|**2024-11-14**|**Communication Compression for Tensor Parallel LLM Inference**|Jan Hansen-Palmus et.al.|[2411.09510](http://arxiv.org/abs/2411.09510)|null|
|**2024-11-14**|**Spider: Any-to-Many Multimodal LLM**|Jinxiang Lai et.al.|[2411.09439](http://arxiv.org/abs/2411.09439)|null|
|**2024-11-13**|**The Limited Impact of Medical Adaptation of Large Language and Vision-Language Models**|Daniel P. Jeong et.al.|[2411.08870](http://arxiv.org/abs/2411.08870)|**[link](https://github.com/taekb/eval-medical-dapt)**|
|**2024-11-13**|**LLMStinger: Jailbreaking LLMs using RL fine-tuned LLMs**|Piyush Jha et.al.|[2411.08862](http://arxiv.org/abs/2411.08862)|null|
|**2024-11-13**|**Evaluating World Models with LLM for Decision Making**|Chang Yang et.al.|[2411.08794](http://arxiv.org/abs/2411.08794)|null|
|**2024-11-13**|**Separating Tongue from Thought: Activation Patching Reveals Language-Agnostic Concept Representations in Transformers**|Clément Dumas et.al.|[2411.08745](http://arxiv.org/abs/2411.08745)|**[link](https://github.com/butanium/llm-lang-agnostic)**|
|**2024-11-13**|**Dynamic Rewarding with Prompt Optimization Enables Tuning-free Self-Alignment of Language Models**|Somanshu Singla et.al.|[2411.08733](http://arxiv.org/abs/2411.08733)|**[link](https://github.com/Singla17/DRPO)**|
|**2024-11-13**|**Theoretical Analysis of Byte-Pair Encoding**|László Kozma et.al.|[2411.08671](http://arxiv.org/abs/2411.08671)|null|
|**2024-11-13**|**A System Level Performance Evaluation for Superconducting Digital Systems**|Joyjit Kundu et.al.|[2411.08645](http://arxiv.org/abs/2411.08645)|null|
|**2024-11-13**|**Towards Secure Intelligent O-RAN Architecture: Vulnerabilities, Threats and Promising Technical Solutions using LLMs**|Mojdeh Karbalaee Motalleb et.al.|[2411.08640](http://arxiv.org/abs/2411.08640)|null|
|**2024-11-13**|**Practitioners' Discussions on Building LLM-based Applications for Production**|Alina Mailach et.al.|[2411.08574](http://arxiv.org/abs/2411.08574)|null|
|**2024-11-13**|**Leveraging LLMs for Predictive Insights in Food Policy and Behavioral Interventions**|Micha Kaiser et.al.|[2411.08563](http://arxiv.org/abs/2411.08563)|null|
|**2024-11-12**|**Learning with Less: Knowledge Distillation from Large Language Models via Unlabeled Data**|Juanhui Li et.al.|[2411.08028](http://arxiv.org/abs/2411.08028)|null|
|**2024-11-12**|**LLMPhy: Complex Physical Reasoning Using Large Language Models and World Models**|Anoop Cherian et.al.|[2411.08027](http://arxiv.org/abs/2411.08027)|null|
|**2024-11-12**|**Language Models as Causal Effect Generators**|Lucius E. J. Bynum et.al.|[2411.08019](http://arxiv.org/abs/2411.08019)|**[link](https://github.com/lbynum/sequence-driven-scms)**|
|**2024-11-12**|**ExpressivityArena: Can LLMs Express Information Implicitly?**|Joshua Tint et.al.|[2411.08010](http://arxiv.org/abs/2411.08010)|null|
|**2024-11-12**|**Can adversarial attacks by large language models be attributed?**|Manuel Cebrian et.al.|[2411.08003](http://arxiv.org/abs/2411.08003)|null|
|**2024-11-12**|**Derivational Morphology Reveals Analogical Generalization in Large Language Models**|Valentin Hofmann et.al.|[2411.07990](http://arxiv.org/abs/2411.07990)|null|
|**2024-11-12**|**From General to Specific: Utilizing General Hallucation to Automatically Measure the Role Relationship Fidelity for Specific Role-Play Agents**|Chuyi Kong et.al.|[2411.07965](http://arxiv.org/abs/2411.07965)|null|
|**2024-11-12**|**Towards Low-bit Communication for Tensor Parallel LLM Inference**|Harry Dong et.al.|[2411.07942](http://arxiv.org/abs/2411.07942)|null|
|**2024-11-12**|**Leveraging Multimodal Models for Enhanced Neuroimaging Diagnostics in Alzheimer's Disease**|Francesco Chiumento et.al.|[2411.07871](http://arxiv.org/abs/2411.07871)|null|
|**2024-11-12**|**Verbosity $\neq$ Veracity: Demystify Verbosity Compensation Behavior of Large Language Models**|Yusen Zhang et.al.|[2411.07858](http://arxiv.org/abs/2411.07858)|**[link](https://github.com/psunlpgroup/verbosityllm)**|
|**2024-11-11**|**UTMath: Math Evaluation with Unit Test via Reasoning-to-Coding Thoughts**|Bo Yang et.al.|[2411.07240](http://arxiv.org/abs/2411.07240)|**[link](https://github.com/utmathgroup/utmath)**|
|**2024-11-11**|**Tooling or Not Tooling? The Impact of Tools on Language Agents for Chemistry Problem Solving**|Botao Yu et.al.|[2411.07228](http://arxiv.org/abs/2411.07228)|null|
|**2024-11-11**|**Comparing Bottom-Up and Top-Down Steering Approaches on In-Context Learning Tasks**|Madeline Brumley et.al.|[2411.07213](http://arxiv.org/abs/2411.07213)|null|
|**2024-11-11**|**DLCR: A Generative Data Expansion Framework via Diffusion for Clothes-Changing Person Re-ID**|Nyle Siddiqui et.al.|[2411.07205](http://arxiv.org/abs/2411.07205)|**[link](https://github.com/croitorualin/dlcr)**|
|**2024-11-11**|**The Super Weight in Large Language Models**|Mengxia Yu et.al.|[2411.07191](http://arxiv.org/abs/2411.07191)|**[link](https://github.com/mengxiayu/llmsuperweight)**|
|**2024-11-11**|**NatureLM-audio: an Audio-Language Foundation Model for Bioacoustics**|David Robinson et.al.|[2411.07186](http://arxiv.org/abs/2411.07186)|null|
|**2024-11-11**|**A Domain-Agnostic Neurosymbolic Approach for Big Social Data Analysis: Evaluating Mental Health Sentiment on Social Media during COVID-19**|Vedant Khandelwal et.al.|[2411.07163](http://arxiv.org/abs/2411.07163)|null|
|**2024-11-11**|**Chinese SimpleQA: A Chinese Factuality Evaluation for Large Language Models**|Yancheng He et.al.|[2411.07140](http://arxiv.org/abs/2411.07140)|null|
|**2024-11-11**|**Stronger Models are NOT Stronger Teachers for Instruction Tuning**|Zhangchen Xu et.al.|[2411.07133](http://arxiv.org/abs/2411.07133)|null|
|**2024-11-11**|**Benchmarking LLMs' Judgments with No Gold Standard**|Shengwei Xu et.al.|[2411.07127](http://arxiv.org/abs/2411.07127)|**[link](https://github.com/yx-lu/benchmarking-llms--judgments-with-no-gold-standard)**|
|**2024-11-08**|**Recycled Attention: Efficient inference for long-context language models**|Fangyuan Xu et.al.|[2411.05787](http://arxiv.org/abs/2411.05787)|null|
|**2024-11-08**|**Fact or Fiction? Can LLMs be Reliable Annotators for Political Truths?**|Veronica Chatrath et.al.|[2411.05775](http://arxiv.org/abs/2411.05775)|null|
|**2024-11-08**|**Multi-hop Evidence Pursuit Meets the Web: Team Papelo at FEVER 2024**|Christopher Malon et.al.|[2411.05762](http://arxiv.org/abs/2411.05762)|null|
|**2024-11-08**|**Unmasking the Limits of Large Language Models: A Systematic Evaluation of Masked Text Processing Ability through MskQA and MskCal**|Fuka Matsuzaki et.al.|[2411.05665](http://arxiv.org/abs/2411.05665)|**[link](https://github.com/isfhub/maskcode)**|
|**2024-11-08**|**The influence of persona and conversational task on social interactions with a LLM-controlled embodied conversational agent**|Leon O. H. Kroczek et.al.|[2411.05653](http://arxiv.org/abs/2411.05653)|null|
|**2024-11-08**|**LightVA: Lightweight Visual Analytics with LLM Agent-Based Task Planning and Execution**|Yuheng Zhao et.al.|[2411.05651](http://arxiv.org/abs/2411.05651)|null|
|**2024-11-08**|**Evaluating Large Language Model Capability in Vietnamese Fact-Checking Data Generation**|Long Truong To et.al.|[2411.05641](http://arxiv.org/abs/2411.05641)|null|
|**2024-11-08**|**A Two-Step Concept-Based Approach for Enhanced Interpretability and Trust in Skin Lesion Diagnosis**|Cristiano Patrício et.al.|[2411.05609](http://arxiv.org/abs/2411.05609)|**[link](https://github.com/cristianopatricio/2-step-concept-based-skin-diagnosis)**|
|**2024-11-08**|**Evaluating and Adapting Large Language Models to Represent Folktales in Low-Resource Languages**|JA Meaney et.al.|[2411.05593](http://arxiv.org/abs/2411.05593)|null|
|**2024-11-08**|**AcceLLM: Accelerating LLM Inference using Redundancy for Load Balancing and Data Locality**|Ilias Bournias et.al.|[2411.05555](http://arxiv.org/abs/2411.05555)|null|
|**2024-11-07**|**Needle Threading: Can LLMs Follow Threads through Near-Million-Scale Haystacks?**|Jonathan Roberts et.al.|[2411.05000](http://arxiv.org/abs/2411.05000)|null|
|**2024-11-07**|**LLM2CLIP: Powerful Language Model Unlock Richer Visual Representation**|Weiquan Huang et.al.|[2411.04997](http://arxiv.org/abs/2411.04997)|**[link](https://github.com/microsoft/LLM2CLIP)**|
|**2024-11-07**|**Mixture-of-Transformers: A Sparse and Scalable Architecture for Multi-Modal Foundation Models**|Weixin Liang et.al.|[2411.04996](http://arxiv.org/abs/2411.04996)|null|
|**2024-11-07**|**Rethinking Bradley-Terry Models in Preference-Based Reward Modeling: Foundations, Theory, and Alternatives**|Hao Sun et.al.|[2411.04991](http://arxiv.org/abs/2411.04991)|**[link](https://github.com/holarissun/rewardmodelingbeyondbradleyterry)**|
|**2024-11-07**|**Enhancing Reverse Engineering: Investigating and Benchmarking Large Language Models for Vulnerability Analysis in Decompiled Binaries**|Dylan Manuel et.al.|[2411.04981](http://arxiv.org/abs/2411.04981)|null|
|**2024-11-07**|**SuffixDecoding: A Model-Free Approach to Speeding Up Large Language Model Inference**|Gabriele Oliaro et.al.|[2411.04975](http://arxiv.org/abs/2411.04975)|null|
|**2024-11-07**|**BitNet a4.8: 4-bit Activations for 1-bit LLMs**|Hongyu Wang et.al.|[2411.04965](http://arxiv.org/abs/2411.04965)|null|
|**2024-11-07**|**Position Paper On Diagnostic Uncertainty Estimation from Large Language Models: Next-Word Probability Is Not Pre-test Probability**|Yanjun Gao et.al.|[2411.04962](http://arxiv.org/abs/2411.04962)|null|
|**2024-11-07**|**CAD-MLLM: Unifying Multimodality-Conditioned CAD Generation With MLLM**|Jingwei Xu et.al.|[2411.04954](http://arxiv.org/abs/2411.04954)|null|
|**2024-11-07**|**GPTKB: Building Very Large Knowledge Bases from Language Models**|Yujia Hu et.al.|[2411.04920](http://arxiv.org/abs/2411.04920)|**[link](https://github.com/Knowledge-aware-AI/GPTKB)**|
|**2024-11-06**|**Medical Adaptation of Large Language and Vision-Language Models: Are We Making Progress?**|Daniel P. Jeong et.al.|[2411.04118](http://arxiv.org/abs/2411.04118)|**[link](https://github.com/taekb/eval-medical-dapt)**|
|**2024-11-06**|**How Transformers Solve Propositional Logic Problems: A Mechanistic Analysis**|Guan Zhe Hong et.al.|[2411.04105](http://arxiv.org/abs/2411.04105)|null|
|**2024-11-06**|**Beemo: Benchmark of Expert-edited Machine-generated Outputs**|Ekaterina Artemova et.al.|[2411.04032](http://arxiv.org/abs/2411.04032)|null|
|**2024-11-06**|**What Really is Commonsense Knowledge?**|Quyet V. Do et.al.|[2411.03964](http://arxiv.org/abs/2411.03964)|null|
|**2024-11-06**|**How Does A Text Preprocessing Pipeline Affect Ontology Syntactic Matching?**|Zhangcheng Qiang et.al.|[2411.03962](http://arxiv.org/abs/2411.03962)|**[link](https://github.com/qzc438/ontology-llm)**|
|**2024-11-06**|**Fine-Grained Guidance for Retrievers: Leveraging LLMs' Feedback in Retrieval-Augmented Generation**|Yuhang Liu et.al.|[2411.03957](http://arxiv.org/abs/2411.03957)|null|
|**2024-11-06**|**Long-Form Text-to-Music Generation with Adaptive Prompts: A Case of Study in Tabletop Role-Playing Games Soundtracks**|Felipe Marra et.al.|[2411.03948](http://arxiv.org/abs/2411.03948)|**[link](https://github.com/felipemarra/babel-bardo)**|
|**2024-11-06**|**Polynomial Composition Activations: Unleashing the Dynamics of Large Language Models**|Zhijian Zhuo et.al.|[2411.03884](http://arxiv.org/abs/2411.03884)|**[link](https://github.com/brycezhuo/polycom)**|
|**2024-11-06**|**MEG: Medical Knowledge-Augmented Large Language Models for Question Answering**|Laura Cabello et.al.|[2411.03883](http://arxiv.org/abs/2411.03883)|**[link](https://github.com/lautel/meg)**|
|**2024-11-06**|**Data Fusion of Synthetic Query Variants With Generative Large Language Models**|Timo Breuer et.al.|[2411.03881](http://arxiv.org/abs/2411.03881)|**[link](https://github.com/breuert/sigirap24)**|
|**2024-05-16**|**When LLMs step into the 3D World: A Survey and Meta-Analysis of 3D Tasks via Multi-modal Large Language Models**|Xianzheng Ma et.al.|[2405.10255](http://arxiv.org/abs/2405.10255)|**[link](https://github.com/activevisionlab/awesome-llm-3d)**|

<p align=right>(<a href=#updated-on-20250131>back to top</a>)</p>

## moe

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-01-29**|**Heuristic-Informed Mixture of Experts for Link Prediction in Multilayer Networks**|Lucio La Cava et.al.|[2501.17557](http://arxiv.org/abs/2501.17557)|null|多层网络的链接预测算法原则上需要有效地考虑整个层次结构，同时捕捉每一层提供的独特上下文。然而，许多现有方法在某些层中特定链接的预测上表现出色，但在其他层中则表现不佳，因为它们未能有效利用不同网络层编码的多样化信息。在本文中，我们提出了MoE-ML-LP，这是首个专为多层链接预测设计的混合专家（MoE）框架。基于多层链接预测的启发式方法，MoE-ML-LP综合了多个专家的决策，从而显著增强了预测能力。我们在真实世界和合成网络上的广泛实验评估表明，MoE-ML-LP始终优于多个基线和其他竞争方法，在平均倒数排名上提高了60%，Hits@1提高了82%，Hits@5提高了55%，Hits@10提高了41%。此外，MoE-ML-LP具有模块化架构，能够无缝集成新开发的专家而无需重新训练整个框架，促进了效率和可扩展性，为链接预测领域的未来进步铺平了道路。|
|**2025-01-28**|**3D-MoE: A Mixture-of-Experts Multi-modal LLM for 3D Vision and Pose Diffusion via Rectified Flow**|Yueen Ma et.al.|[2501.16698](http://arxiv.org/abs/2501.16698)|null|3D视觉和空间推理在准确感知我们的三维世界方面一直被认为优于基于2D图像的传统视觉推理。由于高质量3D数据收集的困难，该领域的研究直到最近才开始加速。随着强大的大型语言模型（LLM）的出现，过去几年中已经开发出了用于3D视觉的多模态LLM。然而，这些模型大多主要集中在3D数据的视觉编码器上。在这篇论文中，我们提出将现有的密集激活LLM转换为混合专家（MoE）模型，这种模型已被证明在处理多模态数据时非常有效。除了利用这些模型的指令跟随能力外，我们还通过附加一个扩散头Pose-DiT进一步实现了具身任务规划，该扩散头采用了一种新颖的校正流扩散调度程序。在3D问答和任务规划任务上的实验结果表明，我们的3D-MoE框架以较少激活参数实现了性能提升。|
|**2025-01-27**|**MoEVD: Enhancing Vulnerability Detection by Mixture-of-Experts (MoE)**|Xu Yang et.al.|[2501.16454](http://arxiv.org/abs/2501.16454)|null|基于深度学习的漏洞检测（DLVD）技术因其能够从先前被攻击的代码中自动学习漏洞模式而受到了广泛关注。尽管早期工具展示了显著的准确性，但DLVD方法在实际应用中仍面临重大挑战。一个主要问题是“一刀切”的设计，即单一模型被训练来处理所有类型的漏洞。这种方法无法捕捉不同类型漏洞的模式，特别是在训练数据集中代表性不足的少见漏洞类型上表现不佳。为了解决这些挑战，我们提出了MoEVD，它采用了混合专家（Mixture-of-Experts, MoE）框架来进行漏洞检测。MoEVD将漏洞检测分解为两个任务：CWE类型分类和特定于CWE的漏洞检测。通过这种方式，在漏洞检测过程中，MoEVD允许特定的专家处理不同类型的漏洞，而不是用一个模型处理所有漏洞。实验结果表明，MoEVD的F1分数达到了0.44，比所有研究中的最先进（SOTA）基线至少提高了12.8%。MoEVD几乎在所有CWE类型上都表现出色，与最佳SOTA基线相比，召回率提高了9%到77.8%。值得注意的是，MoEVD并没有牺牲对长尾CWE类型的性能；相反，其MoE设计使这些类型的性能（F1分数）至少提高了7.3%，有效解决了长尾问题。|
|**2025-01-27**|**Static Batching of Irregular Workloads on GPUs: Framework and Application to Efficient MoE Model Inference**|Yinghan Li et.al.|[2501.16103](http://arxiv.org/abs/2501.16103)|null|长期以来，如何在大规模并行设备上安排和执行不规则的工作负载一直是个难题。我们提出了一种通用框架，该框架能够将不规则工作负载静态批处理到具有运行时任务映射机制的单个内核中。我们将此框架进一步应用于混合专家（MoE）模型推理，并实现了一个优化且高效的CUDA内核。我们的MoE内核在NVIDIA H800 GPU上达到了高达91%的Tensor Core峰值吞吐量，在NVIDIA H20 GPU上达到了95%。|
|**2025-01-25**|**ToMoE: Converting Dense Large Language Models to Mixture-of-Experts through Dynamic Structural Pruning**|Shangqian Gao et.al.|[2501.15316](http://arxiv.org/abs/2501.15316)|null|大型语言模型（LLM）在处理各种复杂任务方面展现了非凡的能力。然而，这些模型巨大的计算和内存成本给资源受限设备上的部署或高效服务带来了重大挑战。先前的方法试图通过永久移除较不重要的模型结构来缓解这些问题，但这些方法往往由于永久删除模型参数而导致显著的性能下降。在这项工作中，我们尝试通过减少活跃参数的数量而不永久移除它们来减轻这个问题。具体来说，我们引入了一种可微分的动态剪枝方法，该方法通过将密集模型的多层感知机（MLP）层转换为专家混合（MoE）架构，使其保持固定数量的活跃参数。我们的方法即使不进行微调，在包括Phi-2、LLaMA-2、LLaMA-3和Qwen-2.5在内的多种模型家族上也始终优于之前的结构剪枝技术。|
|**2025-01-25**|**Each Rank Could be an Expert: Single-Ranked Mixture of Experts LoRA for Multi-Task Learning**|Ziyu Zhao et.al.|[2501.15103](http://arxiv.org/abs/2501.15103)|null|低秩适应（LoRA）由于其高效性和模块化特性，被广泛用于将大型语言模型（LLMs）适应到特定领域。然而，传统的LoRA在多任务场景中面临任务冲突的问题。近期的研究通过采用混合专家（MoE）方法，将每个LoRA模块视为一个专家，从而缓解了任务间的干扰。虽然有效，但这些方法通常将知识隔离在单个任务内，未能充分利用相关任务之间的共享知识。在本文中，我们建立了单个LoRA与多LoRA MoE之间的联系，并将其整合到一个统一的框架中。我们证明了多个LoRA的动态路由在功能上等同于单一LoRA中的秩分割和块级激活。进一步的实验证明，在相同的总参数和激活参数约束下，更细粒度的LoRA分割能够带来更好的性能提升，尤其是在异构任务上。基于这些发现，我们提出了单秩混合专家LoRA（SMoRA），它通过将每个秩视为独立专家的方式，将MoE嵌入到LoRA中。借助动态秩级激活机制，SMoRA促进了更细粒度的知识共享，同时减轻了任务冲突。实验表明，SMoRA激活较少的参数却在多任务场景中实现了更好的性能。|
|**2025-01-24**|**Mean-field limit from general mixtures of experts to quantum neural networks**|Anderson Melchor Hernandez et.al.|[2501.14660](http://arxiv.org/abs/2501.14660)|null|在这项工作中，我们研究了通过梯度流在监督学习问题上训练的专家混合模型（MoE）的渐近行为。我们的主要结果建立了当专家数量趋于无穷大时MoE的混沌传播。我们证明了它们参数对应的经验测度接近于一个解非线性连续性方程的概率测度，并提供了一个仅依赖于专家数量的显式收敛速率。我们将结果应用于由量子神经网络生成的MoE。|
|**2025-01-24**|**Hierarchical Time-Aware Mixture of Experts for Multi-Modal Sequential Recommendation**|Shengzhe Zhang et.al.|[2501.14269](http://arxiv.org/abs/2501.14269)|**[link](https://github.com/SStarCCat/HM4SR)**|**多模态序列推荐（SR）通过利用多模态数据来学习比传统SR方法更全面的项目特征和用户偏好，已成为学术界和工业界的一个重要话题。现有方法通常侧重于通过自适应模态融合来增强多模态信息的有效性，以从用户-项目交互序列中捕捉用户偏好的演变。然而，大多数方法忽略了丰富多模态数据中包含的冗余且与兴趣无关的信息造成的干扰。此外，它们主要依赖基于时间顺序的隐式时间信息，而忽视了能够更有效地表示随时间变化的用户兴趣的显式时间信号。为了解决这些局限性，我们提出了一种具有两层专家混合模型（MoE）和多任务学习策略的时间感知多模态序列推荐方法HM4SR。具体来说，第一层MoE，称为交互MoE，从每个项目的多模态数据中提取与用户兴趣相关的重要信息。然后，第二层MoE，称为时间MoE，通过在模态编码中引入来自时间戳的显式时间嵌入来捕捉用户的动态兴趣。为进一步解决数据稀疏问题，我们提出了三个辅助监督任务：用于项目特征理解的序列级类别预测（CP），对ID进行对比学习（IDCL）以使序列上下文与用户兴趣对齐，以及占位符对比学习（PCL）以整合时间信息与模态进行动态兴趣建模。在四个公开数据集上的广泛实验验证了HM4SR相较于几种最先进方法的有效性。**|
|**2025-01-23**|**CSAOT: Cooperative Multi-Agent System for Active Object Tracking**|Hy Nguyen et.al.|[2501.13994](http://arxiv.org/abs/2501.13994)|null|物体跟踪是许多计算机视觉应用中的关键组成部分，例如自主导航、监控和机器人技术。与依赖静态摄像机视角来检测并跟踪连续帧中物体的被动物体跟踪（POT）不同，主动物体跟踪（AOT）需要一个控制器代理主动调整其视角以在复杂环境中保持对移动目标的视觉接触。现有的AOT解决方案主要是基于单个代理的，在动态和复杂的场景中由于信息收集和处理能力有限，常常导致次优决策。为了缓解这些限制，需要开发一种多代理系统，其中不同的代理执行特定的角色并通过协作来增强在动态和复杂环境中的学习能力和鲁棒性。虽然存在一些针对AOT的多代理方法，但它们通常依赖于外部辅助代理，这需要额外的设备，增加了成本。相比之下，我们提出了一种用于主动物体跟踪的协作系统（CSAOT），该方法利用多代理深度强化学习（MADRL）和专家混合（MoE）框架，使多个代理能够在单一设备上运行，从而提高跟踪性能并降低成本。我们的方法增强了对遮挡和快速运动的鲁棒性，同时优化了摄像头移动以延长跟踪时间。我们在具有动态和静态障碍物的各种交互式地图上验证了CSAOT的有效性。|
|**2025-01-22**|**Autonomy-of-Experts Models**|Ang Lv et.al.|[2501.13074](http://arxiv.org/abs/2501.13074)|null|混合专家（MoE）模型主要使用路由器将标记分配给特定的专家模块，仅激活部分参数，并且通常优于密集模型。我们认为路由器的决策与专家执行之间的分离是一个关键但被忽视的问题，导致次优的专家选择和无效的学习。为了解决这个问题，我们提出了一种新的MoE范式——自主专家（AoE），其中专家自主选择处理输入。AoE基于这样的见解：专家能够意识到自己有效处理标记的能力，这种意识反映在其内部激活的规模上。在AoE中，移除了路由器；相反，专家预先计算输入的内部激活，并根据其激活范数进行排名。只有排名靠前的专家继续进行前向传播，而其他专家则停止。通过低秩权重分解减少了预计算激活的开销。这种自我评估然后比较同伴的方法确保了更好的专家选择和有效的学习。我们预训练了从7亿到40亿参数的语言模型，结果表明AoE在具有可比效率的情况下优于传统的MoE模型。|
|**2025-01-22**|**BLR-MoE: Boosted Language-Routing Mixture of Experts for Domain-Robust Multilingual E2E ASR**|Guodong Ma et.al.|[2501.12602](http://arxiv.org/abs/2501.12602)|null|
|**2025-01-21**|**SCFCRC: Simultaneously Counteract Feature Camouflage and Relation Camouflage for Fraud Detection**|Xiaocheng Zhang et.al.|[2501.12430](http://arxiv.org/abs/2501.12430)|null|
|**2025-01-25**|**Parameters vs FLOPs: Scaling Laws for Optimal Sparsity for Mixture-of-Experts Language Models**|Samira Abnar et.al.|[2501.12370](http://arxiv.org/abs/2501.12370)|null|
|**2025-01-21**|**Demons in the Detail: On Implementing Load Balancing Loss for Training Specialized Mixture-of-Expert Models**|Zihan Qiu et.al.|[2501.11873](http://arxiv.org/abs/2501.11873)|null|
|**2025-01-18**|**FSMoE: A Flexible and Scalable Training System for Sparse Mixture-of-Experts Models**|Xinglin Pan et.al.|[2501.10714](http://arxiv.org/abs/2501.10714)|null|
|**2025-01-17**|**OMoE: Diversifying Mixture of Low-Rank Adaptation by Orthogonal Finetuning**|Jinyuan Feng et.al.|[2501.10062](http://arxiv.org/abs/2501.10062)|null|
|**2025-01-17**|**LLM-Based Routing in Mixture of Experts: A Novel Framework for Trading**|Kuan-Ming Liu et.al.|[2501.09636](http://arxiv.org/abs/2501.09636)|null|
|**2025-01-14**|**MiniMax-01: Scaling Foundation Models with Lightning Attention**|MiniMax et.al.|[2501.08313](http://arxiv.org/abs/2501.08313)|null|
|**2025-01-14**|**GRAPHMOE: Amplifying Cognitive Depth of Mixture-of-Experts Network via Introducing Self-Rethinking Mechanism**|Chen Tang et.al.|[2501.07890](http://arxiv.org/abs/2501.07890)|null|
|**2025-01-12**|**Transforming Vision Transformer: Towards Efficient Multi-Task Asynchronous Learning**|Hanwen Zhong et.al.|[2501.06884](http://arxiv.org/abs/2501.06884)|**[link](https://github.com/yewen1486/emtal)**|
|**2025-01-10**|**TAMER: A Test-Time Adaptive MoE-Driven Framework for EHR Representation Learning**|Yinghao Zhu et.al.|[2501.05661](http://arxiv.org/abs/2501.05661)|**[link](https://github.com/yhzhu99/tamer)**|
|**2025-01-09**|**Optimizing Distributed Deployment of Mixture-of-Experts Model Inference in Serverless Computing**|Mengfan Liu et.al.|[2501.05313](http://arxiv.org/abs/2501.05313)|null|
|**2025-01-07**|**LiMoE: Mixture of LiDAR Representation Learners from Automotive Scenes**|Xiang Xu et.al.|[2501.04004](http://arxiv.org/abs/2501.04004)|**[link](https://github.com/xiangxu-0103/limoe)**|
|**2025-01-07**|**mFabric: An Efficient and Scalable Fabric for Mixture-of-Experts Training**|Xudong Liao et.al.|[2501.03905](http://arxiv.org/abs/2501.03905)|null|
|**2025-01-03**|**MoVE-KD: Knowledge Distillation for VLMs with Mixture of Visual Encoders**|Jiajun Cao et.al.|[2501.01709](http://arxiv.org/abs/2501.01709)|null|
|**2024-12-29**|**Multimodal Variational Autoencoder: a Barycentric View**|Peijie Qiu et.al.|[2412.20487](http://arxiv.org/abs/2412.20487)|null|
|**2024-12-28**|**UniRestorer: Universal Image Restoration via Adaptively Estimating Image Degradation at Proper Granularity**|Jingbo Lin et.al.|[2412.20157](http://arxiv.org/abs/2412.20157)|**[link](https://github.com/mrluin/unirestorer)**|
|**2024-12-28**|**Distilled Transformers with Locally Enhanced Global Representations for Face Forgery Detection**|Yaning Zhang et.al.|[2412.20156](http://arxiv.org/abs/2412.20156)|null|
|**2024-12-27**|**DeepSeek-V3 Technical Report**|DeepSeek-AI et.al.|[2412.19437](http://arxiv.org/abs/2412.19437)|**[link](https://github.com/deepseek-ai/deepseek-v3)**|
|**2024-12-26**|**AskChart: Universal Chart Understanding through Textual Enhancement**|Xudong Yang et.al.|[2412.19146](http://arxiv.org/abs/2412.19146)|**[link](https://github.com/sootung/askchart)**|
|**2024-12-30**|**Graph Mixture of Experts and Memory-augmented Routers for Multivariate Time Series Anomaly Detection**|Xiaoyu Huang et.al.|[2412.19108](http://arxiv.org/abs/2412.19108)|null|
|**2024-12-24**|**Modeling the Centaur: Human-Machine Synergy in Sequential Decision Making**|David Shoresh et.al.|[2412.18593](http://arxiv.org/abs/2412.18593)|**[link](https://github.com/ReserveJudgement/Centaur-GPT)**|
|**2024-12-24**|**BIG-MoE: Bypass Isolated Gating MoE for Generalized Multimodal Face Anti-Spoofing**|Yingjie Ma et.al.|[2412.18065](http://arxiv.org/abs/2412.18065)|**[link](https://github.com/murinj/big-moe)**|
|**2024-12-23**|**UME: Upcycling Mixture-of-Experts for Scalable and Efficient Automatic Speech Recognition**|Li Fu et.al.|[2412.17507](http://arxiv.org/abs/2412.17507)|null|
|**2024-12-23**|**BrainMAP: Learning Multiple Activation Pathways in Brain Networks**|Song Wang et.al.|[2412.17404](http://arxiv.org/abs/2412.17404)|null|
|**2024-12-22**|**Part-Of-Speech Sensitivity of Routers in Mixture of Experts Models**|Elie Antoine et.al.|[2412.16971](http://arxiv.org/abs/2412.16971)|null|
|**2024-12-18**|**GraphLoRA: Empowering LLMs Fine-Tuning via Graph Collaboration of MoE**|Ting Bai et.al.|[2412.16216](http://arxiv.org/abs/2412.16216)|null|
|**2024-12-20**|**Theory of Mixture-of-Experts for Mobile Edge Computing**|Hongbo Li et.al.|[2412.15690](http://arxiv.org/abs/2412.15690)|null|
|**2024-12-19**|**MoEtion: Efficient and Reliable Checkpointing for Mixture-of-Experts Models at Scale**|Swapnil Gandhi et.al.|[2412.15411](http://arxiv.org/abs/2412.15411)|null|
|**2024-12-19**|**Qwen2.5 Technical Report**|Qwen et.al.|[2412.15115](http://arxiv.org/abs/2412.15115)|**[link](https://github.com/qwenlm/qwen2.5)**|
|**2024-12-19**|**ReMoE: Fully Differentiable Mixture-of-Experts with ReLU Routing**|Ziteng Wang et.al.|[2412.14711](http://arxiv.org/abs/2412.14711)|**[link](https://github.com/thu-ml/remoe)**|
|**2024-12-18**|**A Survey on Inference Optimization Techniques for Mixture of Experts Models**|Jiacheng Liu et.al.|[2412.14219](http://arxiv.org/abs/2412.14219)|**[link](https://github.com/moe-inf/awesome-moe-inference)**|
|**2024-12-18**|**SEKE: Specialised Experts for Keyword Extraction**|Matej Martinc et.al.|[2412.14087](http://arxiv.org/abs/2412.14087)|**[link](https://github.com/matejmartinc/seke_keyword_extraction)**|
|**2024-12-17**|**CAMEL: Cross-Attention Enhanced Mixture-of-Experts and Language Bias for Code-Switching Speech Recognition**|He Wang et.al.|[2412.12760](http://arxiv.org/abs/2412.12760)|null|
|**2024-12-16**|**Investigating Mixture of Experts in Dense Retrieval**|Effrosyni Sokli et.al.|[2412.11864](http://arxiv.org/abs/2412.11864)|null|
|**2024-12-16**|**Towards Adversarial Robustness of Model-Level Mixture-of-Experts Architectures for Semantic Segmentation**|Svetlana Pavlitska et.al.|[2412.11608](http://arxiv.org/abs/2412.11608)|**[link](https://github.com/kastel-mobilitylab/mixtures-of-experts)**|
|**2024-12-16**|**Enhancing Healthcare Recommendation Systems with a Multimodal LLMs-based MOE Architecture**|Jingyu Xu et.al.|[2412.11557](http://arxiv.org/abs/2412.11557)|null|
|**2024-12-13**|**DeepSeek-VL2: Mixture-of-Experts Vision-Language Models for Advanced Multimodal Understanding**|Zhiyu Wu et.al.|[2412.10302](http://arxiv.org/abs/2412.10302)|**[link](https://github.com/deepseek-ai/deepseek-vl2)**|
|**2024-12-13**|**Llama 3 Meets MoE: Efficient Upcycling**|Aditya Vavre et.al.|[2412.09952](http://arxiv.org/abs/2412.09952)|**[link](https://github.com/NVIDIA/NeMo)**|
|**2024-12-12**|**Towards a Multimodal Large Language Model with Pixel-Level Insight for Biomedicine**|Xiaoshuang Huang et.al.|[2412.09278](http://arxiv.org/abs/2412.09278)|**[link](https://github.com/shawnhuang497/medplib)**|
|**2024-12-10**|**MoE-CAP: Cost-Accuracy-Performance Benchmarking for Mixture-of-Experts Systems**|Yao Fu et.al.|[2412.07067](http://arxiv.org/abs/2412.07067)|null|
|**2024-12-09**|**UniPaint: Unified Space-time Video Inpainting via Mixture-of-Experts**|Zhen Wan et.al.|[2412.06340](http://arxiv.org/abs/2412.06340)|null|
|**2024-12-06**|**Steps are all you need: Rethinking STEM Education with Prompt Engineering**|Krishnasai Addala et.al.|[2412.05023](http://arxiv.org/abs/2412.05023)|null|
|**2024-12-05**|**Meta-Reinforcement Learning With Mixture of Experts for Generalizable Multi Access in Heterogeneous Wireless Networks**|Zhaoyang Liu et.al.|[2412.03850](http://arxiv.org/abs/2412.03850)|null|
|**2024-12-04**|**Convolutional Neural Networks and Mixture of Experts for Intrusion Detection in 5G Networks and beyond**|Loukas Ilias et.al.|[2412.03483](http://arxiv.org/abs/2412.03483)|null|
|**2024-12-05**|**Yi-Lightning Technical Report**|01. AI et.al.|[2412.01253](http://arxiv.org/abs/2412.01253)|null|
|**2024-11-27**|**Mixture of Cache-Conditional Experts for Efficient Mobile Device Inference**|Andrii Skliar et.al.|[2412.00099](http://arxiv.org/abs/2412.00099)|null|
|**2024-11-26**|**Condense, Don't Just Prune: Enhancing Efficiency and Performance in MoE Layer Pruning**|Mingyu Cao et.al.|[2412.00069](http://arxiv.org/abs/2412.00069)|**[link](https://github.com/duterscmy/cd-moe)**|
|**2024-11-27**|**UOE: Unlearning One Expert Is Enough For Mixture-of-experts LLMS**|Haomin Zhuang et.al.|[2411.18797](http://arxiv.org/abs/2411.18797)|null|
|**2024-11-27**|**Complexity Experts are Task-Discriminative Learners for Any Image Restoration**|Eduard Zamfir et.al.|[2411.18466](http://arxiv.org/abs/2411.18466)|null|
|**2024-11-27**|**Mixture of Experts in Image Classification: What's the Sweet Spot?**|Mathurin Videau et.al.|[2411.18322](http://arxiv.org/abs/2411.18322)|null|
|**2024-11-26**|**$H^3$ Fusion: Helpful, Harmless, Honest Fusion of Aligned LLMs**|Selim Furkan Tekin et.al.|[2411.17792](http://arxiv.org/abs/2411.17792)|**[link](https://github.com/sftekin/h3fusion)**|
|**2024-11-25**|**LDACP: Long-Delayed Ad Conversions Prediction Model for Bidding Strategy**|Peng Cui et.al.|[2411.16095](http://arxiv.org/abs/2411.16095)|null|
|**2024-11-24**|**Hiding Communication Cost in Distributed LLM Training via Micro-batch Co-execution**|Haiquan Wang et.al.|[2411.15871](http://arxiv.org/abs/2411.15871)|null|
|**2024-11-24**|**LLaMA-MoE v2: Exploring Sparsity of LLaMA from Perspective of Mixture-of-Experts with Post-Training**|Xiaoye Qu et.al.|[2411.15708](http://arxiv.org/abs/2411.15708)|**[link](https://github.com/opensparsellms/llama-moe-v2)**|
|**2024-11-23**|**Communication-Efficient Sparsely-Activated Model Training via Sequence Migration and Token Condensation**|Fahao Chen et.al.|[2411.15419](http://arxiv.org/abs/2411.15419)|null|
|**2024-11-20**|**MERLOT: A Distilled LLM-based Mixture-of-Experts Framework for Scalable Encrypted Traffic Classification**|Yuxuan Chen et.al.|[2411.13004](http://arxiv.org/abs/2411.13004)|null|
|**2024-11-19**|**Ultra-Sparse Memory Network**|Zihao Huang et.al.|[2411.12364](http://arxiv.org/abs/2411.12364)|null|
|**2024-11-18**|**MoE-Lightning: High-Throughput MoE Inference on Memory-constrained GPUs**|Shiyi Cao et.al.|[2411.11217](http://arxiv.org/abs/2411.11217)|null|
|**2024-11-16**|**Awaker2.5-VL: Stably Scaling MLLMs with Parameter-Efficient Mixture of Experts**|Jinqiang Long et.al.|[2411.10669](http://arxiv.org/abs/2411.10669)|**[link](https://github.com/metabrainagi/awaker)**|
|**2024-11-21**|**Pro-Prophet: A Systematic Load Balancing Method for Efficient Parallel Training of Large-scale MoE Models**|Wei Wang et.al.|[2411.10003](http://arxiv.org/abs/2411.10003)|null|
|**2024-11-13**|**Lynx: Enabling Efficient MoE Inference through Dynamic Batch-Aware Expert Selection**|Vima Gupta et.al.|[2411.08982](http://arxiv.org/abs/2411.08982)|null|
|**2024-11-13**|**Sparse Upcycling: Inference Inefficient Finetuning**|Sasha Doubov et.al.|[2411.08968](http://arxiv.org/abs/2411.08968)|null|
|**2024-11-13**|**LSH-MoE: Communication-efficient MoE Training via Locality-Sensitive Hashing**|Xiaonan Nie et.al.|[2411.08446](http://arxiv.org/abs/2411.08446)|null|
|**2024-11-12**|**PERFT: Parameter-Efficient Routed Fine-Tuning for Mixture-of-Expert Model**|Yilun Liu et.al.|[2411.08212](http://arxiv.org/abs/2411.08212)|null|
|**2024-11-11**|**Adaptive Conditional Expert Selection Network for Multi-domain Recommendation**|Kuiyao Dong et.al.|[2411.06826](http://arxiv.org/abs/2411.06826)|null|
|**2024-11-09**|**Learning Mixtures of Experts with EM**|Quentin Fruytier et.al.|[2411.06056](http://arxiv.org/abs/2411.06056)|null|
|**2024-11-01**|**SLED: Self Logits Evolution Decoding for Improving Factuality in Large Language Models**|Jianyi Zhang et.al.|[2411.02433](http://arxiv.org/abs/2411.02433)|**[link](https://github.com/JayZhang42/SLED)**|
|**2024-11-04**|**FedMoE-DA: Federated Mixture of Experts via Domain Aware Fine-grained Aggregation**|Ziwei Zhan et.al.|[2411.02115](http://arxiv.org/abs/2411.02115)|null|
|**2024-11-03**|**Facet-Aware Multi-Head Mixture-of-Experts Model for Sequential Recommendation**|Mingrui Liu et.al.|[2411.01457](http://arxiv.org/abs/2411.01457)|null|
|**2024-11-06**|**HOBBIT: A Mixed Precision Expert Offloading System for Fast MoE Inference**|Peng Tang et.al.|[2411.01433](http://arxiv.org/abs/2411.01433)|null|
|**2024-11-07**|**HEXA-MoE: Efficient and Heterogeneous-aware MoE Acceleration with ZERO Computation Redundancy**|Shuqing Luo et.al.|[2411.01288](http://arxiv.org/abs/2411.01288)|**[link](https://github.com/unites-lab/hexa-moe)**|
|**2024-11-02**|**PMoL: Parameter Efficient MoE for Preference Mixing of LLM Alignment**|Dongxu Liu et.al.|[2411.01245](http://arxiv.org/abs/2411.01245)|null|
|**2024-11-01**|**MoE-I $^2$ : Compressing Mixture of Experts Models through Inter-Expert Pruning and Intra-Expert Low-Rank Decomposition**|Cheng Yang et.al.|[2411.01016](http://arxiv.org/abs/2411.01016)|null|
|**2024-11-01**|**LIBMoE: A Library for comprehensive benchmarking Mixture of Experts in Large Language Models**|Nam V. Nguyen et.al.|[2411.00918](http://arxiv.org/abs/2411.00918)|**[link](https://github.com/Fsoft-AIC/LibMoE)**|
|**2024-11-01**|**MoNTA: Accelerating Mixture-of-Experts Training with Network-Traffc-Aware Parallel Optimization**|Jingming Guo et.al.|[2411.00662](http://arxiv.org/abs/2411.00662)|**[link](https://github.com/enflametechnology/deepspeed)**|
|**2024-10-31**|**Stereo-Talker: Audio-driven 3D Human Synthesis with Prior-Guided Mixture-of-Experts**|Xiang Deng et.al.|[2410.23836](http://arxiv.org/abs/2410.23836)|null|

<p align=right>(<a href=#updated-on-20250131>back to top</a>)</p>

## SSMs

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-01-28**|**Mamba-Shedder: Post-Transformer Compression for Efficient Selective Structured State Space Models**|J. Pablo Muñoz et.al.|[2501.17088](http://arxiv.org/abs/2501.17088)|**[link](https://github.com/intellabs/hardware-aware-automated-machine-learning)**|**大型预训练模型在序列建模方面取得了显著成果。Transformer块及其注意力机制是这些模型成功的主要驱动力。最近，提出了选择性结构状态空间模型（SSM）等替代架构，以解决Transformer的低效问题。本文探讨了基于SSM模型的压缩，特别是Mamba及其混合模型。我们研究了在不同粒度下移除选定组件对这些模型的影响，以减少模型大小和计算开销，从而在保持准确性的前提下提高效率。提出的解决方案统称为Mamba-Shedder，在推理过程中实现了最高1.4倍的速度提升，表明通过消除一些冗余可以提高模型效率，并且对整体模型性能的影响极小。代码可从https://github.com/IntelLabs/Hardware-Aware-Automated-Machine-Learning获取。**|
|**2025-01-28**|**Post-Training Quantization for Vision Mamba with k-Scaled Quantization and Reparameterization**|Bo-Yun Shi et.al.|[2501.16738](http://arxiv.org/abs/2501.16738)|null|Mamba模型通过使用结构化的状态空间模型（SSM），提供了线性时间复杂度，并展现出巨大的潜力。Vision Mamba (ViM) 通过引入双向SSM和补丁嵌入，将这一框架扩展到视觉任务中，其性能超越了基于Transformer的模型。虽然模型量化对于高效计算至关重要，但现有工作仅集中在原始的Mamba模型上，而未应用于ViM。此外，这些方法忽略了对SSM层进行量化，这是Mamba的核心部分，简单的量化方法由于其内在结构可能会导致显著的误差传播。在本文中，我们专注于ViM的后训练量化(PTQ)。我们通过三种核心技术来解决这些问题：1）一种k缩放的逐令牌量化方法，用于线性和卷积层；2）一种重新参数化技术，简化隐藏状态的量化；3）一种因子确定方法，通过整合操作减少计算开销。通过这些方法，可以减轻由PTQ引起的误差。在ImageNet-1k上的实验结果表明，由于PTQ导致的准确率下降仅为0.8-1.2%，这突显了我们方法的有效性。|
|**2025-01-27**|**Mixture-of-Mamba: Enhancing Multi-Modal State-Space Models with Modality-Aware Sparsity**|Weixin Liang et.al.|[2501.16295](http://arxiv.org/abs/2501.16295)|**[link](https://github.com/weixin-liang/mixture-of-mamba)**|**状态空间模型（SSM）作为序列建模的有效替代方案，已经崭露头角，但它们无法利用特定模态的特征，这限制了其在多模态预训练中的性能。本文提出了Mixture-of-Mamba，这是一种新的SSM架构，通过特定模态参数化Mamba块引入模态感知稀疏性。基于Mixture-of-Transformers（W. Liang等，arXiv:2411.04996；2024），我们将模态感知稀疏性的优势扩展到SSM中，同时保持其计算效率。我们在三个多模态预训练设置下评估了Mixture-of-Mamba：Transfusion（交织文本和连续图像标记，并采用扩散损失）、Chameleon（交织文本和离散图像标记）以及一个扩展的三模态框架，该框架还包括语音。Mixture-of-Mamba在较早的训练步骤中持续达到相同的损失值，并且显著降低了计算成本。在Transfusion设置下，Mixture-of-Mamba仅使用34.76%的训练FLOPs就达到了相当的图像损失（1.4B规模）。在Chameleon设置下，Mixture-of-Mamba仅用42.50%的FLOPs就达到了类似的图像损失（1.4B规模），并且仅用65.40%的FLOPs就达到了相似的文本损失。在三模态设置下，MoM仅用24.80%的FLOPs就匹配到了语音损失（1.4B规模）。我们的消融研究表明，解耦投影组件具有协同效应，联合解耦比单独修改带来更大的增益。这些结果确立了模态感知稀疏性作为一种通用且有效的设计原则，将其影响从Transformer扩展到SSM，并在多模态预训练中树立了新标杆。我们的代码可以在https://github.com/Weixin-Liang/Mixture-of-Mamba访问。**|
|**2025-01-27**|**Application of Structured State Space Models to High energy physics with locality-sensitive hashing**|Cheng Jiang et.al.|[2501.16237](http://arxiv.org/abs/2501.16237)|null|现代高能物理（HEP）实验越来越受到其数据集庞大和复杂性的挑战，特别是在大规模点云处理和长序列方面。在这项研究中，为了解决这些挑战，我们探索了结构化状态空间模型（SSM）的应用，并提出了一种首次尝试将局部敏感哈希集成到混合或纯Mamba模型中的方法。我们的结果表明，纯SSM可以作为解决具有局部归纳偏置的长序列数据HEP问题的强大骨干。通过将局部敏感哈希集成到Mamba模块中，我们在关键的HEP任务上实现了显著改进，超过了传统骨干模型的推理速度和物理指标，同时减少了计算开销。在关键测试中，我们的方法展示了令人鼓舞的结果，提供了一种可行的替代传统Transformer骨干的方法，大幅减少了FLOPS的同时保持了强大的性能。|
|**2025-01-24**|**A Deep State Space Model for Rainfall-Runoff Simulations**|Yihan Wang et.al.|[2501.14980](http://arxiv.org/abs/2501.14980)|null|研究水循环中的降雨径流过程传统上依赖于概念性或基于物理的水文模型。近年来，深度学习（DL）作为一种替代方法，在水文学界用于降雨径流模拟方面迅速发展。然而，在这项任务中，已有数十年历史的长短期记忆（LSTM）网络仍然是基准，其表现优于包括Transformer在内的新架构。在本研究中，我们提出了一种状态空间模型（SSM），特别是频率调谐对角状态空间序列（S4D-FT）模型，用于降雨径流模拟。所提出的S4D-FT模型与已建立的LSTM模型以及基于物理的萨克拉门托土壤水分计算模型在连续美国（CONUS）的531个流域进行了对比评估。结果表明，S4D-FT在不同区域的表现优于LSTM模型。我们首次将S4D-FT引入降雨径流模拟，挑战了LSTM在水文学界的主导地位，并扩展了可用于水文建模的深度学习工具库。|
|**2025-01-24**|**On the locality bias and results in the Long Range Arena**|Pablo Miralles-González et.al.|[2501.14850](http://arxiv.org/abs/2501.14850)|null|长程竞技场（LRA）基准测试旨在评估Transformer改进及其替代架构在长距离依赖性建模任务中的性能。Transformer及其主要变体在此基准测试中表现不佳，而诸如状态空间模型（SSM）等一系列新架构获得了关注，在LRA中显著优于Transformer。近期的研究表明，通过去噪预训练阶段，Transformer可以在LRA中取得与这些新架构相竞争的结果。在这项工作中，我们讨论并解释了MEGA和SSM等架构在长程竞技场中的优势，以及Transformer最近的性能提升，指出了任务的位置性和局部性。我们展示了尽管LRA是针对长距离依赖性建模的基准，但实际上大部分性能来自于短距离依赖性。通过使用训练技术来缓解数据效率低下问题，Transformer能够通过适当的位编码达到最先进的性能。此外，利用相同的技术，我们能够移除SSM卷积核的所有限制，并学习完全参数化的卷积而不降低性能，这表明SSM背后的设计选择仅仅增加了对这些特定任务的归纳偏置和学习效率。我们的见解表明应谨慎解读LRA结果，并呼吁重新设计该基准。|
|**2025-01-23**|**QMamba: Post-Training Quantization for Vision State Space Models**|Yinglong Li et.al.|[2501.13624](http://arxiv.org/abs/2501.13624)|null|状态空间模型（SSM）作为Mamaba的关键组成部分，由于其高效的长序列建模能力，在视觉模型中受到了越来越多的关注。鉴于在资源受限的边缘设备上部署SSM的计算成本，后训练量化（PTQ）技术具有实现SSM高效部署的潜力。在这项工作中，我们提出了QMamba，据我们所知，这是首个为基于分析SSM中激活分布而设计的视觉SSM的PTQ框架。我们揭示了离散参数的分布表现出长尾偏斜性，而隐藏状态序列的分布则表现出高度动态的变化。相应地，我们设计了长尾偏斜量化（LtSQ）来量化离散参数，并设计了时间组量化（TGQ）来量化隐藏状态，从而减少了量化误差。广泛的实验表明，QMamba在多个模型大小和架构上的视觉模型上优于先进的PTQ方法。值得注意的是，在ImageNet分类任务中使用4位激活时，QMamba比现有方法高出21.0%。|
|**2025-01-22**|**Let SSMs be ConvNets: State-space Modeling with Optimal Tensor Contractions**|Yan Ru Pei et.al.|[2501.13230](http://arxiv.org/abs/2501.13230)|**[link](https://github.com/Brainchip-Inc/Centaurus)**|**我们引入了Centaurus，这是一种由广义状态空间模型（SSM）块组成的网络类。在训练过程中，可以将SSM操作视为张量收缩。然后可以系统地确定每个SSM块的最优张量收缩顺序，以最大化训练效率。这允许在设计SSM块时具有更大的灵活性，而不仅仅是通常实现的深度可分离配置。新的设计选择将从经典的卷积块中汲取灵感，包括组卷积、全卷积和瓶颈块。我们将Centaurus网络架构为这些块的混合体，以平衡网络大小与性能，以及训练和推理期间的内存和计算效率。我们展示了这种异构网络设计在原始音频处理任务中优于其同构对应物，包括关键词识别、语音降噪和自动语音识别（ASR）。对于ASR，Centaurus是第一个在不使用任何非线性递归（LSTMs）、显式卷积（CNNs）或（代理）注意力机制的情况下具有竞争力的全状态空间基础网络。源代码可在github.com/Brainchip-Inc/Centaurus获取。**|
|**2025-01-22**|**GRAMA: Adaptive Graph Autoregressive Moving Average Models**|Moshe Eliasof et.al.|[2501.12732](http://arxiv.org/abs/2501.12732)|null|图状态空间模型（SSMs）最近被引入以增强图神经网络（GNNs）在建模长距离交互方面的能力。尽管取得了成功，现有的方法要么牺牲了排列等变性，要么仅关注成对交互而不是序列。本文基于自回归移动平均（ARMA）和SSM之间的联系，提出了GRAMA，一种基于可学习的自回归移动平均框架的图自适应方法，解决了这些局限性。通过从静态图数据转换为序列图数据，GRAMA利用了ARMA框架的优势，同时保持了排列等变性。此外，GRAMA结合了一种选择性注意力机制，用于动态学习ARMA系数，从而实现高效且灵活的长距离信息传播。我们还建立了GRAMA与选择性SSMs之间的理论联系，揭示了其捕捉长距离依赖关系的能力。在14个合成和真实世界数据集上的广泛实验表明，GRAMA始终优于基础模型，并且与最先进的方法相比具有竞争力。|
|**2025-01-21**|**Automatic selection of the best neural architecture for time series forecasting via multi-objective optimization and Pareto optimality conditions**|Qianying Cao et.al.|[2501.12215](http://arxiv.org/abs/2501.12215)|null|时间序列预测在天气预报、医疗保健、结构健康监测、预测性维护、能源系统和金融市场等广泛应用中发挥着关键作用。虽然LSTM、GRU、Transformer和状态空间模型（SSM）已成为该领域的标准工具，但选择最优架构仍然是一个挑战。性能比较通常依赖于评估指标和所分析的数据集，这使得选择一个普遍最优的模型存在争议。在这项工作中，我们引入了一个灵活的自动化框架，用于通过集成LSTM、GRU、多头注意力和SSM模块来系统地设计和评估多样化的网络架构。利用多目标优化方法，我们的框架确定了块的数量、顺序和组合，以满足特定需求和评估目标。从得到的帕累托最优架构中，用户可以通过自定义偏好函数选择最适合给定上下文的最佳模型。我们在四个不同的实际应用中验证了我们的框架。结果表明，当仅最小化训练时间时，单层GRU或LSTM通常是最佳选择。然而，在最大化准确性或平衡多个目标时，最佳架构往往是包含多种类型块的复合设计。通过使用加权偏好函数，用户可以解决目标之间的权衡问题，揭示新的、特定于上下文的最优架构。我们的研究结果强调，没有单一的神经架构对时间序列预测是普遍最优的。相反，表现最好的模型是一个数据驱动的复合架构，它根据用户定义的标准和评估目标进行定制。|
|**2025-01-20**|**SeRpEnt: Selective Resampling for Expressive State Space Models**|Stefano Rando et.al.|[2501.11729](http://arxiv.org/abs/2501.11729)|null|
|**2025-01-19**|**Decomposing and Fusing Intra- and Inter-Sensor Spatio-Temporal Signal for Multi-Sensor Wearable Human Activity Recognition**|Haoyu Xie et.al.|[2501.10917](http://arxiv.org/abs/2501.10917)|**[link](https://github.com/anakin2555/decomposewhar)**|
|**2025-01-03**|**SSM2Mel: State Space Model to Reconstruct Mel Spectrogram from the EEG**|Cunhang Fan et.al.|[2501.10402](http://arxiv.org/abs/2501.10402)|null|
|**2025-01-08**|**Samba-ASR: State-Of-The-Art Speech Recognition Leveraging Structured State-Space Models**|Syed Abdul Gaffar Shakhadri et.al.|[2501.02832](http://arxiv.org/abs/2501.02832)|null|
|**2025-01-05**|**KM-UNet KAN Mamba UNet for medical image segmentation**|Yibo Zhang et.al.|[2501.02559](http://arxiv.org/abs/2501.02559)|**[link](https://github.com/2760613195/km_unet)**|
|**2025-01-03**|**A Separable Self-attention Inspired by the State Space Model for Computer Vision**|Juntao Zhang et.al.|[2501.02040](http://arxiv.org/abs/2501.02040)|**[link](https://github.com/yws-wxs/vminet)**|
|**2025-01-03**|**Look Back for More: Harnessing Historical Sequential Updates for Personalized Federated Adapter Tuning**|Danni Peng et.al.|[2501.01653](http://arxiv.org/abs/2501.01653)|null|
|**2025-01-02**|**CryptoMamba: Leveraging State Space Models for Accurate Bitcoin Price Prediction**|Mohammad Shahab Sepehri et.al.|[2501.01010](http://arxiv.org/abs/2501.01010)|**[link](https://github.com/MShahabSepehri/CryptoMamba)**|
|**2024-12-31**|**Understanding and Mitigating Bottlenecks of State Space Models through the Lens of Recency and Over-smoothing**|Peihao Wang et.al.|[2501.00658](http://arxiv.org/abs/2501.00658)|**[link](https://github.com/vita-group/ssm-bottleneck)**|
|**2024-12-27**|**Deep Linear Hawkes Processes**|Yuxin Chang et.al.|[2412.19634](http://arxiv.org/abs/2412.19634)|null|
|**2024-12-26**|**On the Expressiveness and Length Generalization of Selective State-Space Models on Regular Languages**|Aleksandar Terzić et.al.|[2412.19350](http://arxiv.org/abs/2412.19350)|**[link](https://github.com/ibm/selective-dense-state-space-model)**|
|**2024-12-25**|**VisionGRU: A Linear-Complexity RNN Model for Efficient Image Analysis**|Shicheng Yin et.al.|[2412.18178](http://arxiv.org/abs/2412.18178)|**[link](https://github.com/yangliu9208/visiongru)**|
|**2024-12-21**|**From Pixels to Gigapixels: Bridging Local Inductive Bias and Long-Range Dependencies with Pixel-Mamba**|Zhongwei Qiu et.al.|[2412.16711](http://arxiv.org/abs/2412.16711)|null|
|**2025-01-02**|**Mamba-SEUNet: Mamba UNet for Monaural Speech Enhancement**|Junyu Wang et.al.|[2412.16626](http://arxiv.org/abs/2412.16626)|null|
|**2024-12-21**|**V"Mean"ba: Visual State Space Models only need 1 hidden dimension**|Tien-Yu Chi et.al.|[2412.16602](http://arxiv.org/abs/2412.16602)|null|
|**2024-12-20**|**Mamba2D: A Natively Multi-Dimensional State-Space Model for Vision Tasks**|Enis Baty et.al.|[2412.16146](http://arxiv.org/abs/2412.16146)|**[link](https://github.com/cocoalex00/Mamba2D)**|
|**2024-12-18**|**State Space Models are Strong Text Rerankers**|Zhichao Xu et.al.|[2412.14354](http://arxiv.org/abs/2412.14354)|null|
|**2024-12-18**|**Detecting Machine-Generated Music with Explainability -- A Challenge and Early Benchmarks**|Yupei Li et.al.|[2412.13421](http://arxiv.org/abs/2412.13421)|null|
|**2024-12-17**|**Expansion Span: Combining Fading Memory and Retrieval in Hybrid State Space Models**|Elvis Nunez et.al.|[2412.13328](http://arxiv.org/abs/2412.13328)|null|
|**2024-12-17**|**GG-SSMs: Graph-Generating State Space Models**|Nikola Zubić et.al.|[2412.12423](http://arxiv.org/abs/2412.12423)|null|
|**2024-12-15**|**Deep Learning-based Approaches for State Space Models: A Selective Review**|Jiahe Lin et.al.|[2412.11211](http://arxiv.org/abs/2412.11211)|null|
|**2024-12-15**|**BarcodeMamba: State Space Models for Biodiversity Analysis**|Tiancheng Gao et.al.|[2412.11084](http://arxiv.org/abs/2412.11084)|**[link](https://github.com/bioscan-ml/barcodemamba)**|
|**2024-12-13**|**XYScanNet: An Interpretable State Space Model for Perceptual Image Deblurring**|Hanzhou Liu et.al.|[2412.10338](http://arxiv.org/abs/2412.10338)|null|
|**2024-12-12**|**Does Representation Matter? Exploring Intermediate Layers in Large Language Models**|Oscar Skean et.al.|[2412.09563](http://arxiv.org/abs/2412.09563)|null|
|**2024-12-09**|**The Computational Limits of State-Space Models and Mamba via the Lens of Circuit Complexity**|Yifang Chen et.al.|[2412.06148](http://arxiv.org/abs/2412.06148)|null|
|**2024-12-07**|**Multimodal Biometric Authentication Using Camera-Based PPG and Fingerprint Fusion**|Xue Xian Zheng et.al.|[2412.05660](http://arxiv.org/abs/2412.05660)|null|
|**2024-12-01**|**Learning Mamba as a Continual Learner**|Chongyang Zhao et.al.|[2412.00776](http://arxiv.org/abs/2412.00776)|null|
|**2024-12-01**|**2DMamba: Efficient State Space Model for Image Representation with Applications on Giga-Pixel Whole Slide Image Classification**|Jingwei Zhang et.al.|[2412.00678](http://arxiv.org/abs/2412.00678)|**[link](https://github.com/atlasanalyticslab/2dmamba)**|
|**2024-11-29**|**SkelMamba: A State Space Model for Efficient Skeleton Action Recognition of Neurological Disorders**|Niki Martinel et.al.|[2411.19544](http://arxiv.org/abs/2411.19544)|null|
|**2024-11-29**|**Look Every Frame All at Once: Video-Ma $^2$ mba for Efficient Long-form Video Understanding with Multi-Axis Gradient Checkpointing**|Hosu Lee et.al.|[2411.19460](http://arxiv.org/abs/2411.19460)|null|
|**2024-11-29**|**Autocorrelation Matters: Understanding the Role of Initialization Schemes for State Space Models**|Fusheng Liu et.al.|[2411.19455](http://arxiv.org/abs/2411.19455)|null|
|**2024-11-29**|**Fast convolution algorithm for state space models**|Gregory Beylkin et.al.|[2411.17729](http://arxiv.org/abs/2411.17729)|null|
|**2024-11-24**|**State-Space Large Audio Language Models**|Saurabhchand Bhati et.al.|[2411.15685](http://arxiv.org/abs/2411.15685)|null|
|**2024-11-26**|**GraphGrad: Efficient Estimation of Sparse Polynomial Representations for General State-Space Models**|Benjamin Cox et.al.|[2411.15637](http://arxiv.org/abs/2411.15637)|null|
|**2024-11-23**|**Mamba-CL: Optimizing Selective State Space Model in Null Space for Continual Learning**|De Cheng et.al.|[2411.15469](http://arxiv.org/abs/2411.15469)|null|
|**2024-11-23**|**MambaVLT: Time-Evolving Multimodal State Space Model for Vision-Language Tracking**|Xinqi Liu et.al.|[2411.15459](http://arxiv.org/abs/2411.15459)|null|
|**2024-11-21**|**Parameter Efficient Mamba Tuning via Projector-targeted Diagonal-centric Linear Transformation**|Seokil Ham et.al.|[2411.15224](http://arxiv.org/abs/2411.15224)|null|
|**2024-11-20**|**Hymba: A Hybrid-head Architecture for Small Language Models**|Xin Dong et.al.|[2411.13676](http://arxiv.org/abs/2411.13676)|null|
|**2024-11-18**|**Bi-Mamba: Towards Accurate 1-Bit State Space Models**|Shengkun Tang et.al.|[2411.11843](http://arxiv.org/abs/2411.11843)|null|
|**2024-11-18**|**Hybrid Data-Driven SSM for Interpretable and Label-Free mmWave Channel Prediction**|Yiyong Sun et.al.|[2411.11576](http://arxiv.org/abs/2411.11576)|null|
|**2024-11-16**|**MetaLA: Unified Optimal Linear Approximation to Softmax Attention Map**|Yuhong Chou et.al.|[2411.10741](http://arxiv.org/abs/2411.10741)|**[link](https://github.com/BICLab/MetaLA)**|
|**2024-11-11**|**AEROMamba: An efficient architecture for audio super-resolution using generative adversarial networks and state space models**|Wallace Abreu et.al.|[2411.07364](http://arxiv.org/abs/2411.07364)|**[link](https://github.com/aeromamba-super-resolution/aeromamba)**|
|**2024-11-11**|**Mamba-based Decoder-Only Approach with Bidirectional Speech Modeling for Speech Recognition**|Yoshiki Masuyama et.al.|[2411.06968](http://arxiv.org/abs/2411.06968)|**[link](https://github.com/YoshikiMas/madeon-asr)**|
|**2024-11-10**|**SEM-Net: Efficient Pixel Modelling for image inpainting with Spatially Enhanced SSM**|Shuang Chen et.al.|[2411.06318](http://arxiv.org/abs/2411.06318)|**[link](https://github.com/chrischen1023/sem-net)**|
|**2024-11-07**|**Zero-Shot Temporal Resolution Domain Adaptation for Spiking Neural Networks**|Sanja Karilanova et.al.|[2411.04760](http://arxiv.org/abs/2411.04760)|null|
|**2024-11-06**|**Bio-xLSTM: Generative modeling, representation and in-context learning of biological and chemical sequences**|Niklas Schmidinger et.al.|[2411.04165](http://arxiv.org/abs/2411.04165)|**[link](https://github.com/ml-jku/chem-xlstm)**|
|**2024-11-06**|**MambaPEFT: Exploring Parameter-Efficient Fine-Tuning for Mamba**|Masakazu Yoshimura et.al.|[2411.03855](http://arxiv.org/abs/2411.03855)|null|
|**2024-11-05**|**A scalable generative model for dynamical system reconstruction from neuroimaging data**|Eric Volkmann et.al.|[2411.02949](http://arxiv.org/abs/2411.02949)|**[link](https://github.com/humml-lab/GTF-ConvSSM)**|
|**2024-11-05**|**Layer-Adaptive State Pruning for Deep State Space Models**|Minseon Gwak et.al.|[2411.02824](http://arxiv.org/abs/2411.02824)|**[link](https://github.com/msgwak/last)**|
|**2024-11-04**|**Recursive Learning of Asymptotic Variational Objectives**|Alessandro Mastrototaro et.al.|[2411.02217](http://arxiv.org/abs/2411.02217)|null|
|**2024-11-07**|**Birdie: Advancing State Space Models with Reward-Driven Objectives and Curricula**|Sam Blouir et.al.|[2411.01030](http://arxiv.org/abs/2411.01030)|**[link](https://github.com/samblouir/birdie)**|
|**2024-10-31**|**SambaMixer: State of Health Prediction of Li-ion Batteries using Mamba State Space Models**|José Ignacio Olalde-Verano et.al.|[2411.00233](http://arxiv.org/abs/2411.00233)|**[link](https://github.com/sascha-kirch/samba-mixer)**|
|**2024-10-31**|**Nudging state-space models for Bayesian filtering under misspecified dynamics**|Fabian Gonzalez et.al.|[2411.00218](http://arxiv.org/abs/2411.00218)|null|
|**2024-10-31**|**NIMBA: Towards Robust and Principled Processing of Point Clouds With SSMs**|Nursena Köprücü et.al.|[2411.00151](http://arxiv.org/abs/2411.00151)|null|
|**2024-10-31**|**In-Context Learned Equalization in Cell-Free Massive MIMO via State-Space Models**|Zihang Song et.al.|[2410.23882](http://arxiv.org/abs/2410.23882)|null|
|**2024-10-28**|**Multi-Agent Reinforcement Learning with Selective State-Space Models**|Jemma Daniel et.al.|[2410.19382](http://arxiv.org/abs/2410.19382)|null|

<p align=right>(<a href=#updated-on-20250131>back to top</a>)</p>

## Communication Intelligence

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-09-21**|**LLM Agents as 6G Orchestrator: A Paradigm for Task-Oriented Physical-Layer Automation**|Zhuoran Xiao et.al.|[2410.03688](http://arxiv.org/abs/2410.03688)|null|生成式预训练模型的快速发展正在推动技术进步从基础应用如聊天机器人向更复杂的基于代理的系统转变。将6G系统与大型语言模型（LLM）代理和数字孪生（DT）相结合，对于管理具有新兴功能（如原生AI服务和感知）的高度复杂通信系统具有巨大潜力和必要性。通过6G导向的代理，基站能够理解各种动态上层任务的传输需求，并自动编排最优系统工作流程。通过持续从6G DT获取反馈进行强化，代理最终可以相应地提高实际系统的性能。与为通用应用设计的现有LLM代理不同，6G导向的代理旨在利用大量额外的专业知识进行高度严谨和精确的规划，这不可避免地需要从模型训练到实施的特定系统设计。本文提出了一种构建面向任务的6G LLM代理的新颖综合方法。我们首先提出一个两阶段持续预训练和微调方案，以建立领域基础模型和多样化的专业专家模型，以满足各种应用场景的需求。此外，还提出了一种基于语义检索的新颖推理框架，以利用现有的通信相关功能。物理层任务分解等示例任务的实验结果表明了所提范式的可行性和有效性。|

<p align=right>(<a href=#updated-on-20250131>back to top</a>)</p>

## RAG

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-01-29**|**GLLM: Self-Corrective G-Code Generation using Large Language Models with User Feedback**|Mohamed Abdelaal et.al.|[2501.17584](http://arxiv.org/abs/2501.17584)|null|本文介绍了一种创新工具GLLM，它利用大型语言模型（LLM）从自然语言指令自动生成计算机数控（CNC）加工所需的G代码。GLLM通过将人类可读的任务描述转换为机器可执行的代码，解决了手动编写G代码的难题。该系统采用经过微调的StarCoder-3B模型，并结合领域特定的训练数据和检索增强生成（RAG）机制。GLLM运用了先进的提示策略和新颖的自我纠正代码生成方法，以确保生成的G代码在语法和语义上的正确性。架构中还包括强大的验证机制，包括语法检查、G代码特定验证以及使用豪斯多夫距离进行的功能正确性评估。通过结合这些技术，GLLM旨在使CNC编程更加普及，让没有丰富编程经验的用户也能轻松使用，同时保持G代码生成的高度准确性和可靠性。|
|**2025-01-29**|**AugmenTest: Enhancing Tests with LLM-Driven Oracles**|Shaker Mahmud Khandaker et.al.|[2501.17461](http://arxiv.org/abs/2501.17461)|null|自动化测试生成对于确保软件应用程序的可靠性和健壮性同时减少所需的工作量至关重要。尽管在测试生成研究方面已经取得了显著进展，但生成有效的测试预言仍然是一个未解决的问题。为了解决这一挑战，我们提出了AugmenTest，这是一种利用大型语言模型（LLM）基于待测软件的可用文档推断正确测试预言的方法。与大多数依赖代码的现有方法不同，AugmenTest利用LLM的语义能力从文档和开发人员注释中推断方法的预期行为，而无需查看代码。AugmenTest包括四种变体：简单提示、扩展提示、带有通用提示的RAG（不包含被测类或方法的上下文）以及带有简单提示的RAG，每种变体为LLM提供了不同程度的上下文信息。为了评估我们的工作，我们选择了142个Java类，并为每个类生成了多个变异体。然后从这些变异体生成测试，仅关注那些在变异体上通过但在原始类上失败的测试，以确保这些测试有效捕捉到错误。这导致了203个具有独特错误的独特测试，用于评估AugmenTest。结果显示，在最保守的情况下，AugmenTest的扩展提示始终优于简单提示，生成正确断言的成功率为30%。相比之下，最先进的TOGA方法的成功率为8.2%。与我们的预期相反，基于RAG的方法并没有带来改进，在最保守的情况下成功率为18.2%。|
|**2025-01-29**|**Leveraging In-Context Learning and Retrieval-Augmented Generation for Automatic Question Generation in Educational Domains**|Subhankar Maity et.al.|[2501.17397](http://arxiv.org/abs/2501.17397)|null|在教育领域，问题生成是一项耗时且认知要求高的任务，因为它需要创建既与上下文相关又具有教育意义的问题。当前的自动问题生成方法往往会产生脱离上下文的问题。在这项工作中，我们探讨了在教育背景下先进的自动问题生成技术，重点关注情境学习（ICL）、检索增强生成（RAG）以及结合这两种方法的新型混合模型。我们使用少量示例通过GPT-4实现ICL，并利用带有检索模块的BART实现RAG。混合模型结合了RAG和ICL来解决这些问题并提高问题质量。评估通过自动指标进行，随后是人工评估指标。我们的结果显示，ICL方法和混合模型在生成更准确和相关的问题方面始终优于其他方法，包括基线模型。|
|**2025-01-28**|**ASTRAL: Automated Safety Testing of Large Language Models**|Miriam Ugarte et.al.|[2501.17132](http://arxiv.org/abs/2501.17132)|null|大型语言模型（LLM）因其能够理解和生成复杂的人类类似内容而受到广泛关注。然而，确保其安全性至关重要，因为它们可能会提供有害和不安全的回应。现有的LLM测试框架虽然处理了各种与安全相关的问题（例如毒品、恐怖主义、虐待动物），但通常由于数据集不平衡和过时而面临挑战。在本文中，我们介绍了ASTRAL，这是一种自动化生成和执行测试用例（即提示）以测试LLM安全性的工具。首先，我们提出了一种新的黑盒覆盖率标准，用于生成跨多种安全类别以及语言写作特征（即不同的风格和说服性写作技巧）平衡且多样化的不安全测试输入。其次，我们提出了一个基于LLM的方法，该方法利用检索增强生成（RAG）、少量示例提示策略和网络浏览来生成最新的测试输入。最后，类似于当前的LLM测试自动化技术，我们利用LLM作为测试预言机来区分安全和不安全的测试输出，从而实现完全自动化的测试方法。我们在知名LLM上进行了广泛的评估，揭示了以下关键发现：i) 当作为测试预言机时，GPT3.5的表现优于其他LLM，能准确检测到不安全的响应，甚至超过了更近期的LLM（例如GPT-4），以及专门设计用来检测不安全LLM输出的LLM（例如LlamaGuard）；ii) 结果证实，我们的方法可以使用相同数量的测试输入发现几乎是现有静态数据集两倍的不安全LLM行为；iii) 我们的黑盒覆盖率标准结合网络浏览可以有效地指导LLM生成最新的不安全测试输入，显著增加发现的不安全LLM行为的数量。|
|**2025-01-28**|**Enhanced Retrieval of Long Documents: Leveraging Fine-Grained Block Representations with Large Language Models**|Minghan Li et.al.|[2501.17039](http://arxiv.org/abs/2501.17039)|null|近年来，大型语言模型（LLMs）在包括信息检索在内的多个领域展示了非凡的能力。以往的做法大多涉及利用这些模型为每个查询、每个段落或每个文档单独创建一个嵌入，这一策略在检索增强生成（RAG）框架中得到了体现和应用。虽然这种方法已被证明是有效的，但我们认为它由于依赖于相对粗粒度的表示方法，在全面捕捉文档级文本的细微差别方面存在不足。为了解决这一局限性，我们引入了一种新的细粒度方法，旨在提高长文档相关性评分的准确性。我们的方法首先将长文档分割成若干块，每一块都使用LLM进行嵌入，以便与查询表示相匹配。在计算相关性得分时，我们通过加权求和的方法汇总查询-块相关性得分，从而得到查询与整个文档的综合得分。尽管这种方法看起来简单，但实验结果表明，该方法优于标准表示方法，并且显著减少了嵌入生成的延迟。此外，通过仔细优化成对损失函数，我们取得了更优的表现。|
|**2025-01-28**|**Multiple Abstraction Level Retrieve Augment Generation**|Zheng Zheng et.al.|[2501.16952](http://arxiv.org/abs/2501.16952)|null|一种由大型语言模型（LLM）支持的检索增强生成（RAG）模型，为适应新数据和知识提供了更快、更经济的解决方案，并且相比预训练的LLM能够提供更加专业的回答。然而，大多数现有的方法依赖于检索前缀大小的片段作为参考以支持问答（Q/A）。这种方法通常用于解决单一抽象层次的信息需求，因为它难以生成跨越多个抽象层次的答案。在RAG设置中，当提供足够的细节时，LLM可以有效地总结并回答问题，但检索过多信息往往会导致“迷失在中间”的问题，并超出令牌限制。我们提出了一种新颖的RAG方法，该方法使用多抽象层次（MAL）的片段，包括多句子级、段落级、章节级和文档级。我们的方法的有效性在一个尚未充分探索的糖科学领域得到了验证。与传统的单层RAG方法相比，我们的方法在糖相关论文上的AI评估答案正确率提高了25.739%。|
|**2025-01-29**|**Optimizing Code Runtime Performance through Context-Aware Retrieval-Augmented Generation**|Manish Acharya et.al.|[2501.16692](http://arxiv.org/abs/2501.16692)|**[link](https://github.com/manishacharya60/rag-optimization)**|**通过自动化代码优化来提升软件性能，为增强执行速度和效率提供了一个有前景的途径。尽管最近在大语言模型（LLM）方面取得了进展，但在深入程序分析方面仍存在显著差距。本研究引入了AUTOPATCH，这是一种基于上下文学习的方法，旨在通过使LLM能够自动生成优化代码来弥合这一差距。受程序员学习和应用知识以优化软件的方式启发，AUTOPATCH集成了三个关键组件：(1) 一种类比驱动框架，将LLM优化与人类认知过程对齐；(2) 一种统一方法，整合历史代码示例和控制流图分析，实现上下文感知学习；(3) 一种通过上下文提示生成优化代码的自动化流程。实验结果表明，对于常见的可执行代码，AUTOPATCH相比GPT-4o实现了7.3%的执行效率提升，展示了其在自动程序运行时优化方面的潜力。**|
|**2025-01-28**|**VeriFact: Verifying Facts in LLM-Generated Clinical Text with Electronic Health Records**|Philip Chung et.al.|[2501.16672](http://arxiv.org/abs/2501.16672)|**[link](https://github.com/philipchung/verifact)**|**确保大型语言模型（LLM）在临床医学中生成文本的事实准确性方法尚不完善。VeriFact是一种人工智能系统，它结合了检索增强生成和LLM作为裁判的功能，以验证LLM生成的文本是否基于患者的电子健康记录（EHR）得到事实支持。为了评估该系统，我们引入了一个新的数据集VeriFact-BHC，该数据集将出院总结中的简短住院过程叙述分解成一系列简单陈述，并由临床医生标注每个陈述是否得到了患者EHR临床记录的支持。虽然临床医生之间的最高一致率为88.5%，但与去噪并裁决后的平均人类临床医生基准相比，VeriFact达到高达92.7%的一致性，表明VeriFact超越了普通临床医生根据患者医疗记录进行事实核查的能力。VeriFact可能通过消除当前的评估瓶颈来加速基于LLM的EHR应用的发展。**|
|**2025-01-27**|**Characterizing Network Structure of Anti-Trans Actors on TikTok**|Maxyn Leitner et.al.|[2501.16507](http://arxiv.org/abs/2501.16507)|null|近期，短格式视频社交媒体网站如TikTok的有效利用，为跨性别/非二元性别的创作者在线上提供了更高的可见度、沟通和社群联系。然而，这些平台也被右翼行为者利用来针对跨性别/非二元性别的人群，使这些反跨性别行为者能够高效地传播仇恨言论和宣传材料。鉴于这两种不同的群体，在TikTok上支持跨性别与反对跨性别的社区之间网络结构有何差异？反跨性别内容在多大程度上被放大了其影响？在本文中，我们收集了一组包含支持与反对跨性别内容的TikTok视频样本，并开发了一个关于跨性别相关情感的分类体系，以实现对TikTok平台上内容的分类，最终分析支持跨性别与反对跨性别社区的回复网络结构。为了完成这项工作，我们雇佣了来自跨性别/非二元性别社区的专业数据标注员，生成了一组高度准确标注的数据子集。基于这个子集，我们采用了一种新颖的分类流程，该流程利用带有注释示例和分类定义的检索增强生成（RAG）技术，将内容分类为支持跨性别、反对跨性别或中立类别。我们发现，将我们的分类体系及其逻辑融入到分类引擎中提高了区分跨性别相关内容的能力。网络分析结果表明，支持跨性别与反对跨性别内容发布者之间存在许多互动，进一步证明了跨性别个体受到针对性攻击的现象，显示出需要更好的内容管理工具。|
|**2025-01-27**|**URAG: Implementing a Unified Hybrid RAG for Precise Answers in University Admission Chatbots -- A Case Study at HCMUT**|Long Nguyen et.al.|[2501.16276](http://arxiv.org/abs/2501.16276)|null|随着人工智能的快速发展，特别是在自然语言处理领域，大型语言模型（LLM）已成为教育问答系统中的关键组成部分，尤其是在大学招生聊天机器人中。为了增强这些系统，开发了诸如检索增强生成（RAG）等先进技术，通过整合特定的大学数据，使LLM能够提供有关招生和学术咨询的信息丰富回答。然而，这些增强的RAG技术通常涉及高昂的运营成本，并需要训练复杂的专门模块，这给实际部署带来了挑战。此外，在教育环境中，提供准确答案以防止误导信息至关重要，而没有适当策略和方法的LLM系统在这方面面临困难。在本文中，我们介绍了一种统一的RAG（URAG）框架，这是一种混合方法，可以显著提高对关键查询的响应准确性。实验结果表明，URAG能够将我们内部轻量级模型的性能提升至与最先进的商业模型相当的水平。此外，为了验证其实际应用性，我们在我们的教育机构进行了案例研究，收到了积极的反馈和赞誉。这项研究不仅证明了URAG的有效性，也突显了其在教育环境中的实际实施可行性。|
|**2025-01-28**|**DBRouting: Routing End User Queries to Databases for Answerability**|Priyangshu Mandal et.al.|[2501.16220](http://arxiv.org/abs/2501.16220)|null|
|**2025-01-27**|**Provence: efficient and robust context pruning for retrieval-augmented generation**|Nadezhda Chirkova et.al.|[2501.16214](http://arxiv.org/abs/2501.16214)|null|
|**2025-01-27**|**Raiders of the Lost Dependency: Fixing Dependency Conflicts in Python using LLMs**|Antony Bartlett et.al.|[2501.16191](http://arxiv.org/abs/2501.16191)|null|
|**2025-01-27**|**PISCO: Pretty Simple Compression for Retrieval-Augmented Generation**|Maxime Louis et.al.|[2501.16075](http://arxiv.org/abs/2501.16075)|null|
|**2025-01-27**|**MultiMend: Multilingual Program Repair with Context Augmentation and Multi-Hunk Patch Generation**|Reza Gharibi et.al.|[2501.16044](http://arxiv.org/abs/2501.16044)|**[link](https://github.com/h4iku/multimend)**|
|**2025-01-27**|**Parametric Retrieval Augmented Generation**|Weihang Su et.al.|[2501.15915](http://arxiv.org/abs/2501.15915)|**[link](https://github.com/oneal2000/prag)**|
|**2025-01-27**|**LemmaHead: RAG Assisted Proof Generation Using Large Language Models**|Tianbo Yang et.al.|[2501.15797](http://arxiv.org/abs/2501.15797)|null|
|**2025-01-27**|**Efficiency Bottlenecks of Convolutional Kolmogorov-Arnold Networks: A Comprehensive Scrutiny with ImageNet, AlexNet, LeNet and Tabular Classification**|Ashim Dahal et.al.|[2501.15757](http://arxiv.org/abs/2501.15757)|**[link](https://github.com/ashimdahal/study-of-convolutional-kolmogorov-arnold-networks)**|
|**2025-01-26**|**Advancing Generative Artificial Intelligence and Large Language Models for Demand Side Management with Electric Vehicles**|Hanwen Zhang et.al.|[2501.15544](http://arxiv.org/abs/2501.15544)|null|
|**2025-01-26**|**Unveiling the Potential of Multimodal Retrieval Augmented Generation with Planning**|Xiaohan Yu et.al.|[2501.15470](http://arxiv.org/abs/2501.15470)|null|
|**2025-01-24**|**Chain-of-Retrieval Augmented Generation**|Liang Wang et.al.|[2501.14342](http://arxiv.org/abs/2501.14342)|null|
|**2025-01-24**|**Fast Think-on-Graph: Wider, Deeper and Faster Reasoning of Large Language Model on Knowledge Graph**|Xujian Liang et.al.|[2501.14300](http://arxiv.org/abs/2501.14300)|**[link](https://github.com/dosonleung/fasttog)**|
|**2025-01-23**|**StreamingRAG: Real-time Contextual Retrieval and Generation Framework**|Murugan Sankaradas et.al.|[2501.14101](http://arxiv.org/abs/2501.14101)|null|
|**2025-01-23**|**GraphRAG under Fire**|Jiacheng Liang et.al.|[2501.14050](http://arxiv.org/abs/2501.14050)|null|
|**2025-01-23**|**CAPRAG: A Large Language Model Solution for Customer Service and Automatic Reporting using Vector and Graph Retrieval-Augmented Generation**|Hamza Landolsi et.al.|[2501.13993](http://arxiv.org/abs/2501.13993)|null|
|**2025-01-23**|**The machine learning platform for developers of large systems**|Alexey Naikov et.al.|[2501.13881](http://arxiv.org/abs/2501.13881)|null|
|**2025-01-23**|**A RAG-Based Institutional Assistant**|Gustavo Kuratomi et.al.|[2501.13880](http://arxiv.org/abs/2501.13880)|null|
|**2025-01-23**|**RPO: Retrieval Preference Optimization for Robust Retrieval-Augmented Generation**|Shi-Qi Yan et.al.|[2501.13726](http://arxiv.org/abs/2501.13726)|null|
|**2025-01-23**|**Retrievals Can Be Detrimental: A Contrastive Backdoor Attack Paradigm on Retrieval-Augmented Diffusion Models**|Hao Fang et.al.|[2501.13340](http://arxiv.org/abs/2501.13340)|null|
|**2025-01-22**|**RAG-Reward: Optimizing RAG with Reward Modeling and RLHF**|Hanning Zhang et.al.|[2501.13264](http://arxiv.org/abs/2501.13264)|null|
|**2025-01-22**|**Adaptive Retrieval Without Self-Knowledge? Bringing Uncertainty Back Home**|Viktor Moskvoretskii et.al.|[2501.12835](http://arxiv.org/abs/2501.12835)|null|
|**2025-01-22**|**Generating Diverse Q&A Benchmarks for RAG Evaluation with DataMorgana**|Simone Filice et.al.|[2501.12789](http://arxiv.org/abs/2501.12789)|null|
|**2025-01-22**|**Preserving Culinary Traditions. A Crowdsourced Digital Collection of Cookbooks**|Giulia Renda et.al.|[2501.12786](http://arxiv.org/abs/2501.12786)|null|
|**2025-01-20**|**ImageRef-VL: Enabling Contextual Image Referencing in Vision-Language Models**|Jingwei Yi et.al.|[2501.12418](http://arxiv.org/abs/2501.12418)|**[link](https://github.com/bytedance/imageref-vl)**|
|**2025-01-21**|**ALoFTRAG: Automatic Local Fine Tuning for Retrieval Augmented Generation**|Peter Devine et.al.|[2501.11929](http://arxiv.org/abs/2501.11929)|**[link](https://github.com/lightblue-tech/aloftrag)**|
|**2025-01-23**|**Med-R $^2$ : Crafting Trustworthy LLM Physicians through Retrieval and Reasoning of Evidence-Based Medicine**|Keer Lu et.al.|[2501.11885](http://arxiv.org/abs/2501.11885)|null|
|**2025-01-21**|**Network-informed Prompt Engineering against Organized Astroturf Campaigns under Extreme Class Imbalance**|Nikos Kanakaris et.al.|[2501.11849](http://arxiv.org/abs/2501.11849)|**[link](https://github.com/nkanak/brag-fake-news-campaigns)**|
|**2025-01-20**|**Poison-RAG: Adversarial Data Poisoning Attacks on Retrieval-Augmented Generation in Recommender Systems**|Fatemeh Nazary et.al.|[2501.11759](http://arxiv.org/abs/2501.11759)|**[link](https://github.com/atenanaz/poison-rag)**|
|**2025-01-20**|**Explainable Lane Change Prediction for Near-Crash Scenarios Using Knowledge Graph Embeddings and Retrieval Augmented Generation**|M. Manzour et.al.|[2501.11560](http://arxiv.org/abs/2501.11560)|null|
|**2025-01-20**|**PIKE-RAG: sPecIalized KnowledgE and Rationale Augmented Generation**|Jinyu Wang et.al.|[2501.11551](http://arxiv.org/abs/2501.11551)|**[link](https://github.com/microsoft/pike-rag)**|
|**2025-01-20**|**RACCOON: A Retrieval-Augmented Generation Approach for Location Coordinate Capture from News Articles**|Jonathan Lin et.al.|[2501.11440](http://arxiv.org/abs/2501.11440)|null|
|**2025-01-20**|**TigerVector: Supporting Vector Search in Graph Databases for Advanced RAGs**|Shige Liu et.al.|[2501.11216](http://arxiv.org/abs/2501.11216)|null|
|**2025-01-19**|**InsQABench: Benchmarking Chinese Insurance Domain Question Answering with Large Language Models**|Jing Ding et.al.|[2501.10943](http://arxiv.org/abs/2501.10943)|**[link](https://github.com/haileyfamo/insqabench)**|
|**2025-01-18**|**Learn-by-interact: A Data-Centric Framework for Self-Adaptive Agents in Realistic Environments**|Hongjin Su et.al.|[2501.10893](http://arxiv.org/abs/2501.10893)|null|
|**2025-01-17**|**AirRAG: Activating Intrinsic Reasoning for Retrieval Augmented Generation via Tree-based Search**|Wenfeng Feng et.al.|[2501.10053](http://arxiv.org/abs/2501.10053)|null|
|**2025-01-17**|**FRAG: A Flexible Modular Framework for Retrieval-Augmented Generation based on Knowledge Graphs**|Zengyi Gao et.al.|[2501.09957](http://arxiv.org/abs/2501.09957)|null|
|**2025-01-17**|**Passage Segmentation of Documents for Extractive Question Answering**|Zuhong Liu et.al.|[2501.09940](http://arxiv.org/abs/2501.09940)|null|
|**2025-01-17**|**Dialogue Benchmark Generation from Knowledge Graphs with Cost-Effective Retrieval-Augmented LLMs**|Reham Omar et.al.|[2501.09928](http://arxiv.org/abs/2501.09928)|null|
|**2025-01-16**|**Conversational Text Extraction with Large Language Models Using Retrieval-Augmented Systems**|Soham Roy et.al.|[2501.09801](http://arxiv.org/abs/2501.09801)|null|
|**2025-01-16**|**OmniThink: Expanding Knowledge Boundaries in Machine Writing through Thinking**|Zekun Xi et.al.|[2501.09751](http://arxiv.org/abs/2501.09751)|null|
|**2025-01-16**|**CyberMentor: AI Powered Learning Tool Platform to Address Diverse Student Needs in Cybersecurity Education**|Tianyu Wang et.al.|[2501.09709](http://arxiv.org/abs/2501.09709)|**[link](https://github.com/tisage/cybermentor)**|
|**2025-01-16**|**Adaptive Contextual Caching for Mobile Edge Large Language Model Service**|Guangyuan Liu et.al.|[2501.09383](http://arxiv.org/abs/2501.09383)|null|
|**2025-01-16**|**To Retrieve or Not to Retrieve? Uncertainty Detection for Dynamic Retrieval Augmented Generation**|Kaustubh D. Dhole et.al.|[2501.09292](http://arxiv.org/abs/2501.09292)|null|
|**2025-01-15**|**Agentic Retrieval-Augmented Generation: A Survey on Agentic RAG**|Aditi Singh et.al.|[2501.09136](http://arxiv.org/abs/2501.09136)|**[link](https://github.com/asinghcsu/agenticrag-survey)**|
|**2025-01-15**|**SteLLA: A Structured Grading System Using LLMs with RAG**|Hefei Qiu et.al.|[2501.09092](http://arxiv.org/abs/2501.09092)|null|
|**2025-01-15**|**Physical AI Agents: Integrating Cognitive Intelligence with Real-World Action**|Fouad Bousetouane et.al.|[2501.08944](http://arxiv.org/abs/2501.08944)|null|
|**2025-01-15**|**Leveraging LLM Agents for Translating Network Configurations**|Yunze Wei et.al.|[2501.08760](http://arxiv.org/abs/2501.08760)|null|
|**2025-01-15**|**Knowledge Graph-based Retrieval-Augmented Generation for Schema Matching**|Chuangtao Ma et.al.|[2501.08686](http://arxiv.org/abs/2501.08686)|**[link](https://github.com/machuangtao/kg-rag4sm)**|
|**2025-01-14**|**ADAM-1: AI and Bioinformatics for Alzheimer's Detection and Microbiome-Clinical Data Integrations**|Ziyuan Huang et.al.|[2501.08324](http://arxiv.org/abs/2501.08324)|null|
|**2025-01-14**|**Addressing the sustainable AI trilemma: a case study on LLM agents and RAG**|Hui Wu et.al.|[2501.08262](http://arxiv.org/abs/2501.08262)|null|
|**2025-01-14**|**Eliciting In-context Retrieval and Reasoning for Long-context Large Language Models**|Yifu Qiu et.al.|[2501.08248](http://arxiv.org/abs/2501.08248)|null|
|**2025-01-14**|**Engineering LLM Powered Multi-agent Framework for Autonomous CloudOps**|Kannan Parthasarathy et.al.|[2501.08243](http://arxiv.org/abs/2501.08243)|null|
|**2025-01-14**|**ASTRID -- An Automated and Scalable TRIaD for the Evaluation of RAG-based Clinical Question Answering Systems**|Mohita Chowdhury et.al.|[2501.08208](http://arxiv.org/abs/2501.08208)|null|
|**2025-01-14**|**Advice for Diabetes Self-Management by ChatGPT Models: Challenges and Recommendations**|Waqar Hussain et.al.|[2501.07931](http://arxiv.org/abs/2501.07931)|null|
|**2025-01-14**|**ReARTeR: Retrieval-Augmented Reasoning with Trustworthy Process Rewarding**|Zhongxiang Sun et.al.|[2501.07861](http://arxiv.org/abs/2501.07861)|null|
|**2025-01-14**|**A Driver Advisory System Based on Large Language Model for High-speed Train**|Y. C. Luo et.al.|[2501.07837](http://arxiv.org/abs/2501.07837)|null|
|**2025-01-14**|**Talk to Right Specialists: Routing and Planning in Multi-agent System for Question Answering**|Feijie Wu et.al.|[2501.07813](http://arxiv.org/abs/2501.07813)|null|
|**2025-01-14**|**Unsupervised Query Routing for Retrieval Augmented Generation**|Feiteng Mu et.al.|[2501.07793](http://arxiv.org/abs/2501.07793)|null|
|**2025-01-13**|**WebWalker: Benchmarking LLMs in Web Traversal**|Jialong Wu et.al.|[2501.07572](http://arxiv.org/abs/2501.07572)|**[link](https://github.com/alibaba-nlp/webwalker)**|
|**2025-01-13**|**RadAlign: Advancing Radiology Report Generation with Vision-Language Concept Alignment**|Difei Gu et.al.|[2501.07525](http://arxiv.org/abs/2501.07525)|**[link](https://github.com/difeigu/radalign)**|
|**2025-01-13**|**Parallel Key-Value Cache Fusion for Position Invariant RAG**|Philhoon Oh et.al.|[2501.07523](http://arxiv.org/abs/2501.07523)|null|
|**2025-01-13**|**Enhancing Retrieval-Augmented Generation: A Study of Best Practices**|Siran Li et.al.|[2501.07391](http://arxiv.org/abs/2501.07391)|**[link](https://github.com/ali-bahrainian/rag_best_practices)**|
|**2025-01-13**|**LLM-Net: Democratizing LLMs-as-a-Service through Blockchain-based Expert Networks**|Zan-Kai Chong et.al.|[2501.07288](http://arxiv.org/abs/2501.07288)|null|
|**2025-01-13**|**Large Language Models: New Opportunities for Access to Science**|Jutta Schnabel et.al.|[2501.07250](http://arxiv.org/abs/2501.07250)|null|
|**2025-01-13**|**ListConRanker: A Contrastive Text Reranker with Listwise Encoding**|Junlong Liu et.al.|[2501.07111](http://arxiv.org/abs/2501.07111)|null|
|**2025-01-13**|**Research on the Online Update Method for Retrieval-Augmented Generation (RAG) Model with Incremental Learning**|Yuxin Fan et.al.|[2501.07063](http://arxiv.org/abs/2501.07063)|null|
|**2025-01-13**|**A Proposed Large Language Model-Based Smart Search for Archive System**|Ha Dung Nguyen et.al.|[2501.07024](http://arxiv.org/abs/2501.07024)|null|
|**2025-01-12**|**Shake-VLA: Vision-Language-Action Model-Based System for Bimanual Robotic Manipulations and Liquid Mixing**|Muhamamd Haris Khan et.al.|[2501.06919](http://arxiv.org/abs/2501.06919)|null|
|**2025-01-10**|**VideoRAG: Retrieval-Augmented Generation over Video Corpus**|Soyeong Jeong et.al.|[2501.05874](http://arxiv.org/abs/2501.05874)|null|
|**2025-01-09**|**LLMQuoter: Enhancing RAG Capabilities Through Efficient Quote Extraction From Large Contexts**|Yuri Facanha Bezerra et.al.|[2501.05554](http://arxiv.org/abs/2501.05554)|**[link](https://github.com/yurifacanha/llmquoter)**|
|**2025-01-09**|**Search-o1: Agentic Search-Enhanced Large Reasoning Models**|Xiaoxi Li et.al.|[2501.05366](http://arxiv.org/abs/2501.05366)|**[link](https://github.com/sunnynexus/search-o1)**|
|**2025-01-09**|**RAG-WM: An Efficient Black-Box Watermarking Approach for Retrieval-Augmented Generation of Large Language Models**|Peizhuo Lv et.al.|[2501.05249](http://arxiv.org/abs/2501.05249)|null|
|**2025-01-09**|**Biomedical Relation Extraction via Adaptive Document-Relation Cross-Mapping and Concept Unique Identifier**|Yufei Shang et.al.|[2501.05155](http://arxiv.org/abs/2501.05155)|null|
|**2025-01-09**|**A General Retrieval-Augmented Generation Framework for Multimodal Case-Based Reasoning Applications**|Ofir Marom et.al.|[2501.05030](http://arxiv.org/abs/2501.05030)|null|
|**2025-01-09**|**SUGAR: Leveraging Contextual Confidence for Smarter Retrieval**|Hanna Zubkova et.al.|[2501.04899](http://arxiv.org/abs/2501.04899)|null|
|**2025-01-08**|**Advancing Retrieval-Augmented Generation for Persian: Development of Language Models, Comprehensive Benchmarks, and Best Practices for Optimization**|Sara Bourbour Hosseinbeigi et.al.|[2501.04858](http://arxiv.org/abs/2501.04858)|null|
|**2025-01-08**|**Re-ranking the Context for Multimodal Retrieval Augmented Generation**|Matin Mortaheb et.al.|[2501.04695](http://arxiv.org/abs/2501.04695)|null|
|**2025-01-08**|**Multi-task retriever fine-tuning for domain-specific and efficient RAG**|Patrice Béchard et.al.|[2501.04652](http://arxiv.org/abs/2501.04652)|null|
|**2025-01-08**|**Knowledge Retrieval Based on Generative AI**|Te-Lun Yang et.al.|[2501.04635](http://arxiv.org/abs/2501.04635)|null|
|**2025-01-08**|**Integrating remote sensing data assimilation, deep learning and large language model for interactive wheat breeding yield prediction**|Guofeng Yang et.al.|[2501.04487](http://arxiv.org/abs/2501.04487)|null|
|**2025-01-08**|**End-to-End Bangla AI for Solving Math Olympiad Problem Benchmark: Leveraging Large Language Model Using Integrated Approach**|H. M. Shadman Tabib et.al.|[2501.04425](http://arxiv.org/abs/2501.04425)|null|
|**2025-01-08**|**How Large is the Universe of RNA-Like Motifs? A Clustering Analysis of RNA Graph Motifs Using Topological Descriptors**|Rui Wang et.al.|[2501.04258](http://arxiv.org/abs/2501.04258)|**[link](https://github.com/wangru25/psgrnaclustering)**|
|**2025-01-07**|**RAG-Check: Evaluating Multimodal Retrieval Augmented Generation Performance**|Matin Mortaheb et.al.|[2501.03995](http://arxiv.org/abs/2501.03995)|null|
|**2025-01-08**|**SenseRAG: Constructing Environmental Knowledge Bases with Proactive Querying for LLM-Based Autonomous Driving**|Xuewen Luo et.al.|[2501.03535](http://arxiv.org/abs/2501.03535)|null|
|**2025-01-07**|**Reading with Intent -- Neutralizing Intent**|Benjamin Reichman et.al.|[2501.03475](http://arxiv.org/abs/2501.03475)|null|
|**2025-01-07**|**MTRAG: A Multi-Turn Conversational Benchmark for Evaluating Retrieval-Augmented Generation Systems**|Yannis Katsis et.al.|[2501.03468](http://arxiv.org/abs/2501.03468)|**[link](https://github.com/ibm/mt-rag-benchmark)**|
|**2025-01-06**|**Retrieval-Augmented TLAPS Proof Generation with Large Language Models**|Yuhao Zhou et.al.|[2501.03073](http://arxiv.org/abs/2501.03073)|null|
|**2025-01-06**|**FlipedRAG: Black-Box Opinion Manipulation Attacks to Retrieval-Augmented Generation of Large Language Models**|Zhuo Chen et.al.|[2501.02968](http://arxiv.org/abs/2501.02968)|null|
|**2025-01-06**|**Graph-based Retrieval Augmented Generation for Dynamic Few-shot Text Classification**|Yubo Wang et.al.|[2501.02844](http://arxiv.org/abs/2501.02844)|null|
|**2025-01-06**|**Foundations of GenIR**|Qingyao Ai et.al.|[2501.02842](http://arxiv.org/abs/2501.02842)|null|
|**2025-01-06**|**Tree-based RAG-Agent Recommendation System: A Case Study in Medical Test Data**|Yahe Yang et.al.|[2501.02727](http://arxiv.org/abs/2501.02727)|null|
|**2025-01-06**|**QuIM-RAG: Advancing Retrieval-Augmented Generation with Inverted Question Matching for Enhanced QA Performance**|Binita Saha et.al.|[2501.02702](http://arxiv.org/abs/2501.02702)|null|
|**2025-01-05**|**Towards Omni-RAG: Comprehensive Retrieval-Augmented Generation for Large Language Models in Medical Applications**|Zhe Chen et.al.|[2501.02460](http://arxiv.org/abs/2501.02460)|null|
|**2025-01-04**|**Knowledge Graph Retrieval-Augmented Generation for LLM-based Recommendation**|Shijie Wang et.al.|[2501.02226](http://arxiv.org/abs/2501.02226)|null|
|**2025-01-04**|**The Efficiency vs. Accuracy Trade-off: Optimizing RAG-Enhanced LLM Recommender Systems Using Multi-Head Early Exit**|Huixue Zhou et.al.|[2501.02173](http://arxiv.org/abs/2501.02173)|null|
|**2025-01-04**|**Personalized Graph-Based Retrieval for Large Language Models**|Steven Au et.al.|[2501.02157](http://arxiv.org/abs/2501.02157)|**[link](https://github.com/pgraphrag-benchmark/pgr-llm)**|
|**2025-01-03**|**Automating Legal Concept Interpretation with LLMs: Retrieval, Generation, and Evaluation**|Kangcheng Luo et.al.|[2501.01743](http://arxiv.org/abs/2501.01743)|null|
|**2025-01-02**|**ValuesRAG: Enhancing Cultural Alignment Through Retrieval-Augmented Contextual Learning**|Wonduk Seo et.al.|[2501.01031](http://arxiv.org/abs/2501.01031)|null|
|**2025-01-03**|**KaLM-Embedding: Superior Training Data Brings A Stronger Embedding Model**|Xinshuo Hu et.al.|[2501.01028](http://arxiv.org/abs/2501.01028)|**[link](https://github.com/HITsz-TMG/KaLM-Embedding)**|
|**2025-01-02**|**Are LLMs effective psychological assessors? Leveraging adaptive RAG for interpretable mental health screening through psychometric practice**|Federico Ravenda et.al.|[2501.00982](http://arxiv.org/abs/2501.00982)|**[link](https://github.com/fede-stack/adaptive-rag-for-psychological-assessment)**|
|**2025-01-01**|**TrustRAG: Enhancing Robustness and Trustworthiness in RAG**|Huichi Zhou et.al.|[2501.00879](http://arxiv.org/abs/2501.00879)|**[link](https://github.com/huichizhou/trustrag)**|
|**2025-01-01**|**Decoding the Flow: CauseMotion for Emotional Causality Analysis in Long-form Conversations**|Yuxuan Zhang et.al.|[2501.00778](http://arxiv.org/abs/2501.00778)|null|
|**2025-01-01**|**Beyond Words: AuralLLM and SignMST-C for Precise Sign Language Production and Bidirectional Accessibility**|Yulong Li et.al.|[2501.00765](http://arxiv.org/abs/2501.00765)|null|
|**2025-01-01**|**Beyond Text: Implementing Multimodal Large Language Model-Powered Multi-Agent Systems Using a No-Code Platform**|Cheonsu Jeong et.al.|[2501.00750](http://arxiv.org/abs/2501.00750)|null|
|**2025-01-03**|**An Overview and Discussion on Using Large Language Models for Implementation Generation of Solutions to Open-Ended Problems**|Hashmath Shaik et.al.|[2501.00562](http://arxiv.org/abs/2501.00562)|null|
|**2024-12-31**|**RAG-Instruct: Boosting LLMs with Diverse Retrieval-Augmented Instructions**|Wanlong Liu et.al.|[2501.00353](http://arxiv.org/abs/2501.00353)|**[link](https://github.com/freedomintelligence/rag-instruct)**|
|**2024-12-31**|**MAIN-RAG: Multi-Agent Filtering Retrieval-Augmented Generation**|Chia-Yuan Chang et.al.|[2501.00332](http://arxiv.org/abs/2501.00332)|null|
|**2024-12-30**|**Plancraft: an evaluation dataset for planning with LLM agents**|Gautier Dagan et.al.|[2412.21033](http://arxiv.org/abs/2412.21033)|**[link](https://github.com/gautierdag/plancraft)**|
|**2024-12-31**|**EdgeRAG: Online-Indexed RAG for Edge Devices**|Korakit Seemakhupt et.al.|[2412.21023](http://arxiv.org/abs/2412.21023)|null|
|**2024-12-30**|**GASLITEing the Retrieval: Exploring Vulnerabilities in Dense Embedding-based Search**|Matan Ben-Tov et.al.|[2412.20953](http://arxiv.org/abs/2412.20953)|**[link](https://github.com/matanbt/gaslite)**|
|**2024-12-30**|**Enhanced Multimodal RAG-LLM for Accurate Visual Question Answering**|Junxiao Xue et.al.|[2412.20927](http://arxiv.org/abs/2412.20927)|null|
|**2024-12-30**|**Retrieval-Augmented Generation for Mobile Edge Computing via Large Language Model**|Runtao Ren et.al.|[2412.20820](http://arxiv.org/abs/2412.20820)|null|
|**2024-12-30**|**TimeRAF: Retrieval-Augmented Foundation model for Zero-shot Time Series Forecasting**|Huanyu Zhang et.al.|[2412.20810](http://arxiv.org/abs/2412.20810)|null|
|**2024-12-30**|**Dialogue Director: Bridging the Gap in Dialogue Visualization for Multimodal Storytelling**|Min Zhang et.al.|[2412.20725](http://arxiv.org/abs/2412.20725)|null|
|**2024-12-29**|**A Comprehensive Framework for Reliable Legal AI: Combining Specialized Expert Systems and Adaptive Refinement**|Sidra Nasir et.al.|[2412.20468](http://arxiv.org/abs/2412.20468)|null|
|**2024-12-29**|**Understanding the Impact of Confidence in Retrieval Augmented Generation: A Case Study in the Medical Domain**|Shintaro Ozaki et.al.|[2412.20309](http://arxiv.org/abs/2412.20309)|null|
|**2024-12-27**|**Casevo: A Cognitive Agents and Social Evolution Simulator**|Zexun Jiang et.al.|[2412.19498](http://arxiv.org/abs/2412.19498)|**[link](https://github.com/rgcass/casevo)**|
|**2024-12-27**|**Retrieval-augmented Generation for GenAI-enabled Semantic Communications**|Shunpu Tang et.al.|[2412.19494](http://arxiv.org/abs/2412.19494)|null|
|**2024-12-26**|**From Interets to Insights: An LLM Approach to Course Recommendations Using Natural Language Queries**|Hugh Van Deventer et.al.|[2412.19312](http://arxiv.org/abs/2412.19312)|**[link](https://github.com/hughvd/um-cai-fellowship)**|
|**2024-12-26**|**RAG with Differential Privacy**|Nicolas Grislain et.al.|[2412.19291](http://arxiv.org/abs/2412.19291)|**[link](https://github.com/sarus-tech/dp-rag)**|
|**2024-12-26**|**Jasper and Stella: distillation of SOTA embedding models**|Dun Zhang et.al.|[2412.19048](http://arxiv.org/abs/2412.19048)|**[link](https://github.com/NLPJCL/RAG-Retrieval)**|
|**2024-12-24**|**DynaGRAG: Improving Language Understanding and Generation through Dynamic Subgraph Representation in Graph Retrieval-Augmented Generation**|Karishma Thakrar et.al.|[2412.18644](http://arxiv.org/abs/2412.18644)|null|
|**2024-12-24**|**GeAR: Graph-enhanced Agent for Retrieval-augmented Generation**|Zhili Shen et.al.|[2412.18431](http://arxiv.org/abs/2412.18431)|null|
|**2024-12-24**|**Pirates of the RAG: Adaptively Attacking LLMs to Leak Knowledge Bases**|Christian Di Maio et.al.|[2412.18295](http://arxiv.org/abs/2412.18295)|null|
|**2024-12-24**|**EvoPat: A Multi-LLM-based Patents Summarization and Analysis Agent**|Suyuan Wang et.al.|[2412.18100](http://arxiv.org/abs/2412.18100)|null|
|**2024-12-24**|**Molly: Making Large Language Model Agents Solve Python Problem More Logically**|Rui Xiao et.al.|[2412.18093](http://arxiv.org/abs/2412.18093)|null|
|**2024-12-24**|**Improving Factuality with Explicit Working Memory**|Mingda Chen et.al.|[2412.18069](http://arxiv.org/abs/2412.18069)|null|
|**2024-12-23**|**Correctness is not Faithfulness in RAG Attributions**|Jonas Wallat et.al.|[2412.18004](http://arxiv.org/abs/2412.18004)|null|
|**2024-12-23**|**Dynamic Multi-Agent Orchestration and Retrieval for Multi-Source Question-Answer Systems using Large Language Models**|Antony Seabra et.al.|[2412.17964](http://arxiv.org/abs/2412.17964)|null|
|**2024-12-23**|**Contrato360 2.0: A Document and Database-Driven Question-Answer System using Large Language Models and Agents**|Antony Seabra et.al.|[2412.17942](http://arxiv.org/abs/2412.17942)|null|
|**2024-12-24**|**RAGONITE: Iterative Retrieval on Induced Databases and Verbalized RDF for Conversational QA over KGs with RAG**|Rishiraj Saha Roy et.al.|[2412.17690](http://arxiv.org/abs/2412.17690)|null|
|**2024-12-23**|**A Survey of Query Optimization in Large Language Models**|Mingyang Song et.al.|[2412.17558](http://arxiv.org/abs/2412.17558)|null|
|**2024-12-23**|**A Silver Bullet or a Compromise for Full Attention? A Comprehensive Study of Gist Token-based Context Compression**|Chenlong Deng et.al.|[2412.17483](http://arxiv.org/abs/2412.17483)|null|
|**2024-12-23**|**Efficient fine-tuning methodology of text embedding models for information retrieval: contrastive learning penalty (clp)**|Jeongsu Yu et.al.|[2412.17364](http://arxiv.org/abs/2412.17364)|**[link](https://github.com/crealabs/enhanced-bge-m3-with-clp-and-moe)**|
|**2024-12-22**|**LLM Agent for Fire Dynamics Simulations**|Leidong Xu et.al.|[2412.17146](http://arxiv.org/abs/2412.17146)|null|
|**2024-12-22**|**The HalluRAG Dataset: Detecting Closed-Domain Hallucinations in RAG Applications Using an LLM's Internal States**|Fabian Ridder et.al.|[2412.17056](http://arxiv.org/abs/2412.17056)|**[link](https://github.com/f4biian/hallurag)**|
|**2024-12-22**|**MINTQA: A Multi-Hop Question Answering Benchmark for Evaluating LLMs on New and Tail Knowledge**|Jie He et.al.|[2412.17032](http://arxiv.org/abs/2412.17032)|null|
|**2024-12-22**|**A Reality Check on Context Utilisation for Retrieval-Augmented Generation**|Lovisa Hagström et.al.|[2412.17031](http://arxiv.org/abs/2412.17031)|**[link](https://github.com/copenlu/context-utilisation-for-rag)**|
|**2024-12-21**|**Towards More Robust Retrieval-Augmented Generation: Evaluating RAG Under Adversarial Poisoning Attacks**|Jinyan Su et.al.|[2412.16708](http://arxiv.org/abs/2412.16708)|**[link](https://github.com/jinyansu1/eval_poisonrag)**|
|**2024-12-21**|**AlzheimerRAG: Multimodal Retrieval Augmented Generation for PubMed articles**|Aritra Kumar Lahiri et.al.|[2412.16701](http://arxiv.org/abs/2412.16701)|null|
|**2024-12-20**|**Towards Interpretable Radiology Report Generation via Concept Bottlenecks using a Multi-Agentic RAG**|Hasan Md Tusfiqur Alam et.al.|[2412.16086](http://arxiv.org/abs/2412.16086)|**[link](https://github.com/tifat58/irr-with-cbm-rag)**|
|**2024-12-20**|**On the Suitability of pre-trained foundational LLMs for Analysis in German Legal Education**|Lorenz Wendlinger et.al.|[2412.15902](http://arxiv.org/abs/2412.15902)|null|
|**2024-12-20**|**Don't Do RAG: When Cache-Augmented Generation is All You Need for Knowledge Tasks**|Brian J Chan et.al.|[2412.15605](http://arxiv.org/abs/2412.15605)|**[link](https://github.com/hhhuang/cag)**|
|**2024-12-20**|**MRAG: A Modular Retrieval Framework for Time-Sensitive Question Answering**|Zhang Siyue et.al.|[2412.15540](http://arxiv.org/abs/2412.15540)|null|
|**2024-12-20**|**XRAG: eXamining the Core -- Benchmarking Foundational Components in Advanced Retrieval-Augmented Generation**|Qianren Mao et.al.|[2412.15529](http://arxiv.org/abs/2412.15529)|**[link](https://github.com/docailab/xrag)**|
|**2024-12-19**|**SKETCH: Structured Knowledge Enhanced Text Comprehension for Holistic Retrieval**|Aakash Mahalingam et.al.|[2412.15443](http://arxiv.org/abs/2412.15443)|null|
|**2024-12-19**|**A Retrieval-Augmented Generation Framework for Academic Literature Navigation in Data Science**|Ahmet Yasin Aytar et.al.|[2412.15404](http://arxiv.org/abs/2412.15404)|null|
|**2024-12-19**|**Face the Facts! Evaluating RAG-based Fact-checking Pipelines in Realistic Settings**|Daniel Russo et.al.|[2412.15189](http://arxiv.org/abs/2412.15189)|**[link](https://github.com/drusso98/face-the-facts)**|
|**2024-12-19**|**Review-Then-Refine: A Dynamic Framework for Multi-Hop Question Answering with Temporal Adaptability**|Xiangsen Chen et.al.|[2412.15101](http://arxiv.org/abs/2412.15101)|null|
|**2024-12-19**|**Knowledge Injection via Prompt Distillation**|Kalle Kujanpää et.al.|[2412.14964](http://arxiv.org/abs/2412.14964)|null|
|**2024-12-19**|**Dehallucinating Parallel Context Extension for Retrieval-Augmented Generation**|Zexiong Ma et.al.|[2412.14905](http://arxiv.org/abs/2412.14905)|null|
|**2024-12-19**|**DynamicKV: Task-Aware Adaptive KV Cache Compression for Long Context LLMs**|Xiabin Zhou et.al.|[2412.14838](http://arxiv.org/abs/2412.14838)|null|
|**2024-12-19**|**Query pipeline optimization for cancer patient question answering systems**|Maolin He et.al.|[2412.14751](http://arxiv.org/abs/2412.14751)|null|
|**2024-12-19**|**CORD: Balancing COnsistency and Rank Distillation for Robust Retrieval-Augmented Generation**|Youngwon Lee et.al.|[2412.14581](http://arxiv.org/abs/2412.14581)|null|
|**2024-12-19**|**PA-RAG: RAG Alignment via Multi-Perspective Preference Optimization**|Jiayi Wu et.al.|[2412.14510](http://arxiv.org/abs/2412.14510)|**[link](https://github.com/wujwyi/pa-rag)**|
|**2024-12-19**|**VISA: Retrieval Augmented Generation with Visual Source Attribution**|Xueguang Ma et.al.|[2412.14457](http://arxiv.org/abs/2412.14457)|null|
|**2024-12-18**|**Multi-OphthaLingua: A Multilingual Benchmark for Assessing and Debiasing LLM Ophthalmological QA in LMICs**|David Restrepo et.al.|[2412.14304](http://arxiv.org/abs/2412.14304)|null|
|**2024-12-18**|**RAG for Effective Supply Chain Security Questionnaire Automation**|Zaynab Batool Reza et.al.|[2412.13988](http://arxiv.org/abs/2412.13988)|null|
|**2024-12-18**|**Language verY Rare for All**|Ibrahim Merad et.al.|[2412.13924](http://arxiv.org/abs/2412.13924)|null|
|**2024-12-18**|**Enhancing Rhetorical Figure Annotation: An Ontology-Based Web Application with RAG Integration**|Ramona Kühn et.al.|[2412.13799](http://arxiv.org/abs/2412.13799)|**[link](https://github.com/kuehnram/findyourfigure)**|
|**2024-12-18**|**Designing an LLM-Based Copilot for Manufacturing Equipment Selection**|Jonas Werheid et.al.|[2412.13774](http://arxiv.org/abs/2412.13774)|null|
|**2024-12-18**|**RAG-RewardBench: Benchmarking Reward Models in Retrieval Augmented Generation for Preference Alignment**|Zhuoran Jin et.al.|[2412.13746](http://arxiv.org/abs/2412.13746)|**[link](https://github.com/jinzhuoran/rag-rewardbench)**|
|**2024-12-18**|**Federated Learning and RAG Integration: A Scalable Approach for Medical Large Language Models**|Jincheol Jung et.al.|[2412.13720](http://arxiv.org/abs/2412.13720)|null|
|**2024-12-18**|**A2H: A UI Converter from Android to HarmonyOS Platform**|Chen Wang et.al.|[2412.13693](http://arxiv.org/abs/2412.13693)|null|
|**2024-12-18**|**EvoWiki: Evaluating LLMs on Evolving Knowledge**|Wei Tang et.al.|[2412.13582](http://arxiv.org/abs/2412.13582)|null|
|**2024-12-17**|**C-FedRAG: A Confidential Federated Retrieval-Augmented Generation System**|Parker Addison et.al.|[2412.13163](http://arxiv.org/abs/2412.13163)|null|
|**2024-12-17**|**OmniEval: An Omnidirectional and Automatic RAG Evaluation Benchmark in Financial Domain**|Shuting Wang et.al.|[2412.13018](http://arxiv.org/abs/2412.13018)|**[link](https://github.com/ruc-nlpir/omnieval)**|
|**2024-12-17**|**Adaptations of AI models for querying the LandMatrix database in natural language**|Fatiha Ait Kbir et.al.|[2412.12961](http://arxiv.org/abs/2412.12961)|**[link](https://github.com/tetis-nlp/landmatrix-graphql-python)**|
|**2024-12-17**|**RAG-Star: Enhancing Deliberative Reasoning with Retrieval Augmented Verification and Refinement**|Jinhao Jiang et.al.|[2412.12881](http://arxiv.org/abs/2412.12881)|null|
|**2024-12-17**|**RemoteRAG: A Privacy-Preserving LLM Cloud RAG Service**|Yihang Cheng et.al.|[2412.12775](http://arxiv.org/abs/2412.12775)|null|
|**2024-12-17**|**What External Knowledge is Preferred by LLMs? Characterizing and Exploring Chain of Evidence in Imperfect Context**|Zhiyuan Chang et.al.|[2412.12632](http://arxiv.org/abs/2412.12632)|null|
|**2024-12-17**|**EXIT: Context-Aware Extractive Compression for Enhancing Retrieval-Augmented Generation**|Taeho Hwang et.al.|[2412.12559](http://arxiv.org/abs/2412.12559)|**[link](https://github.com/thisishwang/exit)**|
|**2024-12-17**|**PERC: Plan-As-Query Example Retrieval for Underrepresented Code Generation**|Jaeseok Yoo et.al.|[2412.12447](http://arxiv.org/abs/2412.12447)|null|
|**2024-12-16**|**LogBabylon: A Unified Framework for Cross-Log File Integration and Analysis**|Rabimba Karanjai et.al.|[2412.12364](http://arxiv.org/abs/2412.12364)|null|
|**2024-12-16**|**BioRAGent: A Retrieval-Augmented Generation System for Showcasing Generative Query Expansion and Domain-Specific Search for Scientific Q&A**|Samy Ateia et.al.|[2412.12358](http://arxiv.org/abs/2412.12358)|**[link](https://github.com/SamyAteia/BioRAGent)**|
|**2024-12-16**|**Agentic AI-Driven Technical Troubleshooting for Enterprise Systems: A Novel Weighted Retrieval-Augmented Generation Paradigm**|Rajat Khanda et.al.|[2412.12006](http://arxiv.org/abs/2412.12006)|null|
|**2024-12-16**|**RetroLLM: Empowering Large Language Models to Retrieve Fine-grained Evidence within Generation**|Xiaoxi Li et.al.|[2412.11919](http://arxiv.org/abs/2412.11919)|**[link](https://github.com/sunnynexus/retrollm)**|
|**2024-12-16**|**Towards Understanding Systems Trade-offs in Retrieval-Augmented Generation Model Inference**|Michael Shen et.al.|[2412.11854](http://arxiv.org/abs/2412.11854)|null|
|**2024-12-16**|**GHIssuemarket: A Sandbox Environment for SWE-Agents Economic Experimentation**|Mohamed A. Fouad et.al.|[2412.11722](http://arxiv.org/abs/2412.11722)|**[link](https://github.com/lascam-ufu/ghissuemarketsandbox)**|
|**2024-12-16**|**Let your LLM generate a few tokens and you will reduce the need for retrieval**|Hervé Déjean et.al.|[2412.11536](http://arxiv.org/abs/2412.11536)|null|
|**2024-12-16**|**Attention with Dependency Parsing Augmentation for Fine-Grained Attribution**|Qiang Ding et.al.|[2412.11404](http://arxiv.org/abs/2412.11404)|null|
|**2024-12-15**|**One-Shot Multilingual Font Generation Via ViT**|Zhiheng Wang et.al.|[2412.11342](http://arxiv.org/abs/2412.11342)|null|
|**2024-12-15**|**RAC3: Retrieval-Augmented Corner Case Comprehension for Autonomous Driving with Vision-Language Models**|Yujin Wang et.al.|[2412.11050](http://arxiv.org/abs/2412.11050)|null|
|**2024-12-14**|**SusGen-GPT: A Data-Centric LLM for Financial NLP and Sustainability Report Generation**|Qilong Wu et.al.|[2412.10906](http://arxiv.org/abs/2412.10906)|**[link](https://github.com/jerrywu-code/susgen)**|
|**2024-12-14**|**VisDoM: Multi-Document QA with Visually Rich Elements Using Multimodal Retrieval-Augmented Generation**|Manan Suri et.al.|[2412.10704](http://arxiv.org/abs/2412.10704)|null|
|**2024-12-13**|**MST-R: Multi-Stage Tuning for Retrieval Systems and Metric Evaluation**|Yash Malviya et.al.|[2412.10313](http://arxiv.org/abs/2412.10313)|**[link](https://github.com/indic-aidias/mst-r)**|
|**2024-12-13**|**VLR-Bench: Multilingual Benchmark Dataset for Vision-Language Retrieval Augmented Generation**|Hyeonseok Lim et.al.|[2412.10151](http://arxiv.org/abs/2412.10151)|null|
|**2024-12-13**|**CaLoRAify: Calorie Estimation with Visual-Text Pairing and LoRA-Driven Visual Language Models**|Dongyu Yao et.al.|[2412.09936](http://arxiv.org/abs/2412.09936)|**[link](https://github.com/kennyyao2001/16824-caloraify)**|
|**2024-12-12**|**Context Canvas: Enhancing Text-to-Image Diffusion Models with Knowledge Graph-Based RAG**|Kavana Venkatesh et.al.|[2412.09614](http://arxiv.org/abs/2412.09614)|null|
|**2024-12-12**|**Assessing the Robustness of Retrieval-Augmented Generation Systems in K-12 Educational Question Answering with Knowledge Discrepancies**|Tianshi Zheng et.al.|[2412.08985](http://arxiv.org/abs/2412.08985)|null|
|**2024-12-11**|**Leveraging Graph-RAG and Prompt Engineering to Enhance LLM-Based Automated Requirement Traceability and Compliance Checks**|Arsalan Masoudifard et.al.|[2412.08593](http://arxiv.org/abs/2412.08593)|null|
|**2024-12-11**|**Bridging Relevance and Reasoning: Rationale Distillation in Retrieval-Augmented Generation**|Pengyue Jia et.al.|[2412.08519](http://arxiv.org/abs/2412.08519)|null|
|**2024-12-11**|**Federated In-Context LLM Agent Learning**|Panlong Wu et.al.|[2412.08054](http://arxiv.org/abs/2412.08054)|null|
|**2024-12-10**|**Granite Guardian**|Inkit Padhi et.al.|[2412.07724](http://arxiv.org/abs/2412.07724)|**[link](https://github.com/ibm-granite/granite-guardian)**|
|**2024-12-10**|**Privacy-Preserving Customer Support: A Framework for Secure and Scalable Interactions**|Anant Prakash Awasthi et.al.|[2412.07687](http://arxiv.org/abs/2412.07687)|null|
|**2024-12-10**|**OmniDocBench: Benchmarking Diverse PDF Document Parsing with Comprehensive Annotations**|Linke Ouyang et.al.|[2412.07626](http://arxiv.org/abs/2412.07626)|**[link](https://github.com/opendatalab/OmniDocBench)**|
|**2024-12-10**|**Adapting to Non-Stationary Environments: Multi-Armed Bandit Enhanced Retrieval-Augmented Generation on Knowledge Graphs**|Xiaqiang Tang et.al.|[2412.07618](http://arxiv.org/abs/2412.07618)|**[link](https://github.com/futureeeeee/dynamic-rag)**|
|**2024-12-10**|**Automatic Database Configuration Debugging using Retrieval-Augmented Language Models**|Sibei Chen et.al.|[2412.07548](http://arxiv.org/abs/2412.07548)|null|
|**2024-12-10**|**RAG-based Question Answering over Heterogeneous Data and Text**|Philipp Christmann et.al.|[2412.07420](http://arxiv.org/abs/2412.07420)|null|
|**2024-12-10**|**Generating Knowledge Graphs from Large Language Models: A Comparative Study of GPT-4, LLaMA 2, and BERT**|Ahan Bhatt et.al.|[2412.07412](http://arxiv.org/abs/2412.07412)|null|
|**2024-12-10**|**When Graph Meets Retrieval Augmented Generation for Wireless Networks: A Tutorial and Case Study**|Yang Xiong et.al.|[2412.07189](http://arxiv.org/abs/2412.07189)|null|
|**2024-12-09**|**Retrieving Semantics from the Deep: an RAG Solution for Gesture Synthesis**|M. Hamza Mughal et.al.|[2412.06786](http://arxiv.org/abs/2412.06786)|null|
|**2024-12-09**|**SiReRAG: Indexing Similar and Related Information for Multihop Reasoning**|Nan Zhang et.al.|[2412.06206](http://arxiv.org/abs/2412.06206)|null|
|**2024-12-08**|**DECO: Life-Cycle Management of Enterprise-Grade Chatbots**|Yiwen Zhu et.al.|[2412.06099](http://arxiv.org/abs/2412.06099)|null|
|**2024-12-08**|**Mixture-of-PageRanks: Replacing Long-Context with Real-Time, Sparse GraphRAG**|Nicholas Alonso et.al.|[2412.06078](http://arxiv.org/abs/2412.06078)|null|
|**2024-12-08**|**1-800-SHARED-TASKS at RegNLP: Lexical Reranking of Semantic Retrieval (LeSeR) for Regulatory Question Answering**|Jebish Purbey et.al.|[2412.06009](http://arxiv.org/abs/2412.06009)|null|
|**2024-12-08**|**Accelerating Manufacturing Scale-Up from Material Discovery Using Agentic Web Navigation and Retrieval-Augmented AI for Process Engineering Schematics Design**|Sakhinana Sagar Srinivas et.al.|[2412.05937](http://arxiv.org/abs/2412.05937)|null|
|**2024-12-08**|**A Collaborative Multi-Agent Approach to Retrieval-Augmented Generation Across Diverse Data**|Aniruddha Salve et.al.|[2412.05838](http://arxiv.org/abs/2412.05838)|null|
|**2024-12-07**|**GEE-OPs: An Operator Knowledge Base for Geospatial Code Generation on the Google Earth Engine Platform Powered by Large Language Models**|Shuyang Hou et.al.|[2412.05587](http://arxiv.org/abs/2412.05587)|null|
|**2024-12-07**|**KG-Retriever: Efficient Knowledge Indexing for Retrieval-Augmented Large Language Models**|Weijie Chen et.al.|[2412.05547](http://arxiv.org/abs/2412.05547)|null|
|**2024-12-06**|**A Graph-Based Approach for Conversational AI-Driven Personal Memory Capture and Retrieval in a Real-world Application**|Savini Kashmira et.al.|[2412.05447](http://arxiv.org/abs/2412.05447)|null|
|**2024-12-06**|**100% Hallucination Elimination Using Acurai**|Michael C. Wood et.al.|[2412.05223](http://arxiv.org/abs/2412.05223)|**[link](https://github.com/AcuChat/acurai-RAGTruth-conflict-resolution)**|
|**2024-12-06**|**ConQRet: Benchmarking Fine-Grained Evaluation of Retrieval Augmented Argumentation with LLM Judges**|Kaustubh D. Dhole et.al.|[2412.05206](http://arxiv.org/abs/2412.05206)|**[link](https://github.com/emory-irlab/conqret-rag)**|
|**2024-12-06**|**SurgBox: Agent-Driven Operating Room Sandbox with Surgery Copilot**|Jinlin Wu et.al.|[2412.05187](http://arxiv.org/abs/2412.05187)|**[link](https://github.com/franciszchen/surgbox)**|
|**2024-12-06**|**QueEn: A Large Language Model for Quechua-English Translation**|Junhao Chen et.al.|[2412.05184](http://arxiv.org/abs/2412.05184)|null|
|**2024-12-06**|**Enhancing Cross-Language Code Translation via Task-Specific Embedding Alignment in Retrieval-Augmented Generation**|Manish Bhattarai et.al.|[2412.05159](http://arxiv.org/abs/2412.05159)|null|
|**2024-12-06**|**Question Answering for Decisionmaking in Green Building Design: A Multimodal Data Reasoning Method Driven by Large Language Models**|Yihui Li et.al.|[2412.04741](http://arxiv.org/abs/2412.04741)|null|
|**2024-12-06**|**Privacy-Preserving Retrieval Augmented Generation with Differential Privacy**|Tatsuki Koga et.al.|[2412.04697](http://arxiv.org/abs/2412.04697)|null|
|**2024-12-05**|**HEAL: Hierarchical Embedding Alignment Loss for Improved Retrieval and Representation Learning**|Manish Bhattarai et.al.|[2412.04661](http://arxiv.org/abs/2412.04661)|**[link](https://github.com/lanl/t-elf)**|
|**2024-12-05**|**Targeting the Core: A Simple and Effective Method to Attack RAG-based Agents via Direct LLM Manipulation**|Xuying Li et.al.|[2412.04415](http://arxiv.org/abs/2412.04415)|null|
|**2024-12-05**|**Retrieval-Augmented Machine Translation with Unstructured Knowledge**|Jiaan Wang et.al.|[2412.04342](http://arxiv.org/abs/2412.04342)|**[link](https://github.com/krystalan/RAGtrans)**|
|**2024-12-05**|**Addressing Hallucinations with RAG and NMISS in Italian Healthcare LLM Chatbots**|Maria Paola Priola et.al.|[2412.04235](http://arxiv.org/abs/2412.04235)|null|
|**2024-12-05**|**Leveraging Large Language Models to Generate Course-specific Semantically Annotated Learning Objects**|Dominic Lohr et.al.|[2412.04185](http://arxiv.org/abs/2412.04185)|null|
|**2024-12-05**|**Exploring AI Text Generation, Retrieval-Augmented Generation, and Detection Technologies: a Comprehensive Overview**|Fnu Neha et.al.|[2412.03933](http://arxiv.org/abs/2412.03933)|null|
|**2024-12-04**|**A Review on Scientific Knowledge Extraction using Large Language Models in Biomedical Sciences**|Gabriel Lino Garcia et.al.|[2412.03531](http://arxiv.org/abs/2412.03531)|null|
|**2024-12-04**|**Advancing Conversational Psychotherapy: Integrating Privacy, Dual-Memory, and Domain Expertise with Large Language Models**|XiuYu Zhang et.al.|[2412.02987](http://arxiv.org/abs/2412.02987)|null|
|**2024-12-03**|**CAISSON: Concept-Augmented Inference Suite of Self-Organizing Neural Networks**|Igor Halperin et.al.|[2412.02835](http://arxiv.org/abs/2412.02835)|null|
|**2024-12-05**|**Hybrid-SQuAD: Hybrid Scholarly Question Answering Dataset**|Tilahun Abedissa Taffa et.al.|[2412.02788](http://arxiv.org/abs/2412.02788)|**[link](https://github.com/semantic-systems/hybrid-squad)**|
|**2024-12-03**|**OCR Hinders RAG: Evaluating the Cascading Impact of OCR on Retrieval-Augmented Generation**|Junyuan Zhang et.al.|[2412.02592](http://arxiv.org/abs/2412.02592)|**[link](https://github.com/opendatalab/OHR-Bench)**|
|**2024-12-03**|**Semantic Tokens in Retrieval Augmented Generation**|Joel Suro et.al.|[2412.02563](http://arxiv.org/abs/2412.02563)|null|
|**2024-12-03**|**Composing Open-domain Vision with RAG for Ocean Monitoring and Conservation**|Sepand Dyanatkar et.al.|[2412.02262](http://arxiv.org/abs/2412.02262)|null|
|**2024-12-03**|**Leveraging Large Language Models to Democratize Access to Costly Financial Datasets for Academic Research**|Julian Junyan Wang et.al.|[2412.02065](http://arxiv.org/abs/2412.02065)|null|
|**2024-12-02**|**Query Performance Explanation through Large Language Model for HTAP Systems**|Haibo Xiu et.al.|[2412.01709](http://arxiv.org/abs/2412.01709)|null|
|**2024-12-02**|**Medchain: Bridging the Gap Between LLM Agents and Clinical Practice through Interactive Sequential Benchmarking**|Jie Liu et.al.|[2412.01605](http://arxiv.org/abs/2412.01605)|null|
|**2024-12-03**|**MBA-RAG: a Bandit Approach for Adaptive Retrieval-Augmented Generation through Question Complexity**|Xiaqiang Tang et.al.|[2412.01572](http://arxiv.org/abs/2412.01572)|**[link](https://github.com/futureeeeee/mba)**|
|**2024-12-01**|**Improving Multimodal LLMs Ability In Geometry Problem Solving, Reasoning, And Multistep Scoring**|Avinash Anand et.al.|[2412.00846](http://arxiv.org/abs/2412.00846)|null|
|**2024-12-03**|**Leveraging LLM for Automated Ontology Extraction and Knowledge Graph Generation**|Mohammad Sadeq Abolhasani et.al.|[2412.00608](http://arxiv.org/abs/2412.00608)|null|
|**2024-11-30**|**Rethinking Strategic Mechanism Design In The Age Of Large Language Models: New Directions For Communication Systems**|Ismail Lotfi et.al.|[2412.00495](http://arxiv.org/abs/2412.00495)|null|
|**2024-11-29**|**Advanced System Integration: Analyzing OpenAPI Chunking for Retrieval-Augmented Generation**|Robin D. Pesl et.al.|[2411.19804](http://arxiv.org/abs/2411.19804)|null|
|**2024-12-02**|**CantorNet: A Sandbox for Testing Geometrical and Topological Complexity Measures**|Michal Lewandowski et.al.|[2411.19713](http://arxiv.org/abs/2411.19713)|**[link](https://github.com/michalmariuszlewandowski/cantornet)**|
|**2024-11-29**|**Know Your RAG: Dataset Taxonomy and Generation Strategies for Evaluating RAG Systems**|Rafael Teixeira de Lima et.al.|[2411.19710](http://arxiv.org/abs/2411.19710)|null|
|**2024-11-29**|**Unimib Assistant: designing a student-friendly RAG-based chatbot for all their needs**|Chiara Antico et.al.|[2411.19554](http://arxiv.org/abs/2411.19554)|null|
|**2024-11-29**|**Knowledge Management for Automobile Failure Analysis Using Graph RAG**|Yuta Ojima et.al.|[2411.19539](http://arxiv.org/abs/2411.19539)|null|
|**2024-11-29**|**RAGDiffusion: Faithful Cloth Generation via External Knowledge Assimilation**|Xianfeng Tan et.al.|[2411.19528](http://arxiv.org/abs/2411.19528)|null|
|**2024-11-29**|**Zero-Indexing Internet Search Augmented Generation for Large Language Models**|Guangxin He et.al.|[2411.19478](http://arxiv.org/abs/2411.19478)|null|
|**2024-11-29**|**Towards Understanding Retrieval Accuracy and Prompt Quality in RAG Systems**|Shengming Zhao et.al.|[2411.19463](http://arxiv.org/abs/2411.19463)|null|
|**2024-11-29**|**Auto-RAG: Autonomous Retrieval-Augmented Generation for Large Language Models**|Tian Yu et.al.|[2411.19443](http://arxiv.org/abs/2411.19443)|**[link](https://github.com/ictnlp/auto-rag)**|
|**2024-11-28**|**Habit Coach: Customising RAG-based chatbots to support behavior change**|Arian Fooroogh Mand Arabi et.al.|[2411.19229](http://arxiv.org/abs/2411.19229)|null|
|**2024-11-27**|**Automated Literature Review Using NLP Techniques and LLM-Based Retrieval-Augmented Generation**|Nurshat Fateh Ali et.al.|[2411.18583](http://arxiv.org/abs/2411.18583)|null|
|**2024-11-27**|**Evaluating and Improving the Robustness of Security Attack Detectors Generated by LLMs**|Samuele Pasini et.al.|[2411.18216](http://arxiv.org/abs/2411.18216)|**[link](https://github.com/PasiniSamuele/Robust-Attack-Detectors-LLM)**|
|**2024-11-26**|**Path-RAG: Knowledge-Guided Key Region Retrieval for Open-ended Pathology Visual Question Answering**|Awais Naeem et.al.|[2411.17073](http://arxiv.org/abs/2411.17073)|**[link](https://github.com/embedded-robotics/path-rag)**|
|**2024-11-23**|**Document Haystacks: Vision-Language Reasoning Over Piles of 1000+ Documents**|Jun Chen et.al.|[2411.16740](http://arxiv.org/abs/2411.16740)|**[link](https://github.com/vision-cair/dochaystacks)**|
|**2024-11-23**|**Multi-Reranker: Maximizing performance of retrieval-augmented generation in the FinanceRAG challenge**|Joohyun Lee et.al.|[2411.16732](http://arxiv.org/abs/2411.16732)|**[link](https://github.com/cv-lee/financerag)**|
|**2024-11-25**|**LaB-RAG: Label Boosted Retrieval Augmented Generation for Radiology Report Generation**|Steven Song et.al.|[2411.16523](http://arxiv.org/abs/2411.16523)|**[link](https://github.com/uc-cdis/label-boosted-RAG-for-RRG)**|
|**2024-11-25**|**AtomR: Atomic Operator-Empowered Large Language Models for Heterogeneous Knowledge Reasoning**|Amy Xin et.al.|[2411.16495](http://arxiv.org/abs/2411.16495)|**[link](https://github.com/THU-KEG/AtomR)**|
|**2024-11-25**|**Human-Calibrated Automated Testing and Validation of Generative Language Models**|Agus Sudjianto et.al.|[2411.16391](http://arxiv.org/abs/2411.16391)|null|
|**2024-11-25**|**Multi-modal Retrieval Augmented Multi-modal Generation: A Benchmark, Evaluate Metrics and Strong Baselines**|Zi-Ao Ma et.al.|[2411.16365](http://arxiv.org/abs/2411.16365)|null|
|**2024-11-25**|**Context Awareness Gate For Retrieval Augmented Generation**|Mohammad Hassan Heydari et.al.|[2411.16133](http://arxiv.org/abs/2411.16133)|**[link](https://github.com/heydaari/CAG)**|
|**2024-11-24**|**RAMIE: Retrieval-Augmented Multi-task Information Extraction with Large Language Models on Dietary Supplements**|Zaifu Zhan et.al.|[2411.15700](http://arxiv.org/abs/2411.15700)|null|
|**2024-11-23**|**From MTEB to MTOB: Retrieval-Augmented Classification for Descriptive Grammars**|Albert Kornilov et.al.|[2411.15577](http://arxiv.org/abs/2411.15577)|**[link](https://github.com/al-the-eigenvalue/rag-on-grammars)**|
|**2024-11-23**|**Traditional Chinese Medicine Case Analysis System for High-Level Semantic Abstraction: Optimized with Prompt and RAG**|Peng Xu et.al.|[2411.15491](http://arxiv.org/abs/2411.15491)|null|
|**2024-11-23**|**Improving Factuality of 3D Brain MRI Report Generation with Paired Image-domain Retrieval and Text-domain Augmentation**|Junhyeok Lee et.al.|[2411.15490](http://arxiv.org/abs/2411.15490)|null|
|**2024-11-22**|**mR $^2$ AG: Multimodal Retrieval-Reflection-Augmented Generation for Knowledge-Based VQA**|Tao Zhang et.al.|[2411.15041](http://arxiv.org/abs/2411.15041)|null|
|**2024-11-22**|**KBAda: Efficient Self Adaptation on Specific Knowledge Bases**|Zheni Zeng et.al.|[2411.14790](http://arxiv.org/abs/2411.14790)|**[link](https://github.com/thunlp/kbalign)**|
|**2024-11-21**|**G-RAG: Knowledge Expansion in Material Science**|Radeen Mostafa et.al.|[2411.14592](http://arxiv.org/abs/2411.14592)|**[link](https://github.com/RadeenXALNW/G-RAG_1.0)**|
|**2024-11-21**|**Towards Knowledge Checking in Retrieval-augmented Generation: A Representation Perspective**|Shenglai Zeng et.al.|[2411.14572](http://arxiv.org/abs/2411.14572)|null|
|**2024-11-21**|**Efficient Aspect-Based Summarization of Climate Change Reports with Small Language Models**|Iacopo Ghinassi et.al.|[2411.14272](http://arxiv.org/abs/2411.14272)|**[link](https://github.com/ighina/llmclimate2024)**|
|**2024-11-21**|**Towards Context-Rich Automated Biodiversity Assessments: Deriving AI-Powered Insights from Camera Trap Data**|Paul Fergus et.al.|[2411.14219](http://arxiv.org/abs/2411.14219)|null|
|**2024-11-21**|**RAG-Thief: Scalable Extraction of Private Data from Retrieval-Augmented Generation Applications with Agent-based Attacks**|Changyue Jiang et.al.|[2411.14110](http://arxiv.org/abs/2411.14110)|null|
|**2024-11-21**|**FastRAG: Retrieval Augmented Generation for Semi-structured Data**|Amar Abane et.al.|[2411.13773](http://arxiv.org/abs/2411.13773)|null|
|**2024-11-20**|**Retrieval-Augmented Generation for Domain-Specific Question Answering: A Case Study on Pittsburgh and CMU**|Haojia Sun et.al.|[2411.13691](http://arxiv.org/abs/2411.13691)|null|
|**2024-11-20**|**On the Way to LLM Personalization: Learning to Remember User Conversations**|Lucie Charlotte Magister et.al.|[2411.13405](http://arxiv.org/abs/2411.13405)|null|
|**2024-11-20**|**AIDBench: A benchmark for evaluating the authorship identification capability of large language models**|Zichen Wen et.al.|[2411.13226](http://arxiv.org/abs/2411.13226)|null|
|**2024-11-20**|**Writing Style Matters: An Examination of Bias and Fairness in Information Retrieval Systems**|Hongliu Cao et.al.|[2411.13173](http://arxiv.org/abs/2411.13173)|null|
|**2024-11-20**|**Unlocking Historical Clinical Trial Data with ALIGN: A Compositional Large Language Model System for Medical Coding**|Nabeel Seedat et.al.|[2411.13163](http://arxiv.org/abs/2411.13163)|null|
|**2024-11-20**|**DMQR-RAG: Diverse Multi-Query Rewriting for RAG**|Zhicong Li et.al.|[2411.13154](http://arxiv.org/abs/2411.13154)|null|
|**2024-11-20**|**Video-RAG: Visually-aligned Retrieval-Augmented Long Video Comprehension**|Yongdong Luo et.al.|[2411.13093](http://arxiv.org/abs/2411.13093)|**[link](https://github.com/leon1207/video-rag-master)**|
|**2024-11-19**|**CodeXEmbed: A Generalist Embedding Model Family for Multiligual and Multi-task Code Retrieval**|Ye Liu et.al.|[2411.12644](http://arxiv.org/abs/2411.12644)|null|
|**2024-11-20**|**Neon: News Entity-Interaction Extraction for Enhanced Question Answering**|Sneha Singhania et.al.|[2411.12449](http://arxiv.org/abs/2411.12449)|null|
|**2024-11-19**|**CUE-M: Contextual Understanding and Enhanced Search with Multimodal Large Language Model**|Dongyoung Go et.al.|[2411.12287](http://arxiv.org/abs/2411.12287)|null|
|**2024-11-19**|**Large Language Models for Material Property Predictions: elastic constant tensor prediction and materials design**|Siyu Liu et.al.|[2411.12280](http://arxiv.org/abs/2411.12280)|null|
|**2024-11-18**|**Molecule Generation with Fragment Retrieval Augmentation**|Seul Lee et.al.|[2411.12078](http://arxiv.org/abs/2411.12078)|null|
|**2024-11-17**|**On-Board Vision-Language Models for Personalized Autonomous Vehicle Motion Control: System Design and Real-World Validation**|Can Cui et.al.|[2411.11913](http://arxiv.org/abs/2411.11913)|null|
|**2024-11-18**|**SayComply: Grounding Field Robotic Tasks in Operational Compliance through Retrieval-Based Language Models**|Muhammad Fadhil Ginting et.al.|[2411.11323](http://arxiv.org/abs/2411.11323)|null|
|**2024-11-17**|**ForPKG-1.0: A Framework for Constructing Forestry Policy Knowledge Graph and Application Analysis**|Jingyun Sun et.al.|[2411.11090](http://arxiv.org/abs/2411.11090)|null|
|**2024-11-17**|**REACCEPT: Automated Co-evolution of Production and Test Code Based on Dynamic Validation and Large Language Models**|Jianlei Chi et.al.|[2411.11033](http://arxiv.org/abs/2411.11033)|null|
|**2024-11-17**|**LLM-assisted Physical Invariant Extraction for Cyber-Physical Systems Anomaly Detection**|Danial Abshari et.al.|[2411.10918](http://arxiv.org/abs/2411.10918)|null|
|**2024-11-16**|**Empowering Meta-Analysis: Leveraging Large Language Models for Scientific Synthesis**|Jawad Ibn Ahad et.al.|[2411.10878](http://arxiv.org/abs/2411.10878)|**[link](https://github.com/EncryptedBinary/Meta_analysis)**|
|**2024-11-14**|**Initial Nugget Evaluation Results for the TREC 2024 RAG Track with the AutoNuggetizer Framework**|Ronak Pradeep et.al.|[2411.09607](http://arxiv.org/abs/2411.09607)|null|
|**2024-11-14**|**Adopting RAG for LLM-Aided Future Vehicle Design**|Vahid Zolfaghari et.al.|[2411.09590](http://arxiv.org/abs/2411.09590)|null|
|**2024-11-14**|**Harnessing multiple LLMs for Information Retrieval: A case study on Deep Learning methodologies in Biodiversity publications**|Vamsi Krishna Kommineni et.al.|[2411.09269](http://arxiv.org/abs/2411.09269)|**[link](https://github.com/fusion-jena/information-retrieval-using-multiple-llm-and-rag)**|
|**2024-11-14**|**Comprehensive and Practical Evaluation of Retrieval-Augmented Generation Systems for Medical Question Answering**|Nghia Trung Ngo et.al.|[2411.09213](http://arxiv.org/abs/2411.09213)|null|
|**2024-11-13**|**Practitioners' Discussions on Building LLM-based Applications for Production**|Alina Mailach et.al.|[2411.08574](http://arxiv.org/abs/2411.08574)|null|
|**2024-11-13**|**Building Trustworthy AI: Transparent AI Systems via Large Language Models, Ontologies, and Logical Reasoning (TranspNet)**|Fadi Al Machot et.al.|[2411.08469](http://arxiv.org/abs/2411.08469)|null|
|**2024-11-13**|**Towards Evaluating Large Language Models for Graph Query Generation**|Siraj Munir et.al.|[2411.08449](http://arxiv.org/abs/2411.08449)|null|
|**2024-11-13**|**Towards Optimizing a Retrieval Augmented Generation using Large Language Model on Academic Data**|Anum Afzal et.al.|[2411.08438](http://arxiv.org/abs/2411.08438)|null|
|**2024-11-13**|**Refining Translations with LLMs: A Constraint-Aware Iterative Prompting Approach**|Shangfeng Chen et.al.|[2411.08348](http://arxiv.org/abs/2411.08348)|null|
|**2024-11-13**|**Are LLMs Prescient? A Continuous Evaluation using Daily News as the Oracle**|Hui Dai et.al.|[2411.08324](http://arxiv.org/abs/2411.08324)|null|
|**2024-11-13**|**A Large-Scale Study of Relevance Assessments with Large Language Models: An Initial Look**|Shivani Upadhyay et.al.|[2411.08275](http://arxiv.org/abs/2411.08275)|null|
|**2024-11-12**|**Retrieval Augmented Time Series Forecasting**|Kutay Tire et.al.|[2411.08249](http://arxiv.org/abs/2411.08249)|**[link](https://github.com/kutaytire/retrieval-augmented-time-series-forecasting)**|
|**2024-11-12**|**Adaptive Meta-Learning for Robust Deepfake Detection: A Multi-Agent Framework to Data Drift and Model Generalization**|Dinesh Srivasthav P et.al.|[2411.08148](http://arxiv.org/abs/2411.08148)|**[link](https://github.com/dineshsrivasthav/adaptive_meta_learning_with_multi_agent_framework)**|
|**2024-11-12**|**Trustful LLMs: Customizing and Grounding Text Generation with Knowledge Bases and Dual Decoders**|Xiaofeng Zhu et.al.|[2411.07870](http://arxiv.org/abs/2411.07870)|null|
|**2024-11-12**|**Query Optimization for Parametric Knowledge Refinement in Retrieval-Augmented Large Language Models**|Youan Cong et.al.|[2411.07820](http://arxiv.org/abs/2411.07820)|null|
|**2024-11-12**|**Likelihood as a Performance Gauge for Retrieval-Augmented Generation**|Tianyu Liu et.al.|[2411.07773](http://arxiv.org/abs/2411.07773)|**[link](https://github.com/lyutyuh/poptimizer)**|
|**2024-11-12**|**Unlocking Legal Knowledge with Multi-Layered Embedding-Based Retrieval**|João Alberto de Oliveira Lima et.al.|[2411.07739](http://arxiv.org/abs/2411.07739)|null|
|**2024-11-12**|**Enhancing Ultra High Resolution Remote Sensing Imagery Analysis with ImageRAG**|Zilun Zhang et.al.|[2411.07688](http://arxiv.org/abs/2411.07688)|null|
|**2024-11-11**|**Controllable Context Sensitivity and the Knob Behind It**|Julian Minder et.al.|[2411.07404](http://arxiv.org/abs/2411.07404)|**[link](https://github.com/kdu4108/context-vs-prior-finetuning)**|
|**2024-11-11**|**Toward Optimal Search and Retrieval for RAG**|Alexandria Leto et.al.|[2411.07396](http://arxiv.org/abs/2411.07396)|**[link](https://github.com/intellabs/rag-retrieval-study)**|
|**2024-11-11**|**ChatGPT Inaccuracy Mitigation during Technical Report Understanding: Are We There Yet?**|Salma Begum Tamanna et.al.|[2411.07360](http://arxiv.org/abs/2411.07360)|null|
|**2024-11-11**|**OpenThaiGPT 1.5: A Thai-Centric Open Source Large Language Model**|Sumeth Yuenyong et.al.|[2411.07238](http://arxiv.org/abs/2411.07238)|null|
|**2024-11-11**|**A Primer on Word Embeddings: AI Techniques for Text Analysis in Social Work**|Brian E. Perron et.al.|[2411.07156](http://arxiv.org/abs/2411.07156)|null|
|**2024-11-11**|**Impact of LLM-based Review Comment Generation in Practice: A Mixed Open-/Closed-source User Study**|Doriane Olewicki et.al.|[2411.07091](http://arxiv.org/abs/2411.07091)|null|
|**2024-11-11**|**Invar-RAG: Invariant LLM-aligned Retrieval for Better Generation**|Ziwei Liu et.al.|[2411.07021](http://arxiv.org/abs/2411.07021)|null|
|**2024-11-11**|**AssistRAG: Boosting the Potential of Large Language Models with an Intelligent Information Assistant**|Yujia Zhou et.al.|[2411.06805](http://arxiv.org/abs/2411.06805)|**[link](https://github.com/smallporridge/assistrag)**|
|**2024-11-10**|**Region-Aware Text-to-Image Generation via Hard Binding and Soft Refinement**|Zhennan Chen et.al.|[2411.06558](http://arxiv.org/abs/2411.06558)|**[link](https://github.com/nju-pcalab/rag-diffusion)**|
|**2024-11-10**|**LProtector: An LLM-driven Vulnerability Detection System**|Ze Sheng et.al.|[2411.06493](http://arxiv.org/abs/2411.06493)|null|
|**2024-11-09**|**Leveraging Retrieval-Augmented Generation for University Knowledge Retrieval**|Arshia Hemmat et.al.|[2411.06237](http://arxiv.org/abs/2411.06237)|null|
|**2024-11-09**|**Exploring Knowledge Boundaries in Large Language Models for Retrieval Judgment**|Zhen Zhang et.al.|[2411.06207](http://arxiv.org/abs/2411.06207)|null|
|**2024-11-09**|**Clustering Algorithms and RAG Enhancing Semi-Supervised Text Classification with Large LLMs**|Shan Zhong et.al.|[2411.06175](http://arxiv.org/abs/2411.06175)|null|
|**2024-11-08**|**FinDVer: Explainable Claim Verification over Long and Hybrid-Content Financial Documents**|Yilun Zhao et.al.|[2411.05764](http://arxiv.org/abs/2411.05764)|**[link](https://github.com/yilunzhao/FinDVer)**|
|**2024-11-08**|**IntellBot: Retrieval Augmented LLM Chatbot for Cyber Threat Knowledge Delivery**|Dincy R. Arikkat et.al.|[2411.05442](http://arxiv.org/abs/2411.05442)|null|
|**2024-11-08**|**Enhancing Cluster Resilience: LLM-agent Based Autonomous Intelligent Cluster Diagnosis System and Evaluation Framework**|Honghao Shi et.al.|[2411.05349](http://arxiv.org/abs/2411.05349)|null|
|**2024-11-08**|**A Taxonomy of AgentOps for Enabling Observability of Foundation Model based Agents**|Liming Dong et.al.|[2411.05285](http://arxiv.org/abs/2411.05285)|null|
|**2024-11-07**|**PentestAgent: Incorporating LLM Agents to Automated Penetration Testing**|Xiangmin Shen et.al.|[2411.05185](http://arxiv.org/abs/2411.05185)|null|
|**2024-11-07**|**Audiobox TTA-RAG: Improving Zero-Shot and Few-Shot Text-To-Audio with Retrieval-Augmented Generation**|Mu Yang et.al.|[2411.05141](http://arxiv.org/abs/2411.05141)|null|
|**2024-11-07**|**M3DocRAG: Multi-modal Retrieval is What You Need for Multi-page Multi-document Understanding**|Jaemin Cho et.al.|[2411.04952](http://arxiv.org/abs/2411.04952)|null|
|**2024-11-07**|**LLM-R: A Framework for Domain-Adaptive Maintenance Scheme Generation Combining Hierarchical Agents and RAG**|Laifa Tao et.al.|[2411.04476](http://arxiv.org/abs/2411.04476)|null|
|**2024-11-07**|**ML-Promise: A Multilingual Dataset for Corporate Promise Verification**|Yohei Seki et.al.|[2411.04473](http://arxiv.org/abs/2411.04473)|null|
|**2024-11-07**|**GPT-Guided Monte Carlo Tree Search for Symbolic Regression in Financial Fraud Detection**|Prashank Kadam et.al.|[2411.04459](http://arxiv.org/abs/2411.04459)|null|
|**2024-11-07**|**Enhancing classroom teaching with LLMs and RAG**|Elizabeth A Mullins et.al.|[2411.04341](http://arxiv.org/abs/2411.04341)|null|
|**2024-11-06**|**Enhancing Security Control Production With Generative AI**|Chen Ling et.al.|[2411.04284](http://arxiv.org/abs/2411.04284)|null|
|**2024-11-06**|**Fine-Grained Guidance for Retrievers: Leveraging LLMs' Feedback in Retrieval-Augmented Generation**|Yuhang Liu et.al.|[2411.03957](http://arxiv.org/abs/2411.03957)|null|
|**2024-11-06**|**RAGulator: Lightweight Out-of-Context Detectors for Grounded Text Generation**|Ian Poey et.al.|[2411.03920](http://arxiv.org/abs/2411.03920)|null|
|**2024-11-06**|**Advanced RAG Models with Graph Structures: Optimizing Complex Knowledge Reasoning and Text Generation**|Yuxin Dong et.al.|[2411.03572](http://arxiv.org/abs/2411.03572)|null|
|**2024-11-05**|**Long Context RAG Performance of Large Language Models**|Quinn Leng et.al.|[2411.03538](http://arxiv.org/abs/2411.03538)|null|
|**2024-11-05**|**HtmlRAG: HTML is Better Than Plain Text for Modeling Retrieved Knowledge in RAG Systems**|Jiejun Tan et.al.|[2411.02959](http://arxiv.org/abs/2411.02959)|**[link](https://github.com/plageon/HtmlRAG)**|
|**2024-11-06**|**Benchmarking Multimodal Retrieval Augmented Generation with Dynamic VQA Dataset and Self-adaptive Planning Agent**|Yangning Li et.al.|[2411.02937](http://arxiv.org/abs/2411.02937)|**[link](https://github.com/alibaba-nlp/omnisearch)**|
|**2024-11-05**|**WASHtsApp -- A RAG-powered WhatsApp Chatbot for supporting rural African clean water access, sanitation and hygiene**|Simon Kloker et.al.|[2411.02850](http://arxiv.org/abs/2411.02850)|null|
|**2024-11-06**|**PersianRAG: A Retrieval-Augmented Generation System for Persian Language**|Hossein Hosseini et.al.|[2411.02832](http://arxiv.org/abs/2411.02832)|null|
|**2024-11-04**|**Zebra-Llama: A Context-Aware Large Language Model for Democratizing Rare Disease Knowledge**|Karthik Soman et.al.|[2411.02657](http://arxiv.org/abs/2411.02657)|**[link](https://github.com/karthiksoman/zebra-Llama)**|
|**2024-11-04**|**TeleOracle: Fine-Tuned Retrieval-Augmented Generation with Long-Context Support for Network**|Nouf Alabbasi et.al.|[2411.02617](http://arxiv.org/abs/2411.02617)|**[link](https://github.com/Nouf-Alabbasi/oKUmura_AI_Telecom_challenge)**|

<p align=right>(<a href=#updated-on-20250131>back to top</a>)</p>

## text2sql

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-01-21**|**Is Long Context All You Need? Leveraging LLM's Extended Context for NL2SQL**|Yeounoh Chung et.al.|[2501.12372](http://arxiv.org/abs/2501.12372)|null|大型语言模型（LLMs）在一系列自然语言处理任务中展示了令人印象深刻的能力。特别是在推理能力和上下文窗口扩展方面的改进，为利用这些强大的模型开辟了新的途径。NL2SQL具有挑战性，因为自然语言问题本质上是模糊的，而生成SQL需要对复杂的数据模式和语义有精确的理解。解决这种语义模糊问题的一种方法是提供更多且充足的上下文信息。在这项工作中，我们探索了Google最先进的大型语言模型（\textit{gemini-1.5-pro}）提供的扩展上下文窗口（即长上下文）在性能和延迟之间的权衡。我们研究了各种上下文信息的影响，包括列示例值、问题与SQL查询对、用户提供的提示、SQL文档和模式。据我们所知，这是首次研究扩展上下文窗口和额外上下文信息如何在准确性和延迟成本方面帮助NL2SQL生成的工作。我们表明，长上下文LLM稳健，并不会迷失在扩展的上下文信息中。此外，基于Google的\textit{gemini-pro-1.5}的长上下文NL2SQL管道在没有微调和昂贵的一致性技术的情况下，在BIRD基准测试（开发集）上实现了67.41%的强劲表现。|
|**2025-01-06**|**Semantic Captioning: Benchmark Dataset and Graph-Aware Few-Shot In-Context Learning for SQL2Text**|Ali Al-Lawati et.al.|[2501.03166](http://arxiv.org/abs/2501.03166)|**[link](https://github.com/aliwister/ast-icl)**|**大型语言模型（LLMs）在各种自然语言处理任务中表现出色，包括将自然语言转换为形式化的代码表示，即语义解析。然而，将代码转换为自然语言的过程，称为语义标注，却较少受到关注。随着LLMs被集成到代码生成、安全分析和教育平台中，这一任务变得越来越重要。本文聚焦于SQL查询的标注（SQL2Text），以应对理解与解释SQL查询的需求，尤其是在LLM生成的代码可能带来潜在安全风险的时代。我们通过引入基于GPT-4o的迭代ICL提示来重新利用Text2SQL数据集，生成多个额外的表述，从而增强了这些数据集在反向任务中的鲁棒性。我们使用基于不同样本选择方法的情境学习（ICL）进行实验，特别强调了较小且计算效率更高的LLMs。我们的研究发现，利用SQL固有的图属性进行ICL样本选择，在BLEU评分上比随机选择最多高出39%，并且比其他方法提供了更好的结果。数据集和代码已发布：https://github.com/aliwister/ast-icl。**|
|**2025-01-03**|**CarbonChat: Large Language Model-Based Corporate Carbon Emission Analysis and Climate Knowledge Q&A System**|Zhixuan Cao et.al.|[2501.02031](http://arxiv.org/abs/2501.02031)|null|随着全球气候变化影响的加剧，企业碳排放已成为全球关注的焦点。为应对大型语言模型中气候变化知识更新滞后、传统增强生成架构在处理复杂问题时缺乏专业性和准确性以及可持续性报告分析成本高且耗时等问题，本文提出了CarbonChat：基于大型语言模型的企业碳排放分析和气候知识问答系统，旨在实现精准的碳排放分析和政策理解。首先，提出了一种多样化的指数模块构建方法，用于处理基于规则和长文本文档的分割及结构化数据提取，从而优化关键信息解析。其次，设计了一种增强的自提示检索-增强生成架构，集成了意图识别、结构化推理链、混合检索和Text2SQL，提高了语义理解和查询转换的效率。接下来，基于温室气体核算框架，建立了14个维度进行碳排放分析，实现了报告总结、相关性评估和定制化响应。最后，通过多层次分块机制、时间戳和幻觉检测功能，确保了分析结果的准确性和可验证性，降低了幻觉率并提高了响应的精确度。|
|**2024-12-22**|**A Plug-and-Play Natural Language Rewriter for Natural Language to SQL**|Peixian Ma et.al.|[2412.17068](http://arxiv.org/abs/2412.17068)|null|现有的自然语言到SQL（NL2SQL）解决方案已经取得了显著进展，但在解释和翻译自然语言查询方面仍然存在挑战，主要原因是用户对数据库模式理解有限或对特定表或列值存在记忆偏差。这些挑战常常导致错误的NL2SQL翻译。为了解决这些问题，我们提出了REWRITER，这是一个即插即用模块，旨在通过自动重写模糊或有缺陷的自然语言查询来增强NL2SQL系统。通过结合数据库知识和内容（例如列值和外键），REWRITER减少了由于有缺陷的自然语言输入引起的错误，并提高了SQL生成的准确性。我们的REWRITER将NL2SQL模型视为黑盒，确保与各种NL2SQL方法兼容，包括基于代理和基于规则的NL2SQL解决方案。REWRITER包含三个关键组件：Checker、Reflector和Rewriter。Checker通过评估生成的SQL的正确性来识别有缺陷的自然语言查询，从而减少不必要的重写和潜在的幻觉。Reflector分析并积累经验以识别自然语言查询中的问题，而Rewriter则根据Reflector的反馈修改查询。在Spider和BIRD基准测试上的广泛实验表明，REWRITER始终能够增强下游模型，在执行准确性上分别平均提高了1.6%和2.0%。|
|**2024-12-17**|**SynthCypher: A Fully Synthetic Data Generation Framework for Text-to-Cypher Querying in Knowledge Graphs**|Aman Tiwari et.al.|[2412.12612](http://arxiv.org/abs/2412.12612)|null|
|**2024-12-13**|**ROUTE: Robust Multitask Tuning and Collaboration for Text-to-SQL**|Yang Qin et.al.|[2412.10138](http://arxiv.org/abs/2412.10138)|**[link](https://github.com/alibaba/route)**|**尽管大型语言模型（LLMs）在文本到SQL（Text2SQL）方面取得了显著进展，但最新的技术仍然局限于闭源LLM（例如GPT-4）的上下文学习中，这限制了它们在开放场景中的应用。为了解决这一挑战，我们提出了一种新颖的鲁棒多任务调优与协作方法（ROUTE），以提高开源LLM在Text2SQL方面的综合能力，从而提供一个更实用的解决方案。我们的方法首先使用多种与SQL生成相关的合成训练数据进行多任务监督微调（SFT）。与现有的基于SFT的Text2SQL方法不同，我们引入了几个额外的SFT任务，包括模式链接、噪声校正和延续写作。参与各种SQL生成任务增强了模型对SQL语法的理解，并提高了其生成高质量SQL查询的能力。此外，受LLM代理的协作模式启发，我们引入了一种多任务协作提示策略（MCP）。该策略利用多个SQL相关任务之间的协作来减少SQL生成过程中的幻觉，从而通过显式的多任务能力最大化提升Text2SQL性能。我们在八个开源LLM和五个广泛使用的基准上进行了广泛的实验和深入分析。结果表明，我们的方法优于最新的Text2SQL方法，并取得了领先的性能。**|
|**2024-12-04**|**DataLab: A Unified Platform for LLM-Powered Business Intelligence**|Luoxuan Weng et.al.|[2412.02205](http://arxiv.org/abs/2412.02205)|null|商业智能（BI）将现代组织中的大量数据转化为可操作的洞察，以支持明智的决策。最近，基于大型语言模型（LLM）的代理通过根据自然语言（NL）查询自动执行任务规划、推理和操作，在可执行环境中简化了BI工作流程。然而，现有的方法主要集中在单个BI任务上，如NL2SQL和NL2VIS。由于BI工作的迭代性和协作性，任务在不同数据角色和工具之间的分散导致了效率低下和潜在错误。在本文中，我们介绍了DataLab，这是一个统一的BI平台，它在一个一站式的基于LLM的代理框架与增强的计算笔记本界面之间实现了无缝集成。DataLab通过在一个单一环境中结合LLM辅助与用户自定义，支持各种数据角色下的广泛BI任务。为了实现这一整合，我们设计了一个针对企业特定BI任务定制的知识域融入模块、一个跨BI工作流促进信息共享的代理间通信机制以及一种单元格上下文管理策略，以提高BI笔记本中上下文利用效率。广泛的实验表明，DataLab在各种流行的研究基准上实现了多种BI任务的最先进性能。此外，在腾讯的真实世界数据集上，DataLab在企业特定BI任务上实现了高达58.58%的准确性提升和61.65%的令牌成本降低。|
|**2024-11-05**|**Grounding Natural Language to SQL Translation with Data-Based Self-Explanations**|Yuankai Fan et.al.|[2411.02948](http://arxiv.org/abs/2411.02948)|**[link](https://github.com/Kaimary/CycleSQL)**|**自然语言接口使非技术用户能够使用自然语言（NL）与数据进行交互。先进的方法通常利用神经序列到序列模型或更近期的复杂大规模语言模型，以端到端的方式实现从自然语言到SQL（NL2SQL）的转换。然而，就像人类一样，这些端到端的翻译模型可能并不总是在第一次尝试时就生成最佳的SQL输出。在本文中，我们提出了CycleSQL，这是一种迭代框架，旨在让端到端翻译模型通过自我评估自主生成最佳输出。CycleSQL的主要思想是引入基于数据的查询结果自然语言解释作为自我提供的反馈，并利用该反馈来迭代验证翻译的正确性，从而提高整体翻译准确性。为了研究CycleSQL，我们在五个广泛使用的基准上对七个现有的翻译模型进行了包括定量和定性评估在内的大量实验。结果显示：1）CycleSQL中引入的反馈循环可以持续改进现有模型的性能，特别是将CycleSQL应用于REDSQL后，在Spider基准的验证集上获得了82.0%（+2.6%）的翻译准确率，在测试集上获得了81.6%（+3.2%）的翻译准确率；2）生成的自然语言解释也可以为用户提供有洞察力的信息，帮助理解翻译结果，从而增强NL2SQL翻译的可解释性。**|
|**2024-10-30**|**BIS: NL2SQL Service Evaluation Benchmark for Business Intelligence Scenarios**|Bora Caglayan et.al.|[2410.22925](http://arxiv.org/abs/2410.22925)|**[link](https://github.com/boracaglayan/bis-nl2sql)**|**近年来，自然语言到结构化查询语言（NL2SQL）的转换在商业智能（BI）应用中得到了广泛的应用。然而，现有的NL2SQL基准并不适合生产环境中的BI场景，因为它们并不是为常见的商业智能问题设计的。为了解决这一问题，我们开发了一个专注于工业BI场景中典型自然语言问题的新基准。我们讨论了构建BI导向基准的挑战以及现有基准的不足之处。此外，我们在基准中引入了反映常见BI询问的问题类别。最后，我们提出了两种新的语义相似性评估指标，用于评估BI应用程序和服务中的NL2SQL能力。**|
|**2024-10-15**|**LR-SQL: A Supervised Fine-Tuning Method for Text2SQL Tasks under Low-Resource Scenarios**|Wen Wuzhenghong et.al.|[2410.11457](http://arxiv.org/abs/2410.11457)|**[link](https://github.com/hongwin/lr-sql)**|**大型语言模型通过监督微调在Text2SQL领域带来了革命性的变化，但一个关键的限制被忽视了：数据库的复杂性导致上下文长度增加，从而增加了模型微调时对GPU内存的需求。为了解决这个问题，我们提出了LR-SQL。LR-SQL包含两个监督微调模型：schema_link模型和SQL_generation模型，其中schema_link模型是整个过程中的重点。在schema_link模型的微调过程中，LR-SQL将完整的数据库分解成具有可调节数量的表的灵活组合，使模型能够从这些分散的片段中学习整个数据库内的关系。此外，为了增强模型在推理过程中感知各种离散片段之间关系的能力，LR-SQL训练模型的思维链能力来完成这一任务。实验结果表明，与现有的微调方法相比，LR-SQL可以减少40%的总GPU内存使用量，而仅在schema_link任务中损失2%的表预测准确性。对于整体的Text2SQL任务，执行准确率下降了0.6%。我们的项目现已在https://github.com/hongWin/LR-SQL上公开。**|
|**2024-08-27**|**Text2SQL is Not Enough: Unifying AI and Databases with TAG**|Asim Biswal et.al.|[2408.14717](http://arxiv.org/abs/2408.14717)|**[link](https://github.com/tag-research/tag-bench)**|**能够通过自然语言问题查询数据库的人工智能系统有望解锁巨大的价值。这样的系统将允许用户利用语言模型的强大推理和知识能力，以及数据管理系统可扩展的计算能力。这些结合的能力将使用户能够对自定义数据源提出任意的自然语言问题。然而，现有的方法和基准测试未能充分探索这一场景。Text2SQL方法仅关注可以通过关系代数表达的自然语言问题，这仅代表了真实用户希望提出的问题的一小部分。同样，检索增强生成（RAG）考虑的是可以通过对数据库中一个或少数几个数据记录进行点查找来回答的有限子集查询。我们提出了表格增强生成（TAG），这是一种统一且通用的方法，用于回答数据库上的自然语言问题。TAG模型代表了语言模型与数据库之间先前未被探索过的广泛互动，并为利用语言模型在数据上的世界知识和推理能力创造了令人兴奋的研究机会。我们系统地开发了研究TAG问题的基准测试，发现标准方法正确回答的问题不超过20%，证实了该领域需要进一步研究的需求。我们在https://github.com/TAG-Research/TAG-Bench上发布了基准测试代码。**|
|**2024-12-04**|**A Survey of NL2SQL with Large Language Models: Where are we, and where are we going?**|Xinyu Liu et.al.|[2408.05109](http://arxiv.org/abs/2408.05109)|**[link](https://github.com/hkustdial/nl2sql_handbook)**|
|**2024-07-21**|**Towards Automated Data Sciences with Natural Language and SageCopilot: Practices and Lessons Learned**|Yuan Liao et.al.|[2407.21040](http://arxiv.org/abs/2407.21040)|null|
|**2024-11-07**|**A Survey on Employing Large Language Models for Text-to-SQL Tasks**|Liang Shi et.al.|[2407.15186](http://arxiv.org/abs/2407.15186)|null|
|**2024-06-12**|**DeTriever: Decoder-representation-based Retriever for Improving NL2SQL In-Context Learning**|Yuxi Feng et.al.|[2406.07913](http://arxiv.org/abs/2406.07913)|null|
|**2024-07-27**|**The Dawn of Natural Language to SQL: Are We Fully Ready?**|Boyan Li et.al.|[2406.01265](http://arxiv.org/abs/2406.01265)|**[link](https://github.com/hkustdial/nl2sql360)**|
|**2024-05-01**|**ChatBI: Towards Natural Language to Complex Business Intelligence SQL**|Jinqing Lian et.al.|[2405.00527](http://arxiv.org/abs/2405.00527)|null|
|**2024-03-29**|**PURPLE: Making a Large Language Model a Better SQL Writer**|Tonghui Ren et.al.|[2403.20014](http://arxiv.org/abs/2403.20014)|null|

<p align=right>(<a href=#updated-on-20250131>back to top</a>)</p>

## PPC

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-01-29**|**Federated Learning With Individualized Privacy Through Client Sampling**|Lucas Lange et.al.|[2501.17634](http://arxiv.org/abs/2501.17634)|**[link](https://github.com/luckyos-code/flidp)**|**随着对用户数据收集的担忧日益增加，个性化隐私作为一种平衡保护和实用性的解决方案逐渐受到关注，它通过考虑不同的用户隐私偏好来实现。与对所有用户实施统一的匿名化程度不同，这种方法允许个人根据自己的舒适度选择隐私设置。基于这一理念，我们提出了一种改进的方法，以在联邦学习（FL）中实现个性化差分隐私（IDP），按照用户的个人隐私偏好处理客户端。我们将集中式环境下的SAMPLE算法扩展到FL中，根据异构隐私预算计算特定于客户端的采样率，并将其整合到改进的IDP-FedAvg算法中。我们在实际的隐私分布和多个数据集下测试了该方法。实验结果表明，我们的方法明显优于统一DP基线，减少了隐私与实用性之间的权衡。与相关工作中分配不同噪声尺度给客户端的SCALE方法相比，我们的方法表现显著更优。然而，在非独立同分布数据的复杂任务中，由于去中心化环境的限制，仍存在挑战。**|
|**2025-01-29**|**A Survey on Cluster-based Federated Learning**|Omar El-Rifai et.al.|[2501.17512](http://arxiv.org/abs/2501.17512)|null|随着联邦学习（FL）在工业和商业中的应用不断扩大，对优化算法的需求也在增加。在FL客户端数据非独立同分布（非IID）且具有高度异构分布的情况下，基本的FL方法似乎表现不佳。为了解决这个问题，最近的研究开始关注个性化联邦学习（PFL），它放宽了单一模型约束，允许从数据或本地模型中学习多个假设。在个性化联邦学习方法中，基于聚类的解决方案（CFL）尤其有趣，尤其是在通过领域知识可以明确将客户端分组的情况下。在本文中，我们研究了CFL的最新工作，提出了：i) CFL个性化解决方案的分类；ii) 文献的结构化综述；iii) CFL的替代用例综述。CCS概念： $\bullet$ 通用和参考 $\rightarrow$ 综述和概述；$\bullet$ 计算方法 $\rightarrow$ 机器学习；$\bullet$ 信息系统 $\rightarrow$ 聚类；$\bullet$ 安全与隐私 $\rightarrow$ 隐私保护协议。|
|**2025-01-29**|**Poisoning Attacks and Defenses to Federated Unlearning**|Wenbin Wang et.al.|[2501.17396](http://arxiv.org/abs/2501.17396)|null|联邦学习允许多个客户端在服务器的协助下协作训练一个全局模型。然而，其分布式特性使其容易受到中毒攻击的影响，恶意客户端可以通过向服务器发送有害的本地模型更新来破坏全局模型。为了解决识别出恶意客户端后从被污染的模型中恢复准确的全局模型的问题，联邦卸载（federated unlearning）应运而生。不过，目前关于联邦卸载的研究主要集中在效率和有效性上，忽视了它所带来的安全挑战。在这项工作中，我们通过提出BadUnlearn——首个针对联邦卸载的中毒攻击——填补了这一空白。在BadUnlearn中，恶意客户端在卸载过程中向服务器发送特别设计的本地模型更新，目的是确保卸载后的模型仍然被污染。为了缓解这些威胁，我们提出了UnlearnGuard，这是一种健壮的联邦卸载框架，可以有效抵御现有的中毒攻击以及我们的BadUnlearn。UnlearnGuard的核心思想是服务器在卸载过程中估计客户端的本地模型更新，并采用过滤策略来验证这些估计的准确性。理论上，我们证明通过UnlearnGuard卸载得到的模型与从头开始训练得到的模型非常接近。实验结果表明，BadUnlearn能够有效地破坏现有的联邦卸载方法，而UnlearnGuard则能够抵御中毒攻击。|
|**2025-01-29**|**Byzantine-Robust Federated Learning over Ring-All-Reduce Distributed Computing**|Minghong Fang et.al.|[2501.17392](http://arxiv.org/abs/2501.17392)|null|联邦学习（FL）作为一种分布式学习范式，因其数据隐私优势和通过并行计算加速收敛而受到关注。传统的联邦学习依赖于服务器-客户端（SC）架构，其中中央服务器协调多个客户端来训练全局模型，但这种方法由于服务器通信瓶颈面临可扩展性挑战。为了解决这个问题，引入了环形全归约（RAR）架构，消除了中央服务器，并实现了带宽最优。然而，RAR的紧密耦合环形拓扑使其面临在基于SC的联邦学习中不存在的独特拜占庭攻击风险。尽管潜力巨大，设计拜占庭鲁棒的RAR联邦学习算法仍然是一个未解决的问题。为填补这一空白，我们提出了BRACE（拜占庭鲁棒环形全归约），这是首个实现拜占庭鲁棒性和通信效率的RAR联邦学习算法。我们提供了BRACE在拜占庭攻击下的收敛性理论保证，展示了其带宽效率，并通过实验验证了其实用有效性。我们的工作为拜占庭鲁棒RAR联邦学习的设计提供了基础理解。|
|**2025-01-29**|**Do We Really Need to Design New Byzantine-robust Aggregation Rules?**|Minghong Fang et.al.|[2501.17381](http://arxiv.org/abs/2501.17381)|null|联邦学习（FL）允许多个客户端通过服务器协作训练一个全局机器学习模型，而无需交换他们的私有训练数据。然而，FL的去中心化特性使其容易受到中毒攻击，恶意客户端可以通过发送被篡改的本地模型更新来操纵全局模型。为应对这些攻击，已经引入了多种旨在抵御拜占庭故障的聚合规则。然而，这些方法仍然可能对复杂的攻击脆弱，或者依赖于对服务器不切实际的假设。在本文中，我们证明了没有必要设计新的拜占庭鲁棒聚合规则；相反，可以通过增强已有聚合规则的鲁棒性来保护FL。为此，我们提出了一种名为FoundationFL的新防御机制，用于对抗中毒攻击。FoundationFL涉及服务器在接受来自客户端的本地模型更新后生成合成更新。然后它应用现有的拜占庭鲁棒基础聚合规则（如Trimmed-mean或Median）将客户端的模型更新与合成更新结合。我们在理论上建立了FoundationFL在拜占庭设置下的收敛性能。在多个真实世界数据集上的综合实验验证了我们的FoundationFL方法的有效性。|
|**2025-01-28**|**Connecting Federated ADMM to Bayes**|Siddharth Swaroop et.al.|[2501.17325](http://arxiv.org/abs/2501.17325)|null|我们建立了两种不同的联邦学习方法之间的新联系，一种基于ADMM，另一种基于变分贝叶斯（VB），并通过结合它们互补的优势提出了新的变体。具体来说，我们展示了在具有各向同性高斯协方差的VB中使用的“站点”参数自然地产生了ADMM中的对偶变量。利用这一点，我们从VB中推导出两个版本的ADMM，分别使用灵活的协方差和函数正则化。通过数值实验，我们验证了性能上的改进。这项工作揭示了两个被认为本质上不同的领域之间的联系，并将它们结合起来以改进联邦学习。|
|**2025-01-28**|**FedEFM: Federated Endovascular Foundation Model with Unseen Data**|Tuong Do et.al.|[2501.16992](http://arxiv.org/abs/2501.16992)|null|在血管内手术中，X射线图像中导管和导丝的精确识别对于降低干预风险至关重要。然而，由于标注数据有限，准确分割导管和导丝结构具有挑战性。基础模型通过收集相似领域的数据来训练模型，并对权重进行微调以适应下游任务，为这一问题提供了一个有前景的解决方案。然而，大规模数据收集受到保护患者隐私需求的限制。本文提出了一种在去中心化联邦学习环境中训练用于血管内介入的基础模型的新方法。为了确保训练的可行性，我们使用可微分的地球移动距离在知识蒸馏框架中解决未见数据的问题。一旦训练完成，我们的基础模型的权重可以为下游任务提供有价值的初始化，从而提高特定任务的性能。大量实验表明，我们的方法达到了新的最先进水平，推动了血管内介入和机器人辅助血管内手术的进步，同时解决了医学领域中的关键数据共享问题。|
|**2025-01-28**|**Heterogeneity-aware Personalized Federated Learning via Adaptive Dual-Agent Reinforcement Learning**|Xi Chen et.al.|[2501.16966](http://arxiv.org/abs/2501.16966)|null|联邦学习（FL）使多个客户端能够在不共享本地数据的情况下协作训练机器学习模型，使其在异构物联网（IoT）环境中具有高度适用性。然而，客户端模型架构和计算能力的内在异质性通常会导致模型精度下降和棘手的掉队问题，这显著影响了训练效果。为了解决这些挑战，本文提出了一种名为HAPFL的新颖异质感知个性化联邦学习方法，该方法通过多层次强化学习（RL）机制优化训练过程。HAPFL结合了三个策略组件：1）基于RL的异质模型分配机制。参数服务器采用基于近端策略优化（PPO）的RL代理，根据客户端性能自适应地分配适当大小的不同模型，有效缓解性能差异。2）基于RL的训练强度调整方案。参数服务器利用另一个基于PPO的RL代理动态微调每个客户端的训练强度，以进一步提高训练效率并减少掉队延迟。3）基于知识蒸馏的相互学习机制。每个客户端部署一个异质本地模型和一个同质轻量级模型LiteModel，这两个模型通过知识蒸馏进行相互学习。这个统一的LiteModel在全球知识聚合和共享中发挥关键作用，显著增强了个性化本地训练的效果。在多个基准数据集上的实验结果表明，HAPFL不仅实现了高精度，还比现有解决方案整体减少了20.9%-40.4%的训练时间，并降低了19.0%-48.0%的掉队延迟。|
|**2025-01-28**|**Federated Learning Strategies for Coordinated Beamforming in Multicell ISAC**|Lai Jiang et.al.|[2501.16951](http://arxiv.org/abs/2501.16951)|null|我们提出了两种基于联邦学习（FL）的多小区综合感知与通信（ISAC）系统的协作波束赋形框架。我们的目标是解决多小区ISAC中的以下困境：1）仅依赖本地信道信息的波束赋形策略可能会产生显著的小区间干扰（ICI），从而降低邻近小区中通信用户和感知接收机的网络性能；2）相反，集中式波束赋形策略可以通过利用全局信道信息来缓解ICI，但它们带来了大量的传输开销和延迟，这对于延迟敏感和资源受限的应用来说可能是不可接受的。为了解决这些挑战，我们首先提出了一种受垂直联邦学习（VFL）范式启发的部分去中心化训练框架。在这个框架中，参与的基站（BSs）在中央服务器的指导下协作设计波束赋形矩阵。中央服务器从基站收集本地信息并提供反馈，使基站能够在不访问全局信道信息的情况下隐式管理ICI。为了使解决方案适用于密集部署的无线网络，我们进一步采取措施减少通信开销，提出了一个基于水平联邦学习（HFL）的完全去中心化设计。具体来说，我们开发了一种新的损失函数来控制干扰泄漏功率，通过完全消除本地信道信息交换，实现更高效的训练过程。数值结果表明，所提出的解决方案在通信和雷达信息速率方面都能达到与基准相当的显著性能改进。|
|**2025-01-28**|**Meta-Federated Learning: A Novel Approach for Real-Time Traffic Flow Management**|Bob Johnson et.al.|[2501.16758](http://arxiv.org/abs/2501.16758)|null|在城市环境中高效管理交通流是一个重大挑战，尤其受到动态变化和现代交通网络产生的大量数据的影响。传统的集中式交通管理系统通常难以应对可扩展性和隐私问题，这限制了它们的有效性。本文介绍了一种结合联邦学习（FL）和元学习（ML）的新方法，以创建一个去中心化、可扩展且自适应的交通管理系统。我们的方法称为元联邦学习，利用FL的分布式特性在边缘设备本地处理数据，从而增强隐私并减少延迟。同时，ML使系统能够快速适应新的交通状况，而无需进行大量的重新训练。我们在模拟的智能交通设备网络中实施了我们的模型，结果表明，与传统模型相比，元联邦学习在预测准确性和响应时间方面显著优于传统模型。此外，我们的方法在应对突发交通模式变化时表现出色，为智慧城市中的实时交通管理提供了一个可扩展的解决方案。本研究不仅为更强大的城市交通系统铺平了道路，还展示了集成FL和ML在其他实际应用中的潜力。|
|**2025-01-28**|**Federated Learning for Efficient Condition Monitoring and Anomaly Detection in Industrial Cyber-Physical Systems**|William Marfo et.al.|[2501.16666](http://arxiv.org/abs/2501.16666)|null|
|**2025-01-27**|**Measuring Heterogeneity in Machine Learning with Distributed Energy Distance**|Mengchen Fan et.al.|[2501.16174](http://arxiv.org/abs/2501.16174)|null|
|**2025-01-27**|**A Unified Analysis of Stochastic Gradient Descent with Arbitrary Data Permutations and Beyond**|Yipeng Li et.al.|[2501.16117](http://arxiv.org/abs/2501.16117)|null|
|**2025-01-27**|**Combating Interference for Over-the-Air Federated Learning: A Statistical Approach via RIS**|Wei Shi et.al.|[2501.16081](http://arxiv.org/abs/2501.16081)|null|
|**2025-01-27**|**Enhancing the Convergence of Federated Learning Aggregation Strategies with Limited Data**|Judith Sáinz-Pardo Díaz et.al.|[2501.15949](http://arxiv.org/abs/2501.15949)|null|
|**2025-01-27**|**Integrating Personalized Federated Learning with Control Systems for Enhanced Performance**|Alice Smith et.al.|[2501.15728](http://arxiv.org/abs/2501.15728)|null|
|**2025-01-27**|**CENSOR: Defense Against Gradient Inversion via Orthogonal Subspace Bayesian Sampling**|Kaiyuan Zhang et.al.|[2501.15718](http://arxiv.org/abs/2501.15718)|**[link](https://github.com/KaiyuanZh/censor)**|
|**2025-01-26**|**FedAlign: Federated Domain Generalization with Cross-Client Feature Alignment**|Sunny Gupta et.al.|[2501.15486](http://arxiv.org/abs/2501.15486)|null|
|**2025-01-26**|**Decentralized Low-Rank Fine-Tuning of Large Language Models**|Sajjad Ghiasvand et.al.|[2501.15361](http://arxiv.org/abs/2501.15361)|null|
|**2025-01-25**|**A Post-Processing-Based Fair Federated Learning Framework**|Yi Zhou et.al.|[2501.15318](http://arxiv.org/abs/2501.15318)|null|
|**2025-01-25**|**A Two-Stage CAE-Based Federated Learning Framework for Efficient Jamming Detection in 5G Networks**|Samhita Kuili et.al.|[2501.15288](http://arxiv.org/abs/2501.15288)|null|
|**2025-01-24**|**Federated Domain Generalization with Data-free On-server Gradient Matching**|Trong-Binh Nguyen et.al.|[2501.14653](http://arxiv.org/abs/2501.14653)|null|
|**2025-01-24**|**Data Assetization via Resources-decoupled Federated Learning**|Jianzhe Zhao et.al.|[2501.14588](http://arxiv.org/abs/2501.14588)|null|
|**2025-01-24**|**Real-world Edge Neural Network Implementations Leak Private Interactions Through Physical Side Channel**|Zhuoran Liu et.al.|[2501.14512](http://arxiv.org/abs/2501.14512)|null|
|**2025-01-24**|**Optimal Strategies for Federated Learning Maintaining Client Privacy**|Uday Bhaskar et.al.|[2501.14453](http://arxiv.org/abs/2501.14453)|null|
|**2025-01-24**|**Advancing MRI Reconstruction: A Systematic Review of Deep Learning and Compressed Sensing Integration**|Mojtaba Safari et.al.|[2501.14158](http://arxiv.org/abs/2501.14158)|**[link](https://github.com/mosaf/awesome-dl-based-cs-mri)**|
|**2025-01-23**|**PBM-VFL: Vertical Federated Learning with Feature and Sample Privacy**|Linh Tran et.al.|[2501.13916](http://arxiv.org/abs/2501.13916)|null|
|**2025-01-23**|**Privacy-Preserving Personalized Federated Prompt Learning for Multimodal Large Language Models**|Linh Tran et.al.|[2501.13904](http://arxiv.org/abs/2501.13904)|null|
|**2025-01-23**|**Unlearning Clients, Features and Samples in Vertical Federated Learning**|Ayush K. Varshney et.al.|[2501.13683](http://arxiv.org/abs/2501.13683)|null|
|**2025-01-23**|**AirTOWN: A Privacy-Preserving Mobile App for Real-time Pollution-Aware POI Suggestion**|Giuseppe Fasano et.al.|[2501.13608](http://arxiv.org/abs/2501.13608)|null|
|**2025-01-23**|**FedPref: Federated Learning Across Heterogeneous Multi-objective Preferences**|Maria Hartmann et.al.|[2501.13604](http://arxiv.org/abs/2501.13604)|**[link](https://gitlab.com/maria.hartmann/FedPref)**|
|**2025-01-22**|**Distributed Intrusion Detection in Dynamic Networks of UAVs using Few-Shot Federated Learning**|Ozlem Ceviz et.al.|[2501.13213](http://arxiv.org/abs/2501.13213)|null|
|**2025-01-22**|**A Selective Homomorphic Encryption Approach for Faster Privacy-Preserving Federated Learning**|Abdulkadir Korkmaz et.al.|[2501.12911](http://arxiv.org/abs/2501.12911)|null|
|**2025-01-22**|**Bad-PFL: Exploring Backdoor Attacks against Personalized Federated Learning**|Mingyuan Fan et.al.|[2501.12736](http://arxiv.org/abs/2501.12736)|null|
|**2025-01-22**|**Anomaly Detection in Double-entry Bookkeeping Data by Federated Learning System with Non-model Sharing Approach**|Sota Mashiko et.al.|[2501.12723](http://arxiv.org/abs/2501.12723)|null|
|**2025-01-22**|**Practical quantum federated learning and its experimental demonstration**|Zhi-Ping Liu et.al.|[2501.12709](http://arxiv.org/abs/2501.12709)|null|
|**2025-01-22**|**FedGrAINS: Personalized SubGraph Federated Learning with Adaptive Neighbor Sampling**|Emir Ceyani et.al.|[2501.12592](http://arxiv.org/abs/2501.12592)|null|
|**2025-01-21**|**Enhancing Privacy in the Early Detection of Sexual Predators Through Federated Learning and Differential Privacy**|Khaoula Chehbouni et.al.|[2501.12537](http://arxiv.org/abs/2501.12537)|null|
|**2025-01-21**|**Federated Discrete Denoising Diffusion Model for Molecular Generation with OpenFL**|Kevin Ta et.al.|[2501.12523](http://arxiv.org/abs/2501.12523)|**[link](https://github.com/securefederatedai/openfl)**|
|**2025-01-21**|**MyDigiTwin: A Privacy-Preserving Framework for Personalized Cardiovascular Risk Prediction and Scenario Exploration**|Héctor Cadavid et.al.|[2501.12193](http://arxiv.org/abs/2501.12193)|**[link](https://github.com/mydigitwinnl/fedavg_vantage6)**|
|**2025-01-21**|**Heterogeneous Federated Learning Systems for Time-Series Power Consumption Prediction with Multi-Head Embedding Mechanism**|Jia-Hao Syu et.al.|[2501.12136](http://arxiv.org/abs/2501.12136)|null|
|**2025-01-21**|**Heterogeneous Federated Learning System for Sparse Healthcare Time-Series Prediction**|Jia-Hao Syu et.al.|[2501.12125](http://arxiv.org/abs/2501.12125)|null|
|**2025-01-21**|**FedCLEAN: byzantine defense by CLustering Errors of Activation maps in Non-IID federated learning environments**|Mehdi Ben Ghali et.al.|[2501.12123](http://arxiv.org/abs/2501.12123)|null|
|**2025-01-21**|**BotDetect: A Decentralized Federated Learning Framework for Detecting Financial Bots on the EVM Blockchains**|Ahmed Mounsf Rafik Bendada et.al.|[2501.12112](http://arxiv.org/abs/2501.12112)|null|
|**2025-01-21**|**Communication-Efficient and Privacy-Adaptable Mechanism for Federated Learning**|Chih Wei Ling et.al.|[2501.12046](http://arxiv.org/abs/2501.12046)|**[link](https://github.com/yokiwuuu/cepam)**|
|**2025-01-21**|**FedMUA: Exploring the Vulnerabilities of Federated Learning to Malicious Unlearning Attacks**|Jian Chen et.al.|[2501.11848](http://arxiv.org/abs/2501.11848)|**[link](https://github.com/ity207/FedMUA)**|
|**2025-01-20**|**Personalized Federated Learning for Cellular VR: Online Learning and Dynamic Caching**|Krishnendu S. Tharakan et.al.|[2501.11745](http://arxiv.org/abs/2501.11745)|null|
|**2025-01-20**|**The Transition from Centralized Machine Learning to Federated Learning for Mental Health in Education: A Survey of Current Methods and Future Directions**|Maryam Ebrahimi et.al.|[2501.11714](http://arxiv.org/abs/2501.11714)|null|
|**2025-01-20**|**Trustformer: A Trusted Federated Transformer**|Ali Abbasi Tadi et.al.|[2501.11706](http://arxiv.org/abs/2501.11706)|null|
|**2025-01-17**|**ColNet: Collaborative Optimization in Decentralized Federated Multi-task Learning Systems**|Chao Feng et.al.|[2501.10347](http://arxiv.org/abs/2501.10347)|null|
|**2025-01-17**|**Client-Centric Federated Adaptive Optimization**|Jianhui Sun et.al.|[2501.09946](http://arxiv.org/abs/2501.09946)|null|
|**2025-01-17**|**HEART: Achieving Timely Multi-Model Training for Vehicle-Edge-Cloud-Integrated Hierarchical Federated Learning**|Xiaohong Yang et.al.|[2501.09934](http://arxiv.org/abs/2501.09934)|null|
|**2025-01-16**|**pFedWN: A Personalized Federated Learning Framework for D2D Wireless Networks with Heterogeneous Data**|Zhou Ni et.al.|[2501.09822](http://arxiv.org/abs/2501.09822)|null|
|**2025-01-16**|**Artificial Intelligence-Driven Clinical Decision Support Systems**|Muhammet Alkan et.al.|[2501.09628](http://arxiv.org/abs/2501.09628)|null|
|**2025-01-16**|**Connectivity for AI enabled cities -- A field survey based study of emerging economies**|Dibakar Das et.al.|[2501.09479](http://arxiv.org/abs/2501.09479)|null|
|**2025-01-16**|**Cooperative Decentralized Backdoor Attacks on Vertical Federated Learning**|Seohyun Lee et.al.|[2501.09320](http://arxiv.org/abs/2501.09320)|null|
|**2025-01-15**|**Mitigating Domain Shift in Federated Learning via Intra- and Inter-Domain Prototypes**|Huy Q. Le et.al.|[2501.08521](http://arxiv.org/abs/2501.08521)|null|
|**2025-01-14**|**Multiplayer Federated Learning: Reaching Equilibrium with Less Communication**|TaeHo Yoon et.al.|[2501.08263](http://arxiv.org/abs/2501.08263)|null|
|**2025-01-14**|**UFGraphFR: An attempt at a federated recommendation system based on user text characteristics**|Xudong Wang et.al.|[2501.08044](http://arxiv.org/abs/2501.08044)|**[link](https://github.com/trueWangSyutung/UFGraphFR)**|
|**2025-01-15**|**Maximizing Uncertainty for Federated learning via Bayesian Optimisation-based Model Poisoning**|Marios Aristodemou et.al.|[2501.08002](http://arxiv.org/abs/2501.08002)|null|
|**2025-01-13**|**A Federated Deep Learning Framework for Cell-Free RSMA Networks**|S. Ali Mousavi et.al.|[2501.07126](http://arxiv.org/abs/2501.07126)|null|
|**2025-01-12**|**ByzSFL: Achieving Byzantine-Robust Secure Federated Learning with Zero-Knowledge Proofs**|Yongming Fan et.al.|[2501.06953](http://arxiv.org/abs/2501.06953)|null|
|**2025-01-12**|**KeTS: Kernel-based Trust Segmentation against Model Poisoning Attacks**|Ankit Gangwal et.al.|[2501.06729](http://arxiv.org/abs/2501.06729)|null|
|**2025-01-11**|**SafeSplit: A Novel Defense Against Client-Side Backdoor Attacks in Split Learning**|Phillip Rieger et.al.|[2501.06650](http://arxiv.org/abs/2501.06650)|null|
|**2025-01-11**|**Reliable Imputed-Sample Assisted Vertical Federated Learning**|Yaopei Zeng et.al.|[2501.06429](http://arxiv.org/abs/2501.06429)|null|
|**2025-01-10**|**Aggregating Low Rank Adapters in Federated Fine-tuning**|Evelyn Trautmann et.al.|[2501.06332](http://arxiv.org/abs/2501.06332)|null|
|**2025-01-10**|**Explainable Federated Bayesian Causal Inference and Its Application in Advanced Manufacturing**|Xiaofeng Xiao et.al.|[2501.06077](http://arxiv.org/abs/2501.06077)|**[link](https://github.com/xx987/xfbci)**|
|**2025-01-10**|**Encoded Spatial Attribute in Multi-Tier Federated Learning**|Asfia Kawnine et.al.|[2501.05934](http://arxiv.org/abs/2501.05934)|null|
|**2025-01-10**|**Collaborative Content Moderation in the Fediverse**|Haris Bin Zia et.al.|[2501.05871](http://arxiv.org/abs/2501.05871)|null|
|**2025-01-10**|**STHFL: Spatio-Temporal Heterogeneous Federated Learning**|Shunxin Guo et.al.|[2501.05775](http://arxiv.org/abs/2501.05775)|null|
|**2025-01-10**|**Constrained Over-the-Air Model Updating for Wireless Online Federated Learning with Delayed Information**|Juncheng Wang et.al.|[2501.05637](http://arxiv.org/abs/2501.05637)|**[link](https://github.com/yituo-liu/INFOCOM2025-COMUDO)**|
|**2025-01-09**|**FedSA: A Unified Representation Learning via Semantic Anchors for Prototype-based Federated Learning**|Yanbing Zhou et.al.|[2501.05496](http://arxiv.org/abs/2501.05496)|null|
|**2025-01-09**|**TAPFed: Threshold Secure Aggregation for Privacy-Preserving Federated Learning**|Runhua Xu et.al.|[2501.05053](http://arxiv.org/abs/2501.05053)|null|
|**2025-01-09**|**A New Perspective on Privacy Protection in Federated Learning with Granular-Ball Computing**|Guannan Lai et.al.|[2501.04940](http://arxiv.org/abs/2501.04940)|**[link](https://github.com/aignlai/grbfl)**|
|**2025-01-08**|**Decentralised Resource Sharing in TinyML: Wireless Bilayer Gossip Parallel SGD for Collaborative Learning**|Ziyuan Bao et.al.|[2501.04817](http://arxiv.org/abs/2501.04817)|null|
|**2025-01-08**|**Gradient Purification: Defense Against Poisoning Attack in Decentralized Federated Learning**|Bin Li et.al.|[2501.04453](http://arxiv.org/abs/2501.04453)|null|
|**2025-01-08**|**Revisiting LocalSGD and SCAFFOLD: Improved Rates and Missing Analysis**|Ruichen Luo et.al.|[2501.04443](http://arxiv.org/abs/2501.04443)|null|
|**2025-01-08**|**Federated Fine-Tuning of LLMs: Framework Comparison and Research Directions**|Na Yan et.al.|[2501.04436](http://arxiv.org/abs/2501.04436)|null|
|**2025-01-08**|**Lossless Privacy-Preserving Aggregation for Decentralized Federated Learning**|Xiaoye Miao et.al.|[2501.04409](http://arxiv.org/abs/2501.04409)|null|
|**2025-01-08**|**AutoDFL: A Scalable and Automated Reputation-Aware Decentralized Federated Learning**|Meryem Malak Dif et.al.|[2501.04331](http://arxiv.org/abs/2501.04331)|**[link](https://github.com/meryemmalakdif/autodfl)**|
|**2025-01-08**|**VerifBFL: Leveraging zk-SNARKs for A Verifiable Blockchained Federated Learning**|Ahmed Ayoub Bellachia et.al.|[2501.04319](http://arxiv.org/abs/2501.04319)|null|
|**2025-01-07**|**FedKD-hybrid: Federated Hybrid Knowledge Distillation for Lithography Hotspot Detection**|Yuqi Li et.al.|[2501.04066](http://arxiv.org/abs/2501.04066)|**[link](https://github.com/itsnotacie/nn-fedkd-hybrid)**|
|**2025-01-07**|**A Survey on Federated Learning in Human Sensing**|Mohan Li et.al.|[2501.04000](http://arxiv.org/abs/2501.04000)|null|
|**2025-01-07**|**Dynamic Authentication and Granularized Authorization with a Cross-Domain Zero Trust Architecture for Federated Learning in Large-Scale IoT Networks**|Xiaoyu Ma et.al.|[2501.03601](http://arxiv.org/abs/2501.03601)|null|
|**2025-01-07**|**A study on performance limitations in Federated Learning**|Karthik Mohan et.al.|[2501.03477](http://arxiv.org/abs/2501.03477)|null|
|**2025-01-07**|**Optimizing Value of Learning in Task-Oriented Federated Meta-Learning Systems**|Bibo Wu et.al.|[2501.03448](http://arxiv.org/abs/2501.03448)|null|
|**2025-01-06**|**Over-the-Air Fair Federated Learning via Multi-Objective Optimization**|Shayan Mohajer Hamidi et.al.|[2501.03392](http://arxiv.org/abs/2501.03392)|**[link](https://github.com/shayanmohajer/ota-ffl)**|
|**2025-01-06**|**FTA-FTL: A Fine-Tuned Aggregation Federated Transfer Learning Scheme for Lithology Microscopic Image Classification**|Keyvan RahimiZadeh et.al.|[2501.03349](http://arxiv.org/abs/2501.03349)|**[link](https://github.com/ahmadtaheri2021/lithology-microscopic-images-mini-dataset)**|
|**2025-01-06**|**The Robustness of Spiking Neural Networks in Federated Learning with Compression Against Non-omniscient Byzantine Attacks**|Manh V. Nguyen et.al.|[2501.03306](http://arxiv.org/abs/2501.03306)|null|
|**2025-01-06**|**Rethinking Byzantine Robustness in Federated Recommendation from Sparse Aggregation Perspective**|Zhongjian Zhang et.al.|[2501.03301](http://arxiv.org/abs/2501.03301)|**[link](https://github.com/zhongjian-zhang/spattack)**|
|**2025-01-06**|**Rate-My-LoRA: Efficient and Adaptive Federated Model Tuning for Cardiac MRI Segmentation**|Xiaoxiao He et.al.|[2501.03223](http://arxiv.org/abs/2501.03223)|null|
|**2025-01-06**|**From Models to Network Topologies: A Topology Inference Attack in Decentralized Federated Learning**|Chao Feng et.al.|[2501.03119](http://arxiv.org/abs/2501.03119)|null|
|**2025-01-06**|**CONTINUUM: Detecting APT Attacks through Spatial-Temporal Graph Neural Networks**|Atmane Ayoub Mansour Bahara et.al.|[2501.02981](http://arxiv.org/abs/2501.02981)|null|
|**2025-01-06**|**Proof-of-Data: A Consensus Protocol for Collaborative Intelligence**|Huiwen Liu et.al.|[2501.02971](http://arxiv.org/abs/2501.02971)|null|
|**2025-01-06**|**AFed: Algorithmic Fair Federated Learning**|Huiqiang Chen et.al.|[2501.02732](http://arxiv.org/abs/2501.02732)|null|
|**2025-01-05**|**Incentive-Compatible Federated Learning with Stackelberg Game Modeling**|Simin Javaherian et.al.|[2501.02662](http://arxiv.org/abs/2501.02662)|null|
|**2025-01-05**|**FedRSClip: Federated Learning for Remote Sensing Scene Classification Using Vision-Language Models**|Hui Lin et.al.|[2501.02461](http://arxiv.org/abs/2501.02461)|null|
|**2025-01-05**|**Efficient Deployment of Large Language Models on Resource-constrained Devices**|Zhiwei Yao et.al.|[2501.02438](http://arxiv.org/abs/2501.02438)|null|
|**2025-01-04**|**Diffusion Model-Based Data Synthesis Aided Federated Semi-Supervised Learning**|Zhongwei Wang et.al.|[2501.02219](http://arxiv.org/abs/2501.02219)|null|
|**2025-01-03**|**Mingling with the Good to Backdoor Federated Learning**|Nuno Neves et.al.|[2501.01913](http://arxiv.org/abs/2501.01913)|null|
|**2025-01-03**|**LCFed: An Efficient Clustered Federated Learning Framework for Heterogeneous Data**|Yuxin Zhang et.al.|[2501.01850](http://arxiv.org/abs/2501.01850)|null|
|**2025-01-03**|**Age-Based Device Selection and Transmit Power Optimization in Over-the-Air Federated Learning**|Jingyuan Liu et.al.|[2501.01828](http://arxiv.org/abs/2501.01828)|null|
|**2025-01-03**|**Uncertainty-Aware Label Refinement on Hypergraphs for Personalized Federated Facial Expression Recognition**|Hu Ding et.al.|[2501.01816](http://arxiv.org/abs/2501.01816)|null|
|**2025-01-03**|**Denoising and Adaptive Online Vertical Federated Learning for Sequential Multi-Sensor Data in Industrial Internet of Things**|Heqiang Wang et.al.|[2501.01693](http://arxiv.org/abs/2501.01693)|null|
|**2025-01-03**|**Look Back for More: Harnessing Historical Sequential Updates for Personalized Federated Adapter Tuning**|Danni Peng et.al.|[2501.01653](http://arxiv.org/abs/2501.01653)|null|
|**2025-01-03**|**Stackelberg Game Based Performance Optimization in Digital Twin Assisted Federated Learning over NOMA Networks**|Bibo Wu et.al.|[2501.01584](http://arxiv.org/abs/2501.01584)|null|
|**2025-01-02**|**Communication-and-Computation Efficient Split Federated Learning: Gradient Aggregation and Resource Management**|Yipeng Liang et.al.|[2501.01078](http://arxiv.org/abs/2501.01078)|null|
|**2025-01-02**|**FAPL-DM-BC: A Secure and Scalable FL Framework with Adaptive Privacy and Dynamic Masking, Blockchain, and XAI for the IoVs**|Sathwik Narkedimilli et.al.|[2501.01063](http://arxiv.org/abs/2501.01063)|null|
|**2025-01-01**|**Gradient Compression and Correlation Driven Federated Learning for Wireless Traffic Prediction**|Chuanting Zhang et.al.|[2501.00732](http://arxiv.org/abs/2501.00732)|**[link](https://github.com/chuanting/fedgcc)**|
|**2025-01-01**|**Beyond Model Scale Limits: End-Edge-Cloud Federated Learning with Self-Rectified Knowledge Agglomeration**|Zhiyuan Wu et.al.|[2501.00693](http://arxiv.org/abs/2501.00693)|null|
|**2024-12-31**|**Federated Dropout: Convergence Analysis and Resource Allocation**|Sijing Xie et.al.|[2501.00379](http://arxiv.org/abs/2501.00379)|null|
|**2024-12-31**|**Federated Deep Subspace Clustering**|Yupei Zhang et.al.|[2501.00230](http://arxiv.org/abs/2501.00230)|null|
|**2024-12-31**|**FedCod: An Efficient Communication Protocol for Cross-Silo Federated Learning with Coding**|Peishen Yan et.al.|[2501.00216](http://arxiv.org/abs/2501.00216)|null|
|**2024-12-30**|**Federated Learning with Workload Reduction through Partial Training of Client Models and Entropy-Based Data Selection**|Hongrui Shi et.al.|[2501.00170](http://arxiv.org/abs/2501.00170)|null|
|**2024-12-30**|**Generalizing in Net-Zero Microgrids: A Study with Federated PPO and TRPO**|Nicolas M Cuadrado Avila et.al.|[2412.20946](http://arxiv.org/abs/2412.20946)|**[link](https://github.com/Optimization-and-Machine-Learning-Lab/energy_fed_trpo)**|
|**2024-12-30**|**Accelerating Energy-Efficient Federated Learning in Cell-Free Networks with Adaptive Quantization**|Afsaneh Mahmoudi et.al.|[2412.20785](http://arxiv.org/abs/2412.20785)|null|
|**2024-12-30**|**Enhancing Privacy in Federated Learning through Quantum Teleportation Integration**|Koffka Khan et.al.|[2412.20762](http://arxiv.org/abs/2412.20762)|null|
|**2024-12-30**|**Blockchain-Empowered Cyber-Secure Federated Learning for Trustworthy Edge Computing**|Ervin Moore et.al.|[2412.20674](http://arxiv.org/abs/2412.20674)|null|
|**2024-12-28**|**Election of Collaborators via Reinforcement Learning for Federated Brain Tumor Segmentation**|Muhammad Irfan Khan et.al.|[2412.20253](http://arxiv.org/abs/2412.20253)|null|
|**2024-12-28**|**Recommender Engine Driven Client Selection in Federated Brain Tumor Segmentation**|Muhammad Irfan Khan et.al.|[2412.20250](http://arxiv.org/abs/2412.20250)|null|
|**2024-12-28**|**Federated Unlearning with Gradient Descent and Conflict Mitigation**|Zibin Pan et.al.|[2412.20200](http://arxiv.org/abs/2412.20200)|**[link](https://github.com/zibinpan/FedOSD)**|
|**2024-12-28**|**Calibre: Towards Fair and Accurate Personalized Federated Learning with Self-Supervised Learning**|Sijia Chen et.al.|[2412.20020](http://arxiv.org/abs/2412.20020)|**[link](https://github.com/tl-system/plato)**|
|**2024-12-28**|**A Robust Federated Learning Framework for Undependable Devices at Scale**|Shilong Wang et.al.|[2412.19991](http://arxiv.org/abs/2412.19991)|null|
|**2024-12-28**|**Caesar: A Low-deviation Compression Approach for Efficient Federated Learning**|Jiaming Yan et.al.|[2412.19989](http://arxiv.org/abs/2412.19989)|null|
|**2024-12-27**|**Asymmetrical Reciprocity-based Federated Learning for Resolving Disparities in Medical Diagnosis**|Jiaqi Wang et.al.|[2412.19654](http://arxiv.org/abs/2412.19654)|**[link](https://github.com/JackqqWang/fedhelp)**|
|**2024-12-26**|**Federated Hybrid Training and Self-Adversarial Distillation: Towards Robust Edge Networks**|Yu Qiao et.al.|[2412.19354](http://arxiv.org/abs/2412.19354)|null|
|**2024-12-26**|**Effective and secure federated online learning to rank**|Shuyi Wang et.al.|[2412.19069](http://arxiv.org/abs/2412.19069)|null|
|**2024-12-25**|**Optimal Federated Learning for Functional Mean Estimation under Heterogeneous Privacy Constraints**|Tony Cai et.al.|[2412.18992](http://arxiv.org/abs/2412.18992)|null|
|**2024-12-25**|**FedCFA: Alleviating Simpson's Paradox in Model Aggregation with Counterfactual Federated Learning**|Zhonghua Jiang et.al.|[2412.18904](http://arxiv.org/abs/2412.18904)|null|
|**2024-12-25**|**Federated Learning with Partially Labeled Data: A Conditional Distillation Approach**|Pochuan Wang et.al.|[2412.18833](http://arxiv.org/abs/2412.18833)|null|
|**2024-12-24**|**FedVCK: Non-IID Robust and Communication-Efficient Federated Learning via Valuable Condensed Knowledge for Medical Image Analysis**|Guochen Yan et.al.|[2412.18557](http://arxiv.org/abs/2412.18557)|null|
|**2024-12-24**|**FedGIG: Graph Inversion from Gradient in Federated Learning**|Tianzhe Xiao et.al.|[2412.18513](http://arxiv.org/abs/2412.18513)|null|
|**2024-12-24**|**An Empirical Analysis of Federated Learning Models Subject to Label-Flipping Adversarial Attack**|Kunal Bhatnagar et.al.|[2412.18507](http://arxiv.org/abs/2412.18507)|null|
|**2024-12-24**|**GeFL: Model-Agnostic Federated Learning with Generative Models**|Honggu Kang et.al.|[2412.18460](http://arxiv.org/abs/2412.18460)|null|
|**2024-12-24**|**Addressing Spatial-Temporal Data Heterogeneity in Federated Continual Learning via Tail Anchor**|Hao Yu et.al.|[2412.18355](http://arxiv.org/abs/2412.18355)|null|
|**2024-12-23**|**Asynchronous Federated Learning: A Scalable Approach for Decentralized Machine Learning**|Ali Forootani et.al.|[2412.17723](http://arxiv.org/abs/2412.17723)|**[link](https://github.com/ali-forootani/asynchronous-federated-learning)**|
|**2024-12-23**|**FedTLU: Federated Learning with Targeted Layer Updates**|Jong-Ik Park et.al.|[2412.17692](http://arxiv.org/abs/2412.17692)|null|
|**2024-12-23**|**Better Knowledge Enhancement for Privacy-Preserving Cross-Project Defect Prediction**|Yuying Wang et.al.|[2412.17317](http://arxiv.org/abs/2412.17317)|null|
|**2024-12-23**|**FedLEC: Effective Federated Learning Algorithm with Spiking Neural Networks Under Label Skews**|Di Yu et.al.|[2412.17305](http://arxiv.org/abs/2412.17305)|null|
|**2024-12-23**|**FedMeld: A Model-dispersal Federated Learning Framework for Space-ground Integrated Networks**|Qian Chen et.al.|[2412.17231](http://arxiv.org/abs/2412.17231)|null|
|**2024-12-22**|**Data value estimation on private gradients**|Zijian Zhou et.al.|[2412.17008](http://arxiv.org/abs/2412.17008)|null|
|**2024-12-22**|**FedCross: Intertemporal Federated Learning Under Evolutionary Games**|Jianfeng Lu et.al.|[2412.16968](http://arxiv.org/abs/2412.16968)|null|
|**2024-12-21**|**Fed-ZOE: Communication-Efficient Over-the-Air Federated Learning via Zeroth-Order Estimation**|Jonggyu Jang et.al.|[2412.16779](http://arxiv.org/abs/2412.16779)|null|
|**2024-12-21**|**Label Privacy in Split Learning for Large Models with Parameter-Efficient Training**|Philip Zmushko et.al.|[2412.16669](http://arxiv.org/abs/2412.16669)|**[link](https://github.com/p3eft-iclr-2025/p3eft-iclr-2025)**|
|**2024-12-21**|**FedGA: Federated Learning with Gradient Alignment for Error Asymmetry Mitigation**|Chenguang Xiao et.al.|[2412.16582](http://arxiv.org/abs/2412.16582)|null|
|**2024-12-20**|**Differentially Private Federated Learning of Diffusion Models for Synthetic Tabular Data Generation**|Timur Sattarov et.al.|[2412.16083](http://arxiv.org/abs/2412.16083)|null|
|**2024-12-20**|**fluke: Federated Learning Utility frameworK for Experimentation and research**|Mirko Polato et.al.|[2412.15728](http://arxiv.org/abs/2412.15728)|null|
|**2024-12-20**|**Code Review Automation Via Multi-task Federated LLM -- An Empirical Study**|Jahnavi Kumar et.al.|[2412.15676](http://arxiv.org/abs/2412.15676)|null|
|**2024-12-20**|**AutoRank: MCDA Based Rank Personalization for LoRA-Enabled Distributed Learning**|Shuaijun Chen et.al.|[2412.15553](http://arxiv.org/abs/2412.15553)|null|
|**2024-12-20**|**The Impact of Cut Layer Selection in Split Federated Learning**|Justin Dachille et.al.|[2412.15536](http://arxiv.org/abs/2412.15536)|null|
|**2024-12-20**|**DualGFL: Federated Learning with a Dual-Level Coalition-Auction Game**|Xiaobing Chen et.al.|[2412.15492](http://arxiv.org/abs/2412.15492)|null|
|**2024-12-19**|**Federated Learning for Coronary Artery Plaque Detection in Atherosclerosis Using IVUS Imaging: A Multi-Hospital Collaboration**|Chiu-Han Hsiao et.al.|[2412.15307](http://arxiv.org/abs/2412.15307)|null|
|**2024-12-19**|**Robust Federated Learning in the Face of Covariate Shift: A Magnitude Pruning with Hybrid Regularization Framework for Enhanced Model Aggregation**|Ozgu Goksu et.al.|[2412.15010](http://arxiv.org/abs/2412.15010)|null|
|**2024-12-19**|**Federated Heavy Hitter Analytics with Local Differential Privacy**|Yuemin Zhang et.al.|[2412.14832](http://arxiv.org/abs/2412.14832)|null|
|**2024-12-19**|**FLAMe: Federated Learning with Attention Mechanism using Spatio-Temporal Keypoint Transformers for Pedestrian Fall Detection in Smart Cities**|Byeonghun Kim et.al.|[2412.14768](http://arxiv.org/abs/2412.14768)|null|
|**2024-12-19**|**LoLaFL: Low-Latency Federated Learning via Forward-only Propagation**|Jierui Zhang et.al.|[2412.14668](http://arxiv.org/abs/2412.14668)|null|
|**2024-12-19**|**Summary of Point Transformer with Federated Learning for Predicting Breast Cancer HER2 Status from Hematoxylin and Eosin-Stained Whole Slide Images**|Kamorudeen A. Amuda et.al.|[2412.14545](http://arxiv.org/abs/2412.14545)|null|
|**2024-12-19**|**FedMUP: Federated Learning driven Malicious User Prediction Model for Secure Data Distribution in Cloud Environments**|Kishu Gupta et.al.|[2412.14495](http://arxiv.org/abs/2412.14495)|null|
|**2024-12-19**|**FedPIA -- Permuting and Integrating Adapters leveraging Wasserstein Barycenters for Finetuning Foundation Models in Multi-Modal Federated Learning**|Pramit Saha et.al.|[2412.14424](http://arxiv.org/abs/2412.14424)|null|
|**2024-12-18**|**Covariances for Free: Exploiting Mean Distributions for Federated Learning with Pre-Trained Models**|Dipam Goswami et.al.|[2412.14326](http://arxiv.org/abs/2412.14326)|null|
|**2024-12-18**|**FedSTaS: Client Stratification and Client Level Sampling for Efficient Federated Learning**|Jordan Slessor et.al.|[2412.14226](http://arxiv.org/abs/2412.14226)|null|
|**2024-12-18**|**On the Robustness of Distributed Machine Learning against Transfer Attacks**|Sébastien Andreina et.al.|[2412.14080](http://arxiv.org/abs/2412.14080)|null|
|**2024-12-18**|**Fed-AugMix: Balancing Privacy and Utility via Data Augmentation**|Haoyang Li et.al.|[2412.13818](http://arxiv.org/abs/2412.13818)|null|
|**2024-12-18**|**Rehearsal-Free Continual Federated Learning with Synergistic Regularization**|Yichen Li et.al.|[2412.13779](http://arxiv.org/abs/2412.13779)|null|
|**2024-12-18**|**Federated Source-free Domain Adaptation for Classification: Weighted Cluster Aggregation for Unlabeled Data**|Junki Mori et.al.|[2412.13757](http://arxiv.org/abs/2412.13757)|null|
|**2024-12-18**|**Federated Learning and RAG Integration: A Scalable Approach for Medical Large Language Models**|Jincheol Jung et.al.|[2412.13720](http://arxiv.org/abs/2412.13720)|null|
|**2024-12-18**|**SemiDFL: A Semi-Supervised Paradigm for Decentralized Federated Learning**|Xinyang Liu et.al.|[2412.13589](http://arxiv.org/abs/2412.13589)|**[link](https://github.com/ez4lionky/SemiDFL)**|
|**2024-12-18**|**Large Language Model Federated Learning with Blockchain and Unlearning for Cross-Organizational Collaboration**|Xuhan Zuo et.al.|[2412.13551](http://arxiv.org/abs/2412.13551)|null|
|**2024-12-18**|**Federated t-SNE and UMAP for Distributed Data Visualization**|Dong Qiao et.al.|[2412.13495](http://arxiv.org/abs/2412.13495)|null|
|**2024-12-18**|**Federated Unlearning Model Recovery in Data with Skewed Label Distributions**|Xinrui Yu et.al.|[2412.13466](http://arxiv.org/abs/2412.13466)|null|
|**2024-12-17**|**Concurrent vertical and horizontal federated learning with fuzzy cognitive maps**|Jose L Salmeron et.al.|[2412.12844](http://arxiv.org/abs/2412.12844)|null|
|**2024-12-17**|**Building Gradient Bridges: Label Leakage from Restricted Gradient Sharing in Federated Learning**|Rui Zhang et.al.|[2412.12640](http://arxiv.org/abs/2412.12640)|null|
|**2024-12-16**|**F-RBA: A Federated Learning-based Framework for Risk-based Authentication**|Hamidreza Fereidouni et.al.|[2412.12324](http://arxiv.org/abs/2412.12324)|null|
|**2024-12-16**|**Efficiently Achieving Secure Model Training and Secure Aggregation to Ensure Bidirectional Privacy-Preservation in Federated Learning**|Xue Yang et.al.|[2412.11737](http://arxiv.org/abs/2412.11737)|null|
|**2024-12-16**|**Just a Simple Transformation is Enough for Data Protection in Vertical Federated Learning**|Andrei Semenov et.al.|[2412.11689](http://arxiv.org/abs/2412.11689)|**[link](https://github.com/andron00e/jast)**|
|**2024-12-16**|**UA-PDFL: A Personalized Approach for Decentralized Federated Learning**|Hangyu Zhu et.al.|[2412.11674](http://arxiv.org/abs/2412.11674)|null|
|**2024-12-16**|**Non-Convex Optimization in Federated Learning via Variance Reduction and Adaptive Learning**|Dipanwita Thakur et.al.|[2412.11660](http://arxiv.org/abs/2412.11660)|null|
|**2024-12-16**|**BA-BFL: Barycentric Aggregation for Bayesian Federated Learning**|Nour Jamoussi et.al.|[2412.11646](http://arxiv.org/abs/2412.11646)|null|
|**2024-12-16**|**Capacity of Hierarchical Secure Coded Gradient Aggregation with Straggling Communication Links**|Qinyi Lu et.al.|[2412.11496](http://arxiv.org/abs/2412.11496)|null|
|**2024-12-16**|**Vertical Federated Unlearning via Backdoor Certification**|Mengde Han et.al.|[2412.11476](http://arxiv.org/abs/2412.11476)|**[link](https://github.com/mengde-han/vfl-unlearn)**|
|**2024-12-16**|**FedCAR: Cross-client Adaptive Re-weighting for Generative Models in Federated Learning**|Minjun Kim et.al.|[2412.11463](http://arxiv.org/abs/2412.11463)|**[link](https://github.com/danny0628/fedcar)**|
|**2024-12-16**|**TRAIL: Trust-Aware Client Scheduling for Semi-Decentralized Federated Learning**|Gangqiang Hu et.al.|[2412.11448](http://arxiv.org/abs/2412.11448)|null|
|**2024-12-16**|**Federated Domain Generalization with Label Smoothing and Balanced Decentralized Training**|Milad Soltany et.al.|[2412.11408](http://arxiv.org/abs/2412.11408)|null|
|**2024-12-13**|**Temporal Causal Discovery in Dynamic Bayesian Networks Using Federated Learning**|Jianhong Chen et.al.|[2412.09814](http://arxiv.org/abs/2412.09814)|**[link](https://github.com/pechen123/2dbn_learning)**|
|**2024-12-12**|**Multi-client Functional Encryption for Set Intersection with Non-monotonic Access Structures in Federated Learning**|Ruyuan Zhang et.al.|[2412.09259](http://arxiv.org/abs/2412.09259)|null|
|**2024-12-12**|**Deep Learning Model Security: Threats and Defenses**|Tianyang Wang et.al.|[2412.08969](http://arxiv.org/abs/2412.08969)|null|
|**2024-12-12**|**Predicting Quality of Video Gaming Experience Using Global-Scale Telemetry Data and Federated Learning**|Zhongyang Zhang et.al.|[2412.08950](http://arxiv.org/abs/2412.08950)|null|
|**2024-12-12**|**Federated Foundation Models on Heterogeneous Time Series**|Shengchao Chen et.al.|[2412.08906](http://arxiv.org/abs/2412.08906)|**[link](https://github.com/shengchaochen82/FFTS)**|
|**2024-12-11**|**Federated Learning for Traffic Flow Prediction with Synthetic Data Augmentation**|Fermin Orozco et.al.|[2412.08460](http://arxiv.org/abs/2412.08460)|null|
|**2024-12-11**|**How Does the Smoothness Approximation Method Facilitate Generalization for Federated Adversarial Learning?**|Wenjun Ding et.al.|[2412.08282](http://arxiv.org/abs/2412.08282)|null|
|**2024-12-12**|**Learn How to Query from Unlabeled Data Streams in Federated Learning**|Yuchang Sun et.al.|[2412.08138](http://arxiv.org/abs/2412.08138)|**[link](https://github.com/hiyuchang/leadq)**|
|**2024-12-11**|**A Tutorial of Personalized Federated Recommender Systems: Recent Advances and Future Directions**|Jing Jiang et.al.|[2412.08071](http://arxiv.org/abs/2412.08071)|null|
|**2024-12-11**|**Federated In-Context LLM Agent Learning**|Panlong Wu et.al.|[2412.08054](http://arxiv.org/abs/2412.08054)|null|
|**2024-12-11**|**dsLassoCov: a federated machine learning approach incorporating covariate control**|Han Cao et.al.|[2412.07991](http://arxiv.org/abs/2412.07991)|null|
|**2024-12-10**|**Evaluating the Potential of Federated Learning for Maize Leaf Disease Prediction**|Thalita Mendonça Antico et.al.|[2412.07872](http://arxiv.org/abs/2412.07872)|null|
|**2024-12-10**|**Privacy-Preserving Customer Support: A Framework for Secure and Scalable Interactions**|Anant Prakash Awasthi et.al.|[2412.07687](http://arxiv.org/abs/2412.07687)|null|
|**2024-12-10**|**Tazza: Shuffling Neural Network Parameters for Secure and Private Federated Learning**|Kichang Lee et.al.|[2412.07454](http://arxiv.org/abs/2412.07454)|null|
|**2024-12-10**|**When UAV Meets Federated Learning: Latency Minimization via Joint Trajectory Design and Resource Allocation**|Xuhui Zhang et.al.|[2412.07428](http://arxiv.org/abs/2412.07428)|null|
|**2024-12-10**|**Learnable Sparse Customization in Heterogeneous Edge Computing**|Jingjing Xue et.al.|[2412.07216](http://arxiv.org/abs/2412.07216)|**[link](https://github.com/sunnyxuejj/FedLPS)**|
|**2024-12-10**|**Hierarchical Split Federated Learning: Convergence Analysis and System Optimization**|Zheng Lin et.al.|[2412.07197](http://arxiv.org/abs/2412.07197)|null|
|**2024-12-10**|**A New Federated Learning Framework Against Gradient Inversion Attacks**|Pengxin Guo et.al.|[2412.07187](http://arxiv.org/abs/2412.07187)|**[link](https://github.com/pengxin-guo/hyperfl)**|
|**2024-12-10**|**Optimizing Personalized Federated Learning through Adaptive Layer-Wise Learning**|Weihang Chen et.al.|[2412.07062](http://arxiv.org/abs/2412.07062)|null|
|**2024-12-09**|**Sequential Compression Layers for Efficient Federated Learning in Foundational Models**|Navyansh Mahla et.al.|[2412.07021](http://arxiv.org/abs/2412.07021)|null|
|**2024-12-09**|**FedSynthCT-Brain: A Federated Learning Framework for Multi-Institutional Brain MRI-to-CT Synthesis**|Ciro Benito Raggio et.al.|[2412.06690](http://arxiv.org/abs/2412.06690)|null|
|**2024-12-09**|**A cautionary tale on the cost-effectiveness of collaborative AI in real-world medical applications**|Francesco Cremonesi et.al.|[2412.06494](http://arxiv.org/abs/2412.06494)|null|
|**2024-12-09**|**Federated Split Learning with Model Pruning and Gradient Quantization in Wireless Networks**|Junhe Zhang et.al.|[2412.06414](http://arxiv.org/abs/2412.06414)|null|
|**2024-12-09**|**H-FedSN: Personalized Sparse Networks for Efficient and Accurate Hierarchical Federated Learning for IoT Applications**|Jiechao Gao et.al.|[2412.06210](http://arxiv.org/abs/2412.06210)|null|
|**2024-12-09**|**Membership Inference Attacks and Defenses in Federated Learning: A Survey**|Li Bai et.al.|[2412.06157](http://arxiv.org/abs/2412.06157)|null|
|**2024-12-09**|**Lightweight Federated Learning with Differential Privacy and Straggler Resilience**|Shu Hong et.al.|[2412.06120](http://arxiv.org/abs/2412.06120)|null|
|**2024-12-09**|**Privacy-Preserving Large Language Models: Mechanisms, Applications, and Future Directions**|Guoshenghui Zhao et.al.|[2412.06113](http://arxiv.org/abs/2412.06113)|null|
|**2024-12-08**|**FedRBE -- a decentralized privacy-preserving federated batch effect correction tool for omics data based on limma**|Yuliya Burankova et.al.|[2412.05894](http://arxiv.org/abs/2412.05894)|null|
|**2024-12-08**|**DapperFL: Domain Adaptive Federated Learning with Model Fusion Pruning for Edge Devices**|Yongzhe Jia et.al.|[2412.05823](http://arxiv.org/abs/2412.05823)|**[link](https://github.com/jyzgh/dapperfl)**|
|**2024-12-07**|**A Game-Theoretic Framework for Privacy-Aware Client Sampling in Federated Learning**|Wenhao Yuan et.al.|[2412.05636](http://arxiv.org/abs/2412.05636)|null|
|**2024-12-06**|**One-shot Federated Learning via Synthetic Distiller-Distillate Communication**|Junyuan Zhang et.al.|[2412.05186](http://arxiv.org/abs/2412.05186)|**[link](https://github.com/carkham/fedsd2c)**|
|**2024-12-06**|**Privacy Drift: Evolving Privacy Concerns in Incremental Learning**|Sayyed Farid Ahamed et.al.|[2412.05183](http://arxiv.org/abs/2412.05183)|null|
|**2024-12-06**|**A Federated Approach to Few-Shot Hate Speech Detection for Marginalized Communities**|Haotian Ye et.al.|[2412.04942](http://arxiv.org/abs/2412.04942)|null|
|**2024-12-06**|**NebulaFL: Effective Asynchronous Federated Learning for JointCloud Computing**|Fei Gao et.al.|[2412.04868](http://arxiv.org/abs/2412.04868)|null|
|**2024-12-05**|**Communication Compression for Distributed Learning without Control Variates**|Tomas Ortega et.al.|[2412.04538](http://arxiv.org/abs/2412.04538)|null|
|**2024-12-05**|**FedDW: Distilling Weights through Consistency Optimization in Heterogeneous Federated Learning**|Jiayu Liu et.al.|[2412.04521](http://arxiv.org/abs/2412.04521)|**[link](https://github.com/liuvvvvv1/feddw)**|
|**2024-12-05**|**FedDUAL: A Dual-Strategy with Adaptive Loss and Dynamic Aggregation for Mitigating Data Heterogeneity in Federated Learning**|Pranab Sahoo et.al.|[2412.04416](http://arxiv.org/abs/2412.04416)|**[link](https://github.com/Pranabiitp/FedDUAL)**|
|**2024-12-05**|**Providing Differential Privacy for Federated Learning Over Wireless: A Cross-layer Framework**|Jiayu Mao et.al.|[2412.04408](http://arxiv.org/abs/2412.04408)|null|
|**2024-12-05**|**Federated Automated Feature Engineering**|Tom Overman et.al.|[2412.04404](http://arxiv.org/abs/2412.04404)|null|
|**2024-12-05**|**Federated Learning in Mobile Networks: A Comprehensive Case Study on Traffic Forecasting**|Nikolaos Pavlidis et.al.|[2412.04081](http://arxiv.org/abs/2412.04081)|**[link](https://github.com/vperifan/federated-time-series-forecasting)**|
|**2024-12-05**|**BEFL: Balancing Energy Consumption in Federated Learning for Mobile Edge IoT**|Zehao Ju et.al.|[2412.03950](http://arxiv.org/abs/2412.03950)|**[link](https://github.com/juzehao/befl)**|
|**2024-12-05**|**Privacy-Preserving in Medical Image Analysis: A Review of Methods and Applications**|Yanming Zhu et.al.|[2412.03924](http://arxiv.org/abs/2412.03924)|null|
|**2024-12-05**|**GP-FL: Model-Based Hessian Estimation for Second-Order Over-the-Air Federated Learning**|Shayan Mohajer Hamidi et.al.|[2412.03867](http://arxiv.org/abs/2412.03867)|null|
|**2024-12-05**|**FedMetaMed: Federated Meta-Learning for Personalized Medication in Distributed Healthcare Systems**|Jiechao Gao et.al.|[2412.03851](http://arxiv.org/abs/2412.03851)|null|
|**2024-12-04**|**Beyond Local Sharpness: Communication-Efficient Global Sharpness-aware Minimization for Federated Learning**|Debora Caldarola et.al.|[2412.03752](http://arxiv.org/abs/2412.03752)|null|
|**2024-12-04**|**Adaptive Personalized Over-the-Air Federated Learning with Reflecting Intelligent Surfaces**|Jiayu Mao et.al.|[2412.03514](http://arxiv.org/abs/2412.03514)|null|
|**2024-12-04**|**Reactive Orchestration for Hierarchical Federated Learning Under a Communication Cost Budget**|Ivan Čilić et.al.|[2412.03385](http://arxiv.org/abs/2412.03385)|null|
|**2024-12-03**|**Proximal Control of UAVs with Federated Learning for Human-Robot Collaborative Domains**|Lucas Nogueira Nobrega et.al.|[2412.02863](http://arxiv.org/abs/2412.02863)|null|
|**2024-12-03**|**Methods with Local Steps and Random Reshuffling for Generally Smooth Non-Convex Federated Optimization**|Yury Demidovich et.al.|[2412.02781](http://arxiv.org/abs/2412.02781)|null|
|**2024-12-03**|**Fractional Order Distributed Optimization**|Andrei Lixandru et.al.|[2412.02546](http://arxiv.org/abs/2412.02546)|null|
|**2024-12-03**|**Defending Against Diverse Attacks in Federated Learning Through Consensus-Based Bi-Level Optimization**|Nicolás García Trillos et.al.|[2412.02535](http://arxiv.org/abs/2412.02535)|**[link](https://github.com/SixuLi/FedCB2O)**|
|**2024-12-03**|**Federated Analytics in Practice: Engineering for Privacy, Scalability and Practicality**|Harish Srinivas et.al.|[2412.02340](http://arxiv.org/abs/2412.02340)|null|
|**2024-12-03**|**FL-QDSNNs: Federated Learning with Quantum Dynamic Spiking Neural Networks**|Nouhaila Innan et.al.|[2412.02293](http://arxiv.org/abs/2412.02293)|null|
|**2024-12-03**|**Learn More by Using Less: Distributed Learning with Energy-Constrained Devices**|Roberto Pereira et.al.|[2412.02289](http://arxiv.org/abs/2412.02289)|null|
|**2024-12-03**|**Towards the efficacy of federated prediction for epidemics on networks**|Chengpeng Fu et.al.|[2412.02161](http://arxiv.org/abs/2412.02161)|**[link](https://github.com/S1mple-yyds/Fed_Epi_Classifier)**|
|**2024-12-03**|**Privacy-Preserving Federated Learning via Homomorphic Adversarial Networks**|Wenhan Dong et.al.|[2412.01650](http://arxiv.org/abs/2412.01650)|null|
|**2024-12-02**|**Review of Mathematical Optimization in Federated Learning**|Shusen Yang et.al.|[2412.01630](http://arxiv.org/abs/2412.01630)|null|
|**2024-12-02**|**FedAH: Aggregated Head for Personalized Federated Learning**|Pengzhan Zhou et.al.|[2412.01295](http://arxiv.org/abs/2412.01295)|**[link](https://github.com/heyuepeng/fedah)**|
|**2024-12-02**|**FedPAW: Federated Learning with Personalized Aggregation Weights for Urban Vehicle Speed Prediction**|Yuepeng He et.al.|[2412.01281](http://arxiv.org/abs/2412.01281)|**[link](https://github.com/heyuepeng/pfllibvsp)**|
|**2024-11-29**|**Rethinking the initialization of Momentum in Federated Learning with Heterogeneous Data**|Chenguang Xiao et.al.|[2411.19798](http://arxiv.org/abs/2411.19798)|null|
|**2024-11-29**|**Gradient Inversion Attack on Graph Neural Networks**|Divya Anand Sinha et.al.|[2411.19440](http://arxiv.org/abs/2411.19440)|null|
|**2024-11-28**|**PEFT-as-an-Attack! Jailbreaking Language Models during Federated Parameter-Efficient Fine-Tuning**|Shenghui Li et.al.|[2411.19335](http://arxiv.org/abs/2411.19335)|null|
|**2024-11-28**|**Controlling Participation in Federated Learning with Feedback**|Michael Cummins et.al.|[2411.19242](http://arxiv.org/abs/2411.19242)|null|
|**2024-11-28**|**Personalized Federated Fine-Tuning for LLMs via Data-Driven Heterogeneous Model Architectures**|Yicheng Zhang et.al.|[2411.19128](http://arxiv.org/abs/2411.19128)|**[link](https://github.com/zyc140345/fedamole)**|
|**2024-11-28**|**Swarm Intelligence-Driven Client Selection for Federated Learning in Cybersecurity applications**|Koffka Khan et.al.|[2411.18877](http://arxiv.org/abs/2411.18877)|null|
|**2024-11-27**|**Locally Differentially Private Online Federated Learning With Correlated Noise**|Jiaojiao Zhang et.al.|[2411.18752](http://arxiv.org/abs/2411.18752)|null|
|**2024-11-27**|**Task Arithmetic Through The Lens Of One-Shot Federated Learning**|Zhixu Tao et.al.|[2411.18607](http://arxiv.org/abs/2411.18607)|null|
|**2024-11-27**|**Federated Learning with Uncertainty and Personalization via Efficient Second-order Optimization**|Shivam Pal et.al.|[2411.18385](http://arxiv.org/abs/2411.18385)|null|
|**2024-11-27**|**FreqX: What neural networks learn is what network designers say**|Zechen Liu et.al.|[2411.18343](http://arxiv.org/abs/2411.18343)|null|
|**2024-11-27**|**Hidden Data Privacy Breaches in Federated Learning**|Xueluan Gong et.al.|[2411.18269](http://arxiv.org/abs/2411.18269)|null|
|**2024-11-26**|**Distributed Sign Momentum with Local Steps for Training Transformers**|Shuhua Yu et.al.|[2411.17866](http://arxiv.org/abs/2411.17866)|null|
|**2024-11-26**|**Adaptive Client Selection with Personalization for Communication Efficient Federated Learning**|Allan M. de Souza et.al.|[2411.17833](http://arxiv.org/abs/2411.17833)|**[link](https://github.com/allanmsouza/acsp-fl)**|
|**2024-11-25**|**Towards Efficient Model-Heterogeneity Federated Learning for Large Models**|Ruofan Jia et.al.|[2411.16796](http://arxiv.org/abs/2411.16796)|null|
|**2024-11-25**|**Distributed, communication-efficient, and differentially private estimation of KL divergence**|Mary Scott et.al.|[2411.16478](http://arxiv.org/abs/2411.16478)|null|
|**2024-11-25**|**Distributed Online Optimization with Stochastic Agent Availability**|Juliette Achddou et.al.|[2411.16477](http://arxiv.org/abs/2411.16477)|null|
|**2024-11-25**|**TIFeD: a Tiny Integer-based Federated learning algorithm with Direct feedback alignment**|Luca Colombo et.al.|[2411.16442](http://arxiv.org/abs/2411.16442)|**[link](https://github.com/ai-tech-research-lab/tifed)**|
|**2024-11-25**|**Privacy-Preserving Federated Foundation Model for Generalist Ultrasound Artificial Intelligence**|Yuncheng Jiang et.al.|[2411.16380](http://arxiv.org/abs/2411.16380)|null|
|**2024-11-25**|**Understanding Generalization of Federated Learning: the Trade-off between Model Stability and Optimization**|Dun Zeng et.al.|[2411.16303](http://arxiv.org/abs/2411.16303)|null|
|**2024-11-26**|**BadSFL: Backdoor Attack against Scaffold Federated Learning**|Xingshuo Han et.al.|[2411.16167](http://arxiv.org/abs/2411.16167)|null|
|**2024-11-25**|**An Empirical Study of Vulnerability Detection using Federated Learning**|Peiheng Zhou et.al.|[2411.16099](http://arxiv.org/abs/2411.16099)|null|
|**2024-11-24**|**eFedLLM: Efficient LLM Inference Based on Federated Learning**|Shengwen Ding et.al.|[2411.16003](http://arxiv.org/abs/2411.16003)|null|
|**2024-11-24**|**FedQP: Towards Accurate Federated Learning using Quadratic Programming Guided Mutation**|Jiawen Weng et.al.|[2411.15847](http://arxiv.org/abs/2411.15847)|null|
|**2024-11-24**|**Modality Alignment Meets Federated Broadcasting**|Yuting Ma et.al.|[2411.15837](http://arxiv.org/abs/2411.15837)|null|
|**2024-11-22**|**LoRA-FAIR: Federated LoRA Fine-Tuning with Aggregation and Initialization Refinement**|Jieming Bian et.al.|[2411.14961](http://arxiv.org/abs/2411.14961)|null|
|**2024-11-22**|**Geminio: Language-Guided Gradient Inversion Attacks in Federated Learning**|Junjie Shan et.al.|[2411.14937](http://arxiv.org/abs/2411.14937)|**[link](https://github.com/HKU-TASR/Geminio)**|
|**2024-11-22**|**FedMLLM: Federated Fine-tuning MLLM on Multimodal Heterogeneity Data**|Binqian Xu et.al.|[2411.14717](http://arxiv.org/abs/2411.14717)|**[link](https://github.com/1xbq1/fedmllm)**|
|**2024-11-21**|**Memory Backdoor Attacks on Neural Networks**|Eden Luzon et.al.|[2411.14516](http://arxiv.org/abs/2411.14516)|null|
|**2024-11-21**|**Towards Adaptive Asynchronous Federated Learning for Human Activity Recognition**|Rastko Gajanin et.al.|[2411.14070](http://arxiv.org/abs/2411.14070)|null|
|**2024-11-21**|**REFOL: Resource-Efficient Federated Online Learning for Traffic Flow Forecasting**|Qingxiang Liu et.al.|[2411.14046](http://arxiv.org/abs/2411.14046)|**[link](https://github.com/yuppielqx/refol)**|
|**2024-11-21**|**FedRAV: Hierarchically Federated Region-Learning for Traffic Object Classification of Autonomous Vehicles**|Yijun Zhai et.al.|[2411.13979](http://arxiv.org/abs/2411.13979)|**[link](https://github.com/yjzhai-cs/fedrav)**|
|**2024-11-21**|**Split Federated Learning Over Heterogeneous Edge Devices: Algorithm and Optimization**|Yunrui Sun et.al.|[2411.13907](http://arxiv.org/abs/2411.13907)|null|
|**2024-11-21**|**Asynchronous Federated Learning Using Outdated Local Updates Over TDMA Channel**|Jaeyoung Song et.al.|[2411.13861](http://arxiv.org/abs/2411.13861)|null|
|**2024-11-20**|**CB $^2$ O: Consensus-Based Bi-Level Optimization**|Nicolás García Trillos et.al.|[2411.13394](http://arxiv.org/abs/2411.13394)|**[link](https://github.com/sixuli/cb2o)**|
|**2024-11-20**|**On-device Content-based Recommendation with Single-shot Embedding Pruning: A Cooperative Game Perspective**|Hung Vinh Tran et.al.|[2411.13052](http://arxiv.org/abs/2411.13052)|null|
|**2024-11-20**|**NCAirFL: CSI-Free Over-the-Air Federated Learning Based on Non-Coherent Detection**|Haifeng Wen et.al.|[2411.13000](http://arxiv.org/abs/2411.13000)|null|
|**2024-11-19**|**Attribute Inference Attacks for Federated Regression Tasks**|Francesco Diana et.al.|[2411.12697](http://arxiv.org/abs/2411.12697)|null|
|**2024-11-19**|**Non-IID data in Federated Learning: A Systematic Review with Taxonomy, Metrics, Methods, Frameworks and Future Directions**|Daniel M. Jimenez G. et.al.|[2411.12377](http://arxiv.org/abs/2411.12377)|null|
|**2024-11-19**|**Hyper-parameter Optimization for Federated Learning with Step-wise Adaptive Mechanism**|Yasaman Saadati et.al.|[2411.12244](http://arxiv.org/abs/2411.12244)|null|
|**2024-11-19**|**DeTrigger: A Gradient-Centric Approach to Backdoor Attack Mitigation in Federated Learning**|Kichang Lee et.al.|[2411.12220](http://arxiv.org/abs/2411.12220)|null|
|**2024-11-18**|**Federated Contrastive Learning of Graph-Level Representations**|Xiang Li et.al.|[2411.12098](http://arxiv.org/abs/2411.12098)|null|
|**2024-11-17**|**F $^3$ OCUS -- Federated Finetuning of Vision-Language Foundation Models with Optimal Client Layer Updating Strategy via Multi-objective Meta-Heuristics**|Pramit Saha et.al.|[2411.11912](http://arxiv.org/abs/2411.11912)|null|
|**2024-11-18**|**A Potential Game Perspective in Federated Learning**|Kang Liu et.al.|[2411.11793](http://arxiv.org/abs/2411.11793)|**[link](https://github.com/DCN-FAU-AvH/FL-Potential-Game)**|
|**2024-11-19**|**Freezing of Gait Detection Using Gramian Angular Fields and Federated Learning from Wearable Sensors**|Shovito Barua Soumma et.al.|[2411.11764](http://arxiv.org/abs/2411.11764)|**[link](https://github.com/shovito66/fogsense)**|
|**2024-11-18**|**FLMarket: Enabling Privacy-preserved Pre-training Data Pricing for Federated Learning**|Zhenyu Wen et.al.|[2411.11713](http://arxiv.org/abs/2411.11713)|null|
|**2024-11-18**|**Toward Personalized Federated Node Classification in One-shot Communication**|Guochen Yan et.al.|[2411.11304](http://arxiv.org/abs/2411.11304)|null|
|**2024-11-17**|**Federated Learning for UAV-Based Spectrum Sensing: Enhancing Accuracy Through SNR-Weighted Model Aggregation**|Kürşat Tekbıyık et.al.|[2411.11159](http://arxiv.org/abs/2411.11159)|null|
|**2024-11-17**|**Efficient Federated Unlearning with Adaptive Differential Privacy Preservation**|Yu Jiang et.al.|[2411.11044](http://arxiv.org/abs/2411.11044)|null|
|**2024-11-17**|**FedUHB: Accelerating Federated Unlearning via Polyak Heavy Ball Method**|Yu Jiang et.al.|[2411.11039](http://arxiv.org/abs/2411.11039)|null|
|**2024-11-16**|**How to Defend Against Large-scale Model Poisoning Attacks in Federated Learning: A Vertical Solution**|Jinbo Wang et.al.|[2411.10673](http://arxiv.org/abs/2411.10673)|null|
|**2024-11-15**|**Electrical Load Forecasting in Smart Grid: A Personalized Federated Learning Approach**|Ratun Rahman et.al.|[2411.10619](http://arxiv.org/abs/2411.10619)|null|
|**2024-11-15**|**FedAli: Personalized Federated Learning with Aligned Prototypes through Optimal Transport**|Sannara Ek et.al.|[2411.10595](http://arxiv.org/abs/2411.10595)|null|
|**2024-11-15**|**Framework for Co-distillation Driven Federated Learning to Address Class Imbalance in Healthcare**|Suraj Racha et.al.|[2411.10383](http://arxiv.org/abs/2411.10383)|**[link](https://github.com/humairafirdowse/codistillation)**|
|**2024-11-15**|**Artificial Intelligence in Pediatric Echocardiography: Exploring Challenges, Opportunities, and Clinical Applications with Explainable AI and Federated Learning**|Mohammed Yaseen Jabarulla et.al.|[2411.10255](http://arxiv.org/abs/2411.10255)|null|
|**2024-11-15**|**Embedding Byzantine Fault Tolerance into Federated Learning via Virtual Data-Driven Consistency Scoring Plugin**|Youngjoon Lee et.al.|[2411.10212](http://arxiv.org/abs/2411.10212)|**[link](https://github.com/NAVER-INTEL-Co-Lab/gaudi-byzantine)**|
|**2024-11-15**|**Evidential Federated Learning for Skin Lesion Image Classification**|Rutger Hendrix et.al.|[2411.10071](http://arxiv.org/abs/2411.10071)|null|
|**2024-11-14**|**FedRewind: Rewinding Continual Model Exchange for Decentralized Federated Learning**|Luca Palazzo et.al.|[2411.09842](http://arxiv.org/abs/2411.09842)|null|
|**2024-11-14**|**Towards efficient compression and communication for prototype-based decentralized learning**|Pablo Fernández-Piñeiro et.al.|[2411.09267](http://arxiv.org/abs/2411.09267)|null|
|**2024-11-13**|**SAFELOC: Overcoming Data Poisoning Attacks in Heterogeneous Federated Machine Learning for Indoor Localization**|Akhil Singampalli et.al.|[2411.09055](http://arxiv.org/abs/2411.09055)|null|
|**2024-11-13**|**FedSub: Introducing class-aware Subnetworks Fusion to Enhance Personalized Federated Learning in Ubiquitous Systems**|Mattia Giovanni Campana et.al.|[2411.08699](http://arxiv.org/abs/2411.08699)|null|
|**2024-11-13**|**Time-constrained Federated Learning (FL) in Push-Pull IoT Wireless Access**|Van Phuc Bui et.al.|[2411.08607](http://arxiv.org/abs/2411.08607)|null|
|**2024-11-12**|**On the Convergence of Continual Federated Learning Using Incrementally Aggregated Gradients**|Satish Kumar Keshri et.al.|[2411.07959](http://arxiv.org/abs/2411.07959)|null|
|**2024-11-12**|**A Stochastic Optimization Framework for Private and Fair Learning From Decentralized Data**|Devansh Gupta et.al.|[2411.07889](http://arxiv.org/abs/2411.07889)|**[link](https://github.com/justaguyalways/stochastic-federated-differentially-private-and-fair-learning)**|
|**2024-11-12**|**Federated Learning for Discrete Optimal Transport with Large Population under Incomplete Information**|Navpreet Kaur et.al.|[2411.07841](http://arxiv.org/abs/2411.07841)|null|
|**2024-11-12**|**Efficient Federated Finetuning of Tiny Transformers with Resource-Constrained Devices**|Kilian Pfeiffer et.al.|[2411.07826](http://arxiv.org/abs/2411.07826)|null|
|**2024-11-12**|**Dual-Criterion Model Aggregation in Federated Learning: Balancing Data Quantity and Quality**|Haizhou Zhang et.al.|[2411.07816](http://arxiv.org/abs/2411.07816)|null|
|**2024-11-12**|**Federated Low-Rank Adaptation with Differential Privacy over Wireless Networks**|Tianqu Kang et.al.|[2411.07806](http://arxiv.org/abs/2411.07806)|null|
|**2024-11-12**|**ALANINE: A Novel Decentralized Personalized Federated Learning For Heterogeneous LEO Satellite Constellation**|Liang Zhao et.al.|[2411.07752](http://arxiv.org/abs/2411.07752)|null|
|**2024-11-12**|**Collaborative and Federated Black-box Optimization: A Bayesian Optimization Perspective**|Raed Al Kontar et.al.|[2411.07523](http://arxiv.org/abs/2411.07523)|null|
|**2024-11-11**|**Federated Learning Client Pruning for Noisy Labels**|Mahdi Morafah et.al.|[2411.07391](http://arxiv.org/abs/2411.07391)|**[link](https://github.com/mmorafah/clipfl)**|
|**2024-11-11**|**TempCharBERT: Keystroke Dynamics for Continuous Access Control Based on Pre-trained Language Models**|Matheus Simão et.al.|[2411.07224](http://arxiv.org/abs/2411.07224)|null|
|**2024-11-11**|**Revisiting Ensembling in One-Shot Federated Learning**|Youssef Allouah et.al.|[2411.07182](http://arxiv.org/abs/2411.07182)|**[link](https://github.com/sacs-epfl/fens)**|
|**2024-11-11**|**WassFFed: Wasserstein Fair Federated Learning**|Zhongxuan Han et.al.|[2411.06881](http://arxiv.org/abs/2411.06881)|null|
|**2024-11-11**|**Model Partition and Resource Allocation for Split Learning in Vehicular Edge Networks**|Lu Yu et.al.|[2411.06773](http://arxiv.org/abs/2411.06773)|null|
|**2024-11-11**|**Sketched Adaptive Federated Deep Learning: A Sharp Convergence Analysis**|Zhijie Chen et.al.|[2411.06770](http://arxiv.org/abs/2411.06770)|null|
|**2024-11-11**|**Movable Antenna-Aided Federated Learning with Over-the-Air Aggregation: Joint Optimization of Positioning, Beamforming, and User Selection**|Yang Zhao et.al.|[2411.06721](http://arxiv.org/abs/2411.06721)|null|
|**2024-11-10**|**Using Diffusion Models as Generative Replay in Continual Federated Learning -- What will Happen?**|Yongsheng Mei et.al.|[2411.06618](http://arxiv.org/abs/2411.06618)|null|
|**2024-11-10**|**Protection against Source Inference Attacks in Federated Learning using Unary Encoding and Shuffling**|Andreas Athanasiou et.al.|[2411.06458](http://arxiv.org/abs/2411.06458)|null|
|**2024-11-10**|**Client Contribution Normalization for Enhanced Federated Learning**|Mayank Kumar Kundalwal et.al.|[2411.06352](http://arxiv.org/abs/2411.06352)|null|
|**2024-11-09**|**TinyML NLP Approach for Semantic Wireless Sentiment Classification**|Ahmed Y. Radwan et.al.|[2411.06291](http://arxiv.org/abs/2411.06291)|null|
|**2024-11-08**|**IPMN Risk Assessment under Federated Learning Paradigm**|Hongyi Pan et.al.|[2411.05697](http://arxiv.org/abs/2411.05697)|null|
|**2024-11-08**|**Network EM Algorithm for Gaussian Mixture Model in Decentralized Federated Learning**|Shuyuan Wu et.al.|[2411.05591](http://arxiv.org/abs/2411.05591)|null|
|**2024-11-08**|**QuanCrypt-FL: Quantized Homomorphic Encryption with Pruning for Secure Federated Learning**|Md Jueal Mia et.al.|[2411.05260](http://arxiv.org/abs/2411.05260)|null|
|**2024-11-07**|**DWFL: Enhancing Federated Learning through Dynamic Weighted Averaging**|Prakash Chourasia et.al.|[2411.05173](http://arxiv.org/abs/2411.05173)|null|
|**2024-11-07**|**EPIC: Enhancing Privacy through Iterative Collaboration**|Prakash Chourasia et.al.|[2411.05167](http://arxiv.org/abs/2411.05167)|null|
|**2024-11-07**|**Fed-LDR: Federated Local Data-infused Graph Creation with Node-centric Model Refinement**|Jiechao Gao et.al.|[2411.04936](http://arxiv.org/abs/2411.04936)|null|
|**2024-11-07**|**Personalized Federated Learning for Cross-view Geo-localization**|Christos Anagnostopoulos et.al.|[2411.04692](http://arxiv.org/abs/2411.04692)|null|
|**2024-11-07**|**FedDP: Privacy-preserving method based on federated learning for histopathology image segmentation**|Liangrui Pan et.al.|[2411.04509](http://arxiv.org/abs/2411.04509)|null|
|**2024-11-06**|**Cooperation and Personalization on a Seesaw: Choice-based FL for Safe Cooperation in Wireless Networks**|Han Zhang et.al.|[2411.04159](http://arxiv.org/abs/2411.04159)|null|
|**2024-11-06**|**Fed-EC: Bandwidth-Efficient Clustering-Based Federated Learning For Autonomous Visual Robot Navigation**|Shreya Gummadi et.al.|[2411.04112](http://arxiv.org/abs/2411.04112)|null|
|**2024-11-06**|**Federated mixed effects logistic regression based on one-time shared summary statistics**|Marie Analiz April Limpoco et.al.|[2411.04002](http://arxiv.org/abs/2411.04002)|**[link](https://github.com/lizlimpocouhasselt/Mixed-effects-logistic-regression-from-summary-statistics)**|
|**2024-11-06**|**Towards Resource-Efficient Federated Learning in Industrial IoT for Multivariate Time Series Analysis**|Alexandros Gkillas et.al.|[2411.03996](http://arxiv.org/abs/2411.03996)|null|
|**2024-11-06**|**Act in Collusion: A Persistent Distributed Multi-Target Backdoor in Federated Learning**|Tao Liu et.al.|[2411.03926](http://arxiv.org/abs/2411.03926)|null|
|**2024-11-06**|**FedRISE: Rating Induced Sign Election of Gradients for Byzantine Tolerant Federated Aggregation**|Joseph Geo Benjamin et.al.|[2411.03861](http://arxiv.org/abs/2411.03861)|null|
|**2024-11-06**|**Overcoming label shift in targeted federated learning**|Edvin Listo Zec et.al.|[2411.03799](http://arxiv.org/abs/2411.03799)|null|
|**2024-11-06**|**Optimal Defenses Against Gradient Reconstruction Attacks**|Yuxiao Chen et.al.|[2411.03746](http://arxiv.org/abs/2411.03746)|**[link](https://github.com/cyx78/optimal_defenses_against_gradient_reconstruction_attacks)**|
|**2024-11-06**|**NeurIPS 2023 Competition: Privacy Preserving Federated Learning Document VQA**|Marlon Tobaben et.al.|[2411.03730](http://arxiv.org/abs/2411.03730)|null|
|**2024-11-06**|**Domain Generalization for Cross-Receiver Radio Frequency Fingerprint Identification**|Ying Zhang et.al.|[2411.03636](http://arxiv.org/abs/2411.03636)|null|
|**2024-11-06**|**Towards Personalized Federated Learning via Comprehensive Knowledge Distillation**|Pengju Wang et.al.|[2411.03569](http://arxiv.org/abs/2411.03569)|null|

<p align=right>(<a href=#updated-on-20250131>back to top</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[contributors-url]: https://github.com/Vincentqyw/cv-arxiv-daily/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[forks-url]: https://github.com/Vincentqyw/cv-arxiv-daily/network/members
[stars-shield]: https://img.shields.io/github/stars/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[stars-url]: https://github.com/Vincentqyw/cv-arxiv-daily/stargazers
[issues-shield]: https://img.shields.io/github/issues/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[issues-url]: https://github.com/Vincentqyw/cv-arxiv-daily/issues

