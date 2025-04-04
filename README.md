[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## Updated on 2025.04.04
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
|**2025-04-03**|**Multi-Mission Tool Bench: Assessing the Robustness of LLM based Agents through Related and Dynamic Missions**|PeiJie Yu et.al.|[2504.02623](http://arxiv.org/abs/2504.02623)|null|大型语言模型（LLM）由于其高级的理解和规划能力，在工具调用代理方面表现出强大的潜力。用户越来越依赖基于LLM的代理通过迭代交互来解决复杂的任务。然而，现有的基准测试主要在单一任务场景中评估代理，未能捕捉到现实世界的复杂性。为了解决这一问题，我们提出了多任务工具基准。在这个基准测试中，每个测试案例包含多个相互关联的任务。这种设计要求代理能够动态适应不断变化的需求。此外，提出的基准测试探索了在固定任务数量内所有可能的任务切换模式。具体来说，我们提出了一种多代理数据生成框架来构建这个基准测试。我们还提出了一种新的方法，使用动态决策树来评估代理决策的准确性和效率。对多样化的开源和闭源LLM进行实验揭示了影响代理鲁棒性的关键因素，并为工具调用领域提供了可操作的见解。|
|**2025-04-02**|**On Simulation-Guided LLM-based Code Generation for Safe Autonomous Driving Software**|Ali Nouri et.al.|[2504.02141](http://arxiv.org/abs/2504.02141)|null|自动驾驶系统（ADS）是一种关键的安全软件系统，负责解释车辆环境并据此做出决策。驾驶环境的无限复杂性，包括不可预见的事件，需要通过迭代的DevOps过程不断改进。然而，DevOps过程本身也很复杂，使得这些改进既耗时又耗费资源。使用大型语言模型（LLM）进行ADS代码生成自动化是解决这一挑战的一个潜在方法。然而，ADS的开发需要严格的验证、确认、评估和鉴定过程，才能在车辆中部署和使用。在这项研究中，我们在工业环境中开发并评估了一个用于自动代码生成和评估的原型，该原型设计了一个包含基于LLM代理、仿真模型和基于规则的反馈生成器的管道。由LLM生成的代码会在仿真模型中针对多个关键交通场景自动评估，并提供评估报告作为反馈给LLM以进行修改或修复错误。我们报告了该原型采用Codellama:34b, DeepSeek (r1:32b 和 Coder:33b), CodeGemma:7b, Mistral:7b, 以及 GPT4 进行自适应巡航控制（ACC）和非监督碰撞规避紧急机动（CAEM）实验的结果。最后，我们通过对两家原始设备制造商（OEM）的11位专家进行访谈研究来评估该工具。|
|**2025-04-02**|**Building Knowledge from Interactions: An LLM-Based Architecture for Adaptive Tutoring and Social Reasoning**|Luca Garello et.al.|[2504.01588](http://arxiv.org/abs/2504.01588)|null|将机器人整合到日常场景中，如辅导或体能训练，需要具备适应性、社交互动性和目标导向性的机器人。虽然大型语言模型在类人交流方面显示出潜力，但其独立使用受到内存限制和上下文不连贯的阻碍。本研究提出了一种多模态、认知启发的框架，以增强基于大型语言模型的自主决策能力，在社交和任务导向的人机交互中发挥作用。具体来说，我们开发了一个基于大型语言模型的机器人教练代理，平衡了社交对话与任务指导以及目标驱动的动力激发。为进一步提高自主性和个性化，我们引入了一种记忆系统，用于选择、存储和检索经验，促进基于跨不同交互构建的知识进行通用推理。初步的人机交互用户研究和合成数据集的离线实验验证了我们的方法，展示了该系统管理复杂交互、自主驱动训练任务以及构建和检索上下文记忆的能力，推动了社会智能机器人的发展。|
|**2025-04-01**|**Catastrophic Forgetting in LLMs: A Comparative Analysis Across Language Tasks**|Naimul Haque et.al.|[2504.01241](http://arxiv.org/abs/2504.01241)|null|大型语言模型（LLMs）在自然语言处理（NLP）方面取得了显著进展，特别是在自然语言理解（NLU）任务中。随着我们朝着由基于LLM的代理自主处理专门任务的代理世界迈进，这些模型需要在不忘记先前学习信息的情况下适应新任务，这是一个被称为灾难性遗忘的挑战。本研究评估了各种开源LLM（特别是参数量小于100亿的模型）在GLUE基准测试中的关键NLU任务上的连续微调性能，包括SST-2、MRPC、CoLA和MNLI。通过采用提示工程和任务特定调整，我们评估并比较了这些模型在学习新任务时保留先前知识的能力。结果表明，像Phi-3.5-mini这样的模型表现出最小的遗忘，并且保持了强大的学习能力，使其非常适合持续学习环境。此外，像Orca-2-7b和Qwen2.5-7B这样的模型在微调后展示了令人印象深刻的学习能力和整体性能。这项工作有助于理解LLM中的灾难性遗忘，并强调了提示工程在优化模型性能以适应持续学习场景中的作用。|
|**2025-04-01**|**Personality-Driven Decision-Making in LLM-Based Autonomous Agents**|Lewis Newsham et.al.|[2504.00727](http://arxiv.org/abs/2504.00727)|null|将大型语言模型（LLMs）嵌入到自主代理中是一个快速发展的领域，它能够实现动态、可配置的行为，而无需进行广泛的特定领域训练。在我们之前的工作中，我们介绍了SANDMAN，这是一种利用五因素OCEAN人格模型的欺骗性代理架构，展示了人格诱导显著影响代理任务规划。基于这些发现，本研究提出了一种新颖的方法来衡量和评估诱导的人格特质如何影响基于LLM的代理的任务选择过程——特别是规划、调度和决策。我们的结果揭示了与诱导的OCEAN属性相一致的不同任务选择模式，强调了为积极的网络防御策略设计高度可信的欺骗性代理的可行性。|
|**2025-04-01**|**GraphMaster: Automated Graph Synthesis via LLM Agents in Data-Limited Environments**|Enjun Du et.al.|[2504.00711](http://arxiv.org/abs/2504.00711)|null|基础模型的时代已经彻底改变了人工智能研究，但图基础模型（GFMs）仍然受到大规模图语料库稀缺性的限制。传统的图数据合成技术主要集中在简单的结构操作上，缺乏生成具有有意义文本属性的语义丰富节点的能力：这是实际应用中的一个关键局限。虽然大型语言模型（LLMs）在文本生成方面表现出色，但其直接应用于图合成受到上下文窗口限制、幻觉现象和结构一致性挑战的阻碍。为了解决这些问题，我们引入了GraphMaster，这是第一个专门为数据有限环境设计的多代理框架。GraphMaster协调四个专门的LLM代理（管理器、感知器、增强器和评估器），通过迭代优化来确保语义连贯性和结构完整性。为了严格评估我们的方法，我们创建了六个标准图基准的新数据有限“子”变体，专门用于在现实约束下测试合成能力。此外，我们开发了一种新的可解释性评估框架，结合了人类评估和基于Grassmann流形的原理分析，提供了语义连贯性的定性和定量度量。实验结果表明，GraphMaster在多个数据集上显著优于传统合成方法，为数据稀缺环境下的GFMs发展奠定了坚实的基础。|
|**2025-04-01**|**AgentNet: Decentralized Evolutionary Coordination for LLM-based Multi-Agent Systems**|Yingxuan Yang et.al.|[2504.00587](http://arxiv.org/abs/2504.00587)|null|大型语言模型（LLM）的快速发展推动了多智能体系统的发展，这些系统中多个基于LLM的智能体协作解决复杂任务。然而，现有的系统主要依赖于集中式协调，这引入了可扩展性瓶颈，限制了适应性，并且产生了单点故障。此外，隐私和专有知识共享方面的担忧阻碍了跨组织合作，导致专业知识孤立。为了解决这些挑战，我们提出了AgentNet，这是一个去中心化的、基于检索增强生成（RAG）的框架，它使基于LLM的智能体能够在有向无环图（DAG）结构的网络中自主进化其能力和高效协作。与依赖静态角色分配或集中控制的传统多智能体系统不同，AgentNet允许智能体动态专业化，调整其连接性，并在不依赖预定义工作流的情况下路由任务。AgentNet的核心设计基于几个关键创新：(1) 完全去中心化范式：移除中央协调器，允许智能体自主协调和专业化，促进容错性和集体智能的涌现。(2) 动态演变的图拓扑：根据任务需求实时调整智能体之间的连接，确保可扩展性和韧性。(3) 适应性学习以精炼专业技能：一种基于检索的记忆系统，使智能体能够持续更新和完善其专业技能。通过消除集中控制，AgentNet增强了容错性，促进了可扩展的专业化，并实现了跨组织的隐私保护合作。通过去中心化协调和最小的数据交换，智能体可以利用多样化的知识来源，同时保护敏感信息。|
|**2025-04-01**|**Automated detection of atomicity violations in large-scale systems**|Hang He et.al.|[2504.00521](http://arxiv.org/abs/2504.00521)|null|在中断驱动的程序中，原子性违规对关键系统中的软件安全构成了重大威胁。这些违规行为发生在异步中断打乱了对共享资源的操作执行顺序时。由于庞大的程序状态空间、应用程序级代码依赖关系以及复杂的领域特定知识，检测原子性违规非常具有挑战性。我们提出了Clover，这是一种混合框架，它结合了静态分析和大型语言模型（LLM）代理来检测现实世界程序中的原子性违规。Clover首先进行静态分析以提取关键代码片段和操作信息。然后启动一个多代理过程，其中专家代理利用领域特定的知识来检测原子性违规，随后由裁判代理进行验证。在RaceBench 2.1、SV-COMP和RWIP上的评估表明，Clover达到了92.3%的精确度/86.6%的召回率，在F1分数上比现有方法提高了27.4-118.2%。|
|**2025-04-01**|**When Persuasion Overrides Truth in Multi-Agent LLM Debates: Introducing a Confidence-Weighted Persuasion Override Rate (CW-POR)**|Mahak Agarwal et.al.|[2504.00374](http://arxiv.org/abs/2504.00374)|null|在许多现实场景中，单一的大型语言模型（LLM）可能会遇到一些相互矛盾的说法——有些是准确的，有些则是明显错误的——并且必须判断哪个是真的。我们在一个单轮、多代理辩论框架中研究了这种风险：一个基于LLM的代理提供来自TruthfulQA的真实答案，另一个则极力辩护一个错误的观点，而同一个LLM架构充当裁判。我们引入了信心加权说服力覆盖率（CW-POR），它不仅捕捉到裁判被误导的频率，还捕捉到它对错误选择的信任程度。我们在五个开源LLM（3B-14B参数）上进行实验，系统地改变代理的冗长程度（30-300词），发现即使是较小的模型也能构造出具有说服力的论点，从而覆盖真实答案——通常带有高度的信心。这些发现强调了稳健校准和对抗性测试的重要性，以防止LLM自信地支持错误信息。|
|**2025-03-31**|**Large Language Models in Numberland: A Quick Test of Their Numerical Reasoning Abilities**|Roussel Rahman et.al.|[2504.00226](http://arxiv.org/abs/2504.00226)|null|人类数学推理的一个基本要素是我们的数感——对数字及其关系的抽象理解——这使我们能够使用有限的计算资源解决涉及大量数字空间的问题。大型语言模型（LLMs）的数学推理能力通常在高级问题上进行测试（如奥林匹克挑战、几何、文字问题和谜题），但其低级数感仍较少被探索。我们引入了“数字乐园”，一个包含100个问题的测试，以评估基于LLM代理的数值推理能力。这些任务包括基本运算、高级计算（例如，指数运算、复数）、质数检查以及24点游戏，旨在测试基础技能及其在解决复杂和不确定问题中的整合应用。我们评估了五个基于LLM的代理：OpenAI的o1和o1-mini、Google Gemini、Microsoft Copilot和Anthropic Claude。它们在前三项允许通过确定性步骤找到解决方案的任务上得分74-95%。而在需要试错搜索的24点游戏中，表现下降到10-73%。我们将最好的24点解题者（o1，准确率为73%）放在25个更难的问题上测试，其得分降至27%，证实了搜索是一个瓶颈。这些结果，加上错误类型，表明LLM的数感较为脆弱，这有些令人惊讶，因为它们在挑战性基准测试中表现出色。LLM数值推理的局限性突显了简单、有针对性测试的作用，以评估并解释LLM的数学技能，确保安全使用。|
|**2025-03-31**|**Get the Agents Drunk: Memory Perturbations in Autonomous Agent-based Recommender Systems**|Shiyi Yang et.al.|[2503.23804](http://arxiv.org/abs/2503.23804)|null|
|**2025-03-30**|**An Analysis of Decoding Methods for LLM-based Agents for Faithful Multi-Hop Question Answering**|Alexander Murphy et.al.|[2503.23415](http://arxiv.org/abs/2503.23415)|null|
|**2025-03-29**|**CodeARC: Benchmarking Reasoning Capabilities of LLM Agents for Inductive Program Synthesis**|Anjiang Wei et.al.|[2503.23145](http://arxiv.org/abs/2503.23145)|null|
|**2025-03-28**|**Understanding Inequality of LLM Fact-Checking over Geographic Regions with Agent and Retrieval models**|Bruno Coelho et.al.|[2503.22877](http://arxiv.org/abs/2503.22877)|null|
|**2025-03-28**|**WorkTeam: Constructing Workflows from Natural Language with Multi-Agents**|Hanchao Liu et.al.|[2503.22473](http://arxiv.org/abs/2503.22473)|null|
|**2025-03-28**|**Evaluating LLM-based Agents for Multi-Turn Conversations: A Survey**|Shengyue Guan et.al.|[2503.22458](http://arxiv.org/abs/2503.22458)|null|
|**2025-03-27**|**Debate-Driven Multi-Agent LLMs for Phishing Email Detection**|Ngoc Tuong Vy Nguyen et.al.|[2503.22038](http://arxiv.org/abs/2503.22038)|null|
|**2025-03-27**|**MemInsight: Autonomous Memory Augmentation for LLM Agents**|Rana Salama et.al.|[2503.21760](http://arxiv.org/abs/2503.21760)|null|
|**2025-03-27**|**GateLens: A Reasoning-Enhanced LLM Agent for Automotive Software Release Analytics**|Arsham Gholamzadeh Khoee et.al.|[2503.21735](http://arxiv.org/abs/2503.21735)|null|
|**2025-03-27**|**debug-gym: A Text-Based Environment for Interactive Debugging**|Xingdi Yuan et.al.|[2503.21557](http://arxiv.org/abs/2503.21557)|null|
|**2025-03-27**|**Large Language Model Agent: A Survey on Methodology, Applications and Challenges**|Junyu Luo et.al.|[2503.21460](http://arxiv.org/abs/2503.21460)|**[link](https://github.com/luo-junyu/awesome-agent-papers)**|
|**2025-03-28**|**EQ-Negotiator: An Emotion-Reasoning LLM Agent in Credit Dialogues**|Yuhan Liu et.al.|[2503.21080](http://arxiv.org/abs/2503.21080)|null|
|**2025-03-26**|**Operating Room Workflow Analysis via Reasoning Segmentation over Digital Twins**|Yiqing Shen et.al.|[2503.21054](http://arxiv.org/abs/2503.21054)|null|
|**2025-03-27**|**Beyond Believability: Accurate Human Behavior Simulation with Fine-Tuned LLMs**|Yuxuan Lu et.al.|[2503.20749](http://arxiv.org/abs/2503.20749)|null|
|**2025-03-25**|**BugCraft: End-to-End Crash Bug Reproduction Using LLM Agents in Minecraft**|Eray Yapağcı et.al.|[2503.20036](http://arxiv.org/abs/2503.20036)|null|
|**2025-03-24**|**A Survey of Large Language Model Agents for Question Answering**|Murong Yue et.al.|[2503.19213](http://arxiv.org/abs/2503.19213)|null|
|**2025-03-24**|**EconEvals: Benchmarks and Litmus Tests for LLM Agents in Unknown Environments**|Sara Fish et.al.|[2503.18825](http://arxiv.org/abs/2503.18825)|null|
|**2025-03-24**|**Defeating Prompt Injections by Design**|Edoardo Debenedetti et.al.|[2503.18813](http://arxiv.org/abs/2503.18813)|null|
|**2025-03-24**|**AgentSpec: Customizable Runtime Enforcement for Safe and Reliable LLM Agents**|Haoyu Wang et.al.|[2503.18666](http://arxiv.org/abs/2503.18666)|null|
|**2025-03-23**|**AgentRxiv: Towards Collaborative Autonomous Research**|Samuel Schmidgall et.al.|[2503.18102](http://arxiv.org/abs/2503.18102)|null|
|**2025-03-23**|**Metaphor-based Jailbreaking Attacks on Text-to-Image Models**|Chenyu Zhang et.al.|[2503.17987](http://arxiv.org/abs/2503.17987)|null|
|**2025-03-23**|**An Empirical Study of the Role of Incompleteness and Ambiguity in Interactions with Large Language Models**|Riya Naik et.al.|[2503.17936](http://arxiv.org/abs/2503.17936)|null|
|**2025-03-22**|**CP-AgentNet: Autonomous and Explainable Communication Protocol Design Using Generative Agents**|Dae Cheol Kwon et.al.|[2503.17850](http://arxiv.org/abs/2503.17850)|null|
|**2025-03-22**|**Can LLMs Automate Fact-Checking Article Writing?**|Dhruv Sahnan et.al.|[2503.17684](http://arxiv.org/abs/2503.17684)|null|
|**2025-03-21**|**Autonomous Radiotherapy Treatment Planning Using DOLA: A Privacy-Preserving, LLM-Based Optimization Agent**|Humza Nusrat et.al.|[2503.17553](http://arxiv.org/abs/2503.17553)|null|
|**2025-03-21**|**CVE-Bench: A Benchmark for AI Agents' Ability to Exploit Real-World Web Application Vulnerabilities**|Yuxuan Zhu et.al.|[2503.17332](http://arxiv.org/abs/2503.17332)|**[link](https://github.com/uiuc-kang-lab/cve-bench)**|
|**2025-03-21**|**A-IDE : Agent-Integrated Denoising Experts**|Uihyun Cho et.al.|[2503.16780](http://arxiv.org/abs/2503.16780)|null|
|**2025-03-20**|**Towards Agentic Recommender Systems in the Era of Multimodal Large Language Models**|Chengkai Huang et.al.|[2503.16734](http://arxiv.org/abs/2503.16734)|null|
|**2025-03-20**|**Survey on Evaluation of LLM-based Agents**|Asaf Yehudai et.al.|[2503.16416](http://arxiv.org/abs/2503.16416)|null|
|**2025-03-20**|**Issue2Test: Generating Reproducing Test Cases from Issue Reports**|Noor Nashid et.al.|[2503.16320](http://arxiv.org/abs/2503.16320)|null|
|**2025-03-20**|**The Lighthouse of Language: Enhancing LLM Agents via Critique-Guided Improvement**|Ruihan Yang et.al.|[2503.16024](http://arxiv.org/abs/2503.16024)|null|
|**2025-03-18**|**Personalized Attacks of Social Engineering in Multi-turn Conversations -- LLM Agents for Simulation and Detection**|Tharindu Kumarage et.al.|[2503.15552](http://arxiv.org/abs/2503.15552)|null|
|**2025-03-19**|**SWEET-RL: Training Multi-Turn LLM Agents on Collaborative Reasoning Tasks**|Yifei Zhou et.al.|[2503.15478](http://arxiv.org/abs/2503.15478)|**[link](https://github.com/facebookresearch/sweet_rl)**|
|**2025-03-19**|**Exploring Large Language Models for Word Games:Who is the Spy?**|Chentian Wei et.al.|[2503.15235](http://arxiv.org/abs/2503.15235)|**[link](https://github.com/ct-wei/who-is-the-spy)**|
|**2025-03-19**|**Aligning Crowd-sourced Human Feedback for Reinforcement Learning on Code Generation by Large Language Models**|Man Fai Wong et.al.|[2503.15129](http://arxiv.org/abs/2503.15129)|null|
|**2025-03-19**|**ChatStitch: Visualizing Through Structures via Surround-View Unsupervised Deep Image Stitching with Collaborative LLM-Agents**|Hao Liang et.al.|[2503.14948](http://arxiv.org/abs/2503.14948)|null|
|**2025-03-18**|**Gricean Norms as a Basis for Effective Collaboration**|Fardin Saad et.al.|[2503.14484](http://arxiv.org/abs/2503.14484)|**[link](https://github.com/fardinsaad/gricean-norms)**|
|**2025-03-18**|**PLAY2PROMPT: Zero-shot Tool Instruction Optimization for LLM Agents via Tool Play**|Wei Fang et.al.|[2503.14432](http://arxiv.org/abs/2503.14432)|null|
|**2025-03-18**|**MANTRA: Enhancing Automated Method-Level Refactoring with Contextual RAG and Multi-Agent LLM Collaboration**|Yisen Xu et.al.|[2503.14340](http://arxiv.org/abs/2503.14340)|null|
|**2025-03-17**|**Why Do Multi-Agent LLM Systems Fail?**|Mert Cemri et.al.|[2503.13657](http://arxiv.org/abs/2503.13657)|**[link](https://github.com/multi-agent-systems-failure-taxonomy/MASFT)**|
|**2025-03-17**|**DAgent: A Relational Database-Driven Data Analysis Report Generation Agent**|Wenyi Xu et.al.|[2503.13269](http://arxiv.org/abs/2503.13269)|null|
|**2025-03-16**|**VeriLA: A Human-Centered Evaluation Framework for Interpretable Verification of LLM Agent Failures**|Yoo Yeon Sung et.al.|[2503.12651](http://arxiv.org/abs/2503.12651)|null|
|**2025-03-16**|**A Survey on the Optimization of Large Language Model-based Agents**|Shangheng Du et.al.|[2503.12434](http://arxiv.org/abs/2503.12434)|null|
|**2025-03-15**|**TFHE-Coder: Evaluating LLM-agentic Fully Homomorphic Encryption Code Generation**|Mayank Kumar et.al.|[2503.12217](http://arxiv.org/abs/2503.12217)|null|
|**2025-03-15**|**Multi-Agent Systems Execute Arbitrary Malicious Code**|Harold Triedman et.al.|[2503.12188](http://arxiv.org/abs/2503.12188)|null|
|**2025-03-15**|**AgentDroid: A Multi-Agent Framework for Detecting Fraudulent Android Applications**|Ruwei Pan et.al.|[2503.12163](http://arxiv.org/abs/2503.12163)|null|
|**2025-03-15**|**Is Multi-Agent Debate (MAD) the Silver Bullet? An Empirical Analysis of MAD in Code Summarization and Translation**|Jina Chun et.al.|[2503.12029](http://arxiv.org/abs/2503.12029)|null|
|**2025-03-18**|**SagaLLM: Context Management, Validation, and Transaction Guarantees for Multi-Agent LLM Planning**|Edward Y. Chang et.al.|[2503.11951](http://arxiv.org/abs/2503.11951)|**[link](https://github.com/genglongling/SagaLLM)**|
|**2025-03-15**|**End-to-End Edge AI Service Provisioning Framework in 6G ORAN**|Yun Tang et.al.|[2503.11933](http://arxiv.org/abs/2503.11933)|null|
|**2025-03-14**|**CoLLMLight: Cooperative Large Language Model Agents for Network-Wide Traffic Signal Control**|Zirui Yuan et.al.|[2503.11739](http://arxiv.org/abs/2503.11739)|**[link](https://github.com/usail-hkust/CoLLMLight)**|
|**2025-03-14**|**Cerebrum (AIOS SDK): A Platform for Agent Development, Deployment, Distribution, and Discovery**|Balaji Rama et.al.|[2503.11444](http://arxiv.org/abs/2503.11444)|**[link](https://github.com/agiresearch/cerebrum)**|
|**2025-03-14**|**API Agents vs. GUI Agents: Divergence and Convergence**|Chaoyun Zhang et.al.|[2503.11069](http://arxiv.org/abs/2503.11069)|null|
|**2025-03-14**|**BannerAgency: Advertising Banner Design with Multimodal LLM Agents**|Heng Wang et.al.|[2503.11060](http://arxiv.org/abs/2503.11060)|null|
|**2025-03-13**|**Teamwork makes the dream work: LLMs-Based Agents for GitHub README.MD Summarization**|Duc S. H. Nguyen et.al.|[2503.10876](http://arxiv.org/abs/2503.10876)|null|
|**2025-03-13**|**Capturing Semantic Flow of ML-based Systems**|Shin Yoo et.al.|[2503.10310](http://arxiv.org/abs/2503.10310)|null|
|**2025-03-13**|**LLM Agents Display Human Biases but Exhibit Distinct Learning Patterns**|Idan Horowitz et.al.|[2503.10248](http://arxiv.org/abs/2503.10248)|null|
|**2025-03-13**|**Advanced Tool Learning and Selection System (ATLASS): A Closed-Loop Framework Using LLM**|Mohd Ariful Haque et.al.|[2503.10071](http://arxiv.org/abs/2503.10071)|null|
|**2025-03-13**|**OR-LLM-Agent: Automating Modeling and Solving of Operations Research Optimization Problem with Reasoning Large Language Model**|Bowen Zhang et.al.|[2503.10009](http://arxiv.org/abs/2503.10009)|**[link](https://github.com/bwz96sco/or_llm_agent)**|
|**2025-03-12**|**A Survey on Trustworthy LLM Agents: Threats and Countermeasures**|Miao Yu et.al.|[2503.09648](http://arxiv.org/abs/2503.09648)|**[link](https://github.com/Ymm-cll/TrustAgent)**|
|**2025-03-12**|**Plan-and-Act: Improving Planning of Agents for Long-Horizon Tasks**|Lutfi Eren Erdogan et.al.|[2503.09572](http://arxiv.org/abs/2503.09572)|null|
|**2025-03-12**|**COLA: A Scalable Multi-Agent Framework For Windows UI Task Automation**|Di Zhao et.al.|[2503.09263](http://arxiv.org/abs/2503.09263)|**[link](https://github.com/alokia/cola-demo)**|
|**2025-03-12**|**LocAgent: Graph-Guided LLM Agents for Code Localization**|Zhaoling Chen et.al.|[2503.09089](http://arxiv.org/abs/2503.09089)|**[link](https://github.com/gersteinlab/locagent)**|
|**2025-03-11**|**ReviewAgents: Bridging the Gap Between Human and AI-Generated Paper Reviews**|Xian Gao et.al.|[2503.08506](http://arxiv.org/abs/2503.08506)|null|
|**2025-03-10**|**DynTaskMAS: A Dynamic Task Graph-driven Framework for Asynchronous and Parallel LLM-based Multi-Agent Systems**|Junwei Yu et.al.|[2503.07675](http://arxiv.org/abs/2503.07675)|null|
|**2025-03-10**|**LLMs syntactically adapt their language use to their conversational partner**|Florian Kandra et.al.|[2503.07457](http://arxiv.org/abs/2503.07457)|null|
|**2025-03-10**|**Experimental Exploration: Investigating Cooperative Interaction Behavior Between Humans and Large Language Model Agents**|Guanxuan Jiang et.al.|[2503.07320](http://arxiv.org/abs/2503.07320)|null|
|**2025-03-10**|**Automated Movie Generation via Multi-Agent CoT Planning**|Weijia Wu et.al.|[2503.07314](http://arxiv.org/abs/2503.07314)|**[link](https://github.com/showlab/movieagent)**|
|**2025-03-10**|**DatawiseAgent: A Notebook-Centric LLM Agent Framework for Automated Data Science**|Ziming You et.al.|[2503.07044](http://arxiv.org/abs/2503.07044)|null|
|**2025-03-10**|**ProjectEval: A Benchmark for Programming Agents Automated Evaluation on Project-Level Code Generation**|Kaiyuan Liu et.al.|[2503.07010](http://arxiv.org/abs/2503.07010)|null|
|**2025-03-10**|**Beyond Code Generation: LLM-supported Exploration of the Program Design Space**|J. D. Zamfirescu-Pereira et.al.|[2503.06911](http://arxiv.org/abs/2503.06911)|null|
|**2025-03-09**|**Exploring LLM Agents for Cleaning Tabular Machine Learning Datasets**|Tommaso Bendinelli et.al.|[2503.06664](http://arxiv.org/abs/2503.06664)|null|
|**2025-03-09**|**Performant LLM Agentic Framework for Conversational AI**|Alex Casella et.al.|[2503.06410](http://arxiv.org/abs/2503.06410)|null|
|**2025-03-08**|**Towards Conversational AI for Disease Management**|Anil Palepu et.al.|[2503.06074](http://arxiv.org/abs/2503.06074)|null|
|**2025-03-08**|**DSGBench: A Diverse Strategic Game Benchmark for Evaluating LLM-based Agents in Complex Decision-Making Environments**|Wenjie Tang et.al.|[2503.06047](http://arxiv.org/abs/2503.06047)|**[link](https://github.com/decibrain-group/dsgbench)**|
|**2025-03-07**|**A Survey of Large Language Model Empowered Agents for Recommendation and Search: Towards Next-Generation Information Retrieval**|Yu Zhang et.al.|[2503.05659](http://arxiv.org/abs/2503.05659)|**[link](https://github.com/tsinghua-fib-lab/llm-agent-for-recommendation-and-search)**|
|**2025-03-07**|**ORANSight-2.0: Foundational LLMs for O-RAN**|Pranshav Gajjar et.al.|[2503.05200](http://arxiv.org/abs/2503.05200)|null|
|**2025-03-06**|**SafeArena: Evaluating the Safety of Autonomous Web Agents**|Ada Defne Tur et.al.|[2503.04957](http://arxiv.org/abs/2503.04957)|null|
|**2025-03-05**|**Cite Before You Speak: Enhancing Context-Response Grounding in E-commerce Conversational LLM-Agents**|Jingying Zeng et.al.|[2503.04830](http://arxiv.org/abs/2503.04830)|null|
|**2025-03-06**|**ToolFuzz -- Automated Agent Tool Testing**|Ivan Milev et.al.|[2503.04479](http://arxiv.org/abs/2503.04479)|null|
|**2025-03-06**|**Measuring temporal effects of agent knowledge by date-controlled tool use**|R. Patrick Xian et.al.|[2503.04188](http://arxiv.org/abs/2503.04188)|null|
|**2025-03-06**|**InterChat: Enhancing Generative Visual Analytics using Multimodal Interactions**|Juntong Chen et.al.|[2503.04110](http://arxiv.org/abs/2503.04110)|null|
|**2025-03-07**|**A Practical Memory Injection Attack against LLM Agents**|Shen Dong et.al.|[2503.03704](http://arxiv.org/abs/2503.03704)|null|
|**2025-03-05**|**Benchmarking LLMs and LLM-based Agents in Practical Vulnerability Detection for Code Repositories**|Alperen Yildiz et.al.|[2503.03586](http://arxiv.org/abs/2503.03586)|null|
|**2025-03-04**|**MPO: Boosting LLM Agents with Meta Plan Optimization**|Weimin Xiong et.al.|[2503.02682](http://arxiv.org/abs/2503.02682)|**[link](https://github.com/weiminxiong/mpo)**|
|**2025-03-04**|**Generator-Assistant Stepwise Rollback Framework for Large Language Model Agent**|Xingzuo Li et.al.|[2503.02519](http://arxiv.org/abs/2503.02519)|**[link](https://github.com/wisper12933/ga-rollback)**|
|**2025-03-04**|**AppAgentX: Evolving GUI Agents as Proficient Smartphone Users**|Wenjia Jiang et.al.|[2503.02268](http://arxiv.org/abs/2503.02268)|null|
|**2025-03-04**|**Haste Makes Waste: Evaluating Planning Abilities of LLMs for Efficient and Feasible Multitasking with Time Constraints Between Actions**|Zirui Wu et.al.|[2503.02238](http://arxiv.org/abs/2503.02238)|**[link](https://github.com/williamzr/recipe2plan)**|
|**2025-03-04**|**ATLaS: Agent Tuning via Learning Critical Steps**|Zhixun Chen et.al.|[2503.02197](http://arxiv.org/abs/2503.02197)|null|
|**2025-03-03**|**Persuasion at Play: Understanding Misinformation Dynamics in Demographic-Aware Human-LLM Interactions**|Angana Borah et.al.|[2503.02038](http://arxiv.org/abs/2503.02038)|null|
|**2025-03-03**|**MultiAgentBench: Evaluating the Collaboration and Competition of LLM agents**|Kunlun Zhu et.al.|[2503.01935](http://arxiv.org/abs/2503.01935)|**[link](https://github.com/multiagentbench/marble)**|
|**2025-03-03**|**Can (A)I Change Your Mind?**|Miriam Havin et.al.|[2503.01844](http://arxiv.org/abs/2503.01844)|null|
|**2025-03-03**|**Student engagement in collaborative learning with AI agents in an LLM-empowered learning environment: A cluster analysis**|Zhanxin Hao et.al.|[2503.01694](http://arxiv.org/abs/2503.01694)|null|
|**2025-03-02**|**Evaluating Personalized Tool-Augmented LLMs from the Perspectives of Personalization and Proactivity**|Yupu Hao et.al.|[2503.00771](http://arxiv.org/abs/2503.00771)|**[link](https://github.com/hypasd-art/etapp)**|
|**2025-02-28**|**ARIES: Autonomous Reasoning with LLMs on Interactive Thought Graph Environments**|Pedro Gimenes et.al.|[2502.21208](http://arxiv.org/abs/2502.21208)|null|
|**2025-02-28**|**PASemiQA: Plan-Assisted Agent for Question Answering on Semi-Structured Data with Text and Relational Information**|Hansi Yang et.al.|[2502.21087](http://arxiv.org/abs/2502.21087)|null|
|**2025-02-28**|**The Power of Personality: A Human Simulation Perspective to Investigate Large Language Model Agents**|Yifan Duan et.al.|[2502.20859](http://arxiv.org/abs/2502.20859)|null|
|**2025-02-28**|**Digital Player: Evaluating Large Language Models based Human-like Agent in Games**|Jiawei Wang et.al.|[2502.20807](http://arxiv.org/abs/2502.20807)|**[link](https://github.com/fuxiailab/civagent)**|
|**2025-02-27**|**Collab-Overcooked: Benchmarking and Evaluating Large Language Models as Collaborative Agents**|Haochen Sun et.al.|[2502.20073](http://arxiv.org/abs/2502.20073)|**[link](https://github.com/yusaemeow/collab-overcooked)**|
|**2025-02-27**|**MIND: Towards Immersive Psychological Healing with Multi-agent Inner Dialogue**|Yujia Chen et.al.|[2502.19860](http://arxiv.org/abs/2502.19860)|null|
|**2025-02-26**|**Language-Driven Opinion Dynamics in Agent-Based Simulations with LLMs**|Erica Cau et.al.|[2502.19098](http://arxiv.org/abs/2502.19098)|null|
|**2025-02-26**|**Letters from Future Self: Augmenting the Letter-Exchange Exercise with LLM-based Agents to Enhance Young Adults' Career Exploration**|Hayeon Jeon et.al.|[2502.18881](http://arxiv.org/abs/2502.18881)|null|
|**2025-02-26**|**AgentSociety Challenge: Designing LLM Agents for User Modeling and Recommendation on Web Platforms**|Yuwei Yan et.al.|[2502.18754](http://arxiv.org/abs/2502.18754)|**[link](https://github.com/tsinghua-fib-lab/agentsocietychallenge)**|
|**2025-02-25**|**Assistance or Disruption? Exploring and Evaluating the Design and Trade-offs of Proactive AI Programming Support**|Kevin Pu et.al.|[2502.18658](http://arxiv.org/abs/2502.18658)|null|
|**2025-02-25**|**IMPROVE: Iterative Model Pipeline Refinement and Optimization Leveraging LLM Agents**|Eric Xue et.al.|[2502.18530](http://arxiv.org/abs/2502.18530)|null|
|**2025-02-25**|**AgentRM: Enhancing Agent Generalization with Reward Modeling**|Yu Xia et.al.|[2502.18407](http://arxiv.org/abs/2502.18407)|null|
|**2025-02-25**|**RefuteBench 2.0 -- Agentic Benchmark for Dynamic Evaluation of LLM Responses to Refutation Instruction**|Jianhao Yan et.al.|[2502.18308](http://arxiv.org/abs/2502.18308)|null|
|**2025-02-25**|**LAG: LLM agents for Leaderboard Auto Generation on Demanding**|Jian Wu et.al.|[2502.18209](http://arxiv.org/abs/2502.18209)|null|
|**2025-02-25**|**LLM Knows Geometry Better than Algebra: Numerical Understanding of LLM-Based Agents in A Trading Arena**|Tianmi Ma et.al.|[2502.17967](http://arxiv.org/abs/2502.17967)|**[link](https://github.com/wekjsdvnm/agent-trading-arena)**|
|**2025-02-25**|**Towards Enhanced Immersion and Agency for LLM-based Interactive Drama**|Hongqiu Wu et.al.|[2502.17878](http://arxiv.org/abs/2502.17878)|**[link](https://github.com/gingasan/interactive-drama)**|
|**2025-02-24**|**Aligning Compound AI Systems via System-level DPO**|Xiangwen Wang et.al.|[2502.17721](http://arxiv.org/abs/2502.17721)|null|
|**2025-02-24**|**A Multi-LLM-Agent-Based Framework for Economic and Public Policy Analysis**|Yuzhi Hao et.al.|[2502.16879](http://arxiv.org/abs/2502.16879)|null|
|**2025-02-24**|**Grounded Persuasive Language Generation for Automated Marketing**|Jibang Wu et.al.|[2502.16810](http://arxiv.org/abs/2502.16810)|null|
|**2025-02-24**|**Multi-Agent Autonomous Driving Systems with Large Language Models: A Survey of Recent Advances**|Yaozu Wu et.al.|[2502.16804](http://arxiv.org/abs/2502.16804)|null|
|**2025-02-24**|**AlphaAgent: LLM-Driven Alpha Mining with Regularized Exploration to Counteract Alpha Decay**|Ziyi Tang et.al.|[2502.16789](http://arxiv.org/abs/2502.16789)|null|
|**2025-02-23**|**Guardians of the Agentic System: Preventing Many Shots Jailbreak with Agentic System**|Saikat Barua et.al.|[2502.16750](http://arxiv.org/abs/2502.16750)|**[link](https://github.com/GitsSaikat/Guardians-Preventing-Jail-Break-Prompts)**|
|**2025-02-23**|**RapidPen: Fully Automated IP-to-Shell Penetration Testing with LLM-based Agents**|Sho Nakatani et.al.|[2502.16730](http://arxiv.org/abs/2502.16730)|null|
|**2025-02-23**|**BioMaze: Benchmarking and Enhancing Large Language Models for Biological Pathway Reasoning**|Haiteng Zhao et.al.|[2502.16660](http://arxiv.org/abs/2502.16660)|**[link](https://github.com/zhao-ht/biomaze)**|
|**2025-02-21**|**Position: Standard Benchmarks Fail -- LLM Agents Present Overlooked Risks for Financial Applications**|Zichen Chen et.al.|[2502.15865](http://arxiv.org/abs/2502.15865)|null|
|**2025-02-21**|**WorldCraft: Photo-Realistic 3D World Creation and Customization via LLM Agents**|Xinhang Liu et.al.|[2502.15601](http://arxiv.org/abs/2502.15601)|null|
|**2025-02-21**|**Construction and Evaluation of LLM-based agents for Semi-Autonomous penetration testing**|Masaya Kobayashi et.al.|[2502.15506](http://arxiv.org/abs/2502.15506)|null|
|**2025-02-21**|**Textual-to-Visual Iterative Self-Verification for Slide Generation**|Yunqing Xu et.al.|[2502.15412](http://arxiv.org/abs/2502.15412)|null|
|**2025-02-21**|**ARS: Automatic Routing Solver with Large Language Models**|Kai Li et.al.|[2502.15359](http://arxiv.org/abs/2502.15359)|**[link](https://github.com/Ahalikai/ARS-Routbench)**|
|**2025-02-21**|**Auto-Bench: An Automated Benchmark for Scientific Discovery in LLMs**|Tingting Chen et.al.|[2502.15224](http://arxiv.org/abs/2502.15224)|null|
|**2025-02-20**|**Is Safety Standard Same for Everyone? User-Specific Safety Evaluation of Large Language Models**|Yeonjun In et.al.|[2502.15086](http://arxiv.org/abs/2502.15086)|**[link](https://github.com/yeonjun-in/u-safebench)**|
|**2025-02-21**|**I-MCTS: Enhancing Agentic AutoML via Introspective Monte Carlo Tree Search**|Zujie Liang et.al.|[2502.14693](http://arxiv.org/abs/2502.14693)|null|
|**2025-02-20**|**InstructAgent: Building User Controllable Recommender via LLM Agent**|Wujiang Xu et.al.|[2502.14662](http://arxiv.org/abs/2502.14662)|**[link](https://github.com/wujiangxu/iagent)**|
|**2025-02-20**|**Plan-over-Graph: Towards Parallelable LLM Agent Schedule**|Shiqi Zhang et.al.|[2502.14563](http://arxiv.org/abs/2502.14563)|**[link](https://github.com/zsq259/plan-over-graph)**|
|**2025-02-20**|**MLGym: A New Framework and Benchmark for Advancing AI Research Agents**|Deepak Nathani et.al.|[2502.14499](http://arxiv.org/abs/2502.14499)|null|
|**2025-02-20**|**Enhancing Language Multi-Agent Learning with Multi-Agent Credit Re-Assignment for Interactive Environment Generalization**|Zhitao He et.al.|[2502.14496](http://arxiv.org/abs/2502.14496)|**[link](https://github.com/THUNLP-MT/CollabUIAgents)**|
|**2025-02-20**|**FlowAgent: Achieving Compliance and Flexibility for Workflow Agents**|Yuchen Shi et.al.|[2502.14345](http://arxiv.org/abs/2502.14345)|**[link](https://github.com/lightblues/flowagent)**|
|**2025-02-20**|**STeCa: Step-level Trajectory Calibration for LLM Agent Learning**|Hanlin Wang et.al.|[2502.14276](http://arxiv.org/abs/2502.14276)|**[link](https://github.com/WangHanLinHenry/STeCa)**|
|**2025-02-19**|**Investigating Non-Transitivity in LLM-as-a-Judge**|Yi Xu et.al.|[2502.14074](http://arxiv.org/abs/2502.14074)|null|
|**2025-02-19**|**Autellix: An Efficient Serving Engine for LLM Agents as General Programs**|Michael Luo et.al.|[2502.13965](http://arxiv.org/abs/2502.13965)|null|
|**2025-02-19**|**DataSciBench: An LLM Agent Benchmark for Data Science**|Dan Zhang et.al.|[2502.13897](http://arxiv.org/abs/2502.13897)|**[link](https://github.com/thudm/datascibench)**|
|**2025-02-19**|**AI Software Engineer: Programming with Trust**|Abhik Roychoudhury et.al.|[2502.13767](http://arxiv.org/abs/2502.13767)|null|
|**2025-02-19**|**An LLM-based Agent for Reliable Docker Environment Configuration**|Ruida Hu et.al.|[2502.13681](http://arxiv.org/abs/2502.13681)|**[link](https://github.com/bytedance/repo2run)**|
|**2025-02-18**|**Demonstrating specification gaming in reasoning models**|Alexander Bondarenko et.al.|[2502.13295](http://arxiv.org/abs/2502.13295)|null|
|**2025-02-18**|**Interactive Agents to Overcome Ambiguity in Software Engineering**|Sanidhya Vijayvargiya et.al.|[2502.13069](http://arxiv.org/abs/2502.13069)|**[link](https://github.com/sani903/interactivesweagents)**|
|**2025-02-18**|**Towards a Design Guideline for RPA Evaluation: A Survey of Large Language Model-Based Role-Playing Agents**|Chaoran Chen et.al.|[2502.13012](http://arxiv.org/abs/2502.13012)|null|
|**2025-02-18**|**Towards more Contextual Agents: An extractor-Generator Optimization Framework**|Mourad Aouini et.al.|[2502.12926](http://arxiv.org/abs/2502.12926)|null|
|**2025-02-18**|**Towards Adaptive Feedback with AI: Comparing the Feedback Quality of LLMs and Teachers on Experimentation Protocols**|Kathrin Seßler et.al.|[2502.12842](http://arxiv.org/abs/2502.12842)|null|
|**2025-02-18**|**DemonAgent: Dynamically Encrypted Multi-Backdoor Implantation Attack on LLM-based Agent**|Pengyu Zhu et.al.|[2502.12575](http://arxiv.org/abs/2502.12575)|**[link](https://github.com/whfelingyu/demonagent)**|
|**2025-02-18**|**UXAgent: An LLM Agent-Based Usability Testing Framework for Web Design**|Yuxuan Lu et.al.|[2502.12561](http://arxiv.org/abs/2502.12561)|**[link](https://github.com/neuhai/uxagent)**|
|**2025-02-18**|**CityEQA: A Hierarchical LLM Agent on Embodied Question Answering Benchmark in City Space**|Yong Zhao et.al.|[2502.12532](http://arxiv.org/abs/2502.12532)|**[link](https://github.com/tsinghua-fib-lab/CityEQA)**|
|**2025-02-18**|**EDGE: Efficient Data Selection for LLM Agents via Guideline Effectiveness**|Yunxiao Zhang et.al.|[2502.12494](http://arxiv.org/abs/2502.12494)|null|
|**2025-02-18**|**EPO: Explicit Policy Optimization for Strategic Reasoning in LLMs via Reinforcement Learning**|Xiaoqian Liu et.al.|[2502.12486](http://arxiv.org/abs/2502.12486)|null|
|**2025-02-18**|**Investigating and Extending Homans' Social Exchange Theory with Large Language Model based Agents**|Lei Wang et.al.|[2502.12450](http://arxiv.org/abs/2502.12450)|**[link](https://github.com/paitesanshi/set)**|
|**2025-02-17**|**HARBOR: Exploring Persona Dynamics in Multi-Agent Competition**|Kenan Jiang et.al.|[2502.12149](http://arxiv.org/abs/2502.12149)|null|
|**2025-02-17**|**Scaling Autonomous Agents via Automatic Reward Modeling And Planning**|Zhenfang Chen et.al.|[2502.12130](http://arxiv.org/abs/2502.12130)|null|
|**2025-02-17**|**A-MEM: Agentic Memory for LLM Agents**|Wujiang Xu et.al.|[2502.12110](http://arxiv.org/abs/2502.12110)|**[link](https://github.com/wujiangxu/agenticmemory)**|
|**2025-02-17**|**Can LLM Agents Maintain a Persona in Discourse?**|Pranav Bhandari et.al.|[2502.11843](http://arxiv.org/abs/2502.11843)|null|
|**2025-02-17**|**LLM Agents Making Agent Tools**|Georg Wölflein et.al.|[2502.11705](http://arxiv.org/abs/2502.11705)|null|
|**2025-02-17**|**Competing LLM Agents in a Non-Cooperative Game of Opinion Polarisation**|Amin Qasmi et.al.|[2502.11649](http://arxiv.org/abs/2502.11649)|null|
|**2025-02-17**|**AGrail: A Lifelong Agent Guardrail with Effective and Adaptive Safety Detection**|Weidi Luo et.al.|[2502.11448](http://arxiv.org/abs/2502.11448)|null|
|**2025-02-17**|**SMART: Self-Aware Agent for Tool Overuse Mitigation**|Cheng Qian et.al.|[2502.11435](http://arxiv.org/abs/2502.11435)|**[link](https://github.com/qiancheng0/open-smartagent)**|
|**2025-02-17**|**\textsc{FLAG-Trader}: Fusion LLM-Agent with Gradient-based Reinforcement Learning for Financial Trading**|Guojun Xiong et.al.|[2502.11433](http://arxiv.org/abs/2502.11433)|null|
|**2025-02-17**|**TimeCAP: Learning to Contextualize, Augment, and Predict Time Series Events with Large Language Model Agents**|Geon Lee et.al.|[2502.11418](http://arxiv.org/abs/2502.11418)|null|
|**2025-02-14**|**Process Reward Models for LLM Agents: Practical Framework and Directions**|Sanjiban Choudhury et.al.|[2502.10325](http://arxiv.org/abs/2502.10325)|**[link](https://github.com/sanjibanc/agent_prm)**|
|**2025-02-14**|**Automated Hypothesis Validation with Agentic Sequential Falsifications**|Kexin Huang et.al.|[2502.09858](http://arxiv.org/abs/2502.09858)|**[link](https://github.com/snap-stanford/POPPER)**|
|**2025-02-13**|**AgentGuard: Repurposing Agentic Orchestrator for Safety Evaluation of Tool Orchestration**|Jizhou Chen et.al.|[2502.09809](http://arxiv.org/abs/2502.09809)|null|
|**2025-02-13**|**MDCrow: Automating Molecular Dynamics Workflows with Large Language Models**|Quintina Campbell et.al.|[2502.09565](http://arxiv.org/abs/2502.09565)|**[link](https://github.com/ur-whitelab/MDCrow)**|
|**2025-02-14**|**RTBAS: Defending LLM Agents Against Prompt Injection and Privacy Leakage**|Peter Yong Zhong et.al.|[2502.08966](http://arxiv.org/abs/2502.08966)|null|
|**2025-02-12**|**If Multi-Agent Debate is the Answer, What is the Question?**|Hangfan Zhang et.al.|[2502.08788](http://arxiv.org/abs/2502.08788)|null|
|**2025-02-12**|**SPeCtrum: A Grounded Framework for Multidimensional Identity Representation in LLM-Based Agent**|Keyeun Lee et.al.|[2502.08599](http://arxiv.org/abs/2502.08599)|**[link](https://github.com/keyeun/spectrum-framework-llm)**|
|**2025-02-12**|**Commercial LLM Agents Are Already Vulnerable to Simple Yet Dangerous Attacks**|Ang Li et.al.|[2502.08586](http://arxiv.org/abs/2502.08586)|null|
|**2025-02-13**|**Faithful, Unfaithful or Ambiguous? Multi-Agent Debate with Initial Stance for Summary Evaluation**|Mahnaz Koupaee et.al.|[2502.08514](http://arxiv.org/abs/2502.08514)|**[link](https://github.com/amazon-science/madisse)**|
|**2025-02-11**|**Symbiotic Cooperation for Web Agents: Harnessing Complementary Strengths of Large and Small LLMs**|Ruichen Zhang et.al.|[2502.07942](http://arxiv.org/abs/2502.07942)|null|
|**2025-02-12**|**MAGELLAN: Metacognitive predictions of learning progress guide autotelic LLM agents in large goal spaces**|Loris Gaven et.al.|[2502.07709](http://arxiv.org/abs/2502.07709)|**[link](https://github.com/LorisGaven/MAGELLAN)**|
|**2025-02-11**|**Approximating Human Strategic Reasoning with LLM-Enhanced Recursive Reasoners Leveraging Multi-agent Hypergames**|Vince Trencsenyi et.al.|[2502.07443](http://arxiv.org/abs/2502.07443)|null|
|**2025-02-11**|**Graph RAG-Tool Fusion**|Elias Lumer et.al.|[2502.07223](http://arxiv.org/abs/2502.07223)|**[link](https://github.com/eliaslumer/graph-rag-tool-fusion-toollinkos)**|
|**2025-02-11**|**Don't Just Demo, Teach Me the Principles: A Principle-Based Multi-Agent Prompting Strategy for Text Classification**|Peipei Wei et.al.|[2502.07165](http://arxiv.org/abs/2502.07165)|null|
|**2025-02-10**|**Interactive Data Harmonization with LLM Agents**|Aécio Santos et.al.|[2502.07132](http://arxiv.org/abs/2502.07132)|null|
|**2025-02-10**|**Repository-level Code Search with Neural Retrieval Methods**|Siddharth Gandhi et.al.|[2502.07067](http://arxiv.org/abs/2502.07067)|**[link](https://github.com/Siddharth-Gandhi/ds)**|
|**2025-02-10**|**SyncMind: Measuring Agent Out-of-Sync Recovery in Collaborative Software Engineering**|Xuehang Guo et.al.|[2502.06994](http://arxiv.org/abs/2502.06994)|null|
|**2025-02-10**|**Position: Episodic Memory is the Missing Piece for Long-Term LLM Agents**|Mathis Pink et.al.|[2502.06975](http://arxiv.org/abs/2502.06975)|null|
|**2025-02-10**|**Visual Agentic AI for Spatial Reasoning with a Dynamic API**|Damiano Marsili et.al.|[2502.06787](http://arxiv.org/abs/2502.06787)|null|
|**2025-02-10**|**Towards Internet-Scale Training For Agents**|Brandon Trabucco et.al.|[2502.06776](http://arxiv.org/abs/2502.06776)|null|
|**2025-02-10**|**Hephaestus: Improving Fundamental Agent Capabilities of Large Language Models through Continual Pre-Training**|Yuchen Zhuang et.al.|[2502.06589](http://arxiv.org/abs/2502.06589)|null|
|**2025-02-10**|**CSR-Bench: Benchmarking LLM Agents in Deployment of Computer Science Research Repositories**|Yijia Xiao et.al.|[2502.06111](http://arxiv.org/abs/2502.06111)|null|
|**2025-02-09**|**HamRaz: A Culture-Based Persian Conversation Dataset for Person-Centered Therapy Using LLM Agents**|Mohammad Amin Abbasi et.al.|[2502.05982](http://arxiv.org/abs/2502.05982)|null|
|**2025-02-09**|**MetaChain: A Fully-Automated and Zero-Code Framework for LLM Agents**|Jiabin Tang et.al.|[2502.05957](http://arxiv.org/abs/2502.05957)|null|
|**2025-02-07**|**MELON: Indirect Prompt Injection Defense via Masked Re-execution and Tool Comparison**|Kaijie Zhu et.al.|[2502.05174](http://arxiv.org/abs/2502.05174)|null|
|**2025-02-07**|**Learning Strategic Language Agents in the Werewolf Game with Iterative Latent Space Policy Optimization**|Zelai Xu et.al.|[2502.04686](http://arxiv.org/abs/2502.04686)|null|
|**2025-02-07**|**Self-Regulation and Requesting Interventions**|So Yeon Min et.al.|[2502.04576](http://arxiv.org/abs/2502.04576)|null|
|**2025-02-06**|**Multi-Agent Reinforcement Learning with Focal Diversity Optimization**|Selim Furkan Tekin et.al.|[2502.04492](http://arxiv.org/abs/2502.04492)|**[link](https://github.com/sftekin/rl-focal)**|
|**2025-02-06**|**Active Task Disambiguation with LLMs**|Katarzyna Kobalczyk et.al.|[2502.04485](http://arxiv.org/abs/2502.04485)|**[link](https://github.com/kasia-kobalczyk/active-task-disambiguation)**|
|**2025-02-04**|**Position: Scaling LLM Agents Requires Asymptotic Analysis with LLM Primitives**|Elliot Meyerson et.al.|[2502.04358](http://arxiv.org/abs/2502.04358)|null|
|**2025-02-06**|**ScoreFlow: Mastering LLM Agent Workflows via Score-based Preference Optimization**|Yinjie Wang et.al.|[2502.04306](http://arxiv.org/abs/2502.04306)|**[link](https://github.com/gen-verse/scoreflow)**|
|**2025-02-06**|**PsyPlay: Personality-Infused Role-Playing Conversational Agents**|Tao Yang et.al.|[2502.03821](http://arxiv.org/abs/2502.03821)|null|
|**2025-02-06**|**MultiQ&A: An Analysis in Measuring Robustness via Automated Crowdsourcing of Question Perturbations and Answers**|Nicole Cho et.al.|[2502.03711](http://arxiv.org/abs/2502.03711)|null|
|**2025-02-05**|**A Schema-Guided Reason-while-Retrieve framework for Reasoning on Scene Graphs with Large-Language-Models (LLMs)**|Yiye Chen et.al.|[2502.03450](http://arxiv.org/abs/2502.03450)|null|
|**2025-02-04**|**Adaptive Self-improvement LLM Agentic System for ML Library Development**|Genghan Zhang et.al.|[2502.02534](http://arxiv.org/abs/2502.02534)|**[link](https://github.com/zhang677/pcl-lite)**|
|**2025-02-03**|**Firewalls to Secure Dynamic LLM Agentic Networks**|Sahar Abdelnabi et.al.|[2502.01822](http://arxiv.org/abs/2502.01822)|null|
|**2025-02-03**|**Position: Towards a Responsible LLM-empowered Multi-Agent Systems**|Jinwei Hu et.al.|[2502.01714](http://arxiv.org/abs/2502.01714)|null|
|**2025-02-03**|**TReMu: Towards Neuro-Symbolic Temporal Reasoning for LLM-Agents with Memory in Multi-Session Dialogues**|Yubin Ge et.al.|[2502.01630](http://arxiv.org/abs/2502.01630)|null|
|**2025-02-04**|**Reinforcement Learning for Long-Horizon Interactive LLM Agents**|Kevin Chen et.al.|[2502.01600](http://arxiv.org/abs/2502.01600)|null|
|**2025-02-03**|**Memento No More: Coaching AI Agents to Master Multiple Tasks via Hints Internalization**|Minttu Alakuijala et.al.|[2502.01562](http://arxiv.org/abs/2502.01562)|null|
|**2025-02-05**|**TwinMarket: A Scalable Behavioral and Social Simulation for Financial Markets**|Yuzhe Yang et.al.|[2502.01506](http://arxiv.org/abs/2502.01506)|**[link](https://github.com/tobyyang7/twinmarket)**|
|**2025-02-03**|**Simulating Rumor Spreading in Social Networks using LLM Agents**|Tianrui Hu et.al.|[2502.01450](http://arxiv.org/abs/2502.01450)|**[link](https://github.com/neerajas-group/rumors-in-multi-agent)**|
|**2025-02-03**|**Plan-Then-Execute: An Empirical Study of User Trust and Team Performance When Using LLM Agents As A Daily Assistant**|Gaole He et.al.|[2502.01390](http://arxiv.org/abs/2502.01390)|**[link](https://github.com/richardhgl/chi2025_plan-then-execute_llmagent)**|
|**2025-02-03**|**ChartCitor: Multi-Agent Framework for Fine-Grained Chart Visual Attribution**|Kanika Goswami et.al.|[2502.00989](http://arxiv.org/abs/2502.00989)|null|
|**2025-01-31**|**Do LLMs Strategically Reveal, Conceal, and Infer Information? A Theoretical and Empirical Analysis in The Chameleon Game**|Mustafa O. Karabag et.al.|[2501.19398](http://arxiv.org/abs/2501.19398)|**[link](https://github.com/mustafakarabag/llmchameleon)**|
|**2025-01-30**|**Leveraging LLM Agents for Automated Optimization Modeling for SASP Problems: A Graph-RAG based Approach**|Tianpeng Pan et.al.|[2501.18320](http://arxiv.org/abs/2501.18320)|null|
|**2025-01-31**|**RepoAudit: An Autonomous LLM-Agent for Repository-Level Code Auditing**|Jinyao Guo et.al.|[2501.18160](http://arxiv.org/abs/2501.18160)|null|
|**2025-01-29**|**Is Conversational XAI All You Need? Human-AI Decision Making With a Conversational XAI Assistant**|Gaole He et.al.|[2501.17546](http://arxiv.org/abs/2501.17546)|**[link](https://github.com/delftcrowd/iui2025_convxai)**|
|**2025-01-28**|**A sketch of an AI control safety case**|Tomek Korbak et.al.|[2501.17315](http://arxiv.org/abs/2501.17315)|null|
|**2025-01-28**|**Large Language Model Critics for Execution-Free Evaluation of Code Changes**|Aashish Yadavally et.al.|[2501.16655](http://arxiv.org/abs/2501.16655)|**[link](https://github.com/amazon-science/code-agent-eval)**|
|**2025-01-27**|**Will Systems of LLM Agents Cooperate: An Investigation into a Social Dilemma**|Richard Willis et.al.|[2501.16173](http://arxiv.org/abs/2501.16173)|**[link](https://github.com/willis-richard/evollm)**|
|**2025-01-27**|**LLM-attacker: Enhancing Closed-loop Adversarial Scenario Generation for Autonomous Driving with Large Language Models**|Yuewen Mei et.al.|[2501.15850](http://arxiv.org/abs/2501.15850)|null|
|**2025-01-25**|**Are Human Interactions Replicable by Generative Agents? A Case Study on Pronoun Usage in Hierarchical Interactions**|Naihao Deng et.al.|[2501.15283](http://arxiv.org/abs/2501.15283)|null|
|**2025-01-24**|**Serving Long-Context LLMs at the Mobile Edge: Test-Time Reinforcement Learning-based Model Caching and Inference Offloading**|Minrui Xu et.al.|[2501.14205](http://arxiv.org/abs/2501.14205)|null|
|**2025-01-24**|**AI Chatbots as Professional Service Agents: Developing a Professional Identity**|Wenwen Li et.al.|[2501.14179](http://arxiv.org/abs/2501.14179)|null|
|**2025-01-23**|**AgentRec: Agent Recommendation Using Sentence Embeddings Aligned to Human Feedback**|Joshua Park et.al.|[2501.13333](http://arxiv.org/abs/2501.13333)|**[link](https://github.com/joshprk/agentrec)**|
|**2025-01-23**|**Hypothesis Generation for Materials Discovery and Design Using Goal-Driven and Constraint-Guided LLM Agents**|Shrinidhi Kumbhar et.al.|[2501.13299](http://arxiv.org/abs/2501.13299)|null|
|**2025-01-21**|**LLM-Agents Driven Automated Simulation Testing and Analysis of small Uncrewed Aerial Systems**|Venkata Sai Aswath Duvvuru et.al.|[2501.11864](http://arxiv.org/abs/2501.11864)|null|
|**2025-01-20**|**Agent-R: Training Language Model Agents to Reflect via Iterative Self-Training**|Siyu Yuan et.al.|[2501.11425](http://arxiv.org/abs/2501.11425)|**[link](https://github.com/bytedance/agent-r)**|
|**2025-01-20**|**Towards Advancing Code Generation with Large Language Models: A Research Roadmap**|Haolin Jin et.al.|[2501.11354](http://arxiv.org/abs/2501.11354)|null|
|**2025-01-20**|**Large Language Model Agents for Radio Map Generation and Wireless Network Planning**|Hongye Quan et.al.|[2501.11283](http://arxiv.org/abs/2501.11283)|null|
|**2025-01-20**|**PlotEdit: Natural Language-Driven Accessible Chart Editing in PDFs via Multimodal LLM Agents**|Kanika Goswami et.al.|[2501.11233](http://arxiv.org/abs/2501.11233)|null|
|**2025-01-18**|**Learn-by-interact: A Data-Centric Framework for Self-Adaptive Agents in Realistic Environments**|Hongjin Su et.al.|[2501.10893](http://arxiv.org/abs/2501.10893)|null|
|**2025-01-18**|**ML-SceGen: A Multi-level Scenario Generation Framework**|Yicheng Xiao et.al.|[2501.10782](http://arxiv.org/abs/2501.10782)|null|
|**2025-01-17**|**PaSa: An LLM Agent for Comprehensive Academic Paper Search**|Yichen He et.al.|[2501.10120](http://arxiv.org/abs/2501.10120)|**[link](https://github.com/bytedance/pasa)**|
|**2025-01-17**|**A Survey on LLM Test-Time Compute via Search: Tasks, LLM Profiling, Search Algorithms, and Relevant Frameworks**|Xinzhe Li et.al.|[2501.10069](http://arxiv.org/abs/2501.10069)|**[link](https://github.com/xinzhel/llm-agent-survey)**|
|**2025-01-15**|**Leveraging LLM Agents for Translating Network Configurations**|Yunze Wei et.al.|[2501.08760](http://arxiv.org/abs/2501.08760)|null|
|**2025-01-14**|**Addressing the sustainable AI trilemma: a case study on LLM agents and RAG**|Hui Wu et.al.|[2501.08262](http://arxiv.org/abs/2501.08262)|null|
|**2025-01-14**|**Flow: A Modular Approach to Automated Agentic Workflow Generation**|Boye Niu et.al.|[2501.07834](http://arxiv.org/abs/2501.07834)|**[link](https://github.com/tmllab/2025_iclr_flow)**|
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
|**2024-12-30**|**Aviary: training language agents on challenging scientific tasks**|Siddharth Narayanan et.al.|[2412.21154](http://arxiv.org/abs/2412.21154)|**[link](https://github.com/future-house/paper-qa)**|
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

<p align=right>(<a href=#updated-on-20250404>back to top</a>)</p>

## llm

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-04-03**|**Sparse Autoencoders Learn Monosemantic Features in Vision-Language Models**|Mateusz Pach et.al.|[2504.02821](http://arxiv.org/abs/2504.02821)|null|稀疏自动编码器（SAEs）最近被证明可以增强大型语言模型（LLMs）的可解释性和可控性。在这项工作中，我们将SAEs的应用扩展到视觉-语言模型（VLMs），如CLIP，并引入了一个全面的框架来评估视觉表示中的单义性。我们的实验结果表明，在VLMs上训练的SAEs显著增强了单个神经元的单义性，同时展现出与专家定义结构（例如iNaturalist分类法）高度一致的层次化表示。最值得注意的是，我们展示了通过应用SAEs对CLIP视觉编码器进行干预可以直接控制多模态LLMs（例如LLaVA）的输出，而无需对底层模型进行任何修改。这些发现强调了SAEs作为一种无监督方法在提高VLMs的可解释性和可控性方面的实用性和有效性。|
|**2025-04-03**|**Generative Evaluation of Complex Reasoning in Large Language Models**|Haowei Lin et.al.|[2504.02810](http://arxiv.org/abs/2504.02810)|null|随着强大的大型语言模型（LLMs）展现出超越人类的推理能力，一个关键问题随之产生：LLMs是否真正地进行推理，还是仅仅从其庞大的、基于网络抓取的训练数据集中回忆答案？一旦公开发布的基准测试被纳入后续LLM的训练集，这些基准测试作为可靠评估工具的有效性就会受到削弱。为了解决这一问题，我们引入了KUMO，这是一个专为评估LLMs推理能力而设计的生成式评估框架。KUMO将LLMs与符号引擎结合，动态生成多样化的多轮次推理任务，这些任务部分可观察且难度可调。通过自动化流程，KUMO持续在开放式领域中生成新颖的任务，促使模型展示出真正的泛化能力而非仅仅是记忆。我们在由KUMO创建的100个领域内的5000项任务上评估了23种最先进LLMs的表现，并将其推理能力与大学生的表现进行了对比。研究发现表明，许多LLMs在简单的推理任务上已经超过了大学水平的表现，而在复杂的推理挑战中，经过推理优化的LLMs达到了大学水平的表现。此外，LLMs在KUMO任务上的表现与新发布的现实世界推理基准测试结果高度相关，这突显了KUMO作为评估LLMs真实推理能力的强大且持久工具的价值。|
|**2025-04-03**|**MegaMath: Pushing the Limits of Open Math Corpora**|Fan Zhou et.al.|[2504.02807](http://arxiv.org/abs/2504.02807)|null|数学推理是人类智能的基石，也是大型语言模型（LLMs）高级能力的关键基准。然而，研究界仍然缺乏一个开放的、大规模的、高质量的语料库，以满足以数学为中心的LLM预训练需求。我们提出了MegaMath，这是一个从多样化、以数学为重点的来源中精心策划的开放数据集，通过以下实践：(1) 重新审视网络数据：我们使用面向数学的HTML优化、基于fasttext的过滤和去重技术，重新从Common Crawl中提取数学文档，以获取互联网上的更高质量数据。(2) 回顾与数学相关的代码数据：我们从大型代码训练语料库Stack-V2中识别出高质量的与数学相关的代码，进一步增强了数据多样性。(3) 探索合成数据：我们从网络数据或代码数据中合成了问答风格的文本、与数学相关的代码以及文本-代码交织块。通过整合这些策略并通过广泛的消融实验验证其有效性，MegaMath提供了3710亿个令牌，在现有开放数学预训练数据集中数量最大且质量最高。|
|**2025-04-03**|**A Survey of Large Language Models in Mental Health Disorder Detection on Social Media**|Zhuohan Ge et.al.|[2504.02800](http://arxiv.org/abs/2504.02800)|null|精神健康问题的检测与干预是全球研究的重点领域，社交媒体数据已被认为是精神健康研究的重要资源。然而，如何利用大型语言模型（LLM）在社交媒体上进行精神健康问题检测面临着重大挑战。因此，本文旨在探索LLM在社交媒体数据分析中的应用潜力，不仅关注最常见的心理障碍如抑郁症和焦虑症，还涵盖精神病性障碍和外化障碍，从不同维度总结了LLM的应用方法，例如文本数据分析和精神障碍检测，并揭示了当前研究的主要挑战和不足。此外，本文还概述了流行的数据库及评估指标。本论文综述为精神健康领域的研究人员提供了一个全面的参考框架，同时展示了LLM在精神健康检测方面的巨大潜力，以促进未来LLM在精神健康干预中的进一步应用。|
|**2025-04-03**|**A Framework for Robust Cognitive Evaluation of LLMs**|Karin de Langis et.al.|[2504.02789](http://arxiv.org/abs/2504.02789)|null|大型语言模型（LLMs）中出现的认知能力已被广泛观察到，但其本质和潜在机制仍不甚明了。越来越多的研究借鉴认知科学来探究LLM的认知，但标准的方法论和实验流程尚未建立。为解决这一空白，我们开发了CognitivEval框架，系统地评估LLM的人工认知能力，特别强调响应收集的稳健性。CognitivEval的关键特性包括：(i) 自动提示变体生成，以及 (ii) 收集生成内容和模型概率估计值的测试。我们的实验表明，这些特性导致了更稳健的实验结果。通过使用CognitivEval，我们复现了认知科学中的五个经典实验，展示了该框架在各种实验任务中的通用性，并获得了几种最先进LLM的认知特征。CognitivEval将公开发布，以促进认知科学社区内的更广泛合作。|
|**2025-04-03**|**From Consumption to Collaboration: Measuring Interaction Patterns to Augment Human Cognition in Open-Ended Tasks**|Joshua Holstein et.al.|[2504.02780](http://arxiv.org/abs/2504.02780)|null|生成式人工智能，尤其是大型语言模型（LLMs）的兴起，正在从根本上改变知识工作中的认知过程，引发了关于它们对人类推理和问题解决能力影响的关键问题。随着这些AI系统越来越多地融入工作流程，它们为增强人类思维提供了前所未有的机会，同时也因为被动接受生成的答案而存在认知退化的风险。这种紧张关系在开放式任务中尤为明显，这些任务的有效解决方案需要深入的情境化和领域知识的整合。与具有既定指标的结构化任务不同，由于缺乏基准答案以及解决方案开发的迭代性质，在此类开放式任务中衡量人机交互的质量面临着重大挑战。为了解决这一问题，我们提出了一种框架，该框架沿着两个维度分析交互模式：认知活动模式（探索与利用）和认知参与模式（建设性与破坏性）。此框架提供了系统的测量方法，以评估何时LLMs是有效的思考工具而非替代人类认知，从而推进了理论理解和实践指导，旨在开发既能保护又能增强人类认知能力的AI系统。|
|**2025-04-03**|**BT-ACTION: A Test-Driven Approach for Modular Understanding of User Instruction Leveraging Behaviour Trees and LLMs**|Alexander Leszczynski et.al.|[2504.02779](http://arxiv.org/abs/2504.02779)|null|自然语言指令通常抽象且复杂，即使对于看似简单的查询，也需要机器人执行多个子任务。例如，当用户要求机器人准备牛油果吐司时，该任务涉及几个连续的步骤。此外，这类指令可能对机器人来说是模糊的或不可行的，或者超出了机器人的现有知识范围。虽然大型语言模型（LLM）提供了强大的语言推理能力来应对这些挑战，但将它们有效地整合到机器人系统中仍然是一个关键问题。为了解决这个问题，我们提出了BT-ACTION，这是一种测试驱动的方法，它结合了行为树（BT）的模块化结构和LLM，以生成连贯的机器人动作序列，从而遵循复杂的用户指令，特别是在厨房辅助场景中准备食谱的情境下。我们在一项包含45名参与者的综合用户研究中评估了BT-ACTION，并将其性能与直接使用LLM提示进行了比较。结果表明，BT-ACTION的模块化设计帮助机器人减少了错误，增加了用户的信任度，参与者明显更偏好利用BT-ACTION的机器人。代码公开在https://github.com/1Eggbert7/BT_LLM。|
|**2025-04-03**|**How Deep Do Large Language Models Internalize Scientific Literature and Citation Practices?**|Andres Algaba et.al.|[2504.02767](http://arxiv.org/abs/2504.02767)|null|科学知识的传播依赖于研究人员如何发现和引用先前的工作。大型语言模型（LLMs）在科学研究过程中的应用为这些引用实践引入了一个新的层面。然而，目前尚不清楚LLMs在多大程度上与人类的引用实践一致、它们在不同领域的表现如何以及可能对引用动态产生何种影响。本文展示了LLMs通过在生成参考文献时持续偏好高引用论文，系统性地强化了引用中的马太效应。尽管存在显著的领域特定差异，这种模式在各个科学领域中都保持不变，这里提到的差异指的是生成参考文献与外部书目数据库中现有记录匹配的比例。通过对GPT-4o为10,000篇论文生成的274,951条参考文献进行分析，我们发现LLM推荐与传统引用模式不同，更倾向于最近的参考文献，这些文献标题较短且作者较少。强调其内容层面的相关性，生成的参考文献在与每篇论文内容的语义一致性方面与真实参考文献相当，并显示出类似的网络效应，同时减少了作者自引。这些发现说明了LLMs如何通过反映和放大已建立的趋势来重塑引用实践并影响科学发现的轨迹。随着LLMs更加深入地融入科学研究过程中，理解它们在塑造科学界如何发现和基于先前工作构建新研究方面的作用变得至关重要。|
|**2025-04-03**|**Enhancing LLM Robustness to Perturbed Instructions: An Empirical Study**|Aryan Agrawal et.al.|[2504.02733](http://arxiv.org/abs/2504.02733)|null|大型语言模型（LLMs）对输入扰动非常敏感，即使是微小的提示变化也可能导致输出显著不同。现有的增强LLM鲁棒性的方法主要集中在扰动数据样本上，而提高对任务级指令扰动的韧性则相对较少被探索。在这项工作中，我们关注任务特定指令中的字符级和词级编辑，这些编辑会显著降低下游性能。我们实验了多种技术来增强LLM的鲁棒性，包括自去噪和表示对齐，测试了不同的模型（Llama 3 和 Flan-T5）、数据集（CoLA, QNLI, SST-2）以及指令（包括任务导向型和角色导向型）。我们发现，平均而言，无论是通过冻结的LLM还是微调后的模型进行自去噪，都能比其他策略（包括更复杂的基线方法如集成和监督方法）实现更高的性能提升。|
|**2025-04-03**|**Why do LLMs attend to the first token?**|Federico Barbero et.al.|[2504.02732](http://arxiv.org/abs/2504.02732)|null|大型语言模型（LLMs）倾向于在序列的第一个标记上进行大量关注，形成了所谓的注意力陷阱。许多研究详细探讨了这一现象，并提出了多种方法来利用或缓解它。注意力陷阱与量化难题、安全问题和流式注意力有关。尽管已有许多研究提供了注意力陷阱发生与否的条件，但一个关键问题仍然没有得到深入解答：为什么LLMs会学习这样的模式，以及它们是如何被使用的？在这项工作中，我们从理论和实验的角度论证，这种机制为LLMs提供了一种避免过度混合的方法，并将其与现有研究中关于信息如何在Transformer中传播的数学分析联系起来。我们进行了实验以验证我们的理论直觉，并展示了上下文长度、深度和数据打包等选择如何影响陷阱行为。我们希望这项研究能够为理解LLMs中的注意力陷阱为何有用提供一个新的实用视角，从而更好地理解训练过程中形成的注意力模式。|
|**2025-04-02**|**Critical Thinking: Which Kinds of Complexity Govern Optimal Reasoning Length?**|Celine Lee et.al.|[2504.01935](http://arxiv.org/abs/2504.01935)|null|
|**2025-04-02**|**Gen-C: Populating Virtual Worlds with Generative Crowds**|Andreas Panayiotou et.al.|[2504.01924](http://arxiv.org/abs/2504.01924)|null|
|**2025-04-03**|**Bridging the Linguistic Divide: A Survey on Leveraging Large Language Models for Machine Translation**|Baban Gain et.al.|[2504.01919](http://arxiv.org/abs/2504.01919)|null|
|**2025-04-02**|**Advancing AI-Scientist Understanding: Making LLM Think Like a Physicist with Interpretable Reasoning**|Yinggan Xu et.al.|[2504.01911](http://arxiv.org/abs/2504.01911)|null|
|**2025-04-02**|**TransientTables: Evaluating LLMs' Reasoning on Temporally Evolving Semi-structured Tables**|Abhilash Shankarampeta et.al.|[2504.01879](http://arxiv.org/abs/2504.01879)|null|
|**2025-04-02**|**From Code Generation to Software Testing: AI Copilot with Context-Based RAG**|Yuchen Wang et.al.|[2504.01866](http://arxiv.org/abs/2504.01866)|null|
|**2025-04-02**|**Cross-Lingual Consistency: A Novel Inference Framework for Advancing Reasoning in Large Language Models**|Zhiwei Yu et.al.|[2504.01857](http://arxiv.org/abs/2504.01857)|null|
|**2025-04-02**|**Code Red! On the Harmfulness of Applying Off-the-shelf Large Language Models to Programming Tasks**|Ali Al-Kaswan et.al.|[2504.01850](http://arxiv.org/abs/2504.01850)|null|
|**2025-04-02**|**LARGE: Legal Retrieval Augmented Generation Evaluation Tool**|Minhu Park et.al.|[2504.01840](http://arxiv.org/abs/2504.01840)|null|
|**2025-04-02**|**YourBench: Easy Custom Evaluation Sets for Everyone**|Sumuk Shashidhar et.al.|[2504.01833](http://arxiv.org/abs/2504.01833)|null|
|**2025-03-31**|**Harnessing the Reasoning Economy: A Survey of Efficient Reasoning for Large Language Models**|Rui Wang et.al.|[2503.24377](http://arxiv.org/abs/2503.24377)|**[link](https://github.com/devoallen/awesome-reasoning-economy-papers)**|
|**2025-03-31**|**Exploring the Effect of Reinforcement Learning on Video Understanding: Insights from SEED-Bench-R1**|Yi Chen et.al.|[2503.24376](http://arxiv.org/abs/2503.24376)|**[link](https://github.com/tencentarc/seed-bench-r1)**|
|**2025-03-31**|**Effectively Controlling Reasoning Models through Thinking Intervention**|Tong Wu et.al.|[2503.24370](http://arxiv.org/abs/2503.24370)|null|
|**2025-03-31**|**ORAL: Prompting Your Large-Scale LoRAs via Conditional Recurrent Diffusion**|Rana Muhammad Shahroz Khan et.al.|[2503.24354](http://arxiv.org/abs/2503.24354)|null|
|**2025-03-31**|**BEATS: Bias Evaluation and Assessment Test Suite for Large Language Models**|Alok Abhishek et.al.|[2503.24310](http://arxiv.org/abs/2503.24310)|null|
|**2025-03-31**|**A Systematic Evaluation of LLM Strategies for Mental Health Text Analysis: Fine-tuning vs. Prompt Engineering vs. RAG**|Arshia Kermani et.al.|[2503.24307](http://arxiv.org/abs/2503.24307)|null|
|**2025-03-31**|**Rec-R1: Bridging Generative Large Language Models and User-Centric Recommendation Systems via Reinforcement Learning**|Jiacheng Lin et.al.|[2503.24289](http://arxiv.org/abs/2503.24289)|**[link](https://github.com/linjc16/Rec-R1)**|
|**2025-03-31**|**Evaluating and Designing Sparse Autoencoders by Approximating Quasi-Orthogonality**|Sewoong Lee et.al.|[2503.24277](http://arxiv.org/abs/2503.24277)|**[link](https://github.com/sewoonglee/top-afa-sae)**|
|**2025-03-31**|**Enhancing Large Language Models (LLMs) for Telecommunications using Knowledge Graphs and Retrieval-Augmented Generation**|Dun Yuan et.al.|[2503.24245](http://arxiv.org/abs/2503.24245)|null|
|**2025-03-31**|**What, How, Where, and How Well? A Survey on Test-Time Scaling in Large Language Models**|Qiyuan Zhang et.al.|[2503.24235](http://arxiv.org/abs/2503.24235)|null|
|**2025-03-28**|**QuestBench: Can LLMs ask the right question to acquire information in reasoning tasks?**|Belinda Z. Li et.al.|[2503.22674](http://arxiv.org/abs/2503.22674)|**[link](https://github.com/google-deepmind/questbench)**|
|**2025-03-28**|**Unicorn: Text-Only Data Synthesis for Vision Language Model Training**|Xiaomin Yu et.al.|[2503.22655](http://arxiv.org/abs/2503.22655)|**[link](https://github.com/yu-xm/unicorn)**|
|**2025-03-28**|**LLM-enabled Instance Model Generation**|Fengjunjie Pan et.al.|[2503.22587](http://arxiv.org/abs/2503.22587)|null|
|**2025-03-28**|**Historical Ink: Exploring Large Language Models for Irony Detection in 19th-Century Spanish**|Kevin Cohen et.al.|[2503.22585](http://arxiv.org/abs/2503.22585)|**[link](https://github.com/historicalink/ironydetection)**|
|**2025-03-28**|**Niyama : Breaking the Silos of LLM Inference Serving**|Kanishk Goel et.al.|[2503.22562](http://arxiv.org/abs/2503.22562)|null|
|**2025-03-28**|**Bridging the Dimensional Chasm: Uncover Layer-wise Dimensional Reduction in Transformers through Token Correlation**|Zhuo-Yang Song et.al.|[2503.22547](http://arxiv.org/abs/2503.22547)|null|
|**2025-03-28**|**Exploiting Mixture-of-Experts Redundancy Unlocks Multimodal Generative Abilities**|Raman Dutt et.al.|[2503.22517](http://arxiv.org/abs/2503.22517)|null|
|**2025-03-28**|**WorkTeam: Constructing Workflows from Natural Language with Multi-Agents**|Hanchao Liu et.al.|[2503.22473](http://arxiv.org/abs/2503.22473)|null|
|**2025-03-28**|**Evaluating LLM-based Agents for Multi-Turn Conversations: A Survey**|Shengyue Guan et.al.|[2503.22458](http://arxiv.org/abs/2503.22458)|null|
|**2025-03-28**|**Entropy-guided sequence weighting for efficient exploration in RL-based LLM fine-tuning**|Abdullah Vanlioglu et.al.|[2503.22456](http://arxiv.org/abs/2503.22456)|null|
|**2025-03-27**|**MemInsight: Autonomous Memory Augmentation for LLM Agents**|Rana Salama et.al.|[2503.21760](http://arxiv.org/abs/2503.21760)|null|
|**2025-03-27**|**GateLens: A Reasoning-Enhanced LLM Agent for Automotive Software Release Analytics**|Arsham Gholamzadeh Khoee et.al.|[2503.21735](http://arxiv.org/abs/2503.21735)|null|
|**2025-03-27**|**Effective Skill Unlearning through Intervention and Abstention**|Yongce Li et.al.|[2503.21730](http://arxiv.org/abs/2503.21730)|**[link](https://github.com/trustworthy-ml-lab/effective_skill_unlearning)**|
|**2025-03-27**|**Collab: Controlled Decoding using Mixture of Agents for LLM Alignment**|Souradip Chakraborty et.al.|[2503.21720](http://arxiv.org/abs/2503.21720)|null|
|**2025-03-27**|**Enhancing Repository-Level Software Repair via Repository-Aware Knowledge Graphs**|Boyang Yang et.al.|[2503.21710](http://arxiv.org/abs/2503.21710)|null|
|**2025-03-27**|**LLM-Gomoku: A Large Language Model-Based System for Strategic Gomoku with Self-Play and Reinforcement Learning**|Hui Wang et.al.|[2503.21683](http://arxiv.org/abs/2503.21683)|null|
|**2025-03-27**|**Evaluating book summaries from internal knowledge in Large Language Models: a cross-model and semantic consistency approach**|Javier Coronado-Blázquez et.al.|[2503.21613](http://arxiv.org/abs/2503.21613)|null|
|**2025-03-27**|**Prompt, Divide, and Conquer: Bypassing Large Language Model Safety Filters via Segmented and Distributed Prompt Processing**|Johan Wahréus et.al.|[2503.21598](http://arxiv.org/abs/2503.21598)|null|
|**2025-03-27**|**Cooking Task Planning using LLM and Verified by Graph Network**|Ryunosuke Takebayashi et.al.|[2503.21564](http://arxiv.org/abs/2503.21564)|null|
|**2025-03-27**|**debug-gym: A Text-Based Environment for Interactive Debugging**|Xingdi Yuan et.al.|[2503.21557](http://arxiv.org/abs/2503.21557)|null|
|**2025-03-26**|**Mobile-MMLU: A Mobile Intelligence Language Understanding Benchmark**|Sondos Mahmoud Bsharat et.al.|[2503.20786](http://arxiv.org/abs/2503.20786)|**[link](https://github.com/vila-lab/mobile-mmlu)**|
|**2025-03-26**|**From Annotation to Adaptation: Metrics, Synthetic Data, and Aspect Extraction for Aspect-Based Sentiment Analysis with Large Language Models**|Nikita Neveditsin et.al.|[2503.20715](http://arxiv.org/abs/2503.20715)|null|
|**2025-03-26**|**TAMA: A Human-AI Collaborative Thematic Analysis Framework Using Multi-Agent LLMs for Clinical Interviews**|Huimin Xu et.al.|[2503.20666](http://arxiv.org/abs/2503.20666)|null|
|**2025-03-26**|**Unlocking Efficient Long-to-Short LLM Reasoning with Model Merging**|Han Wu et.al.|[2503.20641](http://arxiv.org/abs/2503.20641)|**[link](https://github.com/hahahawu/long-to-short-via-model-merging)**|
|**2025-03-26**|**Collaborative Storytelling and LLM: A Linguistic Analysis of Automatically-Generated Role-Playing Game Sessions**|Alessandro Maisto et.al.|[2503.20623](http://arxiv.org/abs/2503.20623)|null|
|**2025-03-26**|**What to Retrieve for Effective Retrieval-Augmented Code Generation? An Empirical Study and Beyond**|Wenchao Gu et.al.|[2503.20589](http://arxiv.org/abs/2503.20589)|null|
|**2025-03-27**|**LLPut: Investigating Large Language Models for Bug Report-Based Input Generation**|Alif Al Hasan et.al.|[2503.20578](http://arxiv.org/abs/2503.20578)|null|
|**2025-03-26**|**Optimizing Case-Based Reasoning System for Functional Test Script Generation with Large Language Models**|Siyuan Guo et.al.|[2503.20576](http://arxiv.org/abs/2503.20576)|null|
|**2025-03-26**|**Low-resource Information Extraction with the European Clinical Case Corpus**|Soumitra Ghosh et.al.|[2503.20568](http://arxiv.org/abs/2503.20568)|null|
|**2025-03-26**|**A Theoretical Framework for Prompt Engineering: Approximating Smooth Functions with Transformer Prompts**|Ryumei Nakada et.al.|[2503.20561](http://arxiv.org/abs/2503.20561)|null|
|**2025-03-25**|**CoLLM: A Large Language Model for Composed Image Retrieval**|Chuong Huynh et.al.|[2503.19910](http://arxiv.org/abs/2503.19910)|**[link](https://github.com/hmchuong/CoLLM)**|
|**2025-03-25**|**CausalRAG: Integrating Causal Graphs into Retrieval-Augmented Generation**|Nengbo Wang et.al.|[2503.19878](http://arxiv.org/abs/2503.19878)|null|
|**2025-03-25**|**Think Twice: Enhancing LLM Reasoning by Scaling Multi-round Test-time Thinking**|Xiaoyu Tian et.al.|[2503.19855](http://arxiv.org/abs/2503.19855)|null|
|**2025-03-25**|**FALCONEye: Finding Answers and Localizing Content in ONE-hour-long videos with multi-modal LLMs**|Carlos Plou et.al.|[2503.19850](http://arxiv.org/abs/2503.19850)|null|
|**2025-03-25**|**A Comparative Analysis of Word Segmentation, Part-of-Speech Tagging, and Named Entity Recognition for Historical Chinese Sources, 1900-1950**|Zhao Fang et.al.|[2503.19844](http://arxiv.org/abs/2503.19844)|null|
|**2025-03-25**|**ORION: A Holistic End-to-End Autonomous Driving Framework by Vision-Language Instructed Action Generation**|Haoyu Fu et.al.|[2503.19755](http://arxiv.org/abs/2503.19755)|null|
|**2025-03-25**|**AdaptiVocab: Enhancing LLM Efficiency in Focused Domains through Lightweight Vocabulary Adaptation**|Itay Nakash et.al.|[2503.19693](http://arxiv.org/abs/2503.19693)|**[link](https://github.com/itay-nakash/AdaptiVocab)**|
|**2025-03-25**|**HausaNLP at SemEval-2025 Task 3: Towards a Fine-Grained Model-Aware Hallucination Detection**|Maryam Bala et.al.|[2503.19650](http://arxiv.org/abs/2503.19650)|null|
|**2025-03-25**|**1.4 Million Open-Source Distilled Reasoning Dataset to Empower Large Language Model Training**|Han Zhao et.al.|[2503.19633](http://arxiv.org/abs/2503.19633)|null|
|**2025-03-25**|**Optimization through In-Context Learning and Iterative LLM Prompting for Nuclear Engineering Design Problems**|M. Rizki Oktavian et.al.|[2503.19620](http://arxiv.org/abs/2503.19620)|null|
|**2025-03-24**|**SlowFast-LLaVA-1.5: A Family of Token-Efficient Video Large Language Models for Long-Form Video Understanding**|Mingze Xu et.al.|[2503.18943](http://arxiv.org/abs/2503.18943)|null|
|**2025-03-24**|**Video-T1: Test-Time Scaling for Video Generation**|Fangfu Liu et.al.|[2503.18942](http://arxiv.org/abs/2503.18942)|null|
|**2025-03-24**|**Exploring Training and Inference Scaling Laws in Generative Retrieval**|Hongru Cai et.al.|[2503.18941](http://arxiv.org/abs/2503.18941)|**[link](https://github.com/HongruCai/SLGR)**|
|**2025-03-24**|**Trajectory Balance with Asynchrony: Decoupling Exploration and Learning for Fast, Scalable LLM Post-Training**|Brian R. Bartoldson et.al.|[2503.18929](http://arxiv.org/abs/2503.18929)|null|
|**2025-03-24**|**xKV: Cross-Layer SVD for KV-Cache Compression**|Chi-Chih Chang et.al.|[2503.18893](http://arxiv.org/abs/2503.18893)|**[link](https://github.com/abdelfattah-lab/xkv)**|
|**2025-03-24**|**AgentDropout: Dynamic Agent Elimination for Token-Efficient and High-Performance LLM-Based Multi-Agent Collaboration**|Zhexuan Wang et.al.|[2503.18891](http://arxiv.org/abs/2503.18891)|**[link](https://github.com/wangzx1219/agentdropout)**|
|**2025-03-24**|**I Have Covered All the Bases Here: Interpreting Reasoning Features in Large Language Models via Sparse Autoencoders**|Andrey Galichin et.al.|[2503.18878](http://arxiv.org/abs/2503.18878)|**[link](https://github.com/airi-institute/sae-reasoning)**|
|**2025-03-24**|**Reimagining Memory Access for LLM Inference: Compression-Aware Memory Controller Design**|Rui Xie et.al.|[2503.18869](http://arxiv.org/abs/2503.18869)|null|
|**2025-03-24**|**Defeating Prompt Injections by Design**|Edoardo Debenedetti et.al.|[2503.18813](http://arxiv.org/abs/2503.18813)|null|
|**2025-03-24**|**Classical Planning with LLM-Generated Heuristics: Challenging the State of the Art with Python Code**|Augusto B. Corrêa et.al.|[2503.18809](http://arxiv.org/abs/2503.18809)|null|
|**2025-03-21**|**Dancing with Critiques: Enhancing LLM Reasoning with Stepwise Natural Language Self-Critique**|Yansi Li et.al.|[2503.17363](http://arxiv.org/abs/2503.17363)|null|
|**2025-03-21**|**OpenVLThinker: An Early Exploration to Complex Vision-Language Reasoning via Iterative Self-Improvement**|Yihe Deng et.al.|[2503.17352](http://arxiv.org/abs/2503.17352)|**[link](https://github.com/yihedeng9/openvlthinker)**|
|**2025-03-21**|**Efficient Intent-Based Filtering for Multi-Party Conversations Using Knowledge Distillation from LLMs**|Reem Gody et.al.|[2503.17336](http://arxiv.org/abs/2503.17336)|null|
|**2025-03-21**|**CVE-Bench: A Benchmark for AI Agents' Ability to Exploit Real-World Web Application Vulnerabilities**|Yuxuan Zhu et.al.|[2503.17332](http://arxiv.org/abs/2503.17332)|**[link](https://github.com/uiuc-kang-lab/cve-bench)**|
|**2025-03-21**|**LLM+MAP: Bimanual Robot Task Planning using Large Language Models and Planning Domain Definition Language**|Kun Chu et.al.|[2503.17309](http://arxiv.org/abs/2503.17309)|**[link](https://github.com/kchu/llm-map)**|
|**2025-03-21**|**Bugdar: AI-Augmented Secure Code Review for GitHub Pull Requests**|John Naulty et.al.|[2503.17302](http://arxiv.org/abs/2503.17302)|null|
|**2025-03-21**|**CASE -- Condition-Aware Sentence Embeddings for Conditional Semantic Textual Similarity Measurement**|Gaifan Zhang et.al.|[2503.17279](http://arxiv.org/abs/2503.17279)|null|
|**2025-03-21**|**SafeMERGE: Preserving Safety Alignment in Fine-Tuned Large Language Models via Selective Layer-Wise Model Merging**|Aladin Djuhera et.al.|[2503.17239](http://arxiv.org/abs/2503.17239)|**[link](https://github.com/aladinD/SafeMERGE)**|
|**2025-03-21**|**FactSelfCheck: Fact-Level Black-Box Hallucination Detection for LLMs**|Albert Sawczyn et.al.|[2503.17229](http://arxiv.org/abs/2503.17229)|null|
|**2025-03-21**|**Automating Adjudication of Cardiovascular Events Using Large Language Models**|Sonish Sivarajkumar et.al.|[2503.17222](http://arxiv.org/abs/2503.17222)|null|
|**2025-03-20**|**Stop Overthinking: A Survey on Efficient Reasoning for Large Language Models**|Yang Sui et.al.|[2503.16419](http://arxiv.org/abs/2503.16419)|**[link](https://github.com/eclipsess/awesome-efficient-reasoning-llms)**|
|**2025-03-20**|**The Emperor's New Clothes in Benchmarking? A Rigorous Examination of Mitigation Strategies for LLM Benchmark Data Contamination**|Yifan Sun et.al.|[2503.16402](http://arxiv.org/abs/2503.16402)|**[link](https://github.com/astral-group/bdc_mitigation_assessment)**|
|**2025-03-20**|**Exploring the Hidden Reasoning Process of Large Language Models by Misleading Them**|Guanyu Chen et.al.|[2503.16401](http://arxiv.org/abs/2503.16401)|null|
|**2025-03-20**|**Deconstructing Long Chain-of-Thought: A Structured Reasoning Optimization Framework for Long CoT Distillation**|Yijia Luo et.al.|[2503.16385](http://arxiv.org/abs/2503.16385)|**[link](https://github.com/elena-luo/SODE)**|
|**2025-03-20**|**LaPIG: Cross-Modal Generation of Paired Thermal and Visible Facial Images**|Leyang Wang et.al.|[2503.16376](http://arxiv.org/abs/2503.16376)|null|
|**2025-03-20**|**CaKE: Circuit-aware Editing Enables Generalizable Knowledge Learners**|Yunzhi Yao et.al.|[2503.16356](http://arxiv.org/abs/2503.16356)|**[link](https://github.com/zjunlp/cake)**|
|**2025-03-20**|**LLM Braces: Straightening Out LLM Predictions with Relevant Sub-Updates**|Ying Shen et.al.|[2503.16334](http://arxiv.org/abs/2503.16334)|null|
|**2025-03-20**|**OmniGeo: Towards a Multimodal Large Language Models for Geospatial Artificial Intelligence**|Long Yuan et.al.|[2503.16326](http://arxiv.org/abs/2503.16326)|null|
|**2025-03-20**|**Bridging Technology and Humanities: Evaluating the Impact of Large Language Models on Social Sciences Research with DeepSeek-R1**|Peiran Gu et.al.|[2503.16304](http://arxiv.org/abs/2503.16304)|null|
|**2025-03-20**|**Reinforcement Learning for Reasoning in Small LLMs: What Works and What Doesn't**|Quy-Anh Dang et.al.|[2503.16219](http://arxiv.org/abs/2503.16219)|**[link](https://github.com/knoveleng/open-rs)**|
|**2025-03-19**|**SWEET-RL: Training Multi-Turn LLM Agents on Collaborative Reasoning Tasks**|Yifei Zhou et.al.|[2503.15478](http://arxiv.org/abs/2503.15478)|**[link](https://github.com/facebookresearch/sweet_rl)**|
|**2025-03-19**|**Cube: A Roblox View of 3D Intelligence**|Foundation AI Team et.al.|[2503.15475](http://arxiv.org/abs/2503.15475)|**[link](https://github.com/roblox/cube)**|
|**2025-03-19**|**From 1,000,000 Users to Every User: Scaling Up Personalized Preference for User-level Alignment**|Jia-Nan Li et.al.|[2503.15463](http://arxiv.org/abs/2503.15463)|**[link](https://github.com/jinaleejnl/alignx)**|
|**2025-03-19**|**Probing the topology of the space of tokens with structured prompts**|Michael Robinson et.al.|[2503.15421](http://arxiv.org/abs/2503.15421)|null|
|**2025-03-19**|**SemEval-2025 Task 1: AdMIRe -- Advancing Multimodal Idiomaticity Representation**|Thomas Pickard et.al.|[2503.15358](http://arxiv.org/abs/2503.15358)|null|
|**2025-03-19**|**TruthLens:A Training-Free Paradigm for DeepFake Detection**|Ritabrata Chakraborty et.al.|[2503.15342](http://arxiv.org/abs/2503.15342)|null|
|**2025-03-19**|**Uncertainty-Guided Chain-of-Thought for Code Generation with LLMs**|Yuqi Zhu et.al.|[2503.15341](http://arxiv.org/abs/2503.15341)|null|
|**2025-03-19**|**Solla: Towards a Speech-Oriented LLM That Hears Acoustic Context**|Junyi Ao et.al.|[2503.15338](http://arxiv.org/abs/2503.15338)|**[link](https://github.com/amphionspace/SA-Eval)**|
|**2025-03-19**|**aiXcoder-7B-v2: Training LLMs to Fully Utilize the Long Context in Repository-level Code Completion**|Jia Li et.al.|[2503.15301](http://arxiv.org/abs/2503.15301)|null|
|**2025-03-19**|**Inside-Out: Hidden Factual Knowledge in LLMs**|Zorik Gekhman et.al.|[2503.15299](http://arxiv.org/abs/2503.15299)|null|
|**2025-03-18**|**Aligning Multimodal LLM with Human Preference: A Survey**|Tao Yu et.al.|[2503.14504](http://arxiv.org/abs/2503.14504)|null|
|**2025-03-18**|**Engineering Scientific Assistants using Interactive Structured Induction of Programs**|Shraddha Surana et.al.|[2503.14488](http://arxiv.org/abs/2503.14488)|null|
|**2025-03-18**|**Gricean Norms as a Basis for Effective Collaboration**|Fardin Saad et.al.|[2503.14484](http://arxiv.org/abs/2503.14484)|**[link](https://github.com/fardinsaad/gricean-norms)**|
|**2025-03-18**|**Creation-MMBench: Assessing Context-Aware Creative Intelligence in MLLM**|Xinyu Fang et.al.|[2503.14478](http://arxiv.org/abs/2503.14478)|**[link](https://github.com/open-compass/creation-mmbench)**|
|**2025-03-18**|**EnvBench: A Benchmark for Automated Environment Setup**|Aleksandra Eliseeva et.al.|[2503.14443](http://arxiv.org/abs/2503.14443)|**[link](https://github.com/JetBrains-Research/EnvBench)**|
|**2025-03-18**|**LLM-FE: Automated Feature Engineering for Tabular Data with LLMs as Evolutionary Optimizers**|Nikhil Abhyankar et.al.|[2503.14434](http://arxiv.org/abs/2503.14434)|**[link](https://github.com/nikhilsab/llmfe)**|
|**2025-03-18**|**PLAY2PROMPT: Zero-shot Tool Instruction Optimization for LLM Agents via Tool Play**|Wei Fang et.al.|[2503.14432](http://arxiv.org/abs/2503.14432)|null|
|**2025-03-18**|**Unifying Text Semantics and Graph Structures for Temporal Text-attributed Graphs with Large Language Models**|Siwei Zhang et.al.|[2503.14411](http://arxiv.org/abs/2503.14411)|null|
|**2025-03-18**|**From "Hallucination" to "Suture": Insights from Language Philosophy to Enhance Large Language Models**|Qiantong Wang et.al.|[2503.14392](http://arxiv.org/abs/2503.14392)|null|
|**2025-03-18**|**How much do LLMs learn from negative examples?**|Shadi Hamdan et.al.|[2503.14391](http://arxiv.org/abs/2503.14391)|null|
|**2025-03-17**|**MetaScale: Test-Time Scaling with Evolving Meta-Thoughts**|Qin Liu et.al.|[2503.13447](http://arxiv.org/abs/2503.13447)|null|
|**2025-03-17**|**Faithfulness of LLM Self-Explanations for Commonsense Tasks: Larger Is Better, and Instruction-Tuning Allows Trade-Offs but Not Pareto Dominance**|Noah Y. Siegel et.al.|[2503.13445](http://arxiv.org/abs/2503.13445)|null|
|**2025-03-17**|**xLSTM 7B: A Recurrent LLM for Fast and Efficient Inference**|Maximilian Beck et.al.|[2503.13427](http://arxiv.org/abs/2503.13427)|**[link](https://github.com/nx-ai/xlstm-jax)**|
|**2025-03-17**|**A Comprehensive Survey on Multi-Agent Cooperative Decision-Making: Scenarios, Approaches, Challenges and Perspectives**|Weiqiang Jin et.al.|[2503.13415](http://arxiv.org/abs/2503.13415)|null|
|**2025-03-18**|**DLPO: Towards a Robust, Efficient, and Generalizable Prompt Optimization Framework from a Deep-Learning Perspective**|Dengyun Peng et.al.|[2503.13413](http://arxiv.org/abs/2503.13413)|**[link](https://github.com/sfasfaffa/dlpo)**|
|**2025-03-17**|**Cream of the Crop: Harvesting Rich, Scalable and Transferable Multi-Modal Data for Instruction Fine-Tuning**|Mengyao Lyu et.al.|[2503.13383](http://arxiv.org/abs/2503.13383)|null|
|**2025-03-17**|**Mitigating Visual Forgetting via Take-along Visual Conditioning for Multi-modal Long CoT Reasoning**|Hai-Long Sun et.al.|[2503.13360](http://arxiv.org/abs/2503.13360)|null|
|**2025-03-17**|**Agents Play Thousands of 3D Video Games**|Zhongwen Xu et.al.|[2503.13356](http://arxiv.org/abs/2503.13356)|null|
|**2025-03-17**|**LearnMate: Enhancing Online Education with LLM-Powered Personalized Learning Plans and Support**|Xinyu Jessica Wang et.al.|[2503.13340](http://arxiv.org/abs/2503.13340)|null|
|**2025-03-17**|**Computation Mechanism Behind LLM Position Generalization**|Chi Han et.al.|[2503.13305](http://arxiv.org/abs/2503.13305)|null|
|**2025-03-14**|**ASMA-Tune: Unlocking LLMs' Assembly Code Comprehension via Structural-Semantic Instruction Tuning**|Xinyi Wang et.al.|[2503.11617](http://arxiv.org/abs/2503.11617)|**[link](https://github.com/wxy3596/asma-tune)**|
|**2025-03-14**|**Broaden your SCOPE! Efficient Multi-turn Conversation Planning for LLMs using Semantic Space**|Zhiliang Chen et.al.|[2503.11586](http://arxiv.org/abs/2503.11586)|**[link](https://github.com/chenzhiliang94/convo-plan-scope)**|
|**2025-03-14**|**Synthesizing Access Control Policies using Large Language Models**|Adarsh Vatsa et.al.|[2503.11573](http://arxiv.org/abs/2503.11573)|null|
|**2025-03-14**|**Implicit Bias-Like Patterns in Reasoning Models**|Messi H. J. Lee et.al.|[2503.11572](http://arxiv.org/abs/2503.11572)|null|
|**2025-03-14**|**Potential of large language model-powered nudges for promoting daily water and energy conservation**|Zonghan Li et.al.|[2503.11531](http://arxiv.org/abs/2503.11531)|null|
|**2025-03-14**|**A Review of DeepSeek Models' Key Innovative Techniques**|Chengen Wang et.al.|[2503.11486](http://arxiv.org/abs/2503.11486)|null|
|**2025-03-14**|**Integrating LLMs in Gamified Systems**|Carlos J. Costa et.al.|[2503.11458](http://arxiv.org/abs/2503.11458)|null|
|**2025-03-14**|**D3: Diversity, Difficulty, and Dependability-Aware Data Selection for Sample-Efficient LLM Instruction Tuning**|Jia Zhang et.al.|[2503.11441](http://arxiv.org/abs/2503.11441)|null|
|**2025-03-14**|**Optimizing Large Language Models for Detecting Symptoms of Comorbid Depression or Anxiety in Chronic Diseases: Insights from Patient Messages**|Jiyeong Kim et.al.|[2503.11384](http://arxiv.org/abs/2503.11384)|null|
|**2025-03-14**|**Modeling Subjectivity in Cognitive Appraisal with Language Models**|Yuxiang Zhou et.al.|[2503.11381](http://arxiv.org/abs/2503.11381)|null|
|**2025-03-13**|**UniGoal: Towards Universal Zero-shot Goal-oriented Navigation**|Hang Yin et.al.|[2503.10630](http://arxiv.org/abs/2503.10630)|null|
|**2025-03-13**|**From TOWER to SPIRE: Adding the Speech Modality to a Text-Only LLM**|Kshitij Ambilduke et.al.|[2503.10620](http://arxiv.org/abs/2503.10620)|**[link](https://github.com/utter-project/SpireLM)**|
|**2025-03-13**|**Siege: Autonomous Multi-Turn Jailbreaking of Large Language Models with Tree Search**|Andy Zhou et.al.|[2503.10619](http://arxiv.org/abs/2503.10619)|null|
|**2025-03-13**|**CoSTA $\ast$ : Cost-Sensitive Toolpath Agent for Multi-turn Image Editing**|Advait Gupta et.al.|[2503.10613](http://arxiv.org/abs/2503.10613)|**[link](https://github.com/tianyi-lab/CoSTAR)**|
|**2025-03-13**|**TruthPrInt: Mitigating LVLM Object Hallucination Via Latent Truthful-Guided Pre-Intervention**|Jinhao Duan et.al.|[2503.10602](http://arxiv.org/abs/2503.10602)|**[link](https://github.com/jinhaoduan/truthprint)**|
|**2025-03-13**|**Unveiling the Mathematical Reasoning in DeepSeek Models: A Comparative Study of Large Language Models**|Afrar Jahin et.al.|[2503.10573](http://arxiv.org/abs/2503.10573)|null|
|**2025-03-13**|**KUDA: Keypoints to Unify Dynamics Learning and Visual Prompting for Open-Vocabulary Robotic Manipulation**|Zixian Liu et.al.|[2503.10546](http://arxiv.org/abs/2503.10546)|null|
|**2025-03-13**|**Probing LLMs for Multilingual Discourse Generalization Through a Unified Label Set**|Florian Eichin et.al.|[2503.10515](http://arxiv.org/abs/2503.10515)|**[link](https://github.com/mainlp/discourse_probes)**|
|**2025-03-13**|**SySLLM: Generating Synthesized Policy Summaries for Reinforcement Learning Agents Using Large Language Models**|Sahar Admoni et.al.|[2503.10509](http://arxiv.org/abs/2503.10509)|null|
|**2025-03-13**|**MMLU-ProX: A Multilingual Benchmark for Advanced Large Language Model Evaluation**|Weihao Xuan et.al.|[2503.10497](http://arxiv.org/abs/2503.10497)|null|
|**2025-03-12**|**MoC: Mixtures of Text Chunking Learners for Retrieval-Augmented Generation System**|Jihao Zhao et.al.|[2503.09600](http://arxiv.org/abs/2503.09600)|**[link](https://github.com/IAAR-Shanghai/Meta-Chunking)**|
|**2025-03-12**|**How to Protect Yourself from 5G Radiation? Investigating LLM Responses to Implicit Misinformation**|Ruohao Guo et.al.|[2503.09598](http://arxiv.org/abs/2503.09598)|**[link](https://github.com/octaviaguo/EchoMist)**|
|**2025-03-12**|**SimLingo: Vision-Only Closed-Loop Autonomous Driving with Language-Action Alignment**|Katrin Renz et.al.|[2503.09594](http://arxiv.org/abs/2503.09594)|null|
|**2025-03-12**|**BIMBA: Selective-Scan Compression for Long-Range Video Question Answering**|Md Mohaiminul Islam et.al.|[2503.09590](http://arxiv.org/abs/2503.09590)|**[link](https://github.com/md-mohaiminul/BIMBA)**|
|**2025-03-12**|**Cost-Optimal Grouped-Query Attention for Long-Context LLMs**|Yingfa Chen et.al.|[2503.09579](http://arxiv.org/abs/2503.09579)|**[link](https://github.com/thunlp/cost-optimal-gqa)**|
|**2025-03-12**|**Plan-and-Act: Improving Planning of Agents for Long-Horizon Tasks**|Lutfi Eren Erdogan et.al.|[2503.09572](http://arxiv.org/abs/2503.09572)|null|
|**2025-03-13**|**Large Language Models for Multi-Facility Location Mechanism Design**|Nguyen Thach et.al.|[2503.09533](http://arxiv.org/abs/2503.09533)|null|
|**2025-03-12**|**Search-R1: Training LLMs to Reason and Leverage Search Engines with Reinforcement Learning**|Bowen Jin et.al.|[2503.09516](http://arxiv.org/abs/2503.09516)|**[link](https://github.com/petergriffinjin/search-r1)**|
|**2025-03-12**|**ReMA: Learning to Meta-think for LLMs with Multi-Agent Reinforcement Learning**|Ziyu Wan et.al.|[2503.09501](http://arxiv.org/abs/2503.09501)|null|
|**2025-03-12**|**BAMBI: Developing Baby Language Models for Italian**|Alice Suozzi et.al.|[2503.09481](http://arxiv.org/abs/2503.09481)|null|
|**2025-03-11**|**Randomness, Not Representation: The Unreliability of Evaluating Cultural Alignment in LLMs**|Ariba Khan et.al.|[2503.08688](http://arxiv.org/abs/2503.08688)|null|
|**2025-03-11**|**Self-Taught Self-Correction for Small Language Models**|Viktor Moskvoretskii et.al.|[2503.08681](http://arxiv.org/abs/2503.08681)|null|
|**2025-03-11**|**Exploring the Word Sense Disambiguation Capabilities of Large Language Models**|Pierpaolo Basile et.al.|[2503.08662](http://arxiv.org/abs/2503.08662)|null|
|**2025-03-11**|**EMMOE: A Comprehensive Benchmark for Embodied Mobile Manipulation in Open Environments**|Dongping Li et.al.|[2503.08604](http://arxiv.org/abs/2503.08604)|null|
|**2025-03-11**|**DeepReview: Improving LLM-based Paper Review with Human-like Deep Thinking Process**|Minjun Zhu et.al.|[2503.08569](http://arxiv.org/abs/2503.08569)|null|
|**2025-03-11**|**Reasoning and Sampling-Augmented MCQ Difficulty Prediction via LLMs**|Wanyong Feng et.al.|[2503.08551](http://arxiv.org/abs/2503.08551)|null|
|**2025-03-11**|**Graph of AI Ideas: Leveraging Knowledge Graphs and LLMs for AI Research Idea Generation**|Xian Gao et.al.|[2503.08549](http://arxiv.org/abs/2503.08549)|null|
|**2025-03-11**|**DAFE: LLM-Based Evaluation Through Dynamic Arbitration for Free-Form Question-Answering**|Sher Badshah et.al.|[2503.08542](http://arxiv.org/abs/2503.08542)|null|
|**2025-03-11**|**Mellow: a small audio language model for reasoning**|Soham Deshmukh et.al.|[2503.08540](http://arxiv.org/abs/2503.08540)|**[link](https://github.com/soham97/mellow)**|
|**2025-03-11**|**Chemical reasoning in LLMs unlocks steerable synthesis planning and reaction mechanism elucidation**|Andres M Bran et.al.|[2503.08537](http://arxiv.org/abs/2503.08537)|**[link](https://github.com/schwallergroup/steer)**|
|**2025-03-10**|**GenAIReading: Augmenting Human Cognition with Interactive Digital Textbooks Using Large Language Models and Image Generation Models**|Ryugo Morita et.al.|[2503.07463](http://arxiv.org/abs/2503.07463)|null|
|**2025-03-10**|**MedAgentsBench: Benchmarking Thinking Models and Agent Frameworks for Complex Medical Reasoning**|Xiangru Tang et.al.|[2503.07459](http://arxiv.org/abs/2503.07459)|**[link](https://github.com/gersteinlab/medagents-benchmark)**|
|**2025-03-10**|**LLMs syntactically adapt their language use to their conversational partner**|Florian Kandra et.al.|[2503.07457](http://arxiv.org/abs/2503.07457)|null|
|**2025-03-10**|**From Idea to Implementation: Evaluating the Influence of Large Language Models in Software Development -- An Opinion Paper**|Sargam Yadav et.al.|[2503.07450](http://arxiv.org/abs/2503.07450)|null|
|**2025-03-10**|**From Text to Visuals: Using LLMs to Generate Math Diagrams with Vector Graphics**|Jaewook Lee et.al.|[2503.07429](http://arxiv.org/abs/2503.07429)|null|
|**2025-03-10**|**RePO: ReLU-based Preference Optimization**|Junkang Wu et.al.|[2503.07426](http://arxiv.org/abs/2503.07426)|**[link](https://github.com/junkangwu/repo)**|
|**2025-03-10**|**Process-Supervised LLM Recommenders via Flow-guided Tuning**|Chongming Gao et.al.|[2503.07377](http://arxiv.org/abs/2503.07377)|**[link](https://github.com/mr-peach0301/flower)**|
|**2025-03-10**|**Assessing the Macro and Micro Effects of Random Seeds on Fine-Tuning Large Language Models**|Hao Zhou et.al.|[2503.07329](http://arxiv.org/abs/2503.07329)|null|
|**2025-03-10**|**Dynamic Path Navigation for Motion Agents with LLM Reasoning**|Yubo Zhao et.al.|[2503.07323](http://arxiv.org/abs/2503.07323)|null|
|**2025-03-10**|**Experimental Exploration: Investigating Cooperative Interaction Behavior Between Humans and Large Language Model Agents**|Guanxuan Jiang et.al.|[2503.07320](http://arxiv.org/abs/2503.07320)|null|
|**2025-03-07**|**A Survey of Large Language Model Empowered Agents for Recommendation and Search: Towards Next-Generation Information Retrieval**|Yu Zhang et.al.|[2503.05659](http://arxiv.org/abs/2503.05659)|**[link](https://github.com/tsinghua-fib-lab/llm-agent-for-recommendation-and-search)**|
|**2025-03-07**|**Learning LLM Preference over Intra-Dialogue Pairs: A Framework for Utterance-level Understandings**|Xuanqing Liu et.al.|[2503.05620](http://arxiv.org/abs/2503.05620)|null|
|**2025-03-07**|**A Survey on Sparse Autoencoders: Interpreting the Internal Mechanisms of Large Language Models**|Dong Shu et.al.|[2503.05613](http://arxiv.org/abs/2503.05613)|null|
|**2025-03-07**|**R1-Searcher: Incentivizing the Search Capability in LLMs via Reinforcement Learning**|Huatong Song et.al.|[2503.05592](http://arxiv.org/abs/2503.05592)|null|
|**2025-03-07**|**Evaluating open-source Large Language Models for automated fact-checking**|Nicolo' Fontana et.al.|[2503.05565](http://arxiv.org/abs/2503.05565)|null|
|**2025-03-07**|**Leveraging Approximate Caching for Faster Retrieval-Augmented Generation**|Shai Bergman et.al.|[2503.05530](http://arxiv.org/abs/2503.05530)|null|
|**2025-03-07**|**PoSSUM: A Protocol for Surveying Social-media Users with Multimodal LLMs**|Roberto Cerina et.al.|[2503.05529](http://arxiv.org/abs/2503.05529)|null|
|**2025-03-07**|**Cognitive Bias Detection Using Advanced Prompt Engineering**|Frederic Lemieux et.al.|[2503.05516](http://arxiv.org/abs/2503.05516)|null|
|**2025-03-07**|**Statistical Guarantees of Correctness Coverage for Medical Multiple-Choice Question Answering**|Yusong Ke et.al.|[2503.05505](http://arxiv.org/abs/2503.05505)|null|
|**2025-03-07**|**Benchmarking LLMs in Recommendation Tasks: A Comparative Evaluation with Conventional Recommenders**|Qijiong Liu et.al.|[2503.05493](http://arxiv.org/abs/2503.05493)|null|
|**2025-03-07**|**Shifting Long-Context LLMs Research from Input to Output**|Yuhao Wu et.al.|[2503.04723](http://arxiv.org/abs/2503.04723)|null|
|**2025-03-06**|**Enough Coin Flips Can Make LLMs Act Bayesian**|Ritwik Gupta et.al.|[2503.04722](http://arxiv.org/abs/2503.04722)|null|
|**2025-03-06**|**Predictable Scale: Part I -- Optimal Hyperparameter Scaling Law in Large Language Model Pretraining**|Houyi Li et.al.|[2503.04715](http://arxiv.org/abs/2503.04715)|null|
|**2025-03-06**|**Universality of Layer-Level Entropy-Weighted Quantization Beyond Model Architecture and Size**|Alireza Behtash et.al.|[2503.04704](http://arxiv.org/abs/2503.04704)|null|
|**2025-03-06**|**UIPE: Enhancing LLM Unlearning by Removing Knowledge Related to Forgetting Targets**|Wenyu Wang et.al.|[2503.04693](http://arxiv.org/abs/2503.04693)|null|
|**2025-03-06**|**LLM-guided Plan and Retrieval: A Strategic Alignment for Interpretable User Satisfaction Estimation in Dialogue**|Sangyeop Kim et.al.|[2503.04675](http://arxiv.org/abs/2503.04675)|null|
|**2025-03-06**|**Implicit Cross-Lingual Rewarding for Efficient Multilingual Preference Alignment**|Wen Yang et.al.|[2503.04647](http://arxiv.org/abs/2503.04647)|null|
|**2025-03-06**|**Mark Your LLM: Detecting the Misuse of Open-Source Large Language Models via Watermarking**|Yijie Xu et.al.|[2503.04636](http://arxiv.org/abs/2503.04636)|null|
|**2025-03-06**|**Better Process Supervision with Bi-directional Rewarding Signals**|Wenxiang Chen et.al.|[2503.04618](http://arxiv.org/abs/2503.04618)|null|
|**2025-03-06**|**Towards Data-Efficient Language Models: A Child-Inspired Approach to Language Learning**|Mohammad Amin Ghanizadeh et.al.|[2503.04611](http://arxiv.org/abs/2503.04611)|null|
|**2025-03-05**|**The MASK Benchmark: Disentangling Honesty From Accuracy in AI Systems**|Richard Ren et.al.|[2503.03750](http://arxiv.org/abs/2503.03750)|null|
|**2025-03-05**|**Towards Understanding Distilled Reasoning Models: A Representational Approach**|David D. Baek et.al.|[2503.03730](http://arxiv.org/abs/2503.03730)|null|
|**2025-03-05**|**Improving LLM Safety Alignment with Dual-Objective Optimization**|Xuandong Zhao et.al.|[2503.03710](http://arxiv.org/abs/2503.03710)|**[link](https://github.com/wicai24/door-alignment)**|
|**2025-03-05**|**Effective LLM Knowledge Learning via Model Generalization**|Mingkang Zhu et.al.|[2503.03705](http://arxiv.org/abs/2503.03705)|null|
|**2025-03-05**|**A Practical Memory Injection Attack against LLM Agents**|Shen Dong et.al.|[2503.03704](http://arxiv.org/abs/2503.03704)|null|
|**2025-03-05**|**Developing and Utilizing a Large-Scale Cantonese Dataset for Multi-Tasking in Large Language Models**|Jiyue Jiang et.al.|[2503.03702](http://arxiv.org/abs/2503.03702)|null|
|**2025-03-05**|**Addressing Overprescribing Challenges: Fine-Tuning Large Language Models for Medication Recommendation Tasks**|Zihao Zhao et.al.|[2503.03687](http://arxiv.org/abs/2503.03687)|**[link](https://github.com/zzhustc2016/lamo)**|
|**2025-03-05**|**Analogical Reasoning Inside Large Language Models: Concept Vectors and the Limits of Abstraction**|Gustaw Opiełka et.al.|[2503.03666](http://arxiv.org/abs/2503.03666)|**[link](https://github.com/gucioopielka/concept_vectors)**|
|**2025-03-05**|**Improving Neutral Point of View Text Generation through Parameter-Efficient Reinforcement Learning and a Small-Scale High-Quality Dataset**|Jessica Hoffmann et.al.|[2503.03654](http://arxiv.org/abs/2503.03654)|null|
|**2025-03-05**|**Psy-Copilot: Visual Chain of Thought for Counseling**|Keqi Chen et.al.|[2503.03645](http://arxiv.org/abs/2503.03645)|null|
|**2025-03-04**|**Wikipedia in the Era of LLMs: Evolution and Risks**|Siming Huang et.al.|[2503.02879](http://arxiv.org/abs/2503.02879)|**[link](https://github.com/hsm316/llm_wikipedia)**|
|**2025-03-04**|**The First Few Tokens Are All You Need: An Efficient and Effective Unsupervised Prefix Fine-Tuning Method for Reasoning Models**|Ke Ji et.al.|[2503.02875](http://arxiv.org/abs/2503.02875)|null|
|**2025-03-04**|**FairSense-AI: Responsible AI Meets Sustainability**|Shaina Raza et.al.|[2503.02865](http://arxiv.org/abs/2503.02865)|null|
|**2025-03-04**|**Calibrating LLM Confidence with Semantic Steering: A Multi-Prompt Aggregation Framework**|Ziang Zhou et.al.|[2503.02863](http://arxiv.org/abs/2503.02863)|null|
|**2025-03-04**|**Shakespearean Sparks: The Dance of Hallucination and Creativity in LLMs' Decoding Layers**|Zicong He et.al.|[2503.02851](http://arxiv.org/abs/2503.02851)|**[link](https://github.com/ziconghe2002/hcl-spark)**|
|**2025-03-04**|**Mask-DPO: Generalizable Fine-grained Factuality Alignment of LLMs**|Yuzhe Gu et.al.|[2503.02846](http://arxiv.org/abs/2503.02846)|**[link](https://github.com/open-compass/anah)**|
|**2025-03-04**|**AlignDistil: Token-Level Language Model Alignment as Adaptive Policy Distillation**|Songming Zhang et.al.|[2503.02832](http://arxiv.org/abs/2503.02832)|null|
|**2025-03-04**|**RAAD-LLM: Adaptive Anomaly Detection Using LLMs and RAG Integration**|Alicia Russell-Gilbert et.al.|[2503.02800](http://arxiv.org/abs/2503.02800)|null|
|**2025-03-04**|**Implicit Bias in LLMs: A Survey**|Xinru Lin et.al.|[2503.02776](http://arxiv.org/abs/2503.02776)|null|
|**2025-03-04**|**BatchGEMBA: Token-Efficient Machine Translation Evaluation with Batched Prompting and Prompt Compression**|Daniil Larionov et.al.|[2503.02756](http://arxiv.org/abs/2503.02756)|null|
|**2025-02-28**|**LLM Post-Training: A Deep Dive into Reasoning Large Language Models**|Komal Kumar et.al.|[2502.21321](http://arxiv.org/abs/2502.21321)|**[link](https://github.com/mbzuai-oryx/awesome-llm-post-training)**|
|**2025-02-28**|**FANformer: Improving Large Language Models Through Effective Periodicity Modeling**|Yihong Dong et.al.|[2502.21309](http://arxiv.org/abs/2502.21309)|null|
|**2025-02-28**|**Contextualizing biological perturbation experiments through language**|Menghua Wu et.al.|[2502.21290](http://arxiv.org/abs/2502.21290)|**[link](https://github.com/genentech/perturbqa)**|
|**2025-02-28**|**Adaptive Keyframe Sampling for Long Video Understanding**|Xi Tang et.al.|[2502.21271](http://arxiv.org/abs/2502.21271)|null|
|**2025-02-28**|**Semantic Volume: Quantifying and Detecting both External and Internal Uncertainty in LLMs**|Xiaomin Li et.al.|[2502.21239](http://arxiv.org/abs/2502.21239)|null|
|**2025-02-28**|**ByteScale: Efficient Scaling of LLM Training with a 2048K Context Length on More Than 12,000 GPUs**|Hao Ge et.al.|[2502.21231](http://arxiv.org/abs/2502.21231)|null|
|**2025-03-03**|**ECLeKTic: a Novel Challenge Set for Evaluation of Cross-Lingual Knowledge Transfer**|Omer Goldman et.al.|[2502.21228](http://arxiv.org/abs/2502.21228)|null|
|**2025-02-28**|**Transformers Learn to Implement Multi-step Gradient Descent with Chain of Thought**|Jianhao Huang et.al.|[2502.21212](http://arxiv.org/abs/2502.21212)|null|
|**2025-02-28**|**Optimizing Large Language Models for ESG Activity Detection in Financial Texts**|Mattia Birti et.al.|[2502.21112](http://arxiv.org/abs/2502.21112)|**[link](https://github.com/mattia-brt/fine_tuning_llm)**|
|**2025-02-28**|**Large Language Model-Based Benchmarking Experiment Settings for Evolutionary Multi-Objective Optimization**|Lie Meng Pang et.al.|[2502.21108](http://arxiv.org/abs/2502.21108)|null|
|**2025-02-27**|**R2-T2: Re-Routing in Test-Time for Multimodal Mixture-of-Experts**|Zhongyang Li et.al.|[2502.20395](http://arxiv.org/abs/2502.20395)|**[link](https://github.com/tianyi-lab/R2-T2)**|
|**2025-02-27**|**Why Are Web AI Agents More Vulnerable Than Standalone LLMs? A Security Analysis**|Jeffrey Yang Fan Chiang et.al.|[2502.20383](http://arxiv.org/abs/2502.20383)|null|
|**2025-02-27**|**Multi-Agent Verification: Scaling Test-Time Compute with Multiple Verifiers**|Shalev Lifshitz et.al.|[2502.20379](http://arxiv.org/abs/2502.20379)|null|
|**2025-02-27**|**PhantomWiki: On-Demand Datasets for Reasoning and Retrieval Evaluation**|Albert Gong et.al.|[2502.20377](http://arxiv.org/abs/2502.20377)|**[link](https://github.com/kilian-group/phantom-wiki)**|
|**2025-02-27**|**Bridging Legal Knowledge and AI: Retrieval-Augmented Generation with Vector Stores, Knowledge Graphs, and Hierarchical Non-negative Matrix Factorization**|Ryan C. Barron et.al.|[2502.20364](http://arxiv.org/abs/2502.20364)|null|
|**2025-02-27**|**Bridging the Creativity Understanding Gap: Small-Scale Human Alignment Enables Expert-Level Humor Ranking in LLMs**|Kuan Lok Zhou et.al.|[2502.20356](http://arxiv.org/abs/2502.20356)|null|
|**2025-02-27**|**KEDRec-LM: A Knowledge-distilled Explainable Drug Recommendation Large Language Model**|Kai Zhang et.al.|[2502.20350](http://arxiv.org/abs/2502.20350)|null|
|**2025-02-27**|**Sparse Auto-Encoder Interprets Linguistic Features in Large Language Models**|Yi Jing et.al.|[2502.20344](http://arxiv.org/abs/2502.20344)|null|
|**2025-02-27**|**Thinking Slow, Fast: Scaling Inference Compute with Distilled Reasoners**|Daniele Paliotta et.al.|[2502.20339](http://arxiv.org/abs/2502.20339)|null|
|**2025-02-27**|**Expertise Is What We Want**|Alan Ashworth et.al.|[2502.20335](http://arxiv.org/abs/2502.20335)|null|
|**2025-02-26**|**Norm Growth and Stability Challenges in Localized Sequential Knowledge Editing**|Akshat Gupta et.al.|[2502.19416](http://arxiv.org/abs/2502.19416)|null|
|**2025-02-26**|**Code to Think, Think to Code: A Survey on Code-Enhanced Reasoning and Reasoning-Driven Code Intelligence in LLMs**|Dayu Yang et.al.|[2502.19411](http://arxiv.org/abs/2502.19411)|**[link](https://github.com/dayuyang1999/awesome-code-reasoning)**|
|**2025-02-26**|**Less or More: Towards Glanceable Explanations for LLM Recommendations Using Ultra-Small Devices**|Xinru Wang et.al.|[2502.19410](http://arxiv.org/abs/2502.19410)|null|
|**2025-02-26**|**Learning Code-Edit Embedding to Model Student Debugging Behavior**|Hasnain Heickal et.al.|[2502.19407](http://arxiv.org/abs/2502.19407)|null|
|**2025-02-26**|**General Reasoning Requires Learning to Reason from the Get-go**|Seungwook Han et.al.|[2502.19402](http://arxiv.org/abs/2502.19402)|null|
|**2025-02-26**|**TheoremExplainAgent: Towards Multimodal Explanations for LLM Theorem Understanding**|Max Ku et.al.|[2502.19400](http://arxiv.org/abs/2502.19400)|null|
|**2025-02-26**|**DataMan: Data Manager for Pre-training Large Language Models**|Ru Peng et.al.|[2502.19363](http://arxiv.org/abs/2502.19363)|null|
|**2025-02-26**|**Can Large Language Models Detect Errors in Long Chain-of-Thought Reasoning?**|Yancheng He et.al.|[2502.19361](http://arxiv.org/abs/2502.19361)|**[link](https://github.com/openstellarteam/deltabench)**|
|**2025-02-26**|**Agentic Reward Modeling: Integrating Human Preferences with Verifiable Correctness Signals for Reliable Reward Systems**|Hao Peng et.al.|[2502.19328](http://arxiv.org/abs/2502.19328)|**[link](https://github.com/thu-keg/agentic-reward-modeling)**|
|**2025-02-26**|**Shh, don't say that! Domain Certification in LLMs**|Cornelius Emde et.al.|[2502.19320](http://arxiv.org/abs/2502.19320)|null|
|**2025-02-25**|**DRAMA: Diverse Augmentation from Large Language Models to Smaller Dense Retrievers**|Xueguang Ma et.al.|[2502.18460](http://arxiv.org/abs/2502.18460)|**[link](https://github.com/facebookresearch/dpr-scale)**|
|**2025-02-25**|**FRIDA to the Rescue! Analyzing Synthetic Data Effectiveness in Object-Based Common Sense Reasoning for Disaster Response**|Mollie Shichman et.al.|[2502.18452](http://arxiv.org/abs/2502.18452)|null|
|**2025-02-25**|**SWE-RL: Advancing LLM Reasoning via Reinforcement Learning on Open Software Evolution**|Yuxiang Wei et.al.|[2502.18449](http://arxiv.org/abs/2502.18449)|null|
|**2025-02-25**|**MAPoRL: Multi-Agent Post-Co-Training for Collaborative Large Language Models with Reinforcement Learning**|Chanwoo Park et.al.|[2502.18439](http://arxiv.org/abs/2502.18439)|null|
|**2025-02-25**|**TextGames: Learning to Self-Play Text-Based Puzzle Games via Language Model Reasoning**|Frederikus Hudi et.al.|[2502.18431](http://arxiv.org/abs/2502.18431)|**[link](https://github.com/fhudi/textgames)**|
|**2025-02-25**|**Monte Carlo Temperature: a robust sampling strategy for LLM's uncertainty quantification methods**|Nicola Cecere et.al.|[2502.18389](http://arxiv.org/abs/2502.18389)|null|
|**2025-02-25**|**How Far are LLMs from Real Search? A Comprehensive Study on Efficiency, Completeness, and Inherent Capabilities**|Minhua Lin et.al.|[2502.18387](http://arxiv.org/abs/2502.18387)|null|
|**2025-02-25**|**BRIDO: Bringing Democratic Order to Abstractive Summarization**|Junhyun Lee et.al.|[2502.18342](http://arxiv.org/abs/2502.18342)|null|
|**2025-02-25**|**RefuteBench 2.0 -- Agentic Benchmark for Dynamic Evaluation of LLM Responses to Refutation Instruction**|Jianhao Yan et.al.|[2502.18308](http://arxiv.org/abs/2502.18308)|null|
|**2025-02-25**|**LDGen: Enhancing Text-to-Image Synthesis via Large Language Model-Driven Language Representation**|Pengzhi Li et.al.|[2502.18302](http://arxiv.org/abs/2502.18302)|null|
|**2025-02-24**|**LongSpec: Long-Context Speculative Decoding with Efficient Drafting and Verification**|Penghui Yang et.al.|[2502.17421](http://arxiv.org/abs/2502.17421)|**[link](https://github.com/sail-sg/longspec)**|
|**2025-02-24**|**The Geometry of Refusal in Large Language Models: Concept Cones and Representational Independence**|Tom Wollschläger et.al.|[2502.17420](http://arxiv.org/abs/2502.17420)|null|
|**2025-02-24**|**From System 1 to System 2: A Survey of Reasoning Large Language Models**|Zhong-Zhi Li et.al.|[2502.17419](http://arxiv.org/abs/2502.17419)|**[link](https://github.com/zzli2022/awesome-slow-reason-system)**|
|**2025-02-24**|**COSMOS: A Hybrid Adaptive Optimizer for Memory-Efficient Training of LLMs**|Liming Liu et.al.|[2502.17410](http://arxiv.org/abs/2502.17410)|**[link](https://github.com/lliu606/cosmos)**|
|**2025-02-24**|**Large Language Models are Powerful EHR Encoders**|Stefan Hegselmann et.al.|[2502.17403](http://arxiv.org/abs/2502.17403)|**[link](https://github.com/stefanhgm/ehrshot-benchmark)**|
|**2025-02-24**|**On Relation-Specific Neurons in Large Language Models**|Yihong Liu et.al.|[2502.17355](http://arxiv.org/abs/2502.17355)|**[link](https://github.com/cisnlp/relation-specific-neurons)**|
|**2025-02-24**|**Time series forecasting based on optimized LLM for fault prediction in distribution power grid insulators**|João Pedro Matos-Carvalho et.al.|[2502.17341](http://arxiv.org/abs/2502.17341)|null|
|**2025-02-24**|**Delta Decompression for MoE-based LLMs Compression**|Hao Gu et.al.|[2502.17298](http://arxiv.org/abs/2502.17298)|**[link](https://github.com/lliai/d2moe)**|
|**2025-02-24**|**Integrating protein sequence embeddings with structure via graph-based deep learning for the prediction of single-residue properties**|Kevin Michalewicz et.al.|[2502.17294](http://arxiv.org/abs/2502.17294)|**[link](https://github.com/kevinmicha/GCN-Bf)**|
|**2025-02-24**|**Capability Instruction Tuning: A New Paradigm for Dynamic LLM Routing**|Yi-Kai Zhang et.al.|[2502.17282](http://arxiv.org/abs/2502.17282)|**[link](https://github.com/now-join-us/cit-llm-routing)**|
|**2025-02-21**|**Privacy Ripple Effects from Adding or Removing Personal Information in Language Model Training**|Jaydeep Borkar et.al.|[2502.15680](http://arxiv.org/abs/2502.15680)|**[link](https://github.com/jaydeepborkar/Assisted-Memorization)**|
|**2025-02-21**|**FLEKE: Federated Locate-then-Edit Knowledge Editing**|Zongkai Zhao et.al.|[2502.15677](http://arxiv.org/abs/2502.15677)|**[link](https://github.com/zongkaiz/fleke)**|
|**2025-02-21**|**AutoToM: Automated Bayesian Inverse Planning and Model Discovery for Open-ended Theory of Mind**|Zhining Zhang et.al.|[2502.15676](http://arxiv.org/abs/2502.15676)|**[link](https://github.com/SCAI-JHU/AutoToM)**|
|**2025-02-21**|**Almost AI, Almost Human: The Challenge of Detecting AI-Polished Writing**|Shoumik Saha et.al.|[2502.15666](http://arxiv.org/abs/2502.15666)|**[link](https://github.com/ShoumikSaha/ai-polished-text)**|
|**2025-02-21**|**Machine-generated text detection prevents language model collapse**|George Drayson et.al.|[2502.15654](http://arxiv.org/abs/2502.15654)|null|
|**2025-02-21**|**Empowering LLMs with Logical Reasoning: A Comprehensive Survey**|Fengxiang Cheng et.al.|[2502.15652](http://arxiv.org/abs/2502.15652)|null|
|**2025-02-21**|**Probe Pruning: Accelerating LLMs through Dynamic Pruning via Model-Probing**|Qi Le et.al.|[2502.15618](http://arxiv.org/abs/2502.15618)|**[link](https://github.com/qi-le1/probe_pruning)**|
|**2025-02-21**|**On the Robustness of Transformers against Context Hijacking for Linear Classification**|Tianle Li et.al.|[2502.15609](http://arxiv.org/abs/2502.15609)|null|
|**2025-02-21**|**Cross-Format Retrieval-Augmented Generation in XR with LLMs for Context-Aware Maintenance Assistance**|Akos Nagy et.al.|[2502.15604](http://arxiv.org/abs/2502.15604)|null|
|**2025-02-21**|**Do Multilingual LLMs Think In English?**|Lisa Schut et.al.|[2502.15603](http://arxiv.org/abs/2502.15603)|null|
|**2025-02-20**|**LServe: Efficient Long-sequence LLM Serving with Unified Sparse Attention**|Shang Yang et.al.|[2502.14866](http://arxiv.org/abs/2502.14866)|**[link](https://github.com/mit-han-lab/omniserve)**|
|**2025-02-20**|**Aligning LLMs to Ask Good Questions A Case Study in Clinical Reasoning**|Shuyue Stella Li et.al.|[2502.14860](http://arxiv.org/abs/2502.14860)|**[link](https://github.com/stellalisy/alfa)**|
|**2025-02-20**|**FR-Spec: Accelerating Large-Vocabulary Language Models via Frequency-Ranked Speculative Sampling**|Weilin Zhao et.al.|[2502.14856](http://arxiv.org/abs/2502.14856)|null|
|**2025-02-20**|**Prompt-to-Leaderboard**|Evan Frick et.al.|[2502.14855](http://arxiv.org/abs/2502.14855)|**[link](https://github.com/lmarena/p2l)**|
|**2025-02-20**|**GATE: Graph-based Adaptive Tool Evolution Across Diverse Tasks**|Jianwen Luo et.al.|[2502.14848](http://arxiv.org/abs/2502.14848)|**[link](https://github.com/ayanami2003/gate)**|
|**2025-02-20**|**Scaling Text-Rich Image Understanding via Code-Guided Synthetic Multimodal Data Generation**|Yue Yang et.al.|[2502.14846](http://arxiv.org/abs/2502.14846)|null|
|**2025-02-20**|**A Survey of Model Architectures in Information Retrieval**|Zhichao Xu et.al.|[2502.14822](http://arxiv.org/abs/2502.14822)|null|
|**2025-02-20**|**eC-Tab2Text: Aspect-Based Text Generation from e-Commerce Product Tables**|Luis Antonio Gutiérrez Guanilo et.al.|[2502.14820](http://arxiv.org/abs/2502.14820)|null|
|**2025-02-20**|**Dynamic Low-Rank Sparse Adaptation for Large Language Models**|Weizhong Huang et.al.|[2502.14816](http://arxiv.org/abs/2502.14816)|**[link](https://github.com/wzhuang-xmu/losa)**|
|**2025-02-20**|**From RAG to Memory: Non-Parametric Continual Learning for Large Language Models**|Bernal Jiménez Gutiérrez et.al.|[2502.14802](http://arxiv.org/abs/2502.14802)|**[link](https://github.com/osu-nlp-group/hipporag)**|
|**2025-02-19**|**Where's the Bug? Attention Probing for Scalable Fault Localization**|Adam Stein et.al.|[2502.13966](http://arxiv.org/abs/2502.13966)|null|
|**2025-02-19**|**Autellix: An Efficient Serving Engine for LLM Agents as General Programs**|Michael Luo et.al.|[2502.13965](http://arxiv.org/abs/2502.13965)|null|
|**2025-02-19**|**MuDAF: Long-Context Multi-Document Attention Focusing through Contrastive Learning on Attention Heads**|Weihao Liu et.al.|[2502.13963](http://arxiv.org/abs/2502.13963)|**[link](https://github.com/NeosKnight233/MuDAF)**|
|**2025-02-19**|**Neurosymbolic artificial intelligence via large language models and coherence-driven inference**|Steve Huntsman et.al.|[2502.13953](http://arxiv.org/abs/2502.13953)|null|
|**2025-02-19**|**Why Safeguarded Ships Run Aground? Aligned Large Language Models' Safety Mechanisms Tend to Be Anchored in The Template Region**|Chak Tou Leong et.al.|[2502.13946](http://arxiv.org/abs/2502.13946)|null|
|**2025-02-19**|**LongPO: Long Context Self-Evolution of Large Language Models through Short-to-Long Preference Optimization**|Guanzheng Chen et.al.|[2502.13922](http://arxiv.org/abs/2502.13922)|**[link](https://github.com/DAMO-NLP-SG/LongPO)**|
|**2025-02-19**|**Exploring Code Language Models for Automated HLS-based Hardware Generation: Benchmark, Infrastructure and Analysis**|Jiahao Gai et.al.|[2502.13921](http://arxiv.org/abs/2502.13921)|null|
|**2025-02-19**|**How Do LLMs Perform Two-Hop Reasoning in Context?**|Tianyu Guo et.al.|[2502.13913](http://arxiv.org/abs/2502.13913)|null|
|**2025-02-19**|**Lost in Sequence: Do Large Language Models Understand Sequential Recommendation?**|Sein Kim et.al.|[2502.13909](http://arxiv.org/abs/2502.13909)|**[link](https://github.com/sein-kim/llm-srec)**|
|**2025-02-19**|**Judging the Judges: A Collection of LLM-Generated Relevance Judgements**|Hossein A. Rahmani et.al.|[2502.13908](http://arxiv.org/abs/2502.13908)|**[link](https://github.com/chuanmeng/qpp-genre)**|
|**2025-02-18**|**Re-Align: Aligning Vision Language Models via Retrieval-Augmented Direct Preference Optimization**|Shuo Xing et.al.|[2502.13146](http://arxiv.org/abs/2502.13146)|**[link](https://github.com/taco-group/re-align)**|
|**2025-02-18**|**UniGuardian: A Unified Defense for Detecting Prompt Injection, Backdoor Attacks and Adversarial Attacks in Large Language Models**|Huawei Lin et.al.|[2502.13141](http://arxiv.org/abs/2502.13141)|**[link](https://github.com/huawei-lin/uniguardian)**|
|**2025-02-18**|**AIDE: AI-Driven Exploration in the Space of Code**|Zhengyao Jiang et.al.|[2502.13138](http://arxiv.org/abs/2502.13138)|**[link](https://github.com/wecoai/aideml)**|
|**2025-02-18**|**Theorem Prover as a Judge for Synthetic Data Generation**|Joshua Ong Jun Leang et.al.|[2502.13137](http://arxiv.org/abs/2502.13137)|null|
|**2025-02-18**|**Facilitating Long Context Understanding via Supervised Chain-of-Thought Reasoning**|Jingyang Lin et.al.|[2502.13127](http://arxiv.org/abs/2502.13127)|null|
|**2025-02-18**|**RuozhiBench: Evaluating LLMs with Logical Fallacies and Misleading Premises**|Zenan Zhai et.al.|[2502.13125](http://arxiv.org/abs/2502.13125)|**[link](https://github.com/LibrAIResearch/ruozhibench)**|
|**2025-02-18**|**Adapting Psycholinguistic Research for LLMs: Gender-inclusive Language in a Coreference Context**|Marion Bartl et.al.|[2502.13120](http://arxiv.org/abs/2502.13120)|null|
|**2025-02-18**|**STEER-ME: Assessing the Microeconomic Reasoning of Large Language Models**|Narun Raman et.al.|[2502.13119](http://arxiv.org/abs/2502.13119)|null|
|**2025-02-18**|**Performance Evaluation of Large Language Models in Statistical Programming**|Xinyi Song et.al.|[2502.13117](http://arxiv.org/abs/2502.13117)|**[link](https://github.com/yili-hong/StatLLM)**|
|**2025-02-18**|**MatterChat: A Multi-Modal LLM for Material Science**|Yingheng Tang et.al.|[2502.13107](http://arxiv.org/abs/2502.13107)|null|
|**2025-02-17**|**Idiosyncrasies in Large Language Models**|Mingjie Sun et.al.|[2502.12150](http://arxiv.org/abs/2502.12150)|**[link](https://github.com/locuslab/llm-idiosyncrasies)**|
|**2025-02-17**|**Fast or Better? Balancing Accuracy and Cost in Retrieval-Augmented Generation with Flexible User Control**|Jinyan Su et.al.|[2502.12145](http://arxiv.org/abs/2502.12145)|**[link](https://github.com/jinyansu1/flare-aug)**|
|**2025-02-17**|**Small Models Struggle to Learn from Strong Reasoners**|Yuetai Li et.al.|[2502.12143](http://arxiv.org/abs/2502.12143)|null|
|**2025-02-17**|**SoftCoT: Soft Chain-of-Thought for Efficient Reasoning with LLMs**|Yige Xu et.al.|[2502.12134](http://arxiv.org/abs/2502.12134)|null|
|**2025-02-17**|**Scaling Autonomous Agents via Automatic Reward Modeling And Planning**|Zhenfang Chen et.al.|[2502.12130](http://arxiv.org/abs/2502.12130)|null|
|**2025-02-17**|**LLMs on the Line: Data Determines Loss-to-Loss Scaling Laws**|Prasanna Mayilvahanan et.al.|[2502.12120](http://arxiv.org/abs/2502.12120)|null|
|**2025-02-17**|**A-MEM: Agentic Memory for LLM Agents**|Wujiang Xu et.al.|[2502.12110](http://arxiv.org/abs/2502.12110)|**[link](https://github.com/wujiangxu/agenticmemory)**|
|**2025-02-17**|**Personality Structured Interview for Large Language Model Simulation in Personality Research**|Pengda Wang et.al.|[2502.12109](http://arxiv.org/abs/2502.12109)|null|
|**2025-02-17**|**Meta-Statistical Learning: Supervised Learning of Statistical Inference**|Maxime Peyrard et.al.|[2502.12088](http://arxiv.org/abs/2502.12088)|null|
|**2025-02-17**|**APB: Accelerating Distributed Long-Context Inference by Passing Compressed Context Blocks across GPUs**|Yuxiang Huang et.al.|[2502.12085](http://arxiv.org/abs/2502.12085)|**[link](https://github.com/thunlp/apb)**|
|**2025-02-14**|**Aspect-Oriented Summarization for Psychiatric Short-Term Readmission Prediction**|WonJin Yoon et.al.|[2502.10388](http://arxiv.org/abs/2502.10388)|null|
|**2025-02-14**|**Enhancing Multilingual LLM Pretraining with Model-Based Data Selection**|Bettina Messmer et.al.|[2502.10361](http://arxiv.org/abs/2502.10361)|null|
|**2025-02-14**|**Evaluating the Meta- and Object-Level Reasoning of Large Language Models for Question Answering**|Nick Ferguson et.al.|[2502.10338](http://arxiv.org/abs/2502.10338)|null|
|**2025-02-14**|**LLM-Powered Preference Elicitation in Combinatorial Assignment**|Ermis Soumalias et.al.|[2502.10308](http://arxiv.org/abs/2502.10308)|null|
|**2025-02-14**|**Open-Source AI-Powered Optimization in Scalene: Advancing Python Performance Profiling with DeepSeek-R1 and LLaMA 3.2**|Saem Hasan et.al.|[2502.10299](http://arxiv.org/abs/2502.10299)|null|
|**2025-02-14**|**Are Large Language Models the future crowd workers of Linguistics?**|Iris Ferrazzo et.al.|[2502.10266](http://arxiv.org/abs/2502.10266)|null|
|**2025-02-14**|**Large Language Models and Synthetic Data for Monitoring Dataset Mentions in Research Papers**|Aivin V. Solatorio et.al.|[2502.10263](http://arxiv.org/abs/2502.10263)|null|
|**2025-02-14**|**VisCon-100K: Leveraging Contextual Web Data for Fine-tuning Vision Language Models**|Gokul Karthik Kumar et.al.|[2502.10250](http://arxiv.org/abs/2502.10250)|null|
|**2025-02-14**|**Efficient Zero-Order Federated Finetuning of Language Models for Resource-Constrained Devices**|Mohamed Aboelenien Ahmed et.al.|[2502.10239](http://arxiv.org/abs/2502.10239)|null|
|**2025-02-14**|**Do Large Language Models Reason Causally Like Us? Even Better?**|Hanna M. Dettki et.al.|[2502.10215](http://arxiv.org/abs/2502.10215)|null|
|**2025-02-13**|**MME-CoT: Benchmarking Chain-of-Thought in Large Multimodal Models for Reasoning Quality, Robustness, and Efficiency**|Dongzhi Jiang et.al.|[2502.09621](http://arxiv.org/abs/2502.09621)|null|
|**2025-02-13**|**Exploring the Potential of Encoder-free Architectures in 3D LMMs**|Yiwen Tang et.al.|[2502.09620](http://arxiv.org/abs/2502.09620)|**[link](https://github.com/ivan-tang-3d/enel)**|
|**2025-02-13**|**Human-LLM Coevolution: Evidence from Academic Writing**|Mingmeng Geng et.al.|[2502.09606](http://arxiv.org/abs/2502.09606)|null|
|**2025-02-13**|**Do LLMs Recognize Your Preferences? Evaluating Personalized Preference Following in LLMs**|Siyan Zhao et.al.|[2502.09597](http://arxiv.org/abs/2502.09597)|**[link](https://github.com/amazon-science/PrefEval)**|
|**2025-02-13**|**KIMAs: A Configurable Knowledge Integrated Multi-Agent System**|Zitao Li et.al.|[2502.09596](http://arxiv.org/abs/2502.09596)|null|
|**2025-02-13**|**Logical forms complement probability in understanding language model (and human) performance**|Yixuan Wang et.al.|[2502.09589](http://arxiv.org/abs/2502.09589)|null|
|**2025-02-13**|**Polymind: Parallel Visual Diagramming with Large Language Models to Support Prewriting Through Microtasks**|Qian Wan et.al.|[2502.09577](http://arxiv.org/abs/2502.09577)|null|
|**2025-02-13**|**Zero-shot generation of synthetic neurosurgical data with large language models**|Austin A. Barr et.al.|[2502.09566](http://arxiv.org/abs/2502.09566)|**[link](https://github.com/aabarr/Synthetic-Neurosurgical-Data)**|
|**2025-02-13**|**MDCrow: Automating Molecular Dynamics Workflows with Large Language Models**|Quintina Campbell et.al.|[2502.09565](http://arxiv.org/abs/2502.09565)|**[link](https://github.com/ur-whitelab/MDCrow)**|
|**2025-02-13**|**Mind the Gap! Choice Independence in Using Multilingual LLMs for Persuasive Co-Writing Tasks in Different Languages**|Shreyan Biswas et.al.|[2502.09532](http://arxiv.org/abs/2502.09532)|null|
|**2025-02-12**|**Ensemble based approach to quantifying uncertainty of LLM based classifications**|Srijith Rajamohan et.al.|[2502.08631](http://arxiv.org/abs/2502.08631)|null|
|**2025-02-12**|**Commercial LLM Agents Are Already Vulnerable to Simple Yet Dangerous Attacks**|Ang Li et.al.|[2502.08586](http://arxiv.org/abs/2502.08586)|null|
|**2025-02-12**|**QA-Expand: Multi-Question Answer Generation for Enhanced Query Expansion in Information Retrieval**|Wonduk Seo et.al.|[2502.08557](http://arxiv.org/abs/2502.08557)|null|
|**2025-02-12**|**Fostering Appropriate Reliance on Large Language Models: The Role of Explanations, Sources, and Inconsistencies**|Sunnie S. Y. Kim et.al.|[2502.08554](http://arxiv.org/abs/2502.08554)|null|
|**2025-02-12**|**LLMs can implicitly learn from mistakes in-context**|Lisa Alazraki et.al.|[2502.08550](http://arxiv.org/abs/2502.08550)|null|
|**2025-02-12**|**The Paradox of Stochasticity: Limited Creativity and Computational Decoupling in Temperature-Varied LLM Outputs of Structured Fictional Data**|Evgenii Evstafev et.al.|[2502.08515](http://arxiv.org/abs/2502.08515)|null|
|**2025-02-12**|**Faithful, Unfaithful or Ambiguous? Multi-Agent Debate with Initial Stance for Summary Evaluation**|Mahnaz Koupaee et.al.|[2502.08514](http://arxiv.org/abs/2502.08514)|**[link](https://github.com/amazon-science/madisse)**|
|**2025-02-12**|**Measuring Diversity in Synthetic Datasets**|Yuchang Zhu et.al.|[2502.08512](http://arxiv.org/abs/2502.08512)|**[link](https://github.com/bluewhalelab/dcscore)**|
|**2025-02-12**|**Explanation based In-Context Demonstrations Retrieval for Multilingual Grammatical Error Correction**|Wei Li et.al.|[2502.08507](http://arxiv.org/abs/2502.08507)|**[link](https://github.com/gmago-leway/fewshotgec)**|
|**2025-02-12**|**From Haystack to Needle: Label Space Reduction for Zero-shot Classification**|Nathan Vandemoortele et.al.|[2502.08436](http://arxiv.org/abs/2502.08436)|null|
|**2025-02-11**|**DarwinLM: Evolutionary Structured Pruning of Large Language Models**|Shengkun Tang et.al.|[2502.07780](http://arxiv.org/abs/2502.07780)|**[link](https://github.com/IST-DASLab/DarwinLM)**|
|**2025-02-11**|**Auditing Prompt Caching in Language Model APIs**|Chenchen Gu et.al.|[2502.07776](http://arxiv.org/abs/2502.07776)|**[link](https://github.com/chenchenygu/auditing-prompt-caching)**|
|**2025-02-11**|**Automatic Robot Task Planning by Integrating Large Language Model with Genetic Programming**|Azizjon Kobilov et.al.|[2502.07772](http://arxiv.org/abs/2502.07772)|null|
|**2025-02-11**|**Great Power Brings Great Responsibility: Personalizing Conversational AI for Diverse Problem-Solvers**|Italo Santos et.al.|[2502.07763](http://arxiv.org/abs/2502.07763)|null|
|**2025-02-11**|**Towards Efficient Optimizer Design for LLM via Structured Fisher Approximation with a Low-Rank Extension**|Wenbo Gong et.al.|[2502.07752](http://arxiv.org/abs/2502.07752)|null|
|**2025-02-11**|**WHODUNIT: Evaluation benchmark for culprit detection in mystery stories**|Kshitij Gupta et.al.|[2502.07747](http://arxiv.org/abs/2502.07747)|**[link](https://github.com/kjgpta/WhoDunIt-Evaluation_benchmark_for_culprit_detection_in_mystery_stories)**|
|**2025-02-11**|**The Economics of Large Language Models: Token Allocation, Fine-Tuning, and Optimal Pricing**|Dirk Bergemann et.al.|[2502.07736](http://arxiv.org/abs/2502.07736)|null|
|**2025-02-11**|**Verifying LLM-Generated Code in the Context of Software Verification with Ada/SPARK**|Marcos Cramer et.al.|[2502.07728](http://arxiv.org/abs/2502.07728)|null|
|**2025-02-11**|**A Framework for LLM-powered Design Assistants**|Swaroop Panda et.al.|[2502.07698](http://arxiv.org/abs/2502.07698)|null|
|**2025-02-11**|**Large Language Models as Proxies for Theories of Human Linguistic Cognition**|Imry Ziv et.al.|[2502.07687](http://arxiv.org/abs/2502.07687)|null|
|**2025-02-10**|**Gradient Multi-Normalization for Stateless and Scalable LLM Training**|Meyer Scetbon et.al.|[2502.06742](http://arxiv.org/abs/2502.06742)|null|
|**2025-02-10**|**VersaPRM: Multi-Domain Process Reward Model via Synthetic Reasoning Data**|Thomas Zeng et.al.|[2502.06737](http://arxiv.org/abs/2502.06737)|null|
|**2025-02-10**|**Dynamic Loss-Based Sample Reweighting for Improved Large Language Model Pretraining**|Daouda Sow et.al.|[2502.06733](http://arxiv.org/abs/2502.06733)|null|
|**2025-02-10**|**Can 1B LLM Surpass 405B LLM? Rethinking Compute-Optimal Test-Time Scaling**|Runze Liu et.al.|[2502.06703](http://arxiv.org/abs/2502.06703)|**[link](https://github.com/RyanLiu112/compute-optimal-tts)**|
|**2025-02-10**|**Boosting Self-Efficacy and Performance of Large Language Models via Verbal Efficacy Stimulations**|Rui Chen et.al.|[2502.06669](http://arxiv.org/abs/2502.06669)|null|
|**2025-02-10**|**Automatic Evaluation of Healthcare LLMs Beyond Question-Answering**|Anna Arias-Duart et.al.|[2502.06666](http://arxiv.org/abs/2502.06666)|null|
|**2025-02-10**|**EfficientLLM: Scalable Pruning-Aware Pretraining for Architecture-Agnostic Edge Language Models**|Xingrun Xing et.al.|[2502.06663](http://arxiv.org/abs/2502.06663)|null|
|**2025-02-10**|**LawGPT: Knowledge-Guided Data Generation and Its Application to Legal LLM**|Zhi Zhou et.al.|[2502.06572](http://arxiv.org/abs/2502.06572)|**[link](https://github.com/LAMDASZ-ML/Knowledge-Guide-Data-Generation)**|
|**2025-02-10**|**Large Language Models Meet Symbolic Provers for Logical Reasoning Evaluation**|Chengwen Qi et.al.|[2502.06563](http://arxiv.org/abs/2502.06563)|**[link](https://github.com/opendatalab/provergen)**|
|**2025-02-10**|**Is API Access to LLMs Useful for Generating Private Synthetic Tabular Data?**|Marika Swanberg et.al.|[2502.06555](http://arxiv.org/abs/2502.06555)|null|
|**2025-02-07**|**NoLiMa: Long-Context Evaluation Beyond Literal Matching**|Ali Modarressi et.al.|[2502.05167](http://arxiv.org/abs/2502.05167)|**[link](https://github.com/adobe-research/NoLiMa)**|
|**2025-02-07**|**DuoGuard: A Two-Player RL-Driven Framework for Multilingual LLM Guardrails**|Yihe Deng et.al.|[2502.05163](http://arxiv.org/abs/2502.05163)|**[link](https://github.com/yihedeng9/duoguard)**|
|**2025-02-07**|**A Lightweight Method to Disrupt Memorized Sequences in LLM**|Parjanya Prajakta Prashant et.al.|[2502.05159](http://arxiv.org/abs/2502.05159)|null|
|**2025-02-07**|**CodeSCM: Causal Analysis for Multi-Modal Code Generation**|Mukur Gupta et.al.|[2502.05150](http://arxiv.org/abs/2502.05150)|**[link](https://github.com/nb15/codeSCM-naacl25)**|
|**2025-02-07**|**An Annotated Reading of 'The Singer of Tales' in the LLM Era**|Kush R. Varshney et.al.|[2502.05148](http://arxiv.org/abs/2502.05148)|null|
|**2025-02-07**|**Flexible and Efficient Grammar-Constrained Decoding**|Kanghee Park et.al.|[2502.05111](http://arxiv.org/abs/2502.05111)|null|
|**2025-02-07**|**ChallengeMe: An Adversarial Learning-enabled Text Summarization Framework**|Xiaoyu Deng et.al.|[2502.05084](http://arxiv.org/abs/2502.05084)|null|
|**2025-02-07**|**Adaptive Graph of Thoughts: Test-Time Adaptive Reasoning Unifying Chain, Tree, and Graph Structures**|Tushar Pandey et.al.|[2502.05078](http://arxiv.org/abs/2502.05078)|**[link](https://github.com/AgnostiqHQ/multi-agent-llm)**|
|**2025-02-07**|**nvAgent: Automated Data Visualization from Natural Language via Collaborative Agent Workflow**|Geliang Ouyang et.al.|[2502.05036](http://arxiv.org/abs/2502.05036)|**[link](https://github.com/geliang0114/nvagent)**|
|**2025-02-07**|**QuEST: Stable Training of LLMs with 1-Bit Weights and Activations**|Andrei Panferov et.al.|[2502.05003](http://arxiv.org/abs/2502.05003)|**[link](https://github.com/IST-DASLab/QuEST)**|
|**2025-02-06**|**Speak Easy: Eliciting Harmful Jailbreaks from LLMs with Simple Interactions**|Yik Siu Chan et.al.|[2502.04322](http://arxiv.org/abs/2502.04322)|**[link](https://github.com/yiksiu-chan/SpeakEasy)**|
|**2025-02-06**|**ChamaleonLLM: Batch-Aware Dynamic Low-Rank Adaptation via Inference-Time Clusters**|Kamer Ali Yuksel et.al.|[2502.04315](http://arxiv.org/abs/2502.04315)|**[link](https://github.com/kayuksel/ChamaleonLLM)**|
|**2025-02-06**|**Beyond Prompt Content: Enhancing LLM Performance via Content-Format Integrated Prompt Optimization**|Yuanye Liu et.al.|[2502.04295](http://arxiv.org/abs/2502.04295)|**[link](https://github.com/henrylau7/cfpo)**|
|**2025-02-06**|**Can LLMs Hack Enterprise Networks? Autonomous Assumed Breach Penetration-Testing Active Directory Networks**|Andreas Happe et.al.|[2502.04227](http://arxiv.org/abs/2502.04227)|null|
|**2025-02-06**|**Keep It Light! Simplifying Image Clustering Via Text-Free Adapters**|Yicen Li et.al.|[2502.04226](http://arxiv.org/abs/2502.04226)|null|
|**2025-02-06**|**Éclair -- Extracting Content and Layout with Integrated Reading Order for Documents**|Ilia Karmanov et.al.|[2502.04223](http://arxiv.org/abs/2502.04223)|null|
|**2025-02-06**|**Sports and Women's Sports: Gender Bias in Text Generation with Olympic Data**|Laura Biester et.al.|[2502.04218](http://arxiv.org/abs/2502.04218)|null|
|**2025-02-06**|**"Short-length" Adversarial Training Helps LLMs Defend "Long-length" Jailbreak Attacks: Theoretical and Empirical Evidence**|Shaopeng Fu et.al.|[2502.04204](http://arxiv.org/abs/2502.04204)|**[link](https://github.com/fshp971/adv-icl)**|
|**2025-02-06**|**The Best Instruction-Tuning Data are Those That Fit**|Dylan Zhang et.al.|[2502.04194](http://arxiv.org/abs/2502.04194)|null|
|**2025-02-06**|**Automated Microservice Pattern Instance Detection Using Infrastructure-as-Code Artifacts and Large Language Models**|Carlos Eduardo Duarte et.al.|[2502.04188](http://arxiv.org/abs/2502.04188)|null|
|**2025-02-05**|**Do Large Language Model Benchmarks Test Reliability?**|Joshua Vendrow et.al.|[2502.03461](http://arxiv.org/abs/2502.03461)|**[link](https://github.com/MadryLab/platinum-benchmarks)**|
|**2025-02-05**|**Adapt-Pruner: Adaptive Structural Pruning for Efficient Small Language Model Training**|Boyao Wang et.al.|[2502.03460](http://arxiv.org/abs/2502.03460)|null|
|**2025-02-05**|**A Schema-Guided Reason-while-Retrieve framework for Reasoning on Scene Graphs with Large-Language-Models (LLMs)**|Yiye Chen et.al.|[2502.03450](http://arxiv.org/abs/2502.03450)|null|
|**2025-02-05**|**BFS-Prover: Scalable Best-First Tree Search for LLM-based Automatic Theorem Proving**|Ran Xin et.al.|[2502.03438](http://arxiv.org/abs/2502.03438)|null|
|**2025-02-05**|**Harnessing Large Language Models for Curated Code Reviews**|Oussama Ben Sghaier et.al.|[2502.03425](http://arxiv.org/abs/2502.03425)|**[link](https://github.com/OussamaSghaier/CuREV)**|
|**2025-02-05**|**Think or Step-by-Step? UnZIPping the Black Box in Zero-Shot Prompts**|Nikta Gohari Sadr et.al.|[2502.03418](http://arxiv.org/abs/2502.03418)|null|
|**2025-02-05**|**Demystifying Long Chain-of-Thought Reasoning in LLMs**|Edward Yeo et.al.|[2502.03373](http://arxiv.org/abs/2502.03373)|**[link](https://github.com/eddycmu/demystify-long-cot)**|
|**2025-02-05**|**ECM: A Unified Electronic Circuit Model for Explaining the Emergence of In-Context Learning and Chain-of-Thought in Large Language Model**|Qiguang Chen et.al.|[2502.03325](http://arxiv.org/abs/2502.03325)|null|
|**2025-02-05**|**Out-of-Distribution Detection using Synthetic Data Generation**|Momin Abbas et.al.|[2502.03323](http://arxiv.org/abs/2502.03323)|null|
|**2025-02-05**|**Intent Representation Learning with Large Language Model for Recommendation**|Yu Wang et.al.|[2502.03307](http://arxiv.org/abs/2502.03307)|**[link](https://github.com/wangyu0627/irllrec)**|
|**2025-02-04**|**A comparison of translation performance between DeepL and Supertext**|Alex Flückiger et.al.|[2502.02577](http://arxiv.org/abs/2502.02577)|**[link](https://github.com/supertext/evaluation_deepl_supertext)**|
|**2025-02-04**|**Are Language Models Up to Sequential Optimization Problems? From Evaluation to a Hegelian-Inspired Enhancement**|Soheil Abbasloo et.al.|[2502.02573](http://arxiv.org/abs/2502.02573)|null|
|**2025-02-04**|**LLMs for Generation of Architectural Components: An Exploratory Empirical Study in the Serverless World**|Shrikara Arun et.al.|[2502.02539](http://arxiv.org/abs/2502.02539)|null|
|**2025-02-04**|**Adaptive Self-improvement LLM Agentic System for ML Library Development**|Genghan Zhang et.al.|[2502.02534](http://arxiv.org/abs/2502.02534)|**[link](https://github.com/zhang677/pcl-lite)**|
|**2025-02-04**|**Satori: Reinforcement Learning with Chain-of-Action-Thought Enhances LLM Reasoning via Autoregressive Search**|Maohao Shen et.al.|[2502.02508](http://arxiv.org/abs/2502.02508)|null|
|**2025-02-04**|**EasySpec: Layer-Parallel Speculative Decoding for Efficient Multi-GPU Utilization**|Yize Wu et.al.|[2502.02493](http://arxiv.org/abs/2502.02493)|null|
|**2025-02-04**|**Multilingual Machine Translation with Open Large Language Models at Practical Scale: An Empirical Study**|Menglong Cui et.al.|[2502.02481](http://arxiv.org/abs/2502.02481)|null|
|**2025-02-04**|**Beyond English: Evaluating Automated Measurement of Moral Foundations in Non-English Discourse with a Chinese Case Study**|Calvin Yixiang Cheng et.al.|[2502.02451](http://arxiv.org/abs/2502.02451)|**[link](https://github.com/calvinchengyx/cross-lan-mft-measure)**|
|**2025-02-04**|**Generative Psycho-Lexical Approach for Constructing Value Systems in Large Language Models**|Haoran Ye et.al.|[2502.02444](http://arxiv.org/abs/2502.02444)|null|
|**2025-02-04**|**LLMER: Crafting Interactive Extended Reality Worlds with JSON Data Generated by Large Language Models**|Jiangong Chen et.al.|[2502.02441](http://arxiv.org/abs/2502.02441)|**[link](https://github.com/snec-lab-psu/llmer)**|
|**2025-01-31**|**Cache Me If You Must: Adaptive Key-Value Quantization for Large Language Models**|Alina Shutova et.al.|[2501.19392](http://arxiv.org/abs/2501.19392)|**[link](https://github.com/goodevening13/aquakv)**|
|**2025-01-31**|**Federated Sketching LoRA: On-Device Collaborative Fine-Tuning of Large Language Models**|Wenzhi Fang et.al.|[2501.19389](http://arxiv.org/abs/2501.19389)|**[link](https://github.com/wenzhifang/Federated-Sketching-LoRA-Implementation)**|
|**2025-02-03**|**SELMA: A Speech-Enabled Language Model for Virtual Assistant Interactions**|Dominik Wagner et.al.|[2501.19377](http://arxiv.org/abs/2501.19377)|null|
|**2025-01-31**|**We're Different, We're the Same: Creative Homogeneity Across LLMs**|Emily Wenger et.al.|[2501.19361](http://arxiv.org/abs/2501.19361)|null|
|**2025-01-31**|**The Energy Loss Phenomenon in RLHF: A New Perspective on Mitigating Reward Hacking**|Yuchun Miao et.al.|[2501.19358](http://arxiv.org/abs/2501.19358)|null|
|**2025-01-31**|**Towards Adaptive Self-Improvement for Smarter Energy Systems**|Alexander Sommer et.al.|[2501.19340](http://arxiv.org/abs/2501.19340)|null|
|**2025-01-31**|**Homogeneity Bias as Differential Sampling Uncertainty in Language Models**|Messi H. J. Lee et.al.|[2501.19337](http://arxiv.org/abs/2501.19337)|null|
|**2025-01-31**|**Reward-Guided Speculative Decoding for Efficient LLM Reasoning**|Baohao Liao et.al.|[2501.19324](http://arxiv.org/abs/2501.19324)|null|
|**2025-01-31**|**MINDSTORES: Memory-Informed Neural Decision Synthesis for Task-Oriented Reinforcement in Embodied Systems**|Anirudh Chari et.al.|[2501.19318](http://arxiv.org/abs/2501.19318)|null|
|**2025-01-31**|**Judge Decoding: Faster Speculative Sampling Requires Going Beyond Model Alignment**|Gregor Bachmann et.al.|[2501.19309](http://arxiv.org/abs/2501.19309)|null|
|**2025-01-30**|**Thoughts Are All Over the Place: On the Underthinking of o1-Like LLMs**|Yue Wang et.al.|[2501.18585](http://arxiv.org/abs/2501.18585)|null|
|**2025-01-30**|**Illusions of Relevance: Using Content Injection Attacks to Deceive Retrievers, Rerankers, and LLM Judges**|Manveer Singh Tamber et.al.|[2501.18536](http://arxiv.org/abs/2501.18536)|**[link](https://github.com/manveertamber/content_injection_attacks)**|
|**2025-01-30**|**Differentially Private Steering for Large Language Model Alignment**|Anmol Goel et.al.|[2501.18532](http://arxiv.org/abs/2501.18532)|**[link](https://github.com/ukplab/iclr2025-psa)**|
|**2025-01-30**|**Learn from the Past: Language-conditioned Object Rearrangement with Large Language Models**|Guanqun Cao et.al.|[2501.18516](http://arxiv.org/abs/2501.18516)|null|
|**2025-01-30**|**Streaming DiLoCo with overlapping communication: Towards a Distributed Free Lunch**|Arthur Douillard et.al.|[2501.18512](http://arxiv.org/abs/2501.18512)|null|
|**2025-01-30**|**CLEAR: Cue Learning using Evolution for Accurate Recognition Applied to Sustainability Data Extraction**|Peter J. Bentley et.al.|[2501.18504](http://arxiv.org/abs/2501.18504)|null|
|**2025-01-30**|**A Tool for In-depth Analysis of Code Execution Reasoning of Large Language Models**|Changshu Liu et.al.|[2501.18482](http://arxiv.org/abs/2501.18482)|null|
|**2025-01-30**|**CLoQ: Enhancing Fine-Tuning of Quantized LLMs via Calibrated LoRA Initialization**|Yanxia Deng et.al.|[2501.18475](http://arxiv.org/abs/2501.18475)|null|
|**2025-01-30**|**ExeCoder: Empowering Large Language Models with Executability Representation for Code Translation**|Minghua He et.al.|[2501.18460](http://arxiv.org/abs/2501.18460)|null|
|**2025-01-30**|**CALM: Unleashing the Cross-Lingual Self-Aligning Ability of Language Model Question Answering**|Yumeng Wang et.al.|[2501.18457](http://arxiv.org/abs/2501.18457)|null|
|**2025-01-29**|**Learning Beyond the Surface: How Far Can Continual Pre-Training with LoRA Enhance LLMs' Domain-Specific Insight Learning?**|Pouya Pezeshkpour et.al.|[2501.17840](http://arxiv.org/abs/2501.17840)|**[link](https://github.com/megagonlabs/insight_miner)**|
|**2025-01-29**|**BreezyVoice: Adapting TTS for Taiwanese Mandarin with Enhanced Polyphone Disambiguation -- Challenges and Insights**|Chan-Jan Hsu et.al.|[2501.17790](http://arxiv.org/abs/2501.17790)|null|
|**2025-01-29**|**2SSP: A Two-Stage Framework for Structured Pruning of LLMs**|Fabrizio Sandri et.al.|[2501.17771](http://arxiv.org/abs/2501.17771)|**[link](https://github.com/fabriziosandri/2ssp)**|
|**2025-01-29**|**Hybrid Graphs for Table-and-Text based Question Answering using LLMs**|Ankush Agarwal et.al.|[2501.17767](http://arxiv.org/abs/2501.17767)|null|
|**2025-01-29**|**Early External Safety Testing of OpenAI's o3-mini: Insights from the Pre-Deployment Evaluation**|Aitor Arrieta et.al.|[2501.17749](http://arxiv.org/abs/2501.17749)|null|
|**2025-01-29**|**Using Code Generation to Solve Open Instances of Combinatorial Design Problems**|Christopher D. Rosin et.al.|[2501.17725](http://arxiv.org/abs/2501.17725)|**[link](https://github.com/constructive-codes/cpro1)**|
|**2025-01-29**|**RICoTA: Red-teaming of In-the-wild Conversation with Test Attempts**|Eujeong Choi et.al.|[2501.17715](http://arxiv.org/abs/2501.17715)|**[link](https://github.com/boychaboy/ricota)**|
|**2025-01-29**|**Planning with Vision-Language Models and a Use Case in Robot-Assisted Teaching**|Xuzhe Dang et.al.|[2501.17665](http://arxiv.org/abs/2501.17665)|null|
|**2025-01-29**|**In-Context Meta LoRA Generation**|Yihua Shao et.al.|[2501.17635](http://arxiv.org/abs/2501.17635)|null|
|**2025-01-29**|**The Imitation Game According To Turing**|Sharon Temtsin et.al.|[2501.17629](http://arxiv.org/abs/2501.17629)|null|
|**2025-01-28**|**FactCG: Enhancing Fact Checkers with Graph-Based Multi-Hop Data**|Deren Lei et.al.|[2501.17144](http://arxiv.org/abs/2501.17144)|**[link](https://github.com/derenlei/factcg)**|
|**2025-01-28**|**ASTRAL: Automated Safety Testing of Large Language Models**|Miriam Ugarte et.al.|[2501.17132](http://arxiv.org/abs/2501.17132)|null|
|**2025-01-28**|**Optimizing Large Language Model Training Using FP4 Quantization**|Ruizhe Wang et.al.|[2501.17116](http://arxiv.org/abs/2501.17116)|null|
|**2025-01-28**|**Unlocking Transparent Alignment Through Enhanced Inverse Constitutional AI for Principle Extraction**|Carl-Leander Henneking et.al.|[2501.17112](http://arxiv.org/abs/2501.17112)|null|
|**2025-01-28**|**Token-by-Token Regeneration and Domain Biases: A Benchmark of LLMs on Advanced Mathematical Problem-Solving**|Evgenii Evstafev et.al.|[2501.17084](http://arxiv.org/abs/2501.17084)|null|
|**2025-01-28**|**Enhanced Retrieval of Long Documents: Leveraging Fine-Grained Block Representations with Large Language Models**|Minghan Li et.al.|[2501.17039](http://arxiv.org/abs/2501.17039)|null|
|**2025-01-28**|**Challenges in Ensuring AI Safety in DeepSeek-R1 Models: The Shortcomings of Reinforcement Learning Strategies**|Manojkumar Parmar et.al.|[2501.17030](http://arxiv.org/abs/2501.17030)|null|
|**2025-01-28**|**Automated Refactoring of Non-Idiomatic Python Code: A Differentiated Replication with LLMs**|Alessandro Midolo et.al.|[2501.17024](http://arxiv.org/abs/2501.17024)|**[link](https://github.com/alemidolo/gptidiomrefactoring)**|
|**2025-01-28**|**Large Language Models for Code Generation: The Practitioners Perspective**|Zeeshan Rasheed et.al.|[2501.16998](http://arxiv.org/abs/2501.16998)|**[link](https://github.com/gpt-laboratory/llm-evaluation)**|
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
|**2025-01-22**|**Correctness Assessment of Code Generated by Large Language Models Using Internal Representations**|Tuan-Dung Bui et.al.|[2501.12934](http://arxiv.org/abs/2501.12934)|**[link](https://github.com/ise-uet-vnu/openia)**|
|**2025-01-21**|**Is Long Context All You Need? Leveraging LLM's Extended Context for NL2SQL**|Yeounoh Chung et.al.|[2501.12372](http://arxiv.org/abs/2501.12372)|**[link](https://github.com/yeounoh/lc_nl2sql)**|
|**2025-01-21**|**Automatic Labelling with Open-source LLMs using Dynamic Label Schema Integration**|Thomas Walshe et.al.|[2501.12332](http://arxiv.org/abs/2501.12332)|null|
|**2025-01-21**|**LLM-Assisted Knowledge Graph Completion for Curriculum and Domain Modelling in Personalized Higher Education Recommendations**|Hasan Abu-Rasheed et.al.|[2501.12300](http://arxiv.org/abs/2501.12300)|null|
|**2025-01-21**|**Condor: Enhance LLM Alignment with Knowledge-Driven Data Synthesis and Refinement**|Maosong Cao et.al.|[2501.12273](http://arxiv.org/abs/2501.12273)|**[link](https://github.com/internlm/condor)**|
|**2025-01-21**|**FOCUS: First Order Concentrated Updating Scheme**|Yizhou Liu et.al.|[2501.12243](http://arxiv.org/abs/2501.12243)|null|
|**2025-01-21**|**CDW-CoT: Clustered Distance-Weighted Chain-of-Thoughts Reasoning**|Yuanheng Fang et.al.|[2501.12226](http://arxiv.org/abs/2501.12226)|null|
|**2025-01-21**|**Leveraging Large Language Models for Realizing Truly Intelligent User Interfaces**|Allard Oelen et.al.|[2501.12221](http://arxiv.org/abs/2501.12221)|null|
|**2025-01-21**|**You Can't Eat Your Cake and Have It Too: The Performance Degradation of LLMs with Jailbreak Defense**|Wuyuao Mai et.al.|[2501.12210](http://arxiv.org/abs/2501.12210)|null|
|**2025-01-21**|**BiMarker: Enhancing Text Watermark Detection for Large Language Models with Bipolar Watermarks**|Zhuang Li et.al.|[2501.12174](http://arxiv.org/abs/2501.12174)|null|
|**2025-01-21**|**Contextualizing Recommendation Explanations with LLMs: A User Study**|Yuanjun Feng et.al.|[2501.12152](http://arxiv.org/abs/2501.12152)|null|
|**2025-01-17**|**Agent4Edu: Generating Learner Response Data by Generative Agents for Intelligent Education Systems**|Weibo Gao et.al.|[2501.10332](http://arxiv.org/abs/2501.10332)|**[link](https://github.com/bigdata-ustc/agent4edu)**|
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
|**2024-12-09**|**Training Large Language Models to Reason in a Continuous Latent Space**|Shibo Hao et.al.|[2412.06769](http://arxiv.org/abs/2412.06769)|**[link](https://github.com/facebookresearch/coconut)**|
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
|**2024-12-02**|**Critical Tokens Matter: Token-Level Contrastive Estimation Enhances LLM's Reasoning Capability**|Zicheng Lin et.al.|[2411.19943](http://arxiv.org/abs/2411.19943)|**[link](https://github.com/chenzhiling9954/critical-tokens-matter)**|
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
|**2024-11-25**|**Profiling Bias in LLMs: Stereotype Dimensions in Contextual Word Embeddings**|Carolin M. Schuster et.al.|[2411.16527](http://arxiv.org/abs/2411.16527)|**[link](https://github.com/carolinmschuster/profiling-bias-in-llms)**|
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
|**2024-11-06**|**Beemo: Benchmark of Expert-edited Machine-generated Outputs**|Ekaterina Artemova et.al.|[2411.04032](http://arxiv.org/abs/2411.04032)|**[link](https://github.com/Toloka/beemo)**|
|**2024-11-06**|**What Really is Commonsense Knowledge?**|Quyet V. Do et.al.|[2411.03964](http://arxiv.org/abs/2411.03964)|null|
|**2024-11-06**|**How Does A Text Preprocessing Pipeline Affect Ontology Syntactic Matching?**|Zhangcheng Qiang et.al.|[2411.03962](http://arxiv.org/abs/2411.03962)|**[link](https://github.com/qzc438/ontology-llm)**|
|**2024-11-06**|**Fine-Grained Guidance for Retrievers: Leveraging LLMs' Feedback in Retrieval-Augmented Generation**|Yuhang Liu et.al.|[2411.03957](http://arxiv.org/abs/2411.03957)|null|
|**2024-11-06**|**Long-Form Text-to-Music Generation with Adaptive Prompts: A Case of Study in Tabletop Role-Playing Games Soundtracks**|Felipe Marra et.al.|[2411.03948](http://arxiv.org/abs/2411.03948)|**[link](https://github.com/felipemarra/babel-bardo)**|
|**2024-11-06**|**Polynomial Composition Activations: Unleashing the Dynamics of Large Language Models**|Zhijian Zhuo et.al.|[2411.03884](http://arxiv.org/abs/2411.03884)|**[link](https://github.com/brycezhuo/polycom)**|
|**2024-11-06**|**MEG: Medical Knowledge-Augmented Large Language Models for Question Answering**|Laura Cabello et.al.|[2411.03883](http://arxiv.org/abs/2411.03883)|**[link](https://github.com/lautel/meg)**|
|**2024-11-06**|**Data Fusion of Synthetic Query Variants With Generative Large Language Models**|Timo Breuer et.al.|[2411.03881](http://arxiv.org/abs/2411.03881)|**[link](https://github.com/breuert/sigirap24)**|
|**2024-05-16**|**When LLMs step into the 3D World: A Survey and Meta-Analysis of 3D Tasks via Multi-modal Large Language Models**|Xianzheng Ma et.al.|[2405.10255](http://arxiv.org/abs/2405.10255)|**[link](https://github.com/activevisionlab/awesome-llm-3d)**|

<p align=right>(<a href=#updated-on-20250404>back to top</a>)</p>

## moe

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-04-03**|**MiLo: Efficient Quantized MoE Inference with Mixture of Low-Rank Compensators**|Beichen Huang et.al.|[2504.02658](http://arxiv.org/abs/2504.02658)|null|一种有效部署具有大量参数的混合专家（MoE）模型的关键方法是量化。然而，最先进的MoE模型在极端量化下（例如4比特以下）会遭受不可忽略的精度损失。为了解决这个问题，我们提出了MiLo，这是一种新方法，通过添加低秩补偿器来增强高度量化的MoE模型。这些补偿器仅消耗少量额外内存，但能显著恢复因极端量化造成的精度损失。MiLo还发现由于其混合密集-稀疏架构，MoE模型在权重上表现出独特的特性，并采用自适应秩选择策略和迭代优化来缩小精度差距。MiLo不依赖于校准数据，这使得它能够泛化到不同的MoE模型和数据集，而不会过度拟合到校准集。为了避免3比特等极端量化带来的硬件效率问题，MiLo开发了对Tensor Core友好的3比特内核，从而实现了3比特量化MoE模型上的测量延迟加速。我们的评估表明，MiLo在各种任务中优于现有方法，在最先进的MoE模型上表现突出。|
|**2025-04-03**|**MegaScale-Infer: Serving Mixture-of-Experts at Scale with Disaggregated Expert Parallelism**|Ruidong Zhu et.al.|[2504.02263](http://arxiv.org/abs/2504.02263)|null|混合专家（MoE）模型在扩展大规模语言模型（LLMs）方面展示了巨大的潜力，能够提升性能并降低计算复杂度。然而，其稀疏激活架构使得前馈网络（FFNs）从计算密集型转变为内存密集型，导致推理过程中GPU利用率显著降低且运营成本增加。我们提出了MegaScale-Infer系统，这是一种高效且成本低廉的大规模MoE模型服务方案。MegaScale-Infer将每个模型层中的注意力机制和FFN模块解耦，允许独立扩展、定制化并行策略以及异构部署。为了充分利用MoE稀疏性带来的解耦优势，MegaScale-Infer引入了乒乓流水线并行技术，该技术将请求批次分割为微批次，并在注意力机制与FFN之间来回传递以完成推理过程。结合各模块特有的模型并行技术，MegaScale-Infer有效隐藏了通信开销并最大化了GPU利用率。为了适应解耦后的注意力机制和FFN模块并最小化数据传输开销（例如，令牌分发），MegaScale-Infer提供了一个高性能的M2N通信库，消除了不必要的GPU到CPU的数据复制、组初始化开销及GPU同步问题。实验结果显示，MegaScale-Infer相较于最先进的解决方案，实现了高达1.90倍的每GPU吞吐量提升。|
|**2025-04-02**|**Advancing MoE Efficiency: A Collaboration-Constrained Routing (C2R) Strategy for Better Expert Parallelism Design**|Mohan Zhang et.al.|[2504.01337](http://arxiv.org/abs/2504.01337)|null|混合专家（MoE）模型通过保持几乎恒定的计算成本成功地扩展了模型规模。它利用一个门控网络来路由输入令牌，并选择性地激活一部分专家网络以处理相应的令牌嵌入。然而，在实践中，由于两个关键原因，MoE 的效率难以实现：不平衡的专家激活导致在模型或专家并行时有大量的空闲时间，以及容量利用率不足；由专家并行中大量专家路由组合引起的巨大通信开销。以往的工作通常将其归因于由门控网络偏好某些专家而忽略其他专家所导致的负载不平衡问题，或者归因于静态执行无法适应运行时动态专家工作负载的问题。在本文中，我们从一个全新的角度——更高阶的视角和分析——探讨了 MoE 路由策略：专家协作与专业化，其中一些专家倾向于广泛与其他专家一起激活（协作型），而另一些则更可能仅与特定子集的专家一起激活（专业型）。我们的实验揭示，大多数专家倾向于过度协作，这导致了由于重复将令牌发送到不同加速器而增加的通信开销。为此，我们提出了一种新的协作约束路由（C2R）策略，以鼓励更多专业化的专家组，同时提高专家利用率，并展示了一种进一步利用专家专业化的高效 MoE 实现。我们在十个下游 NLP 基准测试上实现了 LLaMA-MoE 和 Qwen-MoE 平均性能分别提升 0.51% 和 0.33%，并且减少了 GPU 之间的全对全通信成本，在现有最先进方法 MegaBlocks 的基础上额外节省了 20%-30% 的总运行时间。|
|**2025-04-01**|**Mixture-of-Experts for Distributed Edge Computing with Channel-Aware Gating Function**|Qiuchen Song et.al.|[2504.00819](http://arxiv.org/abs/2504.00819)|null|在分布式混合专家（MoE）系统中，服务器与多个专业化的专家客户端协作进行推理。服务器从输入数据中提取特征，并根据专家的专业领域动态选择专家以生成最终输出。尽管MoE模型因其灵活性和性能优势而广受重视，但将分布式MoE适应于无线网络的有效运行尚未得到探索。在这项工作中，我们引入了一种新的信道感知门控函数用于无线分布式MoE，该函数将信道条件纳入MoE门控机制中。为了训练信道感知门控函数，我们模拟了每个专家通信信道的各种信噪比（SNR），并根据这些SNR向分配给专家的特征中添加噪声。然后，门控函数利用特征和SNR来优化专家选择。与仅考虑特征与专家专长匹配的传统MoE模型不同，我们的方法还考虑了信道条件对专家性能的影响。实验结果表明，所提出的信道感知门控方案优于传统MoE模型。|
|**2025-04-01**|**DynMoLE: Boosting Mixture of LoRA Experts Fine-Tuning with a Hybrid Routing Mechanism**|Dengchun Li et.al.|[2504.00661](http://arxiv.org/abs/2504.00661)|**[link](https://github.com/mikecovlee/DynMoLE)**|**基于指令的大型语言模型（LLMs）微调在各种自然语言处理（NLP）任务中取得了显著的成功。参数高效微调（PEFT）方法，如混合LoRA专家（MoLE），结合了低秩适应（LoRA）的效率和混合专家（MoE）模型的多功能性，在处理多个下游任务方面展现了巨大的潜力。然而，现有的MoLE路由机制通常在计算效率和预测准确性之间存在权衡，并且未能完全解决不同Transformer层对专家选择的不同需求。在这项工作中，我们提出了DynMoLE，这是一种混合路由策略，它根据路由器概率分布的Tsallis熵动态调整专家选择。这种方法减轻了路由器的不确定性，增强了稳定性，并促进了更公平的专家参与，从而加快了收敛速度并提高了模型性能。此外，我们引入了一种基于Tsallis熵的辅助损失，以进一步引导模型减少不确定性地收敛，从而提高训练稳定性和性能。我们在常识推理基准上的广泛实验表明，DynMoLE实现了显著的性能改进，比LoRA高出9.6%，并且超过了最先进的MoLE方法MoLA 2.3%。我们还进行了全面的消融研究，以评估DynMoLE关键组件的贡献。**|
|**2025-03-30**|**Mixture of Routers**|Jia-Chen Zhang et.al.|[2503.23362](http://arxiv.org/abs/2503.23362)|null|监督微调（SFT）是使大型语言模型与人类指令对齐并适应下游任务的一个里程碑。特别是，低秩适应（LoRA）因其参数效率而受到广泛关注。然而，它在提升大型模型性能方面的影响仍然有限。最近的研究表明，将LoRA与专家混合（MoE）结合可以显著提高微调性能。MoE通过动态选择最适合的专家来适应数据集的多样性和复杂性，从而提高任务准确性和效率。尽管取得了令人印象深刻的结果，但最近的研究揭示了MoE路由机制中的问题，如错误分配和专家分配不均衡。受冗余和容错理论原则的启发，我们将专家混合的概念创新地融入到路由机制中，并提出了一种高效的微调方法——路由器混合（MoR）。该方法使用多个子路由器进行联合选择，并采用可学习的主路由器来确定子路由器的权重。结果显示，MoR在大多数任务上优于基线模型，平均性能提高了1%。MoR可以作为一种即插即用、参数高效的微调方法，适用于广泛的应用场景。我们的代码可在此处获取：https://anonymous.4open.science/r/MoR-DFC6。|
|**2025-03-29**|**Beyond Standard MoE: Mixture of Latent Experts for Resource-Efficient Language Models**|Zehua Liu et.al.|[2503.23100](http://arxiv.org/abs/2503.23100)|null|专家混合（MoE）已成为有效扩展大型语言模型（LLM）的关键架构范式，通过为每个输入标记选择性激活参数子集来工作。然而，传统的MoE架构在训练和推理过程中面临重大挑战，包括由于专家模块数量增加而导致的内存使用过高和通信开销过大。在这篇论文中，我们介绍了一种新的参数化方法——潜变量专家混合（MoLE），该方法能够将特定专家映射到共享的潜在空间中。具体来说，所有专家操作被系统地分解为两个主要组成部分：一个共享的投影到低维潜在空间，随后是具有显著减少参数复杂度的专家特定变换。这种分解方法大大减少了参数数量和计算需求。除了在预训练中实现MoLE架构外，我们还建立了一个严格的数学框架，用于将预训练的MoE模型转换为MoLE架构，描述了最佳分解的充分条件，并开发了一个系统的两阶段算法来进行这一转换过程。我们的全面理论分析表明，MoLE在多个维度上显著提高了计算效率，同时保持了模型的表示能力。实证评估证实了我们的理论发现，证明MoLE在大幅降低资源需求的同时，实现了与标准MoE实现相当的性能。|
|**2025-03-26**|**Reasoning Beyond Limits: Advances and Open Problems for LLMs**|Mohamed Amine Ferrag et.al.|[2503.22732](http://arxiv.org/abs/2503.22732)|null|
|**2025-04-01**|**Exploiting Mixture-of-Experts Redundancy Unlocks Multimodal Generative Abilities**|Raman Dutt et.al.|[2503.22517](http://arxiv.org/abs/2503.22517)|null|在这项工作中，我们致力于在保持预训练文本大语言模型（LLMs）原有生成能力几乎不降的前提下（约束C1），同时在有限的参数预算内（约束C2），增强其多模态生成能力。与当前通过增加专用模块从而显著增加参数数量的方法不同，我们提出了一种利用深度模型中未充分利用的容量的方法。具体来说，我们利用混合专家（MoEs）中的参数冗余作为学习新模态的额外容量来源，从而实现更好的参数效率（满足C1）。此外，我们通过仅对新模态的标记应用低秩适应来保持原有的语言生成能力（满足C2）。我们还引入了一种基于Gromov-Wasserstein距离的新参数初始化方案，以改善收敛性和训练稳定性。通过对路由机制的深入分析，我们发现了特定于模态的路径以及专家内部冗余的减少，这可以有效地解锁多模态生成能力。总体而言，我们的方法可以无缝应用于各种当代的大语言模型，为从单模态向多模态架构的转变提供了一条新的途径。|
|**2025-03-27**|**iMedImage Technical Report**|Ran Wei et.al.|[2503.21836](http://arxiv.org/abs/2503.21836)|null|背景：染色体核型分析对于遗传病的诊断至关重要，但检测结构异常仍然具有挑战性。虽然人工智能在医学影像方面显示出潜力，但其在不同模态中的有效性各不相同。利用在多模态医学影像集成方面取得进展的基础模型，我们开发了iMedImage，这是一种端到端的通用医学图像识别模型，在多个成像任务中表现出色，包括染色体异常检测。材料与方法：我们构建了一个涵盖多种模态的综合医学图像数据集，包括来自常见医学领域的染色体、细胞、病理学、超声、X射线、CT和MRI图像。基于该数据集，我们开发了iMedImage模型，该模型包含以下关键特征：（1）对多样模态输入和医学成像任务的统一表示方法；（2）通过思维链（CoT）嵌入和专家混合（MoE）策略增强的多层次（病例级、图像级、斑块级）图像识别能力。结果：测试集包括来自中国六个地区的12家机构的数据，涵盖了三种主流扫描设备，并包含了自然分布、未经筛选的异常案例。在这个多样化的数据集上，该模型实现了全自动染色体分析工作流程，包括分割、核型分析和异常检测，达到了92.75%的敏感性和91.5%的特异性。结论：我们提出了一种用于医学图像分析的端到端基础模型iMedImage，展示了其在各种医学成像任务中的卓越性能。iMedImage为临床医生提供了一种精确的影像分析工具，有助于提高诊断准确性和疾病筛查效率。|
|**2025-03-27**|**LLaVA-CMoE: Towards Continual Mixture of Experts for Large Vision-Language Models**|Hengyuan Zhao et.al.|[2503.21227](http://arxiv.org/abs/2503.21227)|null|尽管将专家混合模型应用于大型语言模型以学习新任务被广泛认为是一种有效的持续学习策略，但仍存在两个主要挑战：（1）随着任务数量的增长，简单的参数扩展策略可能导致模型变得过大；（2）修改现有路由器的参数会导致之前获得的知识被侵蚀。在本文中，我们提出了一种名为LLaVA-CMoE的创新框架，这是一种无需任何回放数据的连续专家混合架构。具体来说，我们开发了一种称为探针引导知识扩展（PGKE）的方法，该方法使用探针专家来评估特定层是否需要额外的知识。这种方法使模型能够根据任务分布自适应地扩展其网络参数，从而显著提高了参数扩展的效率。此外，我们引入了一种称为概率任务定位器（PTL）的分层路由算法，其中高层路由捕捉任务间信息，低层路由关注任务内细节，确保新任务专家不会干扰现有的专家。我们的实验表明，这种高效的架构在Coin基准测试上大幅提高了模型性能，同时保持了合理的参数数量。|
|**2025-03-26**|**Optimal Scaling Laws for Efficiency Gains in a Theoretical Transformer-Augmented Sectional MoE Framework**|Soham Sane et.al.|[2503.20750](http://arxiv.org/abs/2503.20750)|null|
|**2025-03-25**|**BiPrompt-SAM: Enhancing Image Segmentation via Explicit Selection between Point and Text Prompts**|Suzhe Xu et.al.|[2503.19769](http://arxiv.org/abs/2503.19769)|null|
|**2025-03-25**|**M $^2$ CD: A Unified MultiModal Framework for Optical-SAR Change Detection with Mixture of Experts and Self-Distillation**|Ziyuan Liu et.al.|[2503.19406](http://arxiv.org/abs/2503.19406)|null|
|**2025-03-22**|**Every Sample Matters: Leveraging Mixture-of-Experts and High-Quality Data for Efficient and Accurate Code LLM**|Codefuse et.al.|[2503.17793](http://arxiv.org/abs/2503.17793)|null|
|**2025-03-25**|**Expert Race: A Flexible Routing Strategy for Scaling Diffusion Transformer with Mixture of Experts**|Yike Yuan et.al.|[2503.16057](http://arxiv.org/abs/2503.16057)|null|
|**2025-03-20**|**Mixture of Lookup Experts**|Shibo Jie et.al.|[2503.15798](http://arxiv.org/abs/2503.15798)|**[link](https://github.com/jieshibo/mole)**|
|**2025-03-21**|**Leveraging MoE-based Large Language Model for Zero-Shot Multi-Task Semantic Communication**|Sin-Yu Huang et.al.|[2503.15722](http://arxiv.org/abs/2503.15722)|null|
|**2025-03-21**|**Body-Hand Modality Expertized Networks with Cross-attention for Fine-grained Skeleton Action Recognition**|Seungyeon Cho et.al.|[2503.14960](http://arxiv.org/abs/2503.14960)|null|
|**2025-03-17**|**Channel Estimation for Pinching-Antenna Systems (PASS)**|Jian Xiao et.al.|[2503.13268](http://arxiv.org/abs/2503.13268)|null|
|**2025-03-16**|**MoECollab: Democratizing LLM Development Through Collaborative Mixture of Experts**|Harshit et.al.|[2503.12592](http://arxiv.org/abs/2503.12592)|null|
|**2025-03-16**|**MExD: An Expert-Infused Diffusion Model for Whole-Slide Image Classification**|Jianwei Zhao et.al.|[2503.12401](http://arxiv.org/abs/2503.12401)|null|
|**2025-03-14**|**FedALT: Federated Fine-Tuning through Adaptive Local Training with Rest-of-the-World LoRA**|Jieming Bian et.al.|[2503.11880](http://arxiv.org/abs/2503.11880)|null|
|**2025-03-13**|**Samoyeds: Accelerating MoE Models with Structured Sparsity Leveraging Sparse Tensor Cores**|Chenpeng Wu et.al.|[2503.10725](http://arxiv.org/abs/2503.10725)|**[link](https://github.com/guqiqi/Samoyeds)**|
|**2025-03-19**|**dFLMoE: Decentralized Federated Learning via Mixture of Experts for Medical Data Analysis**|Luyuan Xie et.al.|[2503.10412](http://arxiv.org/abs/2503.10412)|null|
|**2025-03-12**|**Double-Stage Feature-Level Clustering-Based Mixture of Experts Framework**|Bakary Badjie et.al.|[2503.09504](http://arxiv.org/abs/2503.09504)|null|
|**2025-03-12**|**Astrea: A MOE-based Visual Understanding Model with Progressive Alignment**|Xiaoda Yang et.al.|[2503.09445](http://arxiv.org/abs/2503.09445)|null|
|**2025-03-12**|**Priority-Aware Preemptive Scheduling for Mixed-Priority Workloads in MoE Inference**|Mohammad Siavashi et.al.|[2503.09304](http://arxiv.org/abs/2503.09304)|null|
|**2025-03-11**|**MoE-Loco: Mixture of Experts for Multitask Locomotion**|Runhan Huang et.al.|[2503.08564](http://arxiv.org/abs/2503.08564)|null|
|**2025-03-11**|**Accelerating MoE Model Inference with Expert Sharding**|Oana Balmau et.al.|[2503.08467](http://arxiv.org/abs/2503.08467)|null|
|**2025-03-10**|**A Comprehensive Survey of Mixture-of-Experts: Algorithms, Theory, and Applications**|Siyuan Mu et.al.|[2503.07137](http://arxiv.org/abs/2503.07137)|**[link](https://github.com/deepseek-ai/DeepEP)**|
|**2025-03-10**|**ResMoE: Space-efficient Compression of Mixture of Experts LLMs via Residual Restoration**|Mengting Ai et.al.|[2503.06881](http://arxiv.org/abs/2503.06881)|**[link](https://github.com/idea-isail-lab-uiuc/resmoe)**|
|**2025-03-10**|**eMoE: Task-aware Memory Efficient Mixture-of-Experts-Based (MoE) Model Inference**|Suraiya Tairin et.al.|[2503.06823](http://arxiv.org/abs/2503.06823)|null|
|**2025-03-09**|**MoFE: Mixture of Frozen Experts Architecture**|Jean Seo et.al.|[2503.06491](http://arxiv.org/abs/2503.06491)|null|
|**2025-03-09**|**Swift Hydra: Self-Reinforcing Generative Framework for Anomaly Detection with Multiple Mamba Models**|Nguyen Do et.al.|[2503.06413](http://arxiv.org/abs/2503.06413)|**[link](https://github.com/nguyendohoangkhoiUF/Swift-Hydra)**|
|**2025-03-07**|**FMT:A Multimodal Pneumonia Detection Model Based on Stacking MOE Framework**|Jingyu Xu et.al.|[2503.05626](http://arxiv.org/abs/2503.05626)|null|
|**2025-03-07**|**Linear-MoE: Linear Sequence Modeling Meets Mixture-of-Experts**|Weigao Sun et.al.|[2503.05447](http://arxiv.org/abs/2503.05447)|**[link](https://github.com/opensparsellms/linear-moe)**|
|**2025-03-10**|**Every FLOP Counts: Scaling a 300B Mixture-of-Experts LING LLM without Premium GPUs**|Ling Team et.al.|[2503.05139](http://arxiv.org/abs/2503.05139)|null|
|**2025-03-07**|**Capacity-Aware Inference: Mitigating the Straggler Effect in Mixture of Experts**|Shwai He et.al.|[2503.05066](http://arxiv.org/abs/2503.05066)|null|
|**2025-03-06**|**Continual Pre-training of MoEs: How robust is your router?**|Benjamin Thérien et.al.|[2503.05029](http://arxiv.org/abs/2503.05029)|null|
|**2025-03-07**|**Question-Aware Gaussian Experts for Audio-Visual Question Answering**|Hongyeob Kim et.al.|[2503.04459](http://arxiv.org/abs/2503.04459)|**[link](https://github.com/AIM-SKKU/QA-TIGER)**|
|**2025-03-06**|**DM-Adapter: Domain-Aware Mixture-of-Adapters for Text-Based Person Retrieval**|Yating Liu et.al.|[2503.04144](http://arxiv.org/abs/2503.04144)|null|
|**2025-03-05**|**Convergence Rates for Softmax Gating Mixture of Experts**|Huy Nguyen et.al.|[2503.03213](http://arxiv.org/abs/2503.03213)|null|
|**2025-03-04**|**MX-Font++: Mixture of Heterogeneous Aggregation Experts for Few-shot Font Generation**|Weihang Wang et.al.|[2503.02799](http://arxiv.org/abs/2503.02799)|**[link](https://github.com/stephensun11/mxfontpp)**|
|**2025-03-04**|**FinArena: A Human-Agent Collaboration Framework for Financial Market Analysis and Forecasting**|Congluo Xu et.al.|[2503.02692](http://arxiv.org/abs/2503.02692)|null|
|**2025-03-04**|**Union of Experts: Adapting Hierarchical Routing to Equivalently Decomposed Transformer**|Yujiao Yang et.al.|[2503.02495](http://arxiv.org/abs/2503.02495)|**[link](https://github.com/yujiaoyang-work/uoe)**|
|**2025-03-03**|**ECG-EmotionNet: Nested Mixture of Expert (NMoE) Adaptation of ECG-Foundation Model for Driver Emotion Recognition**|Nastaran Mansourian et.al.|[2503.01750](http://arxiv.org/abs/2503.01750)|null|
|**2025-03-03**|**DeRS: Towards Extremely Efficient Upcycled Mixture-of-Experts Models**|Yongqi Huang et.al.|[2503.01359](http://arxiv.org/abs/2503.01359)|null|
|**2025-03-03**|**PROPER: A Progressive Learning Framework for Personalized Large Language Models with Group-Level Adaptation**|Linhai Zhang et.al.|[2503.01303](http://arxiv.org/abs/2503.01303)|null|
|**2025-03-02**|**Explainable Classifier for Malignant Lymphoma Subtyping via Cell Graph and Image Fusion**|Daiki Nishiyama et.al.|[2503.00925](http://arxiv.org/abs/2503.00925)|null|
|**2025-03-01**|**Efficiently Editing Mixture-of-Experts Models with Compressed Experts**|Yifei He et.al.|[2503.00634](http://arxiv.org/abs/2503.00634)|null|
|**2025-02-28**|**CoSMoEs: Compact Sparse Mixture of Experts**|Patrick Huber et.al.|[2503.00245](http://arxiv.org/abs/2503.00245)|null|
|**2025-03-01**|**R2-T2: Re-Routing in Test-Time for Multimodal Mixture-of-Experts**|Zhongyang Li et.al.|[2502.20395](http://arxiv.org/abs/2502.20395)|**[link](https://github.com/tianyi-lab/R2-T2)**|
|**2025-02-27**|**Mixture of Experts for Recognizing Depression from Interview and Reading Tasks**|Loukas Ilias et.al.|[2502.20213](http://arxiv.org/abs/2502.20213)|null|
|**2025-02-27**|**Mixture of Experts-augmented Deep Unfolding for Activity Detection in IRS-aided Systems**|Zeyi Ren et.al.|[2502.20183](http://arxiv.org/abs/2502.20183)|null|
|**2025-03-01**|**Comet: Fine-grained Computation-communication Overlapping for Mixture-of-Experts**|Shulai Zhang et.al.|[2502.19811](http://arxiv.org/abs/2502.19811)|**[link](https://github.com/bytedance/flux)**|
|**2025-02-26**|**Drop-Upcycling: Training Sparse Mixture of Experts with Partial Re-initialization**|Taishi Nakamura et.al.|[2502.19261](http://arxiv.org/abs/2502.19261)|null|
|**2025-02-26**|**OneRec: Unifying Retrieve and Rank with Generative Recommender and Iterative Preference Alignment**|Jiaxin Deng et.al.|[2502.18965](http://arxiv.org/abs/2502.18965)|null|
|**2025-02-25**|**Generative AI-enabled Wireless Communications for Robust Low-Altitude Economy Networking**|Changyuan Zhao et.al.|[2502.18118](http://arxiv.org/abs/2502.18118)|null|
|**2025-02-24**|**The Empirical Impact of Reducing Symmetries on the Performance of Deep Ensembles and MoE**|Andrei Chernov et.al.|[2502.17391](http://arxiv.org/abs/2502.17391)|null|
|**2025-02-24**|**Delta Decompression for MoE-based LLMs Compression**|Hao Gu et.al.|[2502.17298](http://arxiv.org/abs/2502.17298)|**[link](https://github.com/lliai/d2moe)**|
|**2025-02-24**|**Evaluating Expert Contributions in a MoE LLM for Quiz-Based Tasks**|Andrei Chernov et.al.|[2502.17187](http://arxiv.org/abs/2502.17187)|null|
|**2025-02-24**|**Muon is Scalable for LLM Training**|Jingyuan Liu et.al.|[2502.16982](http://arxiv.org/abs/2502.16982)|**[link](https://github.com/KellerJordan/Muon)**|
|**2025-02-24**|**BigMac: A Communication-Efficient Mixture-of-Experts Model Structure for Fast Training and Inference**|Zewen Jin et.al.|[2502.16927](http://arxiv.org/abs/2502.16927)|null|
|**2025-02-24**|**ENACT-Heart -- ENsemble-based Assessment Using CNN and Transformer on Heart Sounds**|Jiho Han et.al.|[2502.16914](http://arxiv.org/abs/2502.16914)|null|
|**2025-02-26**|**Make LoRA Great Again: Boosting LoRA with Adaptive Singular Values and Mixture-of-Experts Optimization Alignment**|Chenghao Fan et.al.|[2502.16894](http://arxiv.org/abs/2502.16894)|null|
|**2025-02-22**|**An Autonomous Network Orchestration Framework Integrating Large Language Models with Continual Reinforcement Learning**|Masoud Shokrnezhad et.al.|[2502.16198](http://arxiv.org/abs/2502.16198)|null|
|**2025-02-21**|**Tight Clusters Make Specialized Experts**|Stefan K. Nielsen et.al.|[2502.15315](http://arxiv.org/abs/2502.15315)|**[link](https://github.com/stefvk/acmoe)**|
|**2025-02-20**|**Ray-Tracing for Conditionally Activated Neural Networks**|Claudio Gallicchio et.al.|[2502.14788](http://arxiv.org/abs/2502.14788)|null|
|**2025-02-19**|**Unraveling the Localized Latents: Learning Stratified Manifold Structures in LLM Embedding Space with Sparse Mixture-of-Experts**|Xin Li et.al.|[2502.13577](http://arxiv.org/abs/2502.13577)|null|
|**2025-02-18**|**MoBA: Mixture of Block Attention for Long-Context LLMs**|Enzhe Lu et.al.|[2502.13189](http://arxiv.org/abs/2502.13189)|**[link](https://github.com/moonshotai/moba)**|
|**2025-02-18**|**Every Expert Matters: Towards Effective Knowledge Distillation for Mixture-of-Experts Language Models**|Gyeongman Kim et.al.|[2502.12947](http://arxiv.org/abs/2502.12947)|null|
|**2025-02-17**|**Accurate Expert Predictions in MoE Inference via Cross-Layer Gate**|Zhiyuan Fang et.al.|[2502.12224](http://arxiv.org/abs/2502.12224)|null|
|**2025-02-16**|**ClimateLLM: Efficient Weather Forecasting via Frequency-Aware Large Language Models**|Shixuan Li et.al.|[2502.11059](http://arxiv.org/abs/2502.11059)|null|
|**2025-02-15**|**Semantic Specialization in MoE Appears with Scale: A Study of DeepSeek R1 Expert Specialization**|Matthew Lyle Olson et.al.|[2502.10928](http://arxiv.org/abs/2502.10928)|null|
|**2025-02-11**|**MoHAVE: Mixture of Hierarchical Audio-Visual Experts for Robust Speech Recognition**|Sungnyun Kim et.al.|[2502.10447](http://arxiv.org/abs/2502.10447)|null|
|**2025-02-12**|**Heterogeneous Mixture of Experts for Remote Sensing Image Super-Resolution**|Bowen Chen et.al.|[2502.09654](http://arxiv.org/abs/2502.09654)|null|
|**2025-02-12**|**The MoE-Empowered Edge LLMs Deployment: Architecture, Challenges, and Opportunities**|Ning Li et.al.|[2502.08381](http://arxiv.org/abs/2502.08381)|null|
|**2025-02-12**|**Mixture of Decoupled Message Passing Experts with Entropy Constraint for General Node Classification**|Xuanze Chen et.al.|[2502.08083](http://arxiv.org/abs/2502.08083)|null|
|**2025-02-13**|**Training Sparse Mixture Of Experts Text Embedding Models**|Zach Nussbaum et.al.|[2502.07972](http://arxiv.org/abs/2502.07972)|**[link](https://github.com/nomic-ai/contrastors)**|
|**2025-02-09**|**Klotski: Efficient Mixture-of-Expert Inference via Expert-Aware Multi-Batch Pipeline**|Zhiyuan Fang et.al.|[2502.06888](http://arxiv.org/abs/2502.06888)|null|
|**2025-02-10**|**MoETuner: Optimized Mixture of Expert Serving with Balanced Expert Placement and Token Routing**|Seokjin Go et.al.|[2502.06643](http://arxiv.org/abs/2502.06643)|null|
|**2025-02-10**|**Jakiro: Boosting Speculative Decoding with Decoupled Multi-Head via MoE**|Haiduo Huang et.al.|[2502.06282](http://arxiv.org/abs/2502.06282)|**[link](https://github.com/haiduo/Jakiro)**|
|**2025-02-08**|**Mol-MoE: Training Preference-Guided Routers for Molecule Generation**|Diego Calanzone et.al.|[2502.05633](http://arxiv.org/abs/2502.05633)|null|
|**2025-02-07**|**fMoE: Fine-Grained Expert Offloading for Large Mixture-of-Experts Serving**|Hanfei Yu et.al.|[2502.05370](http://arxiv.org/abs/2502.05370)|null|
|**2025-02-07**|**Towards Foundational Models for Dynamical System Reconstruction: Hierarchical Meta-Learning via Mixture of Experts**|Roussel Desmond Nzoyem et.al.|[2502.05335](http://arxiv.org/abs/2502.05335)|null|
|**2025-02-07**|**Joint MoE Scaling Laws: Mixture of Experts Can Be Memory Efficient**|Jan Ludziejewski et.al.|[2502.05172](http://arxiv.org/abs/2502.05172)|null|
|**2025-02-06**|**Mixture of neural operator experts for learning boundary conditions and model selection**|Dwyer Deighan et.al.|[2502.04562](http://arxiv.org/abs/2502.04562)|null|
|**2025-02-06**|**CMoE: Fast Carving of Mixture-of-Experts for Efficient LLM Inference**|Zehua Pei et.al.|[2502.04416](http://arxiv.org/abs/2502.04416)|**[link](https://github.com/JarvisPei/CMoE)**|
|**2025-02-06**|**Rank Also Matters: Hierarchical Configuration for Mixture of Adapter Experts in LLM Fine-Tuning**|Peizhuang Cong et.al.|[2502.03884](http://arxiv.org/abs/2502.03884)|null|
|**2025-02-05**|**(GG) MoE vs. MLP on Tabular Data**|Andrei Chernov et.al.|[2502.03608](http://arxiv.org/abs/2502.03608)|null|
|**2025-02-05**|**Scaling Laws for Upcycling Mixture-of-Experts Language Models**|Seng Pei Liew et.al.|[2502.03009](http://arxiv.org/abs/2502.03009)|null|
|**2025-02-04**|**ReGNet: Reciprocal Space-Aware Long-Range Modeling and Multi-Property Prediction for Crystals**|Jianan Nie et.al.|[2502.02748](http://arxiv.org/abs/2502.02748)|null|
|**2025-02-04**|**Hecate: Unlocking Efficient Sparse Model Training via Fully Sharded Sparse Data Parallelism**|Yuhao Qing et.al.|[2502.02581](http://arxiv.org/abs/2502.02581)|null|
|**2025-02-07**|**Brief analysis of DeepSeek R1 and its implications for Generative AI**|Sarah Mercer et.al.|[2502.02523](http://arxiv.org/abs/2502.02523)|null|
|**2025-02-04**|**M2R2: Mixture of Multi-Rate Residuals for Efficient Transformer Inference**|Nikhil Bhendawade et.al.|[2502.02040](http://arxiv.org/abs/2502.02040)|null|
|**2025-02-05**|**MJ-VIDEO: Fine-Grained Benchmarking and Rewarding Video Preferences in Video Generation**|Haibo Tong et.al.|[2502.01719](http://arxiv.org/abs/2502.01719)|null|
|**2025-02-04**|**MergeME: Model Merging Techniques for Homogeneous and Heterogeneous MoEs**|Yuhang Zhou et.al.|[2502.00997](http://arxiv.org/abs/2502.00997)|null|
|**2025-02-03**|**CLIP-UP: A Simple and Efficient Mixture-of-Experts CLIP Training Recipe with Sparse Upcycling**|Xinze Wang et.al.|[2502.00965](http://arxiv.org/abs/2502.00965)|null|
|**2025-02-02**|**UniGraph2: Learning a Unified Embedding Space to Bind Multimodal Graphs**|Yufei He et.al.|[2502.00806](http://arxiv.org/abs/2502.00806)|null|
|**2025-01-29**|**Free Agent in Agent-Based Mixture-of-Experts Generative AI Framework**|Jung-Hua Liu et.al.|[2501.17903](http://arxiv.org/abs/2501.17903)|null|
|**2025-01-29**|**Heuristic-Informed Mixture of Experts for Link Prediction in Multilayer Networks**|Lucio La Cava et.al.|[2501.17557](http://arxiv.org/abs/2501.17557)|null|
|**2025-01-28**|**3D-MoE: A Mixture-of-Experts Multi-modal LLM for 3D Vision and Pose Diffusion via Rectified Flow**|Yueen Ma et.al.|[2501.16698](http://arxiv.org/abs/2501.16698)|null|
|**2025-01-27**|**MoEVD: Enhancing Vulnerability Detection by Mixture-of-Experts (MoE)**|Xu Yang et.al.|[2501.16454](http://arxiv.org/abs/2501.16454)|null|
|**2025-01-27**|**Static Batching of Irregular Workloads on GPUs: Framework and Application to Efficient MoE Model Inference**|Yinghan Li et.al.|[2501.16103](http://arxiv.org/abs/2501.16103)|null|
|**2025-01-25**|**ToMoE: Converting Dense Large Language Models to Mixture-of-Experts through Dynamic Structural Pruning**|Shangqian Gao et.al.|[2501.15316](http://arxiv.org/abs/2501.15316)|null|
|**2025-01-25**|**Each Rank Could be an Expert: Single-Ranked Mixture of Experts LoRA for Multi-Task Learning**|Ziyu Zhao et.al.|[2501.15103](http://arxiv.org/abs/2501.15103)|null|
|**2025-01-24**|**Mean-field limit from general mixtures of experts to quantum neural networks**|Anderson Melchor Hernandez et.al.|[2501.14660](http://arxiv.org/abs/2501.14660)|null|
|**2025-01-30**|**Hierarchical Time-Aware Mixture of Experts for Multi-Modal Sequential Recommendation**|Shengzhe Zhang et.al.|[2501.14269](http://arxiv.org/abs/2501.14269)|**[link](https://github.com/SStarCCat/HM4SR)**|
|**2025-01-23**|**CSAOT: Cooperative Multi-Agent System for Active Object Tracking**|Hy Nguyen et.al.|[2501.13994](http://arxiv.org/abs/2501.13994)|null|
|**2025-01-22**|**Autonomy-of-Experts Models**|Ang Lv et.al.|[2501.13074](http://arxiv.org/abs/2501.13074)|null|
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
|**2024-12-23**|**BrainMAP: Learning Multiple Activation Pathways in Brain Networks**|Song Wang et.al.|[2412.17404](http://arxiv.org/abs/2412.17404)|**[link](https://github.com/lzyfischer/brainmap)**|
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

<p align=right>(<a href=#updated-on-20250404>back to top</a>)</p>

## SSMs

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-04-03**|**State-Space Model Inspired Multiple-Input Multiple-Output Spiking Neurons**|Sanja Karilanova et.al.|[2504.02591](http://arxiv.org/abs/2504.02591)|null|在脉冲神经网络（SNNs）中，信息处理的主要单元是具有内部状态的神经元。内部状态根据其与膜电位相关的成分生成输出脉冲，该脉冲随后被传递给网络中的其他神经元。在这里，我们提出了一种通用的多输入多输出（MIMO）脉冲神经元模型，该模型超越了SNN文献中传统的单输入单输出（SISO）模型。我们提出的框架基于将神经元解释为具有线性状态演化和非线性脉冲激活函数的状态空间模型（SSMs）。我们展示了所提出的受SSM启发的神经元模型的各种参数之间的权衡，例如隐藏神经元状态的数量、输入和输出通道的数量，包括单输入多输出（SIMO）和多输入单输出（MISO）模型。我们表明，对于具有少量但内部状态空间较大的神经元的SNN，通过增加神经元的输出通道数量可以获得显著的性能提升。特别是，具有多个输出通道的脉冲神经元网络可以在相同的参考网络架构上达到与使用连续值通信的基线相同的准确度水平。|
|**2025-04-02**|**Mesh Mamba: A Unified State Space Model for Saliency Prediction in Non-Textured and Textured Meshes**|Kaiwei Zhang et.al.|[2504.01466](http://arxiv.org/abs/2504.01466)|**[link](https://github.com/kaviezhang/meshmamba)**|**网格显著性通过识别并强调自然吸引视觉注意力的区域来增强3D视觉的适应性。为了研究几何结构和纹理在塑造视觉注意力方面的相互作用，我们建立了一个全面的网格显著性数据集，这是首次系统地捕捉在有纹理和无纹理视觉条件下的显著性分布差异。此外，我们引入了基于状态空间模型（SSM）的统一显著性预测模型——网格曼巴，该模型设计用于适应各种类型的网格。网格曼巴有效地分析了网格的几何结构，同时无缝地将纹理特征融入拓扑框架中，确保在整个外观增强建模过程中的一致性。更重要的是，通过子图嵌入和双向SSM，该模型能够对局部几何和纹理进行全局上下文建模，保持拓扑结构，并提高对视觉细节和结构复杂性的理解。通过广泛的理论和实证验证，我们的模型不仅在各种网格类型上提高了性能，还展示了高度的可扩展性和通用性，特别是在各种视觉特征的交叉验证中。**|
|**2025-04-01**|**Scaling Up Resonate-and-Fire Networks for Fast Deep Learning**|Thomas E. Huber et.al.|[2504.00719](http://arxiv.org/abs/2504.00719)|null|脉冲神经网络（SNNs）为基于事件的传感器数据的神经形态处理提供了一种有前景的计算范式。特别是共振-放电（RF）神经元，因其生物学合理性、复杂动力学和计算简单性而具有吸引力。尽管理论上预测了其优点，但参数初始化和高效学习方面的挑战阻碍了RF网络的实现，限制了它们仅用于单层网络。在本文中，我们通过从HiPPO框架推导出RF神经元作为结构化状态空间模型（SSM），解决了这些不足。我们引入了S5-RF，这是一种基于S5模型的由RF神经元组成的新SSM层，它具有通用初始化方案，并能在深度架构中快速训练。S5-RF首次将RF网络扩展到多达四层的深度SNN，并在不到三个小时的训练时间内，在Spiking Speech Commands数据集上达到了78.8%的新最先进结果。此外，与解决我们基准测试任务的参考SNN相比，它以更少的脉冲操作实现了相似的性能。我们的代码公开发布在https://github.com/ThomasEHuber/s5-rf。|
|**2025-04-01**|**ParallelFlow: Parallelizing Linear Transformers via Flow Discretization**|Nicola Muca Cirone et.al.|[2504.00492](http://arxiv.org/abs/2504.00492)|null|我们提出了一种通过矩阵值状态空间模型（SSM）分析线性注意力模型的理论框架。我们的方法，称为并行流，提供了一个系统地将时间动态与实现约束解耦的视角，从而能够独立分析关键算法组件：分块、并行化和信息聚合。该框架的核心是将分块过程重新解释为计算系统动态的流。这一联系建立了通往粗糙路径理论数学工具的桥梁，为序列建模架构提供了新的见解。作为具体应用，我们在受近期理论进展启发的广义低秩设置下分析了DeltaNet。我们的方法使我们能够设计文献中现有的硬件高效算法的简单、精简的泛化版本，并且能够提供完全不同的算法，这些新算法受到粗糙路径技术的启发，并具有可证明的更低复杂度。这种双重贡献展示了有原则的理论分析不仅可以解释现有的实用方法，还可以启发根本性的新计算方法。|
|**2025-03-31**|**TransMamba: Flexibly Switching between Transformer and Mamba**|Yixing Li et.al.|[2503.24067](http://arxiv.org/abs/2503.24067)|null|Transformers 是现代大型语言模型的基石，但其二次计算复杂性限制了长序列处理的效率。最近在 Mamba 方面的进展，作为一种具有线性复杂度的状态空间模型（SSM），虽然提供了有希望的效率提升，但在上下文学习和多任务泛化方面存在不稳定性。本文提出了一种新的框架 TransMamba，通过共享参数矩阵（例如 QKV 和 CBx）统一了 Transformer 和 Mamba，从而能够在不同的令牌长度和层之间动态切换注意力机制和 SSM 机制。我们设计了记忆转换器来桥接 Transformer 和 Mamba，通过将注意力输出转换为 SSM 兼容的状态，在转换点（TransPoints）处确保无缝的信息流动。还对 TransPoint 调度进行了深入探索以进一步改进。我们进行了广泛的实验，证明 TransMamba 在训练效率和性能上优于基线，并验证了 Transformer 和 Mamba 范式之间的更深层次的一致性，为下一代序列建模提供了一个可扩展的解决方案。|
|**2025-03-31**|**Free Parametrization of L2-bounded State Space Models**|Leonardo Massai et.al.|[2503.23818](http://arxiv.org/abs/2503.23818)|null|结构化状态空间模型（SSM）作为一种强大的架构在机器学习和控制领域中崭露头角，其特征是堆叠的层，每层由一个线性时不变（LTI）离散时间系统后跟一个非线性函数组成。虽然SSM提供了计算效率并在长序列预测方面表现出色，但其在系统识别和最优控制等应用中的广泛应用受到稳定性和鲁棒性保证的挑战。我们引入了L2RU，这是一种新的SSM参数化方法，通过强制规定所有参数值下的L界来保证输入-输出稳定性和鲁棒性。这种设计消除了对复杂约束的需求，允许使用标准方法如梯度下降进行无约束优化。利用系统理论和凸优化工具，我们推导出具有指定L2界的平方离散时间LTI系统的非保守参数化，这是L2RU架构的基础。此外，我们通过一种针对长输入序列优化的定制初始化策略进一步提升了其性能。通过系统识别任务，我们验证了L2RU的优越性能，展示了其在学习和控制应用中的潜力。|
|**2025-03-29**|**Fast Training of Recurrent Neural Networks with Stationary State Feedbacks**|Paul Caillon et.al.|[2503.23104](http://arxiv.org/abs/2503.23104)|**[link](https://github.com/p0lcai/dsf)**|**循环神经网络（RNN）最近在性能上表现出色，并且在相似参数预算下比Transformer具有更快的推理速度。然而，基于反向传播通过时间（BPTT）算法的递归梯度计算仍然是主要的计算瓶颈。在这项工作中，我们提出了一种新方法，用固定梯度反馈机制替代BPTT，从而在假设时间平稳性的基础上提供精确梯度传播的有效近似。我们的方法利用状态空间模型（SSM）原理定义了一个结构化的反馈矩阵，该矩阵直接从未来时间步传播梯度。这种公式绕过了递归梯度反向传播的需求，显著减少了训练开销，同时保持了网络捕捉长期依赖关系的能力。在语言建模基准测试中的实验显示了具有竞争力的困惑度分数，同时大幅降低了训练成本。这些有希望的结果表明，设计类似SSM的反馈方法可以充分利用RNN在许多实际应用中的效率优势。**|
|**2025-03-29**|**SSM-RDU: A Reconfigurable Dataflow Unit for Long-Sequence State-Space Models**|Sho Ko et.al.|[2503.22937](http://arxiv.org/abs/2503.22937)|null|长序列状态空间模型（如Hyena和Mamba）通过使用更高效的FFT和扫描操作取代了自注意力机制的二次复杂度。然而，现代加速器如GPU由于其刚性的执行模型和对密集矩阵运算的优化，并不适合这些非GEMM工作负载。本文提出了一种基于基线可重构数据流单元（RDU）的架构扩展，以高效支持基于FFT和扫描操作的状态空间模型。通过在计算模块中引入轻量级互连增强，扩展后的RDU能够以低于1%的面积和功耗开销实现FFT和扫描数据流的空间映射。最终，该架构在Hyena上相比GPU实现了5.95倍的速度提升，相比基线RDU实现了1.95倍的速度提升；在Mamba上分别相比GPU和基线RDU实现了2.12倍和1.75倍的速度提升。|
|**2025-04-03**|**Quamba2: A Robust and Scalable Post-training Quantization Framework for Selective State Space Models**|Hung-Yueh Chiang et.al.|[2503.22879](http://arxiv.org/abs/2503.22879)|**[link](https://github.com/enyac-group/quamba)**|**状态空间模型（SSM）由于其一致的内存使用和高性能，正在成为Transformer的一个有吸引力的替代方案。然而，由于存储需求和计算能力的要求，在云服务或资源有限的设备上扩展SSM是具有挑战性的。为了克服这一点，通过低比特宽度数据格式量化SSM可以减少模型大小，并从硬件加速中受益。尽管如此，SSM容易受到量化引起的误差影响，最近的努力集中在优化特定模型或比特宽度以提高效率而不牺牲性能。然而，对于不同的场景需要不同的比特宽度配置，比如W4A8用于提升大批量解码速度，而W4A16则用于增强短提示应用中单用户生成速度。为此，我们提出了Quamba2，它兼容W8A8、W4A8和W4A16，适用于Mamba1和Mamba2骨架，满足了在各种平台上部署SSM日益增长的需求。基于SSM的通道顺序保持和激活持久性，我们提出了一种离线方法，通过对输入 $x$进行排序和聚类来将其量化为8位，并结合每个状态组对输入依赖参数$B$和$C$ 进行量化。为了确保SSM输出中的计算不变性，我们根据聚类序列离线重新排列权重。实验表明，Quamba2-8B超越了多个最先进的SSM量化方法，在预填充和生成阶段分别实现了1.3倍和3倍的速度提升，同时提供了4倍的内存减少，平均精度仅下降了1.6%。在MMLU上的评估展示了我们框架的通用性和鲁棒性。代码和量化模型将在以下网址发布：https://github.com/enyac-group/Quamba。**|
|**2025-04-02**|**Q-MambaIR: Accurate Quantized Mamba for Efficient Image Restoration**|Yujie Chen et.al.|[2503.21970](http://arxiv.org/abs/2503.21970)|null|状态空间模型（SSM）由于能够在线性序列长度上扩展同时有效捕捉长距离依赖关系，在图像恢复（IR）领域受到了广泛关注。然而，将SSM部署到边缘设备上具有挑战性，因为这些设备在内存、计算能力和功耗方面存在限制，这突显了高效压缩策略的需求。虽然低比特量化是一种有效的模型压缩策略，可以减少模型大小并加速IR任务，但当使用超低比特宽度（2-4位）时，SSM会遭受显著的性能下降，主要原因是异常值加剧了量化误差。为了解决这一挑战，我们提出了Q-MambaIR，这是一种准确、高效且灵活的用于图像恢复任务的量化Mamba方法。具体来说，我们引入了一种统计动态平衡可学习标量（DLS），以动态调整量化映射范围，从而减轻由极端值引起的峰值截断损失。此外，我们设计了一种带有自适应阈值的范围浮动灵活分配器（RFA），以灵活地进行数值舍入。这种方法保留了高频细节，并保持了SSM的特征提取能力。值得注意的是，RFA还支持预部署权重量化，在计算效率和模型准确性之间取得了平衡。大量实验表明，在图像恢复任务中，Q-MambaIR始终优于现有的量化SSM，实现了更高的最先进（SOTA）精度结果，同时仅需微不足道的额外训练计算成本和存储节省。|
|**2025-03-27**|**vGamba: Attentive State Space Bottleneck for efficient Long-range Dependencies in Visual Recognition**|Yunusa Haruna et.al.|[2503.21262](http://arxiv.org/abs/2503.21262)|**[link](https://github.com/yunusa2k2/vGamba)**|
|**2025-03-26**|**ReverBERT: A State Space Model for Efficient Text-Driven Speech Style Transfer**|Michael Brown et.al.|[2503.20992](http://arxiv.org/abs/2503.20992)|null|
|**2025-03-25**|**A Comprehensive Analysis of Mamba for 3D Volumetric Medical Image Segmentation**|Chaohan Wang et.al.|[2503.19308](http://arxiv.org/abs/2503.19308)|null|
|**2025-03-22**|**A Survey on Structured State Space Sequence (S4) Models**|Shriyank Somvanshi et.al.|[2503.18970](http://arxiv.org/abs/2503.18970)|null|
|**2025-03-24**|**Exploring State Space Model in Wavelet Domain: An Infrared and Visible Image Fusion Network via Wavelet Transform and State Space Model**|Tianpei Zhang et.al.|[2503.18378](http://arxiv.org/abs/2503.18378)|null|
|**2025-03-23**|**GLADMamba: Unsupervised Graph-Level Anomaly Detection Powered by Selective State Space Model**|Yali Fu et.al.|[2503.17903](http://arxiv.org/abs/2503.17903)|**[link](https://github.com/yali-f/gladmamba)**|
|**2025-03-21**|**MM-UNet: Meta Mamba UNet for Medical Image Segmentation**|Bin Xie et.al.|[2503.17540](http://arxiv.org/abs/2503.17540)|null|
|**2025-03-24**|**An Energy-Adaptive Elastic Equivariant Transformer Framework for Protein Structure Representation**|Zhongyue Zhang et.al.|[2503.16996](http://arxiv.org/abs/2503.16996)|null|
|**2025-03-20**|**SaMam: Style-aware State Space Model for Arbitrary Image Style Transfer**|Hongda Liu et.al.|[2503.15934](http://arxiv.org/abs/2503.15934)|null|
|**2025-03-19**|**State Space Model Meets Transformer: A New Paradigm for 3D Object Detection**|Chuxin Wang et.al.|[2503.14493](http://arxiv.org/abs/2503.14493)|null|
|**2025-03-20**|**MambaIC: State Space Models for High-Performance Learned Image Compression**|Fanhu Zeng et.al.|[2503.12461](http://arxiv.org/abs/2503.12461)|**[link](https://github.com/aurorazengfh/mambaic)**|
|**2025-03-15**|**Text-Driven Video Style Transfer with State-Space Models: Extending StyleMamba for Temporal Coherence**|Chao Li et.al.|[2503.12291](http://arxiv.org/abs/2503.12291)|null|
|**2025-03-15**|**A State Alignment-Centric Approach to Federated System Identification: The FedAlign Framework**|Ertuğrul Keçeci et.al.|[2503.12137](http://arxiv.org/abs/2503.12137)|null|
|**2025-03-18**|**UniMamba: Unified Spatial-Channel Representation Learning with Group-Efficient Mamba for LiDAR-based 3D Object Detection**|Xin Jin et.al.|[2503.12009](http://arxiv.org/abs/2503.12009)|null|
|**2025-03-14**|**Technologies on Effectiveness and Efficiency: A Survey of State Spaces Models**|Xingtai Lv et.al.|[2503.11224](http://arxiv.org/abs/2503.11224)|null|
|**2025-03-13**|**Trajectory Mamba: Efficient Attention-Mamba Forecasting Model Based on Selective SSM**|Yizhou Huang et.al.|[2503.10898](http://arxiv.org/abs/2503.10898)|null|
|**2025-03-13**|**Fixed-Point RNNs: From Diagonal to Dense in a Few Iterations**|Sajad Movahedi et.al.|[2503.10799](http://arxiv.org/abs/2503.10799)|null|
|**2025-03-11**|**MinGRU-Based Encoder for Turbo Autoencoder Frameworks**|Rick Fritschek et.al.|[2503.08451](http://arxiv.org/abs/2503.08451)|null|
|**2025-03-10**|**SegResMamba: An Efficient Architecture for 3D Medical Image Segmentation**|Badhan Kumar Das et.al.|[2503.07766](http://arxiv.org/abs/2503.07766)|null|
|**2025-03-09**|**Global-Aware Monocular Semantic Scene Completion with State Space Models**|Shijie Li et.al.|[2503.06569](http://arxiv.org/abs/2503.06569)|null|
|**2025-03-09**|**Future-Aware Interaction Network For Motion Forecasting**|Shijie Li et.al.|[2503.06565](http://arxiv.org/abs/2503.06565)|null|
|**2025-03-13**|**Spectral State Space Model for Rotation-Invariant Visual Representation Learning**|Sahar Dastani et.al.|[2503.06369](http://arxiv.org/abs/2503.06369)|null|
|**2025-03-07**|**Novel Object 6D Pose Estimation with a Single Reference View**|Jian Liu et.al.|[2503.05578](http://arxiv.org/abs/2503.05578)|**[link](https://github.com/cnjianliu/sinref-6d)**|
|**2025-03-06**|**An Extended State Space Model of Aggregated Electric Vehicles for Flexibility Estimation and Power Control**|Yiping Liu et.al.|[2503.04714](http://arxiv.org/abs/2503.04714)|null|
|**2025-03-05**|**State-offset Tuning: State-based Parameter-Efficient Fine-Tuning for State Space Models**|Wonjun Kang et.al.|[2503.03499](http://arxiv.org/abs/2503.03499)|**[link](https://github.com/furiosa-ai/ssm-state-tuning)**|
|**2025-03-04**|**S4D-Bio Audio Monitoring of Bone Cement Disintegration in Pulsating Fluid Jet Surgery under Laboratory Conditions**|Melanie Schaller et.al.|[2503.02714](http://arxiv.org/abs/2503.02714)|null|
|**2025-03-04**|**SSNet: Saliency Prior and State Space Model-based Network for Salient Object Detection in RGB-D Images**|Gargi Panda et.al.|[2503.02270](http://arxiv.org/abs/2503.02270)|null|
|**2025-03-03**|**DCAMamba: Mamba-based Rapid Response DC Arc Fault Detection**|Lukun Wang et.al.|[2503.01264](http://arxiv.org/abs/2503.01264)|null|
|**2025-02-28**|**Visual Attention Exploration in Vision-Based Mamba Models**|Junpeng Wang et.al.|[2502.20764](http://arxiv.org/abs/2502.20764)|null|
|**2025-02-27**|**Accelerating Model-Based Reinforcement Learning with State-Space World Models**|Maria Krinner et.al.|[2502.20168](http://arxiv.org/abs/2502.20168)|null|
|**2025-02-26**|**On Pruning State-Space LLMs**|Tamer Ghattas et.al.|[2502.18886](http://arxiv.org/abs/2502.18886)|null|
|**2025-02-25**|**Revisiting Convolution Architecture in the Realm of DNA Foundation Models**|Yu Bo et.al.|[2502.18538](http://arxiv.org/abs/2502.18538)|null|
|**2025-02-24**|**PICASO: Permutation-Invariant Context Composition with State Space Models**|Tian Yu Liu et.al.|[2502.17605](http://arxiv.org/abs/2502.17605)|null|
|**2025-02-24**|**MambaFlow: A Novel and Flow-guided State Space Model for Scene Flow Estimation**|Jiehao Luo et.al.|[2502.16907](http://arxiv.org/abs/2502.16907)|**[link](https://github.com/scnu-rislab/mambaflow)**|
|**2025-02-22**|**Linear Attention for Efficient Bidirectional Sequence Modeling**|Arshia Afzal et.al.|[2502.16249](http://arxiv.org/abs/2502.16249)|**[link](https://github.com/lions-epfl/lion)**|
|**2025-02-22**|**Improving Speech Enhancement by Cross- and Sub-band Processing with State Space Model**|Jizhen Li et.al.|[2502.16207](http://arxiv.org/abs/2502.16207)|null|
|**2025-02-24**|**LaTIM: Measuring Latent Token-to-Token Interactions in Mamba Models**|Hugo Pitorro et.al.|[2502.15612](http://arxiv.org/abs/2502.15612)|null|
|**2025-02-21**|**LightMamba: Efficient Mamba Acceleration on FPGA with Quantization and Hardware Co-design**|Renjie Wei et.al.|[2502.15260](http://arxiv.org/abs/2502.15260)|null|
|**2025-02-20**|**Inferring System and Optimal Control Parameters of Closed-Loop Systems from Partial Observations**|Victor Geadah et.al.|[2502.15014](http://arxiv.org/abs/2502.15014)|null|
|**2025-02-18**|**DAMamba: Vision State Space Model with Dynamic Adaptive Scan**|Tanzhe Li et.al.|[2502.12627](http://arxiv.org/abs/2502.12627)|**[link](https://github.com/ltzovo/damamba)**|
|**2025-02-12**|**From Layers to States: A State Space Model Perspective to Deep Neural Network Layer Dynamics**|Qinshuo Liu et.al.|[2502.10463](http://arxiv.org/abs/2502.10463)|null|
|**2025-02-12**|**SS4Rec: Continuous-Time Sequential Recommendation with State Space Models**|Wei Xiao et.al.|[2502.08132](http://arxiv.org/abs/2502.08132)|null|
|**2025-02-14**|**Implicit Language Models are RNNs: Balancing Parallelization and Expressivity**|Mark Schöne et.al.|[2502.07827](http://arxiv.org/abs/2502.07827)|null|
|**2025-02-11**|**A Survey on Mamba Architecture for Vision Applications**|Fady Ibrahim et.al.|[2502.07161](http://arxiv.org/abs/2502.07161)|null|
|**2025-02-18**|**XAMBA: Enabling Efficient State Space Models on Resource-Constrained Neural Processing Units**|Arghadip Das et.al.|[2502.06924](http://arxiv.org/abs/2502.06924)|**[link](https://github.com/arghadippurdue/xamba)**|
|**2025-02-08**|**TrackDiffuser: Nearly Model-Free Bayesian Filtering with Diffusion Model**|Yangguang He et.al.|[2502.05629](http://arxiv.org/abs/2502.05629)|null|
|**2025-02-07**|**CMamba: Learned Image Compression with State Space Models**|Zhuojie Wu et.al.|[2502.04988](http://arxiv.org/abs/2502.04988)|null|
|**2025-02-07**|**SSMLoRA: Enhancing Low-Rank Adaptation with State Space Model**|Jiayang Yu et.al.|[2502.04958](http://arxiv.org/abs/2502.04958)|**[link](https://github.com/yuhkalhic/ssmlora)**|
|**2025-02-07**|**A Foundational Brain Dynamics Model via Stochastic Optimal Control**|Joonhyeong Park et.al.|[2502.04892](http://arxiv.org/abs/2502.04892)|null|
|**2025-02-01**|**Multilingual State Space Models for Structured Question Answering in Indic Languages**|Arpita Vats et.al.|[2502.01673](http://arxiv.org/abs/2502.01673)|**[link](https://github.com/mrinal18/MAMBA_QA)**|
|**2025-02-03**|**Generalization Error Analysis for Selective State-Space Models Through the Lens of Attention**|Arya Honarpisheh et.al.|[2502.01473](http://arxiv.org/abs/2502.01473)|null|
|**2025-02-03**|**Pushing the Boundaries of State Space Models for Image and Video Generation**|Yicong Hong et.al.|[2502.00972](http://arxiv.org/abs/2502.00972)|null|
|**2025-02-01**|**Fast Vision Mamba: Pooling Spatial Dimensions for Accelerated Processing**|Saarthak Kapse et.al.|[2502.00594](http://arxiv.org/abs/2502.00594)|null|
|**2025-02-01**|**Sub-Sequential Physics-Informed Learning with State Space Model**|Chenhui Xu et.al.|[2502.00318](http://arxiv.org/abs/2502.00318)|**[link](https://github.com/minihuihui/pinnmamba)**|
|**2025-02-01**|**A Study on the Performance of U-Net Modifications in Retroperitoneal Tumor Segmentation**|Moein Heidari et.al.|[2502.00314](http://arxiv.org/abs/2502.00314)|**[link](https://github.com/moeinheidari7829/Retroperitoneal_Tumour_Segmentation_SPIE2025)**|
|**2025-01-28**|**Mamba-Shedder: Post-Transformer Compression for Efficient Selective Structured State Space Models**|J. Pablo Muñoz et.al.|[2501.17088](http://arxiv.org/abs/2501.17088)|**[link](https://github.com/intellabs/hardware-aware-automated-machine-learning)**|
|**2025-01-28**|**Post-Training Quantization for Vision Mamba with k-Scaled Quantization and Reparameterization**|Bo-Yun Shi et.al.|[2501.16738](http://arxiv.org/abs/2501.16738)|null|
|**2025-01-27**|**Mixture-of-Mamba: Enhancing Multi-Modal State-Space Models with Modality-Aware Sparsity**|Weixin Liang et.al.|[2501.16295](http://arxiv.org/abs/2501.16295)|**[link](https://github.com/weixin-liang/mixture-of-mamba)**|
|**2025-01-27**|**Application of Structured State Space Models to High energy physics with locality-sensitive hashing**|Cheng Jiang et.al.|[2501.16237](http://arxiv.org/abs/2501.16237)|null|
|**2025-01-24**|**A Deep State Space Model for Rainfall-Runoff Simulations**|Yihan Wang et.al.|[2501.14980](http://arxiv.org/abs/2501.14980)|**[link](https://github.com/WESTENR-OU/S4D_rainfall_runoff_simulations)**|
|**2025-01-24**|**On the locality bias and results in the Long Range Arena**|Pablo Miralles-González et.al.|[2501.14850](http://arxiv.org/abs/2501.14850)|null|
|**2025-01-23**|**QMamba: Post-Training Quantization for Vision State Space Models**|Yinglong Li et.al.|[2501.13624](http://arxiv.org/abs/2501.13624)|null|
|**2025-01-22**|**Let SSMs be ConvNets: State-space Modeling with Optimal Tensor Contractions**|Yan Ru Pei et.al.|[2501.13230](http://arxiv.org/abs/2501.13230)|**[link](https://github.com/Brainchip-Inc/Centaurus)**|
|**2025-01-22**|**GRAMA: Adaptive Graph Autoregressive Moving Average Models**|Moshe Eliasof et.al.|[2501.12732](http://arxiv.org/abs/2501.12732)|null|
|**2025-01-21**|**Automatic selection of the best neural architecture for time series forecasting via multi-objective optimization and Pareto optimality conditions**|Qianying Cao et.al.|[2501.12215](http://arxiv.org/abs/2501.12215)|null|
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
|**2024-11-06**|**MambaPEFT: Exploring Parameter-Efficient Fine-Tuning for Mamba**|Masakazu Yoshimura et.al.|[2411.03855](http://arxiv.org/abs/2411.03855)|**[link](https://github.com/sony/MambaPEFT)**|
|**2024-11-05**|**A scalable generative model for dynamical system reconstruction from neuroimaging data**|Eric Volkmann et.al.|[2411.02949](http://arxiv.org/abs/2411.02949)|**[link](https://github.com/humml-lab/GTF-ConvSSM)**|
|**2024-11-05**|**Layer-Adaptive State Pruning for Deep State Space Models**|Minseon Gwak et.al.|[2411.02824](http://arxiv.org/abs/2411.02824)|**[link](https://github.com/msgwak/last)**|
|**2024-11-04**|**Recursive Learning of Asymptotic Variational Objectives**|Alessandro Mastrototaro et.al.|[2411.02217](http://arxiv.org/abs/2411.02217)|null|
|**2024-11-07**|**Birdie: Advancing State Space Models with Reward-Driven Objectives and Curricula**|Sam Blouir et.al.|[2411.01030](http://arxiv.org/abs/2411.01030)|**[link](https://github.com/samblouir/birdie)**|
|**2024-10-31**|**SambaMixer: State of Health Prediction of Li-ion Batteries using Mamba State Space Models**|José Ignacio Olalde-Verano et.al.|[2411.00233](http://arxiv.org/abs/2411.00233)|**[link](https://github.com/sascha-kirch/samba-mixer)**|
|**2024-10-31**|**Nudging state-space models for Bayesian filtering under misspecified dynamics**|Fabian Gonzalez et.al.|[2411.00218](http://arxiv.org/abs/2411.00218)|null|
|**2024-10-31**|**NIMBA: Towards Robust and Principled Processing of Point Clouds With SSMs**|Nursena Köprücü et.al.|[2411.00151](http://arxiv.org/abs/2411.00151)|null|
|**2024-10-31**|**In-Context Learned Equalization in Cell-Free Massive MIMO via State-Space Models**|Zihang Song et.al.|[2410.23882](http://arxiv.org/abs/2410.23882)|null|
|**2024-10-28**|**Multi-Agent Reinforcement Learning with Selective State-Space Models**|Jemma Daniel et.al.|[2410.19382](http://arxiv.org/abs/2410.19382)|null|

<p align=right>(<a href=#updated-on-20250404>back to top</a>)</p>

## Communication Intelligence

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-09-21**|**LLM Agents as 6G Orchestrator: A Paradigm for Task-Oriented Physical-Layer Automation**|Zhuoran Xiao et.al.|[2410.03688](http://arxiv.org/abs/2410.03688)|null|生成式预训练模型的快速发展正在推动技术进步从基础应用如聊天机器人向更复杂的基于代理的系统转变。将6G系统与大型语言模型（LLM）代理和数字孪生（DT）结合具有巨大的潜力和必要性，以管理具有新出现功能（如原生AI服务和感知）的高度复杂通信系统。通过6G导向的代理，基站可以理解各种动态上层任务的传输需求，自动编排最优系统工作流程。通过不断从6G DT获取反馈进行强化，代理最终能够相应地提高实际系统的性能。不同于现有的为通用应用设计的LLM代理，6G导向的代理旨在利用大量额外的专业知识进行高度严谨和精确的规划，这不可避免地需要从模型训练到实施的特定系统设计。本文提出了一种构建面向任务的6G LLM代理的新综合方法。我们首先提出了一种两阶段持续预训练和微调方案，以建立领域基础模型和多种专业专家模型，以满足各种应用场景的需求。此外，还提出了一种基于语义检索的新推理框架，以利用现有的通信相关功能。物理层任务分解等示例任务的实验结果表明了所提范式的可行性和有效性。|

<p align=right>(<a href=#updated-on-20250404>back to top</a>)</p>

## RAG

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-04-03**|**TeleMoM: Consensus-Driven Telecom Intelligence via Mixture of Models**|Xinquan Wang et.al.|[2504.02712](http://arxiv.org/abs/2504.02712)|null|大型语言模型（LLM）在电信等专业领域面临重大挑战，这些挑战源于技术复杂性、专业术语以及快速变化的知识。传统方法如扩大模型参数或在特定领域的语料库上重新训练计算成本高昂且收益递减，而现有的方法如检索增强生成、专家混合和微调在准确性、效率和协调方面存在困难。为了解决这个问题，我们提出了电信模型混合（TeleMoM），这是一种共识驱动的集成框架，通过整合多个LLM来提高电信领域的决策能力。TeleMoM采用两阶段流程：提议模型生成有理有据的回答，然后由裁决者做出最终决定，并辅以质量检查机制。这种方法利用了不同模型的优势来提高准确性、减少偏见并有效处理特定领域的复杂性。评估结果显示，TeleMoM将答案准确性提高了9.7%，突显了其在电信应用中的有效性。|
|**2025-04-03**|**Retrieval-Augmented Purifier for Robust LLM-Empowered Recommendation**|Liangbo Ning et.al.|[2504.02458](http://arxiv.org/abs/2504.02458)|null|最近，基于大型语言模型（LLM）的推荐系统彻底改变了个性化推荐框架，并引起了广泛关注。尽管取得了显著的成功，但现有的基于LLM的推荐系统已被证明极易受到微小扰动的影响。为了减轻这种脆弱性带来的负面影响，一个潜在的解决方案是利用基于物品-物品共现的协同信号，从攻击者插入的用户历史交互中净化恶意的协同知识。另一方面，由于检索增强生成（RAG）技术能够扩展LLM不足的内部知识，这为通过引入外部协同知识来增强基于LLM的推荐系统的鲁棒性提供了前所未有的机会。因此，在本文中，我们提出了一种新颖的框架RETURN，通过检索外部协同信号来净化被污染的用户画像，并以即插即用的方式增强基于LLM的推荐系统的鲁棒性。具体而言，我们提出了检索增强的扰动定位方法，通过从协同物品图中检索外部知识来识别用户历史序列中的潜在扰动。之后，我们进一步检索协同知识，通过删除或替换策略来清除这些扰动，并引入一种鲁棒的集成推荐策略来生成最终的鲁棒预测。在三个真实数据集上的大量实验表明了所提出的RETURN的有效性。|
|**2025-04-03**|**Adapting Large Language Models for Multi-Domain Retrieval-Augmented-Generation**|Alexandre Misrahi et.al.|[2504.02411](http://arxiv.org/abs/2504.02411)|null|检索增强生成（RAG）可以提高大型语言模型的事实准确性，但在多领域应用中面临挑战，如缺乏多样化的基准测试和较差的跨领域泛化能力。本工作的第一个贡献是引入了一个包含来自8个来源、涵盖13个领域的多种问答任务的多样化基准测试。我们的第二个贡献是系统地测试了典型的RAG调优策略在跨领域泛化方面的表现。虽然我们的发现表明标准微调无法有效泛化，但我们展示了使用教师生成的标签进行序列级蒸馏可以提高跨领域性能，因为它提供了更连贯的监督。我们的研究结果突出了提高多领域RAG鲁棒性的关键策略。|
|**2025-04-02**|**One Pic is All it Takes: Poisoning Visual Document Retrieval Augmented Generation with a Single Image**|Ezzeldin Shereen et.al.|[2504.02132](http://arxiv.org/abs/2504.02132)|null|多模态检索增强生成（M-RAG）最近作为一种通过事实知识库（KB）抑制大型多模态模型（LMMs）产生幻觉的方法而出现。然而，M-RAG也为攻击者引入了新的攻击途径，这些攻击者旨在通过向知识库中注入恶意条目来破坏系统。在这项工作中，我们提出了一种针对M-RAG的投毒攻击，目标是视觉文档检索应用，其中知识库包含文档页面的图像。我们的目标是制作一个单一的图像，该图像能够被多种不同的用户查询检索，并且始终影响生成模型产生的输出，从而对M-RAG系统发起一种通用的拒绝服务（DoS）攻击。我们展示了尽管我们的攻击对广泛使用、最先进的检索器（嵌入模型）和生成器（LMMs）有效，但对鲁棒性强的嵌入模型可能无效。我们的攻击不仅突显了M-RAG管道对投毒攻击的脆弱性，也揭示了一个潜在的基本弱点，即使在良性环境中也可能阻碍其性能。|
|**2025-04-02**|**CoRAG: Collaborative Retrieval-Augmented Generation**|Aashiq Muhamed et.al.|[2504.01883](http://arxiv.org/abs/2504.01883)|null|检索增强生成（RAG）模型在知识密集型任务中表现出色，尤其是在少样本学习约束下。我们提出了CoRAG框架，将RAG扩展到协作环境中，客户端通过协作段落存储库共同训练共享模型。为了评估CoRAG，我们引入了CRAB基准测试，用于协作同质开放领域问答。实验表明，在资源有限的情况下，CoRAG始终优于参数化协作学习方法和本地训练的RAG模型。进一步分析揭示了共享存储库中相关段落的关键重要性，以及引入无关段落的意外益处，同时指出硬负例可能对性能产生负面影响。这在协作RAG中引入了一个新的考量：利用集体丰富知识库与整合其他客户端潜在有害段落的风险之间的权衡。我们的研究结果强调了CoRAG的可行性，同时也突出了关键的设计挑战和未来研究的有前景方向。|
|**2025-04-02**|**From Code Generation to Software Testing: AI Copilot with Context-Based RAG**|Yuchen Wang et.al.|[2504.01866](http://arxiv.org/abs/2504.01866)|null|快速的大规模软件开发对传统测试方法提出了越来越高的要求，经常导致在效率、准确性和覆盖率方面出现瓶颈。我们提出了一种关于软件测试的新视角，认为减少错误和编写更少错误的代码是两个相互关联的问题，它们共享一个共同的目标，即在有限的资源下减少错误。我们将之前关于AI辅助编程的工作（支持代码自动补全和聊天机器人驱动的问答）扩展到软件测试领域。我们引入了用于测试的Copilot系统，该系统能够与代码库更新同步进行错误检测，并利用基于上下文的检索增强生成（RAG）来提升大型语言模型（LLMs）的能力。我们的评估显示，在错误检测准确性上提高了31.2%，关键测试覆盖率增加了12.6%，用户接受率提高了10.5%，这突显了AI驱动技术在现代软件开发实践中的变革潜力。|
|**2025-04-02**|**LARGE: Legal Retrieval Augmented Generation Evaluation Tool**|Minhu Park et.al.|[2504.01840](http://arxiv.org/abs/2504.01840)|**[link](https://github.com/hoorangyee/lrage)**|**最近，构建检索增强生成（RAG）系统以增强大型语言模型（LLM）的能力已成为一种常见做法。特别是在法律领域，先前的司法判决在遵循先例的原则下起着重要作用，这强调了基于（检索到的）先前文档作出决策的重要性。然而，RAG系统的整体性能取决于许多组件：(1) 检索语料库，(2) 检索算法，(3) 重排序器，(4) LLM骨干模型，以及(5) 评估指标。本文提出了LRAGE，一个专注于法律领域的开源工具，用于全面评估RAG系统。LRAGE提供了图形用户界面和命令行界面，以促进无缝实验，并研究上述五个组件的变化如何影响整体准确性。我们使用包括韩语（KBL）、英语（LegalBench）和中文（LawBench）在内的多语言法律基准验证了LRAGE，展示了当改变上述五个组件时，整体准确性的变化情况。源代码可在https://github.com/hoorangyee/LRAGE获取。**|
|**2025-04-02**|**Reasoning LLMs for User-Aware Multimodal Conversational Agents**|Hamed Rahimi et.al.|[2504.01700](http://arxiv.org/abs/2504.01700)|null|在社交机器人中，个性化对于促进有效的人机交互至关重要，但系统经常面临冷启动问题，即初始用户偏好或特征不可用。本文提出了一种名为USER-LLM R1的新框架，该框架通过动态用户画像和模型初始化来解决这一挑战。我们的方法集成了链式思维（CoT）推理模型，以迭代方式推断用户偏好，并使用视觉-语言模型（VLMs）从多模态输入中初始化用户画像，从而从第一次接触开始实现个性化交互。利用检索增强生成（RAG）架构，系统在固有的CoT过程中动态细化用户表示，确保上下文相关且适应性强的响应。在ElderlyTech-VQA基准上的评估表明，与最先进的基线相比，ROUGE-1 (+23.2%)、ROUGE-2 (+0.6%) 和 ROUGE-L (+8%) F1分数显著提高，消融研究强调了推理模型规模对性能的影响。人类评估进一步验证了该框架的有效性，特别是在老年用户中，定制化响应增强了参与度和信任。论文还严格讨论并解决了包括隐私保护和偏见缓解在内的伦理考虑，以确保负责任的部署。|
|**2025-04-02**|**PROPHET: An Inferable Future Forecasting Benchmark with Causal Intervened Likelihood Estimation**|Zhengwei Tao et.al.|[2504.01509](http://arxiv.org/abs/2504.01509)|null|预测未来事件是人工智能的终极目标之一。基于大型语言模型（LLM）的系统在预测未来事件方面展现了显著潜力，引起了研究界的广泛关注。目前，已经建立了多个基准来评估预测能力，将事件预测形式化为检索增强生成（RAG）和推理任务。在这些基准中，每个预测问题都通过相关的新闻文章进行回答。然而，由于没有考虑问题是否能够得到有效或充分的支持理由，这些基准中的一些问题可能是本质上不可推断的。为了解决这个问题，我们引入了一个新的基准PROPHET，它包含可推断的预测问题及其相关的新闻文章用于检索。为了确保基准的可推断性，我们提出了一种统计度量方法——因果干预似然（CIL），通过因果推断来评估可推断性。在构建这个基准时，我们首先收集了近期的趋势预测问题，然后使用CIL对数据进行过滤，从而得到了一个可推断的事件预测基准。通过广泛的实验，我们首先验证了CIL的有效性，并深入探讨了借助CIL进行事件预测的问题。随后，我们在PROPHET上评估了几种代表性的预测系统，得出了对未来方向有价值的见解。|
|**2025-04-03**|**GeoRAG: A Question-Answering Approach from a Geographical Perspective**|Jian Wang et.al.|[2504.01458](http://arxiv.org/abs/2504.01458)|null|地理问题回答（GeoQA）旨在处理地理领域的自然语言查询，以满足复杂的用户需求并提高信息检索效率。然而，传统的问答系统存在理解能力有限、检索准确性低、交互性弱以及对复杂任务处理不足的问题，阻碍了精确信息的获取。本研究提出了GeoRAG，这是一种知识增强的问答框架，通过领域特定的微调和提示工程与检索增强生成（RAG）技术相结合，以提高地理知识检索的准确性和用户交互。该方法包括四个组成部分：(1) 从3267个语料库（研究论文、专著和技术报告）构建结构化的地理知识库，通过多代理方法将其分类为七个维度：语义理解、空间位置、几何形态、属性特征、特征关系、演化过程和操作机制。这产生了145234个分类条目和875432个多维问答对。(2) 基于BERT-Base-Chinese的多标签文本分类器，训练用于通过地理维度分类来分析查询类型。(3) 利用问答对数据评估查询文档相关性的检索评估器，优化检索精度。(4) 设计GeoPrompt模板，动态集成用户查询与检索到的信息，通过特定维度的提示增强响应质量。比较实验表明，GeoRAG在多个基础模型上相对于传统RAG表现出更优的性能，验证了其通用性。这项工作通过提出在特定领域上下文中部署大型语言模型的新范式，推进了地理人工智能的发展，并对提高GeoQA系统在实际应用中的可扩展性和准确性具有重要意义。|
|**2025-04-03**|**GTR: Graph-Table-RAG for Cross-Table Question Answering**|Jiaru Zou et.al.|[2504.01346](http://arxiv.org/abs/2504.01346)|null|
|**2025-04-02**|**Biomedical Question Answering via Multi-Level Summarization on a Local Knowledge Graph**|Lingxiao Guan et.al.|[2504.01309](http://arxiv.org/abs/2504.01309)|null|
|**2025-04-03**|**Scaling Test-Time Inference with Policy-Optimized, Dynamic Retrieval-Augmented Generation via KV Caching and Decoding**|Sakhinana Sagar Srinivas et.al.|[2504.01281](http://arxiv.org/abs/2504.01281)|null|
|**2025-04-01**|**Medical large language models are easily distracted**|Krithik Vishwanath et.al.|[2504.01201](http://arxiv.org/abs/2504.01201)|**[link](https://github.com/nyuolab/MedDistractQA)**|
|**2025-03-31**|**A Systematic Evaluation of LLM Strategies for Mental Health Text Analysis: Fine-tuning vs. Prompt Engineering vs. RAG**|Arshia Kermani et.al.|[2503.24307](http://arxiv.org/abs/2503.24307)|null|
|**2025-03-31**|**Enhancing Large Language Models (LLMs) for Telecommunications using Knowledge Graphs and Retrieval-Augmented Generation**|Dun Yuan et.al.|[2503.24245](http://arxiv.org/abs/2503.24245)|null|
|**2025-03-31**|**Better wit than wealth: Dynamic Parametric Retrieval Augmented Generation for Test-time Knowledge Enhancement**|Yuqiao Tan et.al.|[2503.23895](http://arxiv.org/abs/2503.23895)|**[link](https://github.com/trae1oung/dyprag)**|
|**2025-04-02**|**CrossFormer: Cross-Segment Semantic Fusion for Document Segmentation**|Tongke Ni et.al.|[2503.23671](http://arxiv.org/abs/2503.23671)|null|
|**2025-03-30**|**SCORE: Story Coherence and Retrieval Enhancement for AI Narratives**|Qiang Yi et.al.|[2503.23512](http://arxiv.org/abs/2503.23512)|null|
|**2025-03-30**|**A Multi-agent Onboarding Assistant based on Large Language Models, Retrieval Augmented Generation, and Chain-of-Thought**|Andrei Cristian Ionescu et.al.|[2503.23421](http://arxiv.org/abs/2503.23421)|null|
|**2025-03-30**|**An Analysis of Decoding Methods for LLM-based Agents for Faithful Multi-Hop Question Answering**|Alexander Murphy et.al.|[2503.23415](http://arxiv.org/abs/2503.23415)|null|
|**2025-03-30**|**SalesRLAgent: A Reinforcement Learning Approach for Real-Time Sales Conversion Prediction and Optimization**|Nandakishor M et.al.|[2503.23303](http://arxiv.org/abs/2503.23303)|null|
|**2025-03-30**|**GRASP: Municipal Budget AI Chatbots for Enhancing Civic Engagement**|Jerry Xu et.al.|[2503.23299](http://arxiv.org/abs/2503.23299)|null|
|**2025-03-29**|**Citegeist: Automated Generation of Related Work Analysis on the arXiv Corpus**|Claas Beger et.al.|[2503.23229](http://arxiv.org/abs/2503.23229)|**[link](https://github.com/chenneking/citegeist)**|
|**2025-03-28**|**Preference-based Learning with Retrieval Augmented Generation for Conversational Question Answering**|Magdalena Kaiser et.al.|[2503.22303](http://arxiv.org/abs/2503.22303)|**[link](https://github.com/magkai/PRAISE)**|
|**2025-03-28**|**BanglAssist: A Bengali-English Generative AI Chatbot for Code-Switching and Dialect-Handling in Customer Service**|Francesco Kruk et.al.|[2503.22283](http://arxiv.org/abs/2503.22283)|null|
|**2025-03-28**|**Multi-Task Semantic Communications via Large Models**|Wanli Ni et.al.|[2503.22064](http://arxiv.org/abs/2503.22064)|null|
|**2025-03-27**|**AutoPsyC: Automatic Recognition of Psychodynamic Conflicts from Semi-structured Interviews with Large Language Models**|Sayed Muddashir Hossain et.al.|[2503.21911](http://arxiv.org/abs/2503.21911)|null|
|**2025-03-27**|**OntoAligner: A Comprehensive Modular and Robust Python Toolkit for Ontology Alignment**|Hamed Babaei Giglou et.al.|[2503.21902](http://arxiv.org/abs/2503.21902)|**[link](https://github.com/sciknoworg/ontoaligner)**|
|**2025-03-27**|**MemInsight: Autonomous Memory Augmentation for LLM Agents**|Rana Salama et.al.|[2503.21760](http://arxiv.org/abs/2503.21760)|null|
|**2025-03-27**|**ReaRAG: Knowledge-guided Reasoning Enhances Factuality of Large Reasoning Models with Iterative Retrieval Augmented Generation**|Zhicheng Lee et.al.|[2503.21729](http://arxiv.org/abs/2503.21729)|null|
|**2025-03-27**|**HyperGraphRAG: Retrieval-Augmented Generation with Hypergraph-Structured Knowledge Representation**|Haoran Luo et.al.|[2503.21322](http://arxiv.org/abs/2503.21322)|**[link](https://github.com/LHRLAB/HyperGraphRAG)**|
|**2025-03-27**|**Tricking Retrievers with Influential Tokens: An Efficient Black-Box Corpus Poisoning Attack**|Cheng Wang et.al.|[2503.21315](http://arxiv.org/abs/2503.21315)|null|
|**2025-03-27**|**Real-Time Evaluation Models for RAG: Who Detects Hallucinations Best?**|Ashish Sardana et.al.|[2503.21157](http://arxiv.org/abs/2503.21157)|null|
|**2025-03-26**|**DEMENTIA-PLAN: An Agent-Based Framework for Multi-Knowledge Graph Retrieval-Augmented Generation in Dementia Care**|Yutong Song et.al.|[2503.20950](http://arxiv.org/abs/2503.20950)|null|
|**2025-03-26**|**Leveraging LLMs, IDEs, and Semantic Embeddings for Automated Move Method Refactoring**|Fraol Batole et.al.|[2503.20934](http://arxiv.org/abs/2503.20934)|null|
|**2025-03-26**|**MCTS-RAG: Enhancing Retrieval-Augmented Generation with Monte Carlo Tree Search**|Yunhai Hu et.al.|[2503.20757](http://arxiv.org/abs/2503.20757)|null|
|**2025-03-26**|**What to Retrieve for Effective Retrieval-Augmented Code Generation? An Empirical Study and Beyond**|Wenchao Gu et.al.|[2503.20589](http://arxiv.org/abs/2503.20589)|null|
|**2025-03-26**|**RALLRec+: Retrieval Augmented Large Language Model Recommendation with Reasoning**|Sichun Luo et.al.|[2503.20430](http://arxiv.org/abs/2503.20430)|**[link](https://github.com/sichunluo/rallrec_plus)**|
|**2025-03-26**|**Dewey Long Context Embedding Model: A Technical Report**|Dun Zhang et.al.|[2503.20376](http://arxiv.org/abs/2503.20376)|null|
|**2025-03-25**|**CausalRAG: Integrating Causal Graphs into Retrieval-Augmented Generation**|Nengbo Wang et.al.|[2503.19878](http://arxiv.org/abs/2503.19878)|null|
|**2025-03-25**|**Motif Counting in Complex Networks: A Comprehensive Survey**|Haozhe Yin et.al.|[2503.19573](http://arxiv.org/abs/2503.19573)|null|
|**2025-03-25**|**G-DexGrasp: Generalizable Dexterous Grasping Synthesis Via Part-Aware Prior Retrieval and Prior-Assisted Generation**|Juntao Jian et.al.|[2503.19457](http://arxiv.org/abs/2503.19457)|null|
|**2025-03-25**|**RGL: A Graph-Centric, Modular Framework for Efficient Retrieval-Augmented Generation on Graphs**|Yuan Li et.al.|[2503.19314](http://arxiv.org/abs/2503.19314)|**[link](https://github.com/PyRGL/rgl)**|
|**2025-03-24**|**Video SimpleQA: Towards Factuality Evaluation in Large Video Language Models**|Meng Cao et.al.|[2503.18923](http://arxiv.org/abs/2503.18923)|null|
|**2025-03-24**|**Synthetic Function Demonstrations Improve Generation in Low-Resource Programming Languages**|Nick McKenna et.al.|[2503.18760](http://arxiv.org/abs/2503.18760)|null|
|**2025-03-24**|**ModiGen: A Large Language Model-Based Workflow for Multi-Task Modelica Code Generation**|Jiahui Xiang et.al.|[2503.18460](http://arxiv.org/abs/2503.18460)|null|
|**2025-03-24**|**Fact-checking AI-generated news reports: Can LLMs catch their own lies?**|Jiayi Yao et.al.|[2503.18293](http://arxiv.org/abs/2503.18293)|null|
|**2025-03-23**|**GINGER: Grounded Information Nugget-Based Generation of Responses**|Weronika Łajewska et.al.|[2503.18174](http://arxiv.org/abs/2503.18174)|**[link](https://github.com/iai-group/ginger-response-generation)**|
|**2025-03-23**|**Retrieval Augmented Generation and Understanding in Vision: A Survey and New Outlook**|Xu Zheng et.al.|[2503.18016](http://arxiv.org/abs/2503.18016)|null|
|**2025-03-23**|**Experience Retrieval-Augmentation with Electronic Health Records Enables Accurate Discharge QA**|Justice Ou et.al.|[2503.17933](http://arxiv.org/abs/2503.17933)|**[link](https://github.com/jou2024/EXPRAG)**|
|**2025-03-23**|**MedPlan:A Two-Stage RAG-Based System for Personalized Medical Plan Generation**|Hsin-Ling Hsu et.al.|[2503.17900](http://arxiv.org/abs/2503.17900)|null|
|**2025-03-21**|**Autonomous Radiotherapy Treatment Planning Using DOLA: A Privacy-Preserving, LLM-Based Optimization Agent**|Humza Nusrat et.al.|[2503.17553](http://arxiv.org/abs/2503.17553)|null|
|**2025-03-21**|**An LLM-Powered Clinical Calculator Chatbot Backed by Verifiable Clinical Calculators and their Metadata**|Niranjan Kumar et.al.|[2503.17550](http://arxiv.org/abs/2503.17550)|null|
|**2025-03-21**|**Bugdar: AI-Augmented Secure Code Review for GitHub Pull Requests**|John Naulty et.al.|[2503.17302](http://arxiv.org/abs/2503.17302)|null|
|**2025-03-21**|**RustEvo^2: An Evolving Benchmark for API Evolution in LLM-based Rust Code Generation**|Linxi Liang et.al.|[2503.16922](http://arxiv.org/abs/2503.16922)|**[link](https://github.com/sysuselab/rustevo)**|
|**2025-03-20**|**Investigating Retrieval-Augmented Generation in Quranic Studies: A Study of 13 Open-Source Large Language Models**|Zahra Khalila et.al.|[2503.16581](http://arxiv.org/abs/2503.16581)|null|
|**2025-03-20**|**FutureGen: LLM-RAG Approach to Generate the Future Work of Scientific Article**|Ibrahim Al Azher et.al.|[2503.16561](http://arxiv.org/abs/2503.16561)|null|
|**2025-03-20**|**Towards Lighter and Robust Evaluation for Retrieval Augmented Generation**|Alex-Razvan Ispas et.al.|[2503.16161](http://arxiv.org/abs/2503.16161)|**[link](https://github.com/razvanip13/towards_lighter_and_robust_evaluation)**|
|**2025-03-20**|**Tuning LLMs by RAG Principles: Towards LLM-native Memory**|Jiale Wei et.al.|[2503.16071](http://arxiv.org/abs/2503.16071)|**[link](https://github.com/mindverse/rag-tuned-llm)**|
|**2025-03-20**|**Parameters vs. Context: Fine-Grained Control of Knowledge Reliance in Language Models**|Baolong Bi et.al.|[2503.15888](http://arxiv.org/abs/2503.15888)|**[link](https://github.com/byronbbl/ck-plug)**|
|**2025-03-21**|**Typed-RAG: Type-aware Multi-Aspect Decomposition for Non-Factoid Question Answering**|DongGeon Lee et.al.|[2503.15879](http://arxiv.org/abs/2503.15879)|**[link](https://github.com/teamnlp/typed-rag)**|
|**2025-03-20**|**DroidTTP: Mapping Android Applications with TTP for Cyber Threat Intelligence**|Dincy R Arikkat et.al.|[2503.15866](http://arxiv.org/abs/2503.15866)|null|
|**2025-03-19**|**Enhancing Pancreatic Cancer Staging with Large Language Models: The Role of Retrieval-Augmented Generation**|Hisashi Johno et.al.|[2503.15664](http://arxiv.org/abs/2503.15664)|null|
|**2025-03-19**|**Does Context Matter? ContextualJudgeBench for Evaluating LLM-based Judges in Contextual Settings**|Austin Xu et.al.|[2503.15620](http://arxiv.org/abs/2503.15620)|**[link](https://github.com/salesforceairesearch/contextualjudgebench)**|
|**2025-03-19**|**Evaluating Bias in Retrieval-Augmented Medical Question-Answering Systems**|Yuelyu Ji et.al.|[2503.15454](http://arxiv.org/abs/2503.15454)|null|
|**2025-03-19**|**When LLMs Meet API Documentation: Can Retrieval Augmentation Aid Code Generation Just as It Helps Developers?**|Jingyi Chen et.al.|[2503.15231](http://arxiv.org/abs/2503.15231)|null|
|**2025-03-19**|**When Pigs Get Sick: Multi-Agent AI for Swine Disease Detection**|Tittaya Mairittha et.al.|[2503.15204](http://arxiv.org/abs/2503.15204)|null|
|**2025-03-19**|**Optimizing Retrieval Strategies for Financial Question Answering Documents in Retrieval-Augmented Generation Systems**|Sejong Kim et.al.|[2503.15191](http://arxiv.org/abs/2503.15191)|**[link](https://github.com/seohyunwoo-0407/gar)**|
|**2025-03-19**|**Graph-Based Re-ranking: Emerging Techniques, Limitations, and Opportunities**|Md Shahir Zaoad et.al.|[2503.14802](http://arxiv.org/abs/2503.14802)|null|
|**2025-03-18**|**RAGO: Systematic Performance Optimization for Retrieval-Augmented Generation Serving**|Wenqi Jiang et.al.|[2503.14649](http://arxiv.org/abs/2503.14649)|null|
|**2025-03-18**|**Command R7B Arabic: A Small, Enterprise Focused, Multilingual, and Culturally Aware Arabic LLM**|Yazeed Alnumay et.al.|[2503.14603](http://arxiv.org/abs/2503.14603)|null|
|**2025-03-18**|**From "Hallucination" to "Suture": Insights from Language Philosophy to Enhance Large Language Models**|Qiantong Wang et.al.|[2503.14392](http://arxiv.org/abs/2503.14392)|null|
|**2025-03-18**|**Good/Evil Reputation Judgment of Celebrities by LLMs via Retrieval Augmented Generation**|Rikuto Tsuchida et.al.|[2503.14382](http://arxiv.org/abs/2503.14382)|null|
|**2025-03-18**|**MANTRA: Enhancing Automated Method-Level Refactoring with Contextual RAG and Multi-Agent LLM Collaboration**|Yisen Xu et.al.|[2503.14340](http://arxiv.org/abs/2503.14340)|null|
|**2025-03-18**|**JuDGE: Benchmarking Judgment Document Generation for Chinese Legal System**|Weihang Su et.al.|[2503.14258](http://arxiv.org/abs/2503.14258)|**[link](https://github.com/oneal2000/judge)**|
|**2025-03-19**|**KG-IRAG: A Knowledge Graph-Based Iterative Retrieval-Augmented Generation Framework for Temporal Reasoning**|Ruiyi Yang et.al.|[2503.14234](http://arxiv.org/abs/2503.14234)|null|
|**2025-03-18**|**LLM-based Unit Test Generation for Dynamically-Typed Programs**|Runlin Liu et.al.|[2503.14000](http://arxiv.org/abs/2503.14000)|null|
|**2025-03-18**|**MDocAgent: A Multi-Modal Multi-Agent Framework for Document Understanding**|Siwei Han et.al.|[2503.13964](http://arxiv.org/abs/2503.13964)|**[link](https://github.com/aiming-lab/mdocagent)**|
|**2025-03-18**|**MoK-RAG: Mixture of Knowledge Paths Enhanced Retrieval-Augmented Generation for Embodied AI Environments**|Zhengsheng Guo et.al.|[2503.13882](http://arxiv.org/abs/2503.13882)|null|
|**2025-03-18**|**RAD: Retrieval-Augmented Decision-Making of Meta-Actions with Vision-Language Models in Autonomous Driving**|Yujin Wang et.al.|[2503.13861](http://arxiv.org/abs/2503.13861)|null|
|**2025-03-18**|**Empowering GraphRAG with Knowledge Filtering and Integration**|Kai Guo et.al.|[2503.13804](http://arxiv.org/abs/2503.13804)|null|
|**2025-03-17**|**Toward Generative 6G Simulation: An Experimental Multi-Agent LLM and ns-3 Integration**|Farhad Rezazadeh et.al.|[2503.13402](http://arxiv.org/abs/2503.13402)|null|
|**2025-03-17**|**Generative AI for Software Architecture. Applications, Trends, Challenges, and Future Directions**|Matteo Esposito et.al.|[2503.13310](http://arxiv.org/abs/2503.13310)|null|
|**2025-03-17**|**LLM-Match: An Open-Sourced Patient Matching Model Based on Large Language Models and Retrieval-Augmented Generation**|Xiaodi Li et.al.|[2503.13281](http://arxiv.org/abs/2503.13281)|null|
|**2025-03-17**|**Safeguarding LLM Embeddings in End-Cloud Collaboration via Entropy-Driven Perturbation**|Shuaifan Jin et.al.|[2503.12896](http://arxiv.org/abs/2503.12896)|null|
|**2025-03-17**|**RAG-RL: Advancing Retrieval-Augmented Generation via RL and Curriculum Learning**|Jerry Huang et.al.|[2503.12759](http://arxiv.org/abs/2503.12759)|null|
|**2025-03-16**|**Logic-RAG: Augmenting Large Multimodal Models with Visual-Spatial Knowledge for Road Scene Understanding**|Imran Kabir et.al.|[2503.12663](http://arxiv.org/abs/2503.12663)|**[link](https://github.com/imran2205/logicrag)**|
|**2025-03-15**|**Integrating Chain-of-Thought and Retrieval Augmented Generation Enhances Rare Disease Diagnosis from Clinical Notes**|Da Wu et.al.|[2503.12286](http://arxiv.org/abs/2503.12286)|null|
|**2025-03-15**|**Agentic Search Engine for Real-Time IoT Data**|Abdelrahman Elewah et.al.|[2503.12255](http://arxiv.org/abs/2503.12255)|**[link](https://github.com/SensorsConnect/IoT-Agentic-Search-Engine)**|
|**2025-03-15**|**TFHE-Coder: Evaluating LLM-agentic Fully Homomorphic Encryption Code Generation**|Mayank Kumar et.al.|[2503.12217](http://arxiv.org/abs/2503.12217)|null|
|**2025-03-15**|**PredicateFix: Repairing Static Analysis Alerts with Bridging Predicates**|Yuan-An Xiao et.al.|[2503.12205](http://arxiv.org/abs/2503.12205)|null|
|**2025-03-14**|**AIstorian lets AI be a historian: A KG-powered multi-agent system for accurate biography generation**|Fengyu Li et.al.|[2503.11346](http://arxiv.org/abs/2503.11346)|**[link](https://github.com/zju-daily/aistorian)**|
|**2025-03-14**|**MUSS: Multilevel Subset Selection for Relevance and Diversity**|Vu Nguyen et.al.|[2503.11126](http://arxiv.org/abs/2503.11126)|null|
|**2025-03-13**|**Taxonomic Reasoning for Rare Arthropods: Combining Dense Image Captioning and RAG for Interpretable Classification**|Nathaniel Lesperance et.al.|[2503.10886](http://arxiv.org/abs/2503.10886)|null|
|**2025-03-13**|**AttentionRAG: Attention-Guided Context Pruning in Retrieval-Augmented Generation**|Yixiong Fang et.al.|[2503.10720](http://arxiv.org/abs/2503.10720)|null|
|**2025-03-12**|**CALLM: Context-Aware Emotion Analysis in Cancer Survivors Using LLMs and Retrieval-Augmented Mobile Diaries**|Zhiyuan Wang et.al.|[2503.10707](http://arxiv.org/abs/2503.10707)|null|
|**2025-03-13**|**SurgRAW: Multi-Agent Workflow with Chain-of-Thought Reasoning for Surgical Intelligence**|Chang Han Low et.al.|[2503.10265](http://arxiv.org/abs/2503.10265)|null|
|**2025-03-13**|**Retrieval-Augmented Generation with Hierarchical Knowledge**|Haoyu Huang et.al.|[2503.10150](http://arxiv.org/abs/2503.10150)|**[link](https://github.com/hhy-huang/HiRAG)**|
|**2025-03-12**|**Conversational Gold: Evaluating Personalized Conversational Search System using Gold Nuggets**|Zahra Abbasiantaeb et.al.|[2503.09902](http://arxiv.org/abs/2503.09902)|**[link](https://github.com/irlabamsterdam/cone-rag)**|
|**2025-03-12**|**What's In Your Field? Mapping Scientific Research with Knowledge Graphs and Large Language Models**|Abhipsha Das et.al.|[2503.09894](http://arxiv.org/abs/2503.09894)|**[link](https://github.com/chiral-carbon/kg-for-science)**|
|**2025-03-12**|**Probabilistic Reasoning with LLMs for k-anonymity Estimation**|Jonathan Zheng et.al.|[2503.09674](http://arxiv.org/abs/2503.09674)|null|
|**2025-03-12**|**Complementarity, Augmentation, or Substitutivity? The Impact of Generative Artificial Intelligence on the U.S. Federal Workforce**|William G. Resh et.al.|[2503.09637](http://arxiv.org/abs/2503.09637)|null|
|**2025-03-12**|**MoC: Mixtures of Text Chunking Learners for Retrieval-Augmented Generation System**|Jihao Zhao et.al.|[2503.09600](http://arxiv.org/abs/2503.09600)|**[link](https://github.com/IAAR-Shanghai/Meta-Chunking)**|
|**2025-03-12**|**Memory-enhanced Retrieval Augmentation for Long Video Understanding**|Huaying Yuan et.al.|[2503.09149](http://arxiv.org/abs/2503.09149)|null|
|**2025-03-12**|**Everything Can Be Described in Words: A Simple Unified Multi-Modal Framework with Semantic and Temporal Alignment**|Xiaowei Bi et.al.|[2503.09081](http://arxiv.org/abs/2503.09081)|null|
|**2025-03-12**|**Leveraging Retrieval Augmented Generative LLMs For Automated Metadata Description Generation to Enhance Data Catalogs**|Mayank Singh et.al.|[2503.09003](http://arxiv.org/abs/2503.09003)|null|
|**2025-03-11**|**Exploiting Instruction-Following Retrievers for Malicious Information Retrieval**|Parishad BehnamGhader et.al.|[2503.08644](http://arxiv.org/abs/2503.08644)|null|
|**2025-03-11**|**RAG-Adapter: A Plug-and-Play RAG-enhanced Framework for Long Video Understanding**|Xichen Tan et.al.|[2503.08576](http://arxiv.org/abs/2503.08576)|null|
|**2025-03-11**|**OpenRAG: Optimizing RAG End-to-End via In-Context Retrieval Learning**|Jiawei Zhou et.al.|[2503.08398](http://arxiv.org/abs/2503.08398)|null|
|**2025-03-11**|**Towards Scalable and Cross-Lingual Specialist Language Models for Oncology**|Morteza Rohanian et.al.|[2503.08323](http://arxiv.org/abs/2503.08323)|null|
|**2025-03-11**|**DeepRAG: Building a Custom Hindi Embedding Model for Retrieval Augmented Generation from Scratch**|Nandakishor M et.al.|[2503.08213](http://arxiv.org/abs/2503.08213)|null|
|**2025-03-11**|**A Cascading Cooperative Multi-agent Framework for On-ramp Merging Control Integrating Large Language Models**|Miao Zhang et.al.|[2503.08199](http://arxiv.org/abs/2503.08199)|null|
|**2025-03-11**|**Privacy-Enhancing Paradigms within Federated Multi-Agent Systems**|Zitong Shi et.al.|[2503.08175](http://arxiv.org/abs/2503.08175)|null|
|**2025-03-11**|**LLM-based Corroborating and Refuting Evidence Retrieval for Scientific Claim Verification**|Siyuan Wang et.al.|[2503.07937](http://arxiv.org/abs/2503.07937)|null|
|**2025-03-10**|**Talking to GDELT Through Knowledge Graphs**|Audun Myers et.al.|[2503.07584](http://arxiv.org/abs/2503.07584)|null|
|**2025-03-10**|**Advancing Vietnamese Information Retrieval with Learning Objective and Benchmark**|Phu-Vinh Nguyen et.al.|[2503.07470](http://arxiv.org/abs/2503.07470)|null|
|**2025-03-10**|**LLM-C3MOD: A Human-LLM Collaborative System for Cross-Cultural Hate Speech Moderation**|Junyeong Park et.al.|[2503.07237](http://arxiv.org/abs/2503.07237)|null|
|**2025-03-10**|**Generative AI in Transportation Planning: A Survey**|Longchao Da et.al.|[2503.07158](http://arxiv.org/abs/2503.07158)|null|
|**2025-03-10**|**CtrlRAG: Black-box Adversarial Attacks Based on Masked Language Models in Retrieval-Augmented Language Generation**|Runqi Sui et.al.|[2503.06950](http://arxiv.org/abs/2503.06950)|null|
|**2025-03-09**|**Delusions of Large Language Models**|Hongshen Xu et.al.|[2503.06709](http://arxiv.org/abs/2503.06709)|null|
|**2025-03-09**|**Human Cognition Inspired RAG with Knowledge Graph for Complex Problem Solving**|Yao Cheng et.al.|[2503.06567](http://arxiv.org/abs/2503.06567)|null|
|**2025-03-09**|**HuixiangDou2: A Robustly Optimized GraphRAG Approach**|Huanjun Kong et.al.|[2503.06474](http://arxiv.org/abs/2503.06474)|**[link](https://github.com/tpoisonooo/huixiangdou2)**|
|**2025-03-09**|**Graph Retrieval-Augmented LLM for Conversational Recommendation Systems**|Zhangchi Qiu et.al.|[2503.06430](http://arxiv.org/abs/2503.06430)|null|
|**2025-03-08**|**Poisoned-MRAG: Knowledge Poisoning Attacks to Multimodal Retrieval Augmented Generation**|Yinuo Liu et.al.|[2503.06254](http://arxiv.org/abs/2503.06254)|null|
|**2025-03-07**|**TPU-Gen: LLM-Driven Custom Tensor Processing Unit Generator**|Deepak Vungarala et.al.|[2503.05951](http://arxiv.org/abs/2503.05951)|null|
|**2025-03-07**|**R1-Searcher: Incentivizing the Search Capability in LLMs via Reinforcement Learning**|Huatong Song et.al.|[2503.05592](http://arxiv.org/abs/2503.05592)|null|
|**2025-03-07**|**Quantifying the Robustness of Retrieval-Augmented Language Models Against Spurious Features in Grounding Data**|Shiping Yang et.al.|[2503.05587](http://arxiv.org/abs/2503.05587)|null|
|**2025-03-07**|**Leveraging Approximate Caching for Faster Retrieval-Augmented Generation**|Shai Bergman et.al.|[2503.05530](http://arxiv.org/abs/2503.05530)|null|
|**2025-03-07**|**Automatic Teaching Platform on Vision Language Retrieval Augmented Generation**|Ruslan Gokhman et.al.|[2503.05464](http://arxiv.org/abs/2503.05464)|null|
|**2025-03-07**|**VLMs Play StarCraft II: A Benchmark and Multimodal Decision Method**|Weiyu Ma et.al.|[2503.05383](http://arxiv.org/abs/2503.05383)|**[link](https://github.com/camel-ai/vlm-play-starcraft2)**|
|**2025-03-07**|**Personalized Text Generation with Contrastive Activation Steering**|Jinghao Zhang et.al.|[2503.05213](http://arxiv.org/abs/2503.05213)|null|
|**2025-03-07**|**Path Pooling: Train-Free Structure Enhancement for Efficient Knowledge Graph Retrieval-Augmented Generation**|Hairu Wang et.al.|[2503.05203](http://arxiv.org/abs/2503.05203)|null|
|**2025-03-07**|**ORANSight-2.0: Foundational LLMs for O-RAN**|Pranshav Gajjar et.al.|[2503.05200](http://arxiv.org/abs/2503.05200)|null|
|**2025-03-07**|**FinTMMBench: Benchmarking Temporal-Aware Multi-Modal RAG in Finance**|Fengbin Zhu et.al.|[2503.05185](http://arxiv.org/abs/2503.05185)|null|
|**2025-03-07**|**Interpersonal Memory Matters: A New Task for Proactive Dialogue Utilizing Conversational History**|Bowen Wu et.al.|[2503.05150](http://arxiv.org/abs/2503.05150)|null|
|**2025-03-06**|**More Documents, Same Length: Isolating the Challenge of Multiple Documents in RAG**|Shahar Levy et.al.|[2503.04388](http://arxiv.org/abs/2503.04388)|null|
|**2025-03-06**|**In-depth Analysis of Graph-based RAG in a Unified Framework**|Yingli Zhou et.al.|[2503.04338](http://arxiv.org/abs/2503.04338)|null|
|**2025-03-04**|**Optimizing open-domain question answering with graph-based retrieval augmented generation**|Joyce Cahoon et.al.|[2503.02922](http://arxiv.org/abs/2503.02922)|null|
|**2025-03-04**|**Wikipedia in the Era of LLMs: Evolution and Risks**|Siming Huang et.al.|[2503.02879](http://arxiv.org/abs/2503.02879)|**[link](https://github.com/hsm316/llm_wikipedia)**|
|**2025-03-06**|**RAAD-LLM: Adaptive Anomaly Detection Using LLMs and RAG Integration**|Alicia Russell-Gilbert et.al.|[2503.02800](http://arxiv.org/abs/2503.02800)|null|
|**2025-03-04**|**ImpedanceGPT: VLM-driven Impedance Control of Swarm of Mini-drones for Intelligent Navigation in Dynamic Environment**|Faryal Batool et.al.|[2503.02723](http://arxiv.org/abs/2503.02723)|null|
|**2025-03-04**|**FinArena: A Human-Agent Collaboration Framework for Financial Market Analysis and Forecasting**|Congluo Xu et.al.|[2503.02692](http://arxiv.org/abs/2503.02692)|null|
|**2025-03-05**|**OkraLong: A Flexible Retrieval-Augmented Framework for Long-Text Query Processing**|Yulong Hui et.al.|[2503.02603](http://arxiv.org/abs/2503.02603)|null|
|**2025-03-04**|**PennyLang: Pioneering LLM-Based Quantum Code Generation with a Novel PennyLane-Centric Dataset**|Haider Asif et.al.|[2503.02497](http://arxiv.org/abs/2503.02497)|null|
|**2025-03-03**|**Cracking Vector Search Indexes**|Vasilis Mageirakos et.al.|[2503.01823](http://arxiv.org/abs/2503.01823)|null|
|**2025-03-03**|**SAGE: A Framework of Precise Retrieval for RAG**|Jintao Zhang et.al.|[2503.01713](http://arxiv.org/abs/2503.01713)|null|
|**2025-03-03**|**Generate, Discriminate, Evolve: Enhancing Context Faithfulness via Fine-Grained Sentence-Level Self-Evolution**|Kun Li et.al.|[2503.01695](http://arxiv.org/abs/2503.01695)|null|
|**2025-03-04**|**SePer: Measure Retrieval Utility Through The Lens Of Semantic Perplexity Reduction**|Lu Dai et.al.|[2503.01478](http://arxiv.org/abs/2503.01478)|**[link](https://github.com/sepermetric/seper)**|
|**2025-02-28**|**RuCCoD: Towards Automated ICD Coding in Russian**|Aleksandr Nesterov et.al.|[2502.21263](http://arxiv.org/abs/2502.21263)|**[link](https://github.com/auto-icd-coding/ruccod)**|
|**2025-02-28**|**Generating patient cohorts from electronic health records using two-step retrieval-augmented text-to-SQL generation**|Angelo Ziletti et.al.|[2502.21107](http://arxiv.org/abs/2502.21107)|null|
|**2025-02-28**|**PASemiQA: Plan-Assisted Agent for Question Answering on Semi-Structured Data with Text and Relational Information**|Hansi Yang et.al.|[2502.21087](http://arxiv.org/abs/2502.21087)|null|
|**2025-02-28**|**GUIDE: LLM-Driven GUI Generation Decomposition for Automated Prototyping**|Kristian Kolthoff et.al.|[2502.21068](http://arxiv.org/abs/2502.21068)|null|
|**2025-02-28**|**The RAG Paradox: A Black-Box Attack Exploiting Unintentional Vulnerabilities in Retrieval-Augmented Generation Systems**|Chanwoo Choi et.al.|[2502.20995](http://arxiv.org/abs/2502.20995)|null|
|**2025-02-28**|**TeleRAG: Efficient Retrieval-Augmented Generation Inference with Lookahead Retrieval**|Chien-Yu Lin et.al.|[2502.20969](http://arxiv.org/abs/2502.20969)|null|
|**2025-02-28**|**Fine-Grained Retrieval-Augmented Generation for Visual Question Answering**|Zhengxuan Zhang et.al.|[2502.20964](http://arxiv.org/abs/2502.20964)|null|
|**2025-02-28**|**Retrieval Augmented Generation for Topic Modeling in Organizational Research: An Introduction with Empirical Demonstration**|Gerion Spielberger et.al.|[2502.20963](http://arxiv.org/abs/2502.20963)|null|
|**2025-03-03**|**A Pilot Empirical Study on When and How to Use Knowledge Graphs as Retrieval Augmented Generation**|Xujie Yuan et.al.|[2502.20854](http://arxiv.org/abs/2502.20854)|null|
|**2025-02-28**|**LADs: Leveraging LLMs for AI-Driven DevOps**|Ahmad Faraz Khan et.al.|[2502.20825](http://arxiv.org/abs/2502.20825)|null|
|**2025-02-27**|**Bridging Legal Knowledge and AI: Retrieval-Augmented Generation with Vector Stores, Knowledge Graphs, and Hierarchical Non-negative Matrix Factorization**|Ryan C. Barron et.al.|[2502.20364](http://arxiv.org/abs/2502.20364)|null|
|**2025-02-27**|**Long-Context Inference with Retrieval-Augmented Speculative Decoding**|Guanzheng Chen et.al.|[2502.20330](http://arxiv.org/abs/2502.20330)|**[link](https://github.com/john-ai-lab/rapid)**|
|**2025-02-27**|**From Retrieval to Generation: Comparing Different Approaches**|Abdelrahman Abdallah et.al.|[2502.20245](http://arxiv.org/abs/2502.20245)|null|
|**2025-02-27**|**ChineseEcomQA: A Scalable E-commerce Concept Evaluation Benchmark for Large Language Models**|Haibin Chen et.al.|[2502.20196](http://arxiv.org/abs/2502.20196)|**[link](https://github.com/OpenStellarTeam/ChineseEcomQA)**|
|**2025-02-27**|**Bisecting K-Means in RAG for Enhancing Question-Answering Tasks Performance in Telecommunications**|Pedro Sousa et.al.|[2502.20188](http://arxiv.org/abs/2502.20188)|null|
|**2025-02-27**|**LLM-driven Effective Knowledge Tracing by Integrating Dual-channel Difficulty**|Jiahui Cen et.al.|[2502.19915](http://arxiv.org/abs/2502.19915)|null|
|**2025-02-27**|**Does Your Voice Assistant Remember? Analyzing Conversational Context Recall and Utilization in Voice Interaction Models**|Heeseung Kim et.al.|[2502.19759](http://arxiv.org/abs/2502.19759)|null|
|**2025-02-26**|**Agentic Mixture-of-Workflows for Multi-Modal Chemical Search**|Tiffany J. Callahan et.al.|[2502.19629](http://arxiv.org/abs/2502.19629)|null|
|**2025-02-26**|**Trustworthy Answers, Messier Data: Bridging the Gap in Low-Resource Retrieval-Augmented Generation for Domain Expert Systems**|Nayoung Choi et.al.|[2502.19596](http://arxiv.org/abs/2502.19596)|null|
|**2025-02-26**|**Leveraging Retrieval-Augmented Generation and Large Language Models to Predict SERCA-Binding Protein Fragments from Cardiac Proteomics Data**|Taylor A Phillips et.al.|[2502.19574](http://arxiv.org/abs/2502.19574)|null|
|**2025-02-26**|**Agent-centric Information Access**|Evangelos Kanoulas et.al.|[2502.19298](http://arxiv.org/abs/2502.19298)|null|
|**2025-02-26**|**Efficient Federated Search for Retrieval-Augmented Generation**|Rachid Guerraoui et.al.|[2502.19280](http://arxiv.org/abs/2502.19280)|null|
|**2025-02-26**|**Bi'an: A Bilingual Benchmark and Model for Hallucination Detection in Retrieval-Augmented Generation**|Zhouyu Jiang et.al.|[2502.19209](http://arxiv.org/abs/2502.19209)|null|
|**2025-02-26**|**MEBench: Benchmarking Large Language Models for Cross-Document Multi-Entity Question Answering**|Teng Lin et.al.|[2502.18993](http://arxiv.org/abs/2502.18993)|null|
|**2025-02-26**|**OntologyRAG: Better and Faster Biomedical Code Mapping with Retrieval-Augmented Generation (RAG) Leveraging Ontology Knowledge Graphs and Large Language Models**|Hui Feng et.al.|[2502.18992](http://arxiv.org/abs/2502.18992)|**[link](https://github.com/iqvianlp/ontologyrag)**|
|**2025-02-26**|**Kanana: Compute-efficient Bilingual Language Models**|Kanana LLM Team et.al.|[2502.18934](http://arxiv.org/abs/2502.18934)|null|
|**2025-02-26**|**Talking like Piping and Instrumentation Diagrams (P&IDs)**|Achmad Anggawirya Alimin et.al.|[2502.18928](http://arxiv.org/abs/2502.18928)|null|
|**2025-02-26**|**END: Early Noise Dropping for Efficient and Effective Context Denoising**|Hongye Jin et.al.|[2502.18915](http://arxiv.org/abs/2502.18915)|null|
|**2025-02-26**|**Automated Code Generation and Validation for Software Components of Microcontrollers**|Sebastian Haug et.al.|[2502.18905](http://arxiv.org/abs/2502.18905)|null|
|**2025-02-26**|**Judge as A Judge: Improving the Evaluation of Retrieval-Augmented Generation through the Judge-Consistency of Large Language Models**|Shuliang Liu et.al.|[2502.18817](http://arxiv.org/abs/2502.18817)|null|
|**2025-02-25**|**Rank1: Test-Time Compute for Reranking in Information Retrieval**|Orion Weller et.al.|[2502.18418](http://arxiv.org/abs/2502.18418)|**[link](https://github.com/orionw/rank1)**|
|**2025-02-25**|**KiRAG: Knowledge-Driven Iterative Retriever for Enhancing Retrieval-Augmented Generation**|Jinyuan Fang et.al.|[2502.18397](http://arxiv.org/abs/2502.18397)|null|
|**2025-02-25**|**LevelRAG: Enhancing Retrieval-Augmented Generation with Multi-hop Logic Planning over Rewriting Augmented Searchers**|Zhuocheng Zhang et.al.|[2502.18139](http://arxiv.org/abs/2502.18139)|**[link](https://github.com/ictnlp/LevelRAG)**|
|**2025-02-25**|**Detecting Knowledge Boundary of Vision Large Language Models by Sampling-Based Inference**|Zhuo Chen et.al.|[2502.18023](http://arxiv.org/abs/2502.18023)|null|
|**2025-02-25**|**ViDoRAG: Visual Document Retrieval-Augmented Generation via Dynamic Iterative Reasoning Agents**|Qiuchen Wang et.al.|[2502.18017](http://arxiv.org/abs/2502.18017)|**[link](https://github.com/Alibaba-NLP/ViDoRAG)**|
|**2025-02-25**|**RankCoT: Refining Knowledge for Retrieval-Augmented Generation through Ranking Chain-of-Thoughts**|Mingyan Wu et.al.|[2502.17888](http://arxiv.org/abs/2502.17888)|**[link](https://github.com/neuir/rankcot)**|
|**2025-02-25**|**Neural Graph Matching Improves Retrieval Augmented Generation in Molecular Machine Learning**|Runzhong Wang et.al.|[2502.17874](http://arxiv.org/abs/2502.17874)|null|
|**2025-02-25**|**Say Less, Mean More: Leveraging Pragmatics in Retrieval-Augmented Generation**|Haris Riaz et.al.|[2502.17839](http://arxiv.org/abs/2502.17839)|null|
|**2025-02-25**|**MM-PoisonRAG: Disrupting Multimodal RAG with Local and Global Poisoning Attacks**|Hyeonjeong Ha et.al.|[2502.17832](http://arxiv.org/abs/2502.17832)|**[link](https://github.com/hyeonjeongha/mm-poisonrag)**|
|**2025-02-24**|**Evaluating the Effect of Retrieval Augmentation on Social Biases**|Tianhui Zhang et.al.|[2502.17611](http://arxiv.org/abs/2502.17611)|null|
|**2025-02-24**|**Mitigating Bias in RAG: Controlling the Embedder**|Taeyoun Kim et.al.|[2502.17390](http://arxiv.org/abs/2502.17390)|null|
|**2025-02-24**|**Benchmarking Retrieval-Augmented Generation in Multi-Modal Contexts**|Zhenghao Liu et.al.|[2502.17297](http://arxiv.org/abs/2502.17297)|**[link](https://github.com/neuir/m2rag)**|
|**2025-02-24**|**MEMERAG: A Multilingual End-to-End Meta-Evaluation Benchmark for Retrieval Augmented Generation**|María Andrea Cruz Blandón et.al.|[2502.17163](http://arxiv.org/abs/2502.17163)|null|
|**2025-02-24**|**LettuceDetect: A Hallucination Detection Framework for RAG Applications**|Ádám Kovács et.al.|[2502.17125](http://arxiv.org/abs/2502.17125)|**[link](https://github.com/KRLabsOrg/LettuceDetect)**|
|**2025-02-24**|**Language Model Re-rankers are Steered by Lexical Similarities**|Lovisa Hagström et.al.|[2502.17036](http://arxiv.org/abs/2502.17036)|null|
|**2025-02-24**|**Graphy'our Data: Towards End-to-End Modeling, Exploring and Generating Report from Raw Data**|Longbin Lai et.al.|[2502.16868](http://arxiv.org/abs/2502.16868)|null|
|**2025-02-24**|**A Hybrid Approach to Information Retrieval and Answer Generation for Regulatory Texts**|Jhon Rayo et.al.|[2502.16767](http://arxiv.org/abs/2502.16767)|**[link](https://github.com/oyar99/ir-ag-reg)**|
|**2025-02-23**|**Code Summarization Beyond Function Level**|Vladimir Makharev et.al.|[2502.16704](http://arxiv.org/abs/2502.16704)|**[link](https://github.com/kilimanj4r0/code-summarization-beyond-function-level)**|
|**2025-02-23**|**Retrieval-Augmented Visual Question Answering via Built-in Autoregressive Search Engines**|Xinwei Long et.al.|[2502.16641](http://arxiv.org/abs/2502.16641)|null|
|**2025-02-23**|**Visual-RAG: Benchmarking Text-to-Image Retrieval Augmented Generation for Visual Knowledge Intensive Queries**|Yin Wu et.al.|[2502.16636](http://arxiv.org/abs/2502.16636)|**[link](https://github.com/LuciusLan/Visual-RAG)**|
|**2025-02-21**|**Cross-Format Retrieval-Augmented Generation in XR with LLMs for Context-Aware Maintenance Assistance**|Akos Nagy et.al.|[2502.15604](http://arxiv.org/abs/2502.15604)|null|
|**2025-02-21**|**Chats-Grid: An Iterative Retrieval Q&A Optimization Scheme Leveraging Large Model and Retrieval Enhancement Generation in smart grid**|Yunfeng Li et.al.|[2502.15583](http://arxiv.org/abs/2502.15583)|null|
|**2025-02-21**|**Pub-Guard-LLM: Detecting Fraudulent Biomedical Articles with Reliable Explanations**|Lihu Chen et.al.|[2502.15429](http://arxiv.org/abs/2502.15429)|**[link](https://github.com/tigerchen52/pub_guard_llm)**|
|**2025-02-21**|**Retrieval-Augmented Speech Recognition Approach for Domain Challenges**|Peng Shen et.al.|[2502.15264](http://arxiv.org/abs/2502.15264)|null|
|**2025-02-21**|**From Documents to Dialogue: Building KG-RAG Enhanced AI Assistants**|Manisha Mukherjee et.al.|[2502.15237](http://arxiv.org/abs/2502.15237)|null|
|**2025-02-21**|**Chain-of-Rank: Enhancing Large Language Models for Domain-Specific RAG in Edge Device**|Juntae Lee et.al.|[2502.15134](http://arxiv.org/abs/2502.15134)|null|
|**2025-02-20**|**Reducing Hallucinations of Medical Multimodal Large Language Models with Visual Retrieval-Augmented Generation**|Yun-Wei Chu et.al.|[2502.15040](http://arxiv.org/abs/2502.15040)|null|
|**2025-02-20**|**Is Relevance Propagated from Retriever to Generator in RAG?**|Fangzheng Tian et.al.|[2502.15025](http://arxiv.org/abs/2502.15025)|null|
|**2025-02-20**|**A Socratic RAG Approach to Connect Natural Language Queries on Research Topics with Knowledge Organization Systems**|Lew Lefton et.al.|[2502.15005](http://arxiv.org/abs/2502.15005)|null|
|**2025-02-20**|**Benchmarking Multimodal RAG through a Chart-based Document Question-Answering Generation Framework**|Yuming Yang et.al.|[2502.14864](http://arxiv.org/abs/2502.14864)|**[link](https://github.com/nomothings/charge)**|
|**2025-02-20**|**From RAG to Memory: Non-Parametric Continual Learning for Large Language Models**|Bernal Jiménez Gutiérrez et.al.|[2502.14802](http://arxiv.org/abs/2502.14802)|**[link](https://github.com/osu-nlp-group/hipporag)**|
|**2025-02-20**|**On the Influence of Context Size and Model Choice in Retrieval-Augmented Generation Systems**|Juraj Vladika et.al.|[2502.14759](http://arxiv.org/abs/2502.14759)|**[link](https://github.com/jvladika/ContextRAG)**|
|**2025-02-20**|**WavRAG: Audio-Integrated Retrieval Augmented Generation for Spoken Dialogue Models**|Yifu Chen et.al.|[2502.14727](http://arxiv.org/abs/2502.14727)|null|
|**2025-02-20**|**FIND: Fine-grained Information Density Guided Adaptive Retrieval-Augmented Generation for Disease Diagnosis**|Mingyi Jia et.al.|[2502.14614](http://arxiv.org/abs/2502.14614)|null|
|**2025-02-20**|**EpMAN: Episodic Memory AttentioN for Generalizing to Longer Contexts**|Subhajit Chaudhury et.al.|[2502.14280](http://arxiv.org/abs/2502.14280)|null|
|**2025-02-20**|**Fact or Guesswork? Evaluating Large Language Model's Medical Knowledge with Structured One-Hop Judgment**|Jiaxi Li et.al.|[2502.14275](http://arxiv.org/abs/2502.14275)|null|
|**2025-02-20**|**PaperHelper: Knowledge-Based LLM QA Paper Reading Assistant**|Congrui Yin et.al.|[2502.14271](http://arxiv.org/abs/2502.14271)|null|
|**2025-02-19**|**Collaborative Retrieval for Large Language Model-based Conversational Recommender Systems**|Yaochen Zhu et.al.|[2502.14137](http://arxiv.org/abs/2502.14137)|**[link](https://github.com/yaochenzhu/crag)**|
|**2025-02-19**|**Towards Context-Robust LLMs: A Gated Representation Fine-tuning Approach**|Shenglai Zeng et.al.|[2502.14100](http://arxiv.org/abs/2502.14100)|null|
|**2025-02-19**|**RAG-Gym: Optimizing Reasoning and Search Agents with Process Supervision**|Guangzhi Xiong et.al.|[2502.13957](http://arxiv.org/abs/2502.13957)|null|
|**2025-02-19**|**DH-RAG: A Dynamic Historical Context-Powered Retrieval-Augmented Generation Method for Multi-Turn Dialogue**|Feiyuan Zhang et.al.|[2502.13847](http://arxiv.org/abs/2502.13847)|null|
|**2025-02-19**|**In-Place Updates of a Graph Index for Streaming Approximate Nearest Neighbor Search**|Haike Xu et.al.|[2502.13826](http://arxiv.org/abs/2502.13826)|null|
|**2025-02-19**|**TrustRAG: An Information Assistant with Retrieval Augmented Generation**|Yixing Fan et.al.|[2502.13719](http://arxiv.org/abs/2502.13719)|**[link](https://github.com/gomate-community/trustrag)**|
|**2025-02-19**|**Are Large Language Models In-Context Graph Learners?**|Jintang Li et.al.|[2502.13562](http://arxiv.org/abs/2502.13562)|null|
|**2025-02-19**|**VLAS: Vision-Language-Action Model With Speech Instructions For Customized Robot Manipulation**|Wei Zhao et.al.|[2502.13508](http://arxiv.org/abs/2502.13508)|**[link](https://github.com/whichwhichgone/VLAS)**|
|**2025-02-19**|**Towards Geo-Culturally Grounded LLM Generations**|Piyawat Lertvittayakumjorn et.al.|[2502.13497](http://arxiv.org/abs/2502.13497)|null|
|**2025-02-19**|**What are Models Thinking about? Understanding Large Language Model Hallucinations "Psychology" through Model Inner State Analysis**|Peiran Wang et.al.|[2502.13490](http://arxiv.org/abs/2502.13490)|null|
|**2025-02-19**|**HawkBench: Investigating Resilience of RAG Methods on Stratified Information-Seeking Tasks**|Hongjin Qian et.al.|[2502.13465](http://arxiv.org/abs/2502.13465)|null|
|**2025-02-19**|**RGAR: Recurrence Generation-augmented Retrieval for Factual-aware Medical Question Answering**|Sichu Liang et.al.|[2502.13361](http://arxiv.org/abs/2502.13361)|null|
|**2025-02-18**|**Oreo: A Plug-in Context Reconstructor to Enhance Retrieval-Augmented Generation**|Sha Li et.al.|[2502.13019](http://arxiv.org/abs/2502.13019)|null|
|**2025-02-18**|**Adaptive Knowledge Graphs Enhance Medical Question Answering: Bridging the Gap Between LLMs and Evolving Medical Knowledge**|Mohammad Reza Rezaei et.al.|[2502.13010](http://arxiv.org/abs/2502.13010)|null|
|**2025-02-18**|**Infinite Retrieval: Attention Enhanced LLMs in Long-Context Processing**|Xiaoju Ye et.al.|[2502.12962](http://arxiv.org/abs/2502.12962)|null|
|**2025-02-18**|**RAPID: Retrieval Augmented Training of Differentially Private Diffusion Models**|Tanqiu Jiang et.al.|[2502.12794](http://arxiv.org/abs/2502.12794)|**[link](https://github.com/tanqiujiang/rapid)**|
|**2025-02-18**|**MomentSeeker: A Comprehensive Benchmark and A Strong Baseline For Moment Retrieval Within Long Videos**|Huaying Yuan et.al.|[2502.12558](http://arxiv.org/abs/2502.12558)|null|
|**2025-02-18**|**Efficient OpAmp Adaptation for Zoom Attention to Golden Contexts**|Haoyuan Wu et.al.|[2502.12502](http://arxiv.org/abs/2502.12502)|null|
|**2025-02-18**|**Emulating Retrieval Augmented Generation via Prompt Engineering for Enhanced Long Context Comprehension in LLMs**|Joon Park et.al.|[2502.12462](http://arxiv.org/abs/2502.12462)|null|
|**2025-02-18**|**HopRAG: Multi-Hop Reasoning for Logic-Aware Retrieval-Augmented Generation**|Hao Liu et.al.|[2502.12442](http://arxiv.org/abs/2502.12442)|null|
|**2025-02-17**|**REAL-MM-RAG: A Real-World Multi-Modal Retrieval Benchmark**|Navve Wasserman et.al.|[2502.12342](http://arxiv.org/abs/2502.12342)|null|
|**2025-02-17**|**Fast or Better? Balancing Accuracy and Cost in Retrieval-Augmented Generation with Flexible User Control**|Jinyan Su et.al.|[2502.12145](http://arxiv.org/abs/2502.12145)|**[link](https://github.com/jinyansu1/flare-aug)**|
|**2025-02-17**|**REVERSUM: A Multi-staged Retrieval-Augmented Generation Method to Enhance Wikipedia Tail Biographies through Personal Narratives**|Sayantan Adak et.al.|[2502.12137](http://arxiv.org/abs/2502.12137)|**[link](https://github.com/sayantan11995/wikipedia_enrichment)**|
|**2025-02-17**|**CONSTRUCTA: Automating Commercial Construction Schedules in Fabrication Facilities with Large Language Models**|Yifan Zhang et.al.|[2502.12066](http://arxiv.org/abs/2502.12066)|null|
|**2025-02-17**|**Exploring Large Language Models in Healthcare: Insights into Corpora Sources, Customization Strategies, and Evaluation Metrics**|Shuqi Yang et.al.|[2502.11861](http://arxiv.org/abs/2502.11861)|null|
|**2025-02-17**|**FineFilter: A Fine-grained Noise Filtering Mechanism for Retrieval-Augmented Large Language Models**|Qianchi Zhang et.al.|[2502.11811](http://arxiv.org/abs/2502.11811)|null|
|**2025-02-17**|**Cognitive-Aligned Document Selection for Retrieval-augmented Generation**|Bingyu Wan et.al.|[2502.11770](http://arxiv.org/abs/2502.11770)|null|
|**2025-02-17**|**Multi-Modal Retrieval Augmentation for Open-Ended and Knowledge-Intensive Video Question Answering**|Md Zarif Ul Alam et.al.|[2502.11747](http://arxiv.org/abs/2502.11747)|null|
|**2025-02-17**|**FaMTEB: Massive Text Embedding Benchmark in Persian Language**|Erfan Zinvandi et.al.|[2502.11571](http://arxiv.org/abs/2502.11571)|null|
|**2025-02-17**|**Does RAG Really Perform Bad For Long-Context Processing?**|Kun Luo et.al.|[2502.11444](http://arxiv.org/abs/2502.11444)|null|
|**2025-02-17**|**Revisiting Robust RAG: Do We Still Need Complex Robust Training in the Era of Powerful LLMs?**|Hanxing Ding et.al.|[2502.11400](http://arxiv.org/abs/2502.11400)|null|
|**2025-02-14**|**CLaMP 3: Universal Music Information Retrieval Across Unaligned Modalities and Unseen Languages**|Shangda Wu et.al.|[2502.10362](http://arxiv.org/abs/2502.10362)|**[link](https://github.com/sanderwood/clamp3)**|
|**2025-02-14**|**Agentic Verification for Ambiguous Query Disambiguation**|Youngwon Lee et.al.|[2502.10352](http://arxiv.org/abs/2502.10352)|null|
|**2025-02-14**|**NeuroXVocal: Detection and Explanation of Alzheimer's Disease through Non-invasive Analysis of Picture-prompted Speech**|Nikolaos Ntampakis et.al.|[2502.10108](http://arxiv.org/abs/2502.10108)|null|
|**2025-02-14**|**LaRA: Benchmarking Retrieval-Augmented Generation and Long-Context LLMs - No Silver Bullet for LC or RAG Routing**|Kuan Li et.al.|[2502.09977](http://arxiv.org/abs/2502.09977)|null|
|**2025-02-14**|**ChatIoT: Large Language Model-based Security Assistant for Internet of Things with Retrieval-Augmented Generation**|Ye Dong et.al.|[2502.09896](http://arxiv.org/abs/2502.09896)|null|
|**2025-02-14**|**ArchRAG: Attributed Community-based Hierarchical Retrieval-Augmented Generation**|Shu Wang et.al.|[2502.09891](http://arxiv.org/abs/2502.09891)|null|
|**2025-02-13**|**Knowledge-Enhanced Program Repair for Data Science Code**|Shuyin Ouyang et.al.|[2502.09771](http://arxiv.org/abs/2502.09771)|null|
|**2025-02-13**|**Do LLMs Recognize Your Preferences? Evaluating Personalized Preference Following in LLMs**|Siyan Zhao et.al.|[2502.09597](http://arxiv.org/abs/2502.09597)|**[link](https://github.com/amazon-science/PrefEval)**|
|**2025-02-13**|**KIMAs: A Configurable Knowledge Integrated Multi-Agent System**|Zitao Li et.al.|[2502.09596](http://arxiv.org/abs/2502.09596)|null|
|**2025-02-13**|**ImageRAG: Dynamic Image Retrieval for Reference-Guided Image Generation**|Rotem Shalev-Arkushin et.al.|[2502.09411](http://arxiv.org/abs/2502.09411)|null|
|**2025-02-13**|**SQuARE: Sequential Question Answering Reasoning Engine for Enhanced Chain-of-Thought in Large Language Models**|Daniel Fleischer et.al.|[2502.09390](http://arxiv.org/abs/2502.09390)|**[link](https://github.com/intellabs/rag-fit)**|
|**2025-02-13**|**KET-RAG: A Cost-Efficient Multi-Granular Indexing Framework for Graph-RAG**|Yiqian Huang et.al.|[2502.09304](http://arxiv.org/abs/2502.09304)|**[link](https://github.com/waetr/KET-RAG)**|
|**2025-02-13**|**Improving TCM Question Answering through Tree-Organized Self-Reflective Retrieval with LLMs**|Chang Liu et.al.|[2502.09156](http://arxiv.org/abs/2502.09156)|null|
|**2025-02-13**|**Enhancing RAG with Active Learning on Conversation Records: Reject Incapables and Answer Capables**|Xuzhao Geng et.al.|[2502.09073](http://arxiv.org/abs/2502.09073)|null|
|**2025-02-13**|**Diversity Enhances an LLM's Performance in RAG and Long-context Task**|Zhchao Wang et.al.|[2502.09017](http://arxiv.org/abs/2502.09017)|null|
|**2025-02-12**|**Ask in Any Modality: A Comprehensive Survey on Multimodal Retrieval-Augmented Generation**|Mohammad Mahdi Abootorabi et.al.|[2502.08826](http://arxiv.org/abs/2502.08826)|**[link](https://github.com/llm-lab-org/multimodal-rag-survey)**|
|**2025-02-12**|**From PowerPoint UI Sketches to Web-Based Applications: Pattern-Driven Code Generation for GIS Dashboard Development Using Knowledge-Augmented LLMs, Context-Aware Visual Prompting, and the React Framework**|Haowen Xu et.al.|[2502.08756](http://arxiv.org/abs/2502.08756)|null|
|**2025-02-12**|**Systematic Knowledge Injection into Large Language Models via Diverse Augmentation for Domain-Specific RAG**|Kushagra Bhushan et.al.|[2502.08356](http://arxiv.org/abs/2502.08356)|**[link](https://github.com/kushagrabhushan/Systematic-Knowledge-Injection)**|
|**2025-02-12**|**UniCoRN: Unified Commented Retrieval Network with LMMs**|Maximilian Jaritz et.al.|[2502.08254](http://arxiv.org/abs/2502.08254)|null|
|**2025-02-12**|**ParetoRAG: Leveraging Sentence-Context Attention for Robust and Efficient Retrieval-Augmented Generation**|Ruobing Yao et.al.|[2502.08178](http://arxiv.org/abs/2502.08178)|null|
|**2025-02-12**|**Cognify: Supercharging Gen-AI Workflows With Hierarchical Autotuning**|Zijian He et.al.|[2502.08056](http://arxiv.org/abs/2502.08056)|**[link](https://github.com/GenseeAI/cognify)**|
|**2025-02-11**|**Training Sparse Mixture Of Experts Text Embedding Models**|Zach Nussbaum et.al.|[2502.07972](http://arxiv.org/abs/2502.07972)|**[link](https://github.com/nomic-ai/contrastors)**|
|**2025-02-11**|**Elevating Legal LLM Responses: Harnessing Trainable Logical Structures and Semantic Knowledge with Legal Reasoning**|Rujing Yao et.al.|[2502.07912](http://arxiv.org/abs/2502.07912)|**[link](https://github.com/RujingYao/LSIM)**|
|**2025-02-11**|**Graph RAG-Tool Fusion**|Elias Lumer et.al.|[2502.07223](http://arxiv.org/abs/2502.07223)|**[link](https://github.com/eliaslumer/graph-rag-tool-fusion-toollinkos)**|
|**2025-02-10**|**GraNNite: Enabling High-Performance Execution of Graph Neural Networks on Resource-Constrained Neural Processing Units**|Arghadip Das et.al.|[2502.06921](http://arxiv.org/abs/2502.06921)|**[link](https://github.com/arghadippurdue/GraNNite)**|
|**2025-02-10**|**Transparent NLP: Using RAG and LLM Alignment for Privacy Q&A**|Anna Leschanowsky et.al.|[2502.06652](http://arxiv.org/abs/2502.06652)|null|
|**2025-02-10**|**Combining Large Language Models with Static Analyzers for Code Review Generation**|Imen Jaoua et.al.|[2502.06633](http://arxiv.org/abs/2502.06633)|null|
|**2025-02-10**|**C-3PO: Compact Plug-and-Play Proxy Optimization to Achieve Human-like Retrieval-Augmented Generation**|Guoxin Chen et.al.|[2502.06205](http://arxiv.org/abs/2502.06205)|null|
|**2025-02-10**|**Optimizing Knowledge Integration in Retrieval-Augmented Generation with Self-Selection**|Yan Weng et.al.|[2502.06148](http://arxiv.org/abs/2502.06148)|null|
|**2025-02-11**|**RALLRec: Improving Retrieval Augmented Large Language Model Recommendation with Representation Learning**|Jian Xu et.al.|[2502.06101](http://arxiv.org/abs/2502.06101)|**[link](https://github.com/jianxu95/rallrec)**|
|**2025-02-09**|**MetaChain: A Fully-Automated and Zero-Code Framework for LLM Agents**|Jiabin Tang et.al.|[2502.05957](http://arxiv.org/abs/2502.05957)|null|
|**2025-02-11**|**Enhancing Financial Time-Series Forecasting with Retrieval-Augmented Large Language Models**|Mengxi Xiao et.al.|[2502.05878](http://arxiv.org/abs/2502.05878)|null|
|**2025-02-09**|**Quality Assurance for LLM-RAG Systems: Empirical Insights from Tourism Application Testing**|Bestoun S. Ahmed et.al.|[2502.05782](http://arxiv.org/abs/2502.05782)|null|
|**2025-02-08**|**AI-Driven Electronic Health Records System for Enhancing Patient Data Management and Diagnostic Support in Egypt**|Arwa Alorbany et.al.|[2502.05603](http://arxiv.org/abs/2502.05603)|null|
|**2025-02-08**|**APE: Faster and Longer Context-Augmented Generation via Adaptive Parallel Encoding**|Xinyu Yang et.al.|[2502.05431](http://arxiv.org/abs/2502.05431)|null|
|**2025-02-07**|**Enhancing Health Information Retrieval with RAG by Prioritizing Topical Relevance and Factual Accuracy**|Rishabh Uapadhyay et.al.|[2502.04666](http://arxiv.org/abs/2502.04666)|null|
|**2025-02-07**|**Agentic Reasoning: Reasoning LLMs with Tools for the Deep Research**|Junde Wu et.al.|[2502.04644](http://arxiv.org/abs/2502.04644)|**[link](https://github.com/theworldofagents/agentic-reasoning)**|
|**2025-02-06**|**MedRAG: Enhancing Retrieval-augmented Generation with Knowledge Graph-Elicited Reasoning for Healthcare Copilot**|Xuejiao Zhao et.al.|[2502.04413](http://arxiv.org/abs/2502.04413)|**[link](https://github.com/snowteam2023/medrag)**|
|**2025-02-05**|**MARAGE: Transferable Multi-Model Adversarial Attack for Retrieval-Augmented Generation Data Extraction**|Xiao Hu et.al.|[2502.04360](http://arxiv.org/abs/2502.04360)|null|
|**2025-02-04**|**Open Foundation Models in Healthcare: Challenges, Paradoxes, and Opportunities with GenAI Driven Personalized Prescription**|Mahdi Alkaeed et.al.|[2502.04356](http://arxiv.org/abs/2502.04356)|null|
|**2025-02-06**|**MRAMG-Bench: A BeyondText Benchmark for Multimodal Retrieval-Augmented Multimodal Generation**|Qinhan Yu et.al.|[2502.04176](http://arxiv.org/abs/2502.04176)|null|
|**2025-02-06**|**LLMs to Support a Domain Specific Knowledge Assistant**|Maria-Flavia Lovin et.al.|[2502.04095](http://arxiv.org/abs/2502.04095)|null|
|**2025-02-06**|**Enhancing Online Learning Efficiency Through Heterogeneous Resource Integration with a Multi-Agent RAG System**|Devansh Srivastav et.al.|[2502.03948](http://arxiv.org/abs/2502.03948)|null|
|**2025-02-06**|**Experiments with Large Language Models on Retrieval-Augmented Generation for Closed-Source Simulation Software**|Andreas Baumann et.al.|[2502.03916](http://arxiv.org/abs/2502.03916)|null|
|**2025-02-05**|**MedBioLM: Optimizing Medical and Biological QA with Fine-Tuned Large Language Models and Retrieval-Augmented Generation**|Seonok Kim et.al.|[2502.03004](http://arxiv.org/abs/2502.03004)|null|
|**2025-02-05**|**OverThink: Slowdown Attacks on Reasoning LLMs**|Abhinav Kumar et.al.|[2502.02542](http://arxiv.org/abs/2502.02542)|**[link](https://github.com/akumar2709/overthink_public)**|
|**2025-02-05**|**Rankify: A Comprehensive Python Toolkit for Retrieval, Re-Ranking, and Retrieval-Augmented Generation**|Abdelrahman Abdallah et.al.|[2502.02464](http://arxiv.org/abs/2502.02464)|**[link](https://github.com/DataScienceUIBK/Rankify)**|
|**2025-02-04**|**Personalization Toolkit: Training Free Personalization of Large Vision Language Models**|Soroush Seifi et.al.|[2502.02452](http://arxiv.org/abs/2502.02452)|null|
|**2025-02-04**|**Conversation AI Dialog for Medicare powered by Finetuning and Retrieval Augmented Generation**|Atharva Mangeshkumar Agrawal et.al.|[2502.02249](http://arxiv.org/abs/2502.02249)|null|
|**2025-02-04**|**LLMSecConfig: An LLM-Based Approach for Fixing Software Container Misconfigurations**|Ziyang Ye et.al.|[2502.02009](http://arxiv.org/abs/2502.02009)|null|
|**2025-02-04**|**MPIC: Position-Independent Multimodal Context Caching System for Efficient MLLM Serving**|Shiju Zhao et.al.|[2502.01960](http://arxiv.org/abs/2502.01960)|null|
|**2025-02-03**|**Position: Towards a Responsible LLM-empowered Multi-Agent Systems**|Jinwei Hu et.al.|[2502.01714](http://arxiv.org/abs/2502.01714)|null|
|**2025-02-03**|**VideoRAG: Retrieval-Augmented Generation with Extreme Long-Context Videos**|Xubin Ren et.al.|[2502.01549](http://arxiv.org/abs/2502.01549)|**[link](https://github.com/hkuds/videorag)**|
|**2025-02-03**|**CondAmbigQA: A Benchmark and Dataset for Conditional Ambiguous Question Answering**|Zongxi Li et.al.|[2502.01523](http://arxiv.org/abs/2502.01523)|null|
|**2025-02-03**|**Topic-FlipRAG: Topic-Orientated Adversarial Opinion Manipulation Attacks to Retrieval-Augmented Generation Models**|Yuyang Gong et.al.|[2502.01386](http://arxiv.org/abs/2502.01386)|null|
|**2025-01-28**|**SafeRAG: Benchmarking Security in Retrieval-Augmented Generation of Large Language Model**|Xun Liang et.al.|[2501.18636](http://arxiv.org/abs/2501.18636)|**[link](https://github.com/iaar-shanghai/saferag)**|
|**2025-01-30**|**Can we Retrieve Everything All at Once? ARM: An Alignment-Oriented LLM-based Retrieval Method**|Peter Baile Chen et.al.|[2501.18539](http://arxiv.org/abs/2501.18539)|null|
|**2025-01-30**|**RbFT: Robust Fine-tuning for Retrieval-Augmented Generation against Retrieval Defects**|Yiteng Tu et.al.|[2501.18365](http://arxiv.org/abs/2501.18365)|**[link](https://github.com/StibiumT16/Robust-Fine-tuning)**|
|**2025-01-30**|**Leveraging LLM Agents for Automated Optimization Modeling for SASP Problems: A Graph-RAG based Approach**|Tianpeng Pan et.al.|[2501.18320](http://arxiv.org/abs/2501.18320)|null|
|**2025-01-29**|**GLLM: Self-Corrective G-Code Generation using Large Language Models with User Feedback**|Mohamed Abdelaal et.al.|[2501.17584](http://arxiv.org/abs/2501.17584)|null|
|**2025-01-29**|**AugmenTest: Enhancing Tests with LLM-Driven Oracles**|Shaker Mahmud Khandaker et.al.|[2501.17461](http://arxiv.org/abs/2501.17461)|**[link](https://github.com/se-fbk/augmentest)**|
|**2025-01-29**|**Leveraging In-Context Learning and Retrieval-Augmented Generation for Automatic Question Generation in Educational Domains**|Subhankar Maity et.al.|[2501.17397](http://arxiv.org/abs/2501.17397)|null|
|**2025-01-28**|**ASTRAL: Automated Safety Testing of Large Language Models**|Miriam Ugarte et.al.|[2501.17132](http://arxiv.org/abs/2501.17132)|null|
|**2025-01-28**|**Enhanced Retrieval of Long Documents: Leveraging Fine-Grained Block Representations with Large Language Models**|Minghan Li et.al.|[2501.17039](http://arxiv.org/abs/2501.17039)|null|
|**2025-01-28**|**Multiple Abstraction Level Retrieve Augment Generation**|Zheng Zheng et.al.|[2501.16952](http://arxiv.org/abs/2501.16952)|null|
|**2025-01-29**|**Optimizing Code Runtime Performance through Context-Aware Retrieval-Augmented Generation**|Manish Acharya et.al.|[2501.16692](http://arxiv.org/abs/2501.16692)|**[link](https://github.com/manishacharya60/rag-optimization)**|
|**2025-01-28**|**VeriFact: Verifying Facts in LLM-Generated Clinical Text with Electronic Health Records**|Philip Chung et.al.|[2501.16672](http://arxiv.org/abs/2501.16672)|**[link](https://github.com/philipchung/verifact)**|
|**2025-01-27**|**Characterizing Network Structure of Anti-Trans Actors on TikTok**|Maxyn Leitner et.al.|[2501.16507](http://arxiv.org/abs/2501.16507)|null|
|**2025-01-27**|**URAG: Implementing a Unified Hybrid RAG for Precise Answers in University Admission Chatbots -- A Case Study at HCMUT**|Long Nguyen et.al.|[2501.16276](http://arxiv.org/abs/2501.16276)|null|
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
|**2025-01-23**|**Med-R $^2$ : Crafting Trustworthy LLM Physicians through Retrieval and Reasoning of Evidence-Based Medicine**|Keer Lu et.al.|[2501.11885](http://arxiv.org/abs/2501.11885)|**[link](https://github.com/8023looker/med-rr)**|
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
|**2025-01-16**|**OmniThink: Expanding Knowledge Boundaries in Machine Writing through Thinking**|Zekun Xi et.al.|[2501.09751](http://arxiv.org/abs/2501.09751)|**[link](https://github.com/zjunlp/omnithink)**|
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
|**2025-01-10**|**VideoRAG: Retrieval-Augmented Generation over Video Corpus**|Soyeong Jeong et.al.|[2501.05874](http://arxiv.org/abs/2501.05874)|**[link](https://github.com/starsuzi/videorag)**|
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
|**2024-12-22**|**MINTQA: A Multi-Hop Question Answering Benchmark for Evaluating LLMs on New and Tail Knowledge**|Jie He et.al.|[2412.17032](http://arxiv.org/abs/2412.17032)|**[link](https://github.com/probe2/multi-hop)**|
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
|**2024-12-18**|**A2H: A UI Converter from Android to HarmonyOS Platform**|Chen Wang et.al.|[2412.13693](http://arxiv.org/abs/2412.13693)|**[link](https://github.com/openselab/uitrans)**|
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

<p align=right>(<a href=#updated-on-20250404>back to top</a>)</p>

## text2sql

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-04-03**|**LearNAT: Learning NL2SQL with AST-guided Task Decomposition for Large Language Models**|Weibin Liao et.al.|[2504.02327](http://arxiv.org/abs/2504.02327)|null|自然语言到SQL（NL2SQL）已成为实现与数据库无缝交互的关键任务。最近，大型语言模型（LLMs）在这一领域展示了显著的性能。然而，现有的NL2SQL方法主要依赖于通过提示工程来利用闭源LLM，而开源模型通常需要微调以获取特定领域的知识。尽管付出了这些努力，开源LLM在处理复杂的NL2SQL任务时仍然遇到困难，这是因为用户查询目标的间接表达以及用户查询和数据库模式之间的语义差距。受强化学习在数学问题解决中促进LLM逐步推理的应用启发，我们提出了LearNAT（基于AST引导的任务分解的学习NL2SQL），这是一种新颖的框架，通过任务分解和强化学习提高开源LLM在复杂NL2SQL任务上的表现。LearNAT引入了三个关键组件：(1) 分解合成过程，该过程利用抽象语法树（ASTs）来指导任务分解的有效搜索和剪枝策略；(2) 边界感知强化学习，它通过带有AST边界的DPO进行细粒度的步骤级优化；(3) 自适应示例推理机制，用于动态选择相关示例以增强分解能力。在两个基准数据集Spider和BIRD上的广泛实验表明，LearNAT使70亿参数的开源LLM能够达到与GPT-4相当的性能，同时提供了更高的效率和可访问性。|
|**2025-04-02**|**Review, Refine, Repeat: Understanding Iterative Decoding of AI Agents with Dynamic Evaluation and Selection**|Souradip Chakraborty et.al.|[2504.01931](http://arxiv.org/abs/2504.01931)|null|尽管AI代理在各种任务中表现出色，但在复杂的多模态应用、结构化生成和策略规划方面仍存在困难。通过标准微调进行改进通常是不切实际的，因为解决代理任务通常依赖于黑盒API访问，而无法控制模型参数。像最佳N选（BON）采样这样的推理时间方法提供了一个简单但有效的替代方案来提高性能。然而，BON缺乏迭代反馈整合机制。因此，我们提出了迭代代理解码（IAD），它结合了迭代细化与动态候选评估和选择，并由验证器指导。IAD在如何设计和整合反馈方面有所不同，特别优化以从奖励分数中提取最大信号。我们在Sketch2Code、Text2SQL和Webshop上对基线进行了详细比较，结果显示IAD在关键指标上始终优于基线，在Sketch2Code和Text2SQL（有无大型语言模型裁判）上实现了3-6%的绝对增益，在Webshop上的多个指标上实现了8-10%的增益。为了更好地理解IAD的增益来源，我们进行了对照实验，以分离自适应反馈与随机采样的影响，发现IAD的改进主要由验证器指导的细化驱动，而不仅仅是采样多样性。我们还展示了当由最优验证器指导时，IAD和BON都表现出随计算量增加而提升的推理时间扩展性。我们的分析强调了验证器质量在有效推理时间优化中的关键作用，并探讨了噪声和稀疏奖励对扩展行为的影响。这些发现共同提供了关于有效推理时间优化权衡和原则的关键见解。|
|**2025-03-30**|**Distill-C: Enhanced NL2SQL via Distilled Customization with LLMs**|Cong Duy Vu Hoang et.al.|[2504.00048](http://arxiv.org/abs/2504.00048)|null|随着大型语言模型（LLMs）在商业应用中的日益普及，人们对自然语言到SQL（NL2SQL）解决方案的兴趣也越来越大，其中高性能和高效率的需求相互竞争。特定领域和客户的具体要求进一步复杂化了这个问题。为了解决这一难题，我们引入了Distill-C，这是一个针对NL2SQL任务定制的蒸馏框架。Distill-C利用大型教师LLM通过一个强大且可扩展的管道生成高质量的合成数据。通过对这些合成数据进行微调，较小且开源的LLM能够与大十倍的教师模型相媲美甚至超越。在多个具有挑战性的基准测试中评估，Distill-C在执行准确率上相比来自三个不同LLM家族的基础模型平均提高了36%。此外，在三个内部客户基准测试中，Distill-C相对于基础模型表现出了22.6%的性能提升。我们的结果表明，Distill-C是一种有效、高性能且通用的方法，用于部署轻量级但功能强大的NL2SQL模型，在保持低计算成本的同时提供卓越的准确性。|
|**2025-03-22**|**Feather-SQL: A Lightweight NL2SQL Framework with Dual-Model Collaboration Paradigm for Small Language Models**|Wenqi Pei et.al.|[2503.17811](http://arxiv.org/abs/2503.17811)|null|自然语言转SQL（NL2SQL）在大型语言模型（LLMs）中取得了显著进展。然而，这些模型通常依赖于闭源系统和高计算资源，在数据隐私和部署方面带来了挑战。相比之下，小型语言模型（SLMs）在NL2SQL任务上表现不佳，且与现有框架不兼容。为了解决这些问题，我们引入了Feather-SQL，这是一种针对SLMs的新轻量级框架。Feather-SQL通过1）模式剪枝和链接，2）多路径和多候选生成来提高SQL的可执行性和准确性。此外，我们还引入了1+1模型协作范式，该范式将一个强大的通用聊天模型与一个经过微调的SQL专家模型配对，结合了强大的分析推理能力和高精度的SQL生成能力。在BIRD上的实验结果表明，Feather-SQL提高了SLMs在NL2SQL任务上的性能，对于未经微调的模型提升了约10%的性能。所提出的范式将SLMs的准确率上限提高到了54.76%，突显了其有效性。|
|**2025-03-15**|**NL2SQL-BUGs: A Benchmark for Detecting Semantic Errors in NL2SQL Translation**|Xinyu Liu et.al.|[2503.11984](http://arxiv.org/abs/2503.11984)|null|自然语言到SQL（即NL2SQL）的转换对于普及数据库访问至关重要，但即使是目前最先进的模型也经常生成语义上不正确的SQL查询，这阻碍了这些技术被数据库供应商广泛采用。虽然现有的NL2SQL基准测试主要关注正确的查询转换，但我们认为，一个专门用于识别NL2SQL转换中常见错误的基准同样重要，因为准确检测这些错误是任何后续修正（无论是由人类还是模型执行）的前提。为了解决这一空白，我们提出了NL2SQL-BUGs，这是首个专门用于检测和分类NL2SQL转换中语义错误的基准。NL2SQL-BUGs采用两层分类法系统地对语义错误进行分类，涵盖了9个主要类别和31个子类别。该基准包含2018个专家标注的实例，每个实例包括一个自然语言查询、数据库模式和SQL查询，并对语义不正确的查询进行了详细的错误标注。通过全面的实验，我们展示了当前大型语言模型在语义错误检测方面存在显著局限性，平均检测准确率仅为75.16%。尽管如此，这些模型成功检测到了广泛使用的NL2SQL数据集BIRD中的106个错误（占6.91%），这些错误之前是该基准中的标注错误。这突显了在NL2SQL系统中进行语义错误检测的重要性。|
|**2025-03-04**|**NLI4DB: A Systematic Review of Natural Language Interfaces for Databases**|Mengyi Liu et.al.|[2503.02435](http://arxiv.org/abs/2503.02435)|null|随着在生活各个领域对数据库查询需求的不断增加，研究人员对自然语言接口数据库（NLIDB）给予了极大的关注。本文全面综述了最近提出的NLIDB系统。首先简要介绍了自然语言处理技术、可执行数据库语言以及自然语言与可执行语言之间的中间表示，然后概述了从自然语言到可执行数据库语言的翻译过程。翻译过程分为三个阶段：(i) 自然语言预处理，(ii) 自然语言理解，和 (iii) 自然语言翻译。在预处理阶段采用了传统方法和数据驱动方法。传统方法依赖于预定义的规则和语法，涉及正则表达式、依存关系解析和命名实体识别等技术。数据驱动方法依赖大规模数据和机器学习模型，使用词嵌入和模式链接等技术。自然语言理解方法分为三类：(i) 基于规则的方法，(ii) 基于机器学习的方法，和 (iii) 混合方法。随后，我们描述了在关系数据库和时空数据库上构建可执行语言的一般过程。接着介绍了将自然语言转换为可执行语言的常见基准测试和评估指标，并探讨了生成新基准测试的方法。最后，总结了NLIDB系统的分类、发展和改进，并讨论了与NLIDB相关的深度语言理解和数据库交互技术，包括(i) 使用大语言模型进行Text2SQL任务，(ii) 从SQL生成自然语言解释，和 (iii) 将语音查询转换为SQL。|
|**2025-02-23**|**SQLong: Enhanced NL2SQL for Longer Contexts with LLMs**|Dai Quoc Nguyen et.al.|[2502.16747](http://arxiv.org/abs/2502.16747)|null|开放权重的大型语言模型（LLMs）在自然语言到SQL（NL2SQL）任务中显著提升了性能。然而，当处理大型数据库模式时，由于上下文长度增加，其效果会减弱。为了解决这一限制，我们提出了SQLong，这是一种新颖且高效的数据增强框架，旨在提高LLM在长上下文场景下的NL2SQL任务性能。SQLong通过向现有数据库模式添加额外的合成CREATE TABLE命令和相应的数据行来生成增强的数据集，这些数据是从训练数据中的多样化模式中采样得到的。这种方法有效地在微调和评估过程中模拟了长上下文场景。通过对Spider和BIRD数据集的实验，我们证明了使用SQLong增强数据进行微调的LLM明显优于那些在标准数据集上训练的LLM。这表明SQLong的实际应用及其对提高复杂数据库模式下NL2SQL能力的影响。|
|**2025-03-23**|**Balancing Content Size in RAG-Text2SQL System**|Prakhar Gurawa et.al.|[2502.15723](http://arxiv.org/abs/2502.15723)|null|大型语言模型（LLMs）已成为将自然语言查询转换为SQL命令的有前景的解决方案，使得数据库交互变得无缝。然而，这些文本到SQL（Text2SQL）系统面临固有的局限性，如幻觉、过时的知识和不可追踪的推理。为了解决这些挑战，将检索增强生成（RAG）与Text2SQL模型集成的方法越来越受到关注。RAG作为一种检索机制，提供必要的上下文信息，如表结构和元数据，以增强查询生成过程。尽管具有潜力，但RAG + Text2SQL系统易受检索文档的质量和大小的影响。虽然更丰富的文档内容可以提高模式相关性和检索准确性，但它也引入了噪声，增加了幻觉的风险，并随着Text2SQL模型提示大小的增加降低了查询保真度。本研究探讨了文档大小和质量之间的微妙权衡，旨在找到优化系统性能的平衡点。我们识别出性能下降的关键阈值，并提出缓解这些挑战的可行策略。此外，我们还探讨了Text2SQL模型中的幻觉现象，强调精心策划的文档呈现对减少错误的关键作用。我们的发现为增强RAG + Text2SQL系统的鲁棒性提供了路线图，并为实际应用提供了实用见解。|
|**2025-02-17**|**SQL-o1: A Self-Reward Heuristic Dynamic Search Method for Text-to-SQL**|Shuai Lyu et.al.|[2502.11741](http://arxiv.org/abs/2502.11741)|**[link](https://github.com/shuailyu0110/sql-o1)**|**文本到SQL（Text2SQL）任务旨在将自然语言查询转换为可执行的SQL查询。得益于大型语言模型（LLMs）的应用，该领域已经取得了显著进展。然而，诸如模型可扩展性、有限的生成空间以及SQL生成中的连贯性问题等挑战仍然存在。为了解决这些问题，我们提出了SQL-o1，这是一种基于自奖励的启发式搜索方法，旨在增强LLMs在SQL查询生成中的推理能力。SQL-o1结合了蒙特卡洛树搜索（MCTS）进行启发式过程级搜索，并构建了一个Schema-Aware数据集，以帮助模型更好地理解数据库模式。在Bird和Spider数据集上的大量实验表明，与最新的基线方法相比，SQL-o1在复杂的Bird数据集上提高了10.8%的执行准确性，甚至超过了基于GPT-4的方法。此外，SQL-o1在少样本学习场景中表现出色，并显示出强大的跨模型迁移能力。我们的代码公开在：https://github.com/ShuaiLyu0110/SQL-o1。**|
|**2025-01-30**|**Fundamental Challenges in Evaluating Text2SQL Solutions and Detecting Their Limitations**|Cedric Renggli et.al.|[2501.18197](http://arxiv.org/abs/2501.18197)|null|在这项工作中，我们深入探讨了评估Text2SQL解决方案的基本挑战，并强调了潜在的失败原因以及依赖现有基准中的聚合指标可能带来的风险。我们指出了当前开放基准中的两个主要未解决的限制：（1）评估数据中的数据质量问题，这主要是由于未能捕捉自然语言描述转化为结构化查询时的概率性质（例如，自然语言的模糊性），以及（2）使用不同的匹配函数作为SQL等价性的近似方法所引入的偏差。为了将这两个限制置于具体情境中，我们提出了一种统一的分类法，涵盖所有可能导致预测和评估错误的Text2SQL限制。然后，我们通过使用最先进的Text2SQL解决方案和基准对这些限制进行了调查，以此来论证该分类法。我们用实际例子描述了限制的原因，并为分类法中的每个类别提出了潜在的缓解方案。最后，我们强调了在部署此类缓解策略或尝试自动应用该分类法时遇到的开放性挑战。|
|**2025-03-20**|**Is Long Context All You Need? Leveraging LLM's Extended Context for NL2SQL**|Yeounoh Chung et.al.|[2501.12372](http://arxiv.org/abs/2501.12372)|**[link](https://github.com/yeounoh/lc_nl2sql)**|
|**2025-02-08**|**Semantic Captioning: Benchmark Dataset and Graph-Aware Few-Shot In-Context Learning for SQL2Text**|Ali Al-Lawati et.al.|[2501.03166](http://arxiv.org/abs/2501.03166)|**[link](https://github.com/aliwister/ast-icl)**|
|**2025-01-03**|**CarbonChat: Large Language Model-Based Corporate Carbon Emission Analysis and Climate Knowledge Q&A System**|Zhixuan Cao et.al.|[2501.02031](http://arxiv.org/abs/2501.02031)|null|
|**2024-12-22**|**A Plug-and-Play Natural Language Rewriter for Natural Language to SQL**|Peixian Ma et.al.|[2412.17068](http://arxiv.org/abs/2412.17068)|null|
|**2024-12-17**|**SynthCypher: A Fully Synthetic Data Generation Framework for Text-to-Cypher Querying in Knowledge Graphs**|Aman Tiwari et.al.|[2412.12612](http://arxiv.org/abs/2412.12612)|null|
|**2024-12-13**|**ROUTE: Robust Multitask Tuning and Collaboration for Text-to-SQL**|Yang Qin et.al.|[2412.10138](http://arxiv.org/abs/2412.10138)|**[link](https://github.com/alibaba/route)**|
|**2024-12-04**|**DataLab: A Unified Platform for LLM-Powered Business Intelligence**|Luoxuan Weng et.al.|[2412.02205](http://arxiv.org/abs/2412.02205)|null|
|**2024-11-05**|**Grounding Natural Language to SQL Translation with Data-Based Self-Explanations**|Yuankai Fan et.al.|[2411.02948](http://arxiv.org/abs/2411.02948)|**[link](https://github.com/Kaimary/CycleSQL)**|
|**2024-10-30**|**BIS: NL2SQL Service Evaluation Benchmark for Business Intelligence Scenarios**|Bora Caglayan et.al.|[2410.22925](http://arxiv.org/abs/2410.22925)|**[link](https://github.com/boracaglayan/bis-nl2sql)**|
|**2024-10-15**|**LR-SQL: A Supervised Fine-Tuning Method for Text2SQL Tasks under Low-Resource Scenarios**|Wen Wuzhenghong et.al.|[2410.11457](http://arxiv.org/abs/2410.11457)|**[link](https://github.com/hongwin/lr-sql)**|
|**2024-08-27**|**Text2SQL is Not Enough: Unifying AI and Databases with TAG**|Asim Biswal et.al.|[2408.14717](http://arxiv.org/abs/2408.14717)|**[link](https://github.com/tag-research/tag-bench)**|
|**2024-12-04**|**A Survey of NL2SQL with Large Language Models: Where are we, and where are we going?**|Xinyu Liu et.al.|[2408.05109](http://arxiv.org/abs/2408.05109)|**[link](https://github.com/hkustdial/nl2sql_handbook)**|
|**2024-07-21**|**Towards Automated Data Sciences with Natural Language and SageCopilot: Practices and Lessons Learned**|Yuan Liao et.al.|[2407.21040](http://arxiv.org/abs/2407.21040)|null|
|**2024-11-07**|**A Survey on Employing Large Language Models for Text-to-SQL Tasks**|Liang Shi et.al.|[2407.15186](http://arxiv.org/abs/2407.15186)|null|
|**2024-06-12**|**DeTriever: Decoder-representation-based Retriever for Improving NL2SQL In-Context Learning**|Yuxi Feng et.al.|[2406.07913](http://arxiv.org/abs/2406.07913)|null|
|**2024-07-27**|**The Dawn of Natural Language to SQL: Are We Fully Ready?**|Boyan Li et.al.|[2406.01265](http://arxiv.org/abs/2406.01265)|**[link](https://github.com/hkustdial/nl2sql360)**|
|**2024-05-01**|**ChatBI: Towards Natural Language to Complex Business Intelligence SQL**|Jinqing Lian et.al.|[2405.00527](http://arxiv.org/abs/2405.00527)|null|
|**2024-03-29**|**PURPLE: Making a Large Language Model a Better SQL Writer**|Tonghui Ren et.al.|[2403.20014](http://arxiv.org/abs/2403.20014)|null|

<p align=right>(<a href=#updated-on-20250404>back to top</a>)</p>

## PPC

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-04-03**|**Tree-based Models for Vertical Federated Learning: A Survey**|Bingchen Qian et.al.|[2504.02285](http://arxiv.org/abs/2504.02285)|null|基于树的模型由于其有效性、鲁棒性和可解释性，在各种实际应用中取得了巨大成功，这激发了人们近年来在垂直联邦学习（VFL）场景中应用这些模型。本文从通信和计算协议的角度出发，对在VFL中应用基于树的模型进行了全面的研究，以提供一个整体的视角。我们将VFL中的基于树的模型分为两类：特征聚合模型和标签分散模型，并详细讨论了它们的特点、优势、隐私保护机制及应用。本研究还重点关注了基于树的模型在VFL中的实现，总结了几项设计原则，以更好地满足学术研究和工业部署的各种需求。我们进行了一系列实验，提供了关于不同类型基于树的模型之间差异和进展的经验观察。|
|**2025-04-03**|**Secure Generalization through Stochastic Bidirectional Parameter Updates Using Dual-Gradient Mechanism**|Shourya Goel et.al.|[2504.02213](http://arxiv.org/abs/2504.02213)|null|联邦学习（FL）由于能够在分散的客户端上进行隐私保护的协同训练，而无需直接将敏感数据上传到中央服务器，因此受到了越来越多的关注。然而，最近的研究强调了即使在FL框架内，私人数据也有可能被对手暴露的风险。一般来说，现有的方法在确保对隐私泄露具有抵抗力的同时牺牲了性能。我们通过提出的随机双向参数更新机制克服了这些问题，并在全球服务器上生成了多样化的模型。通过使用多样化的模型，我们在FL设置中提高了泛化能力和特征表示，这也有助于提高模型对抗隐私泄露的鲁棒性，而不损害模型的实用性。我们利用过去FL轮次中的全局模型，在服务器端对参数空间进行系统扰动，以确保模型泛化和抵抗隐私攻击的能力。我们通过对模型参数进行细粒度级别的系统扰动（即改变模型各层中的每个卷积滤波器），为每个客户端生成邻近区域内的多样化模型，从而从泛化和安全性的角度改进模型。我们在四个基准数据集上评估了所提出的方法，验证了其优越性。在模型实用性和抵抗隐私泄露的鲁棒性方面，我们超越了最先进的方法。我们通过多个定量和定性结果证明了该方法的有效性。|
|**2025-04-02**|**Like Oil and Water: Group Robustness Methods and Poisoning Defenses May Be at Odds**|Michael-Andrei Panaitescu-Liess et.al.|[2504.02142](http://arxiv.org/abs/2504.02142)|null|群体鲁棒性已成为机器学习（ML）中的主要关注点，因为传统的训练范式被发现会在少数群体上产生高错误率。在没有明确的群体标注的情况下，提出的解决方案依赖于旨在识别并在训练过程中放大少数样本的启发式方法。在我们的工作中，我们首先揭示了这些方法的一个关键缺陷：无法区分合法的少数样本和训练集中的中毒样本。通过同时放大中毒样本，群体鲁棒性方法无意中提高了对手的成功率——例如，从没有放大时的0%提高到超过97%。值得注意的是，我们在经验证据的基础上补充了一个不可能性结果，证明了在某些假设下标准启发式的这种无能为力。此外，仔细检查最近的集中式和联邦学习中的中毒防御方法，我们观察到它们依赖类似的启发式方法来识别哪些样本应被视为中毒样本并予以消除。因此，少数样本与中毒样本一同被消除，这损害了群体鲁棒性——例如，从没有消除少数样本时的55%下降到消除后的41%。最后，由于它们使用相似的启发式方法追求相反的目标，我们试图通过结合群体鲁棒性方法和中毒防御方法来缓解这种权衡的努力未能成功。通过揭示这种紧张关系，我们也希望强调基准驱动的ML学术研究如何可能掩盖不同指标之间的权衡，并带来潜在的负面影响。|
|**2025-04-02**|**On Model Protection in Federated Learning against Eavesdropping Attacks**|Dipankar Maity et.al.|[2504.02114](http://arxiv.org/abs/2504.02114)|null|在这项研究中，我们探讨了联邦学习算法对窃听敌手的防护能力。在我们的模型中，敌手能够截获从客户端传输到服务器的模型更新，从而创建自己对模型的估计。与以往主要关注保护客户端数据的研究不同，我们的工作转向保护客户端模型本身。通过理论分析，我们考察了各种因素如客户端选择的概率、局部目标函数的结构、服务器端的全局聚合以及窃听者的能力如何影响整体的保护水平。我们还通过数值实验验证了我们的发现，通过评估敌手达到的模型准确性来衡量保护效果。最后，我们将我们的结果与基于差分隐私的方法进行了比较，强调了这些方法在此特定情境下的局限性。|
|**2025-04-02**|**Efficient Federated Learning Tiny Language Models for Mobile Network Feature Prediction**|Daniel Becking et.al.|[2504.01947](http://arxiv.org/abs/2504.01947)|null|在电信领域，自治网络（ANs）根据特定需求（例如带宽）和可用资源自动调整配置。这些网络依赖于持续监控和智能机制来自我优化、自我修复和自我保护，如今通过神经网络（NNs）的增强来实现预测建模和模式识别。在这里，联邦学习（FL）允许多个配备有神经网络的自治网络单元协同训练模型，同时保护数据隐私。然而，联邦学习需要频繁传输大量神经数据，因此需要一种高效且标准化的压缩策略以确保可靠的通信。为了解决这一问题，我们研究了NNCodec，这是一种Fraunhofer实现的ISO/IEC神经网络编码（NNC）标准，在一个新颖的联邦学习框架中集成了微型语言模型（TLMs），用于各种移动网络特征预测（如ping、信噪比或频段频率）。我们在柏林V2X数据集上的实验结果表明，NNCodec实现了透明压缩（即性能损失可忽略不计），同时将通信开销降低到1%以下，展示了结合NNC与FL在协作学习的自治移动网络中的有效性。|
|**2025-04-02**|**Client Selection in Federated Learning with Data Heterogeneity and Network Latencies**|Harsh Vardhan et.al.|[2504.01921](http://arxiv.org/abs/2504.01921)|null|联邦学习（FL）是一种分布式机器学习范式，其中多个客户端基于其私有数据进行本地训练，然后将更新后的模型发送到中央服务器进行全局聚合。FL的实际收敛受到多种因素的挑战，主要障碍是客户端之间的异质性。这种异质性表现为关于本地数据分布的数据异质性和模型传输到服务器期间的延迟异质性。虽然先前的研究已经引入了各种有效的客户端选择方法来减轻这两种异质性中的任一负面影响，但在同时存在这两种异质性的实际场景中，尚缺乏有效的方法。在本文中，我们提出了两种新的理论最优客户端选择方案，可以同时处理这两种异质性。我们的方法涉及每轮通过最小化理论运行时间至收敛来解决简单的优化问题。在9个非独立同分布数据集、2种实际延迟分布和非凸神经网络模型上的实证评估表明，我们的算法至少与现有最佳基线相当，最多比它们好20倍。|
|**2025-04-02**|**CO-DEFEND: Continuous Decentralized Federated Learning for Secure DoH-Based Threat Detection**|Diego Cajaraville-Aboy et.al.|[2504.01882](http://arxiv.org/abs/2504.01882)|null|使用DNS over HTTPS (DoH)隧道技术的攻击者可以将恶意活动隐藏在加密的DNS流量中，这对网络安全构成了严重威胁，因为它允许恶意行为者绕过传统的监控和入侵检测系统，同时逃避常规流量分析技术的检测。机器学习(ML)技术可以用来检测DoH隧道；然而，其有效性依赖于包含良性与恶意流量的大规模数据集。由于隐私问题，跨实体共享此类数据集具有挑战性。在这项工作中，我们提出了CO-DEFEND（用于安全DoH基础威胁检测的连续去中心化联邦学习），这是一个去中心化联邦学习(DFL)框架，它使多个实体能够在保护数据隐私的同时协作训练分类机器学习模型，并增强对单点故障的抵御能力。所提出的DFL框架是可扩展且保护隐私的，基于一个联邦过程，该过程允许多个实体利用实时处理中的传入DoH流在线训练本地模型。此外，我们将四种经典的机器学习算法——支持向量机(SVM)、逻辑回归(LR)、决策树(DT)和随机森林(RF)——适应于联邦场景，并将其结果与神经网络等计算更复杂的替代方案进行比较。我们通过使用CIRA-CIC-DoHBrw-2020数据集来对比我们的提议方法与现有的机器学习方法，以展示其在检测恶意DoH隧道方面的有效性和带来的好处。|
|**2025-04-02**|**A Randomized Zeroth-Order Hierarchical Framework for Heterogeneous Federated Learning**|Yuyang Qiu et.al.|[2504.01839](http://arxiv.org/abs/2504.01839)|null|异构性在联邦学习（FL）中是一个关键且具有挑战性的方面，它显著影响模型性能和收敛性。在这篇论文中，我们提出了一种新的框架，将异构FL表述为一个层次优化问题。这一新框架通过双层公式化同时捕捉了本地和全局的训练过程，并能够实现以下功能：(i) 通过个性化学习框架解决客户端异质性；(ii) 捕捉服务器端的预训练过程；(iii) 通过非标准聚合更新全局模型；(iv) 允许不同数量的本地步骤；以及(v) 捕捉客户端的本地约束。我们设计并分析了一种隐式零阶FL方法（ZO-HFL），该方法提供了针对服务器代理和单个客户端代理的非渐近收敛保证，以及服务器代理和客户端代理在几乎确定意义上的渐近保证。值得注意的是，我们的方法不依赖于异构FL中的标准假设，如梯度差异有界条件。我们在图像分类任务上实现了我们的方法，并在不同的异构设置下与其他方法进行了比较。|
|**2025-04-02**|**A Two-Timescale Approach for Wireless Federated Learning with Parameter Freezing and Power Control**|Jinhao Ouyang et.al.|[2504.01752](http://arxiv.org/abs/2504.01752)|null|联邦学习（FL）使分布式设备能够在保护数据隐私的同时协作训练共享的机器学习（ML）模型。然而，资源有限的移动设备在模型参数的计算和通信成本上面临巨大挑战。在这篇论文中，我们观察到在训练过程中，模型参数往往在收敛之前很久就已经趋于稳定。基于这一观察，我们提出了一种两时间尺度的联邦学习框架，通过联合优化冻结稳定参数和控制不稳定参数的传输功率来平衡能耗与收敛性。首先，我们分析了模型参数冻结和不可靠传输对收敛速率的影响。接下来，我们将参数冻结比例和传输功率的两时间尺度优化问题形式化，以在能量预算约束下最小化模型收敛误差。为了解决这个问题，我们使用Lyapunov优化方法将问题分解为并行子问题，并进一步将每个子问题分解为两个不同时间尺度的问题。最优的参数冻结和功率控制策略是在线推导的。实验结果表明，所提出的方案优于基准方案。|
|**2025-04-02**|**Sky of Unlearning (SoUL): Rewiring Federated Machine Unlearning via Selective Pruning**|Md Mahabub Uz Zaman et.al.|[2504.01705](http://arxiv.org/abs/2504.01705)|null|无人机互联网（IoD）在数据收集和分析方面的协作已成为监控和环境监测等应用的关键。联邦学习（FL）使无人机能够以分散的方式训练机器学习模型，同时保护数据隐私。然而，在IoD网络中实施FL容易受到诸如数据投毒和模型逆向工程等攻击。联邦遗忘（FU）通过消除对抗性数据贡献来缓解这些风险，防止其对模型的影响。本文提出了一种名为天空遗忘（SoUL）的联邦遗忘框架，该框架能高效地移除被遗忘数据的影响，同时保持模型性能。设计了一种选择性剪枝算法，用于识别并移除在遗忘过程中起关键作用但对整体性能影响最小的神经元。仿真结果表明，SoUL优于现有的遗忘方法，达到了与完全重新训练相当的准确性，并减少了计算和通信开销，使其成为资源受限的IoD网络中可扩展且高效的解决方案。|
|**2025-04-02**|**Split Federated Learning for UAV-Enabled Integrated Sensing, Computation, and Communication**|Xiangwang Hou et.al.|[2504.01443](http://arxiv.org/abs/2504.01443)|null|
|**2025-04-02**|**Age-Aware Partial Gradient Update Strategy for Federated Learning Over the Air**|Ruihao Du et.al.|[2504.01357](http://arxiv.org/abs/2504.01357)|null|
|**2025-04-01**|**Towards Resilient Federated Learning in CyberEdge Networks: Recent Advances and Future Trends**|Kai Li et.al.|[2504.01240](http://arxiv.org/abs/2504.01240)|null|
|**2025-04-01**|**Personalized Federated Training of Diffusion Models with Privacy Guarantees**|Kumar Kshitij Patel et.al.|[2504.00952](http://arxiv.org/abs/2504.00952)|null|
|**2025-03-31**|**Federated Structured Sparse PCA for Anomaly Detection in IoT Networks**|Chenyi Huang et.al.|[2503.23981](http://arxiv.org/abs/2503.23981)|null|
|**2025-03-31**|**Communication-Efficient and Personalized Federated Foundation Model Fine-Tuning via Tri-Matrix Adaptation**|Yongle Li et.al.|[2503.23869](http://arxiv.org/abs/2503.23869)|null|
|**2025-03-31**|**Blockchain for Federated Learning in the Internet of Things: Trustworthy Adaptation, Standards, and the Road Ahead**|Farhana Javed et.al.|[2503.23823](http://arxiv.org/abs/2503.23823)|null|
|**2025-03-30**|**Buffer is All You Need: Defending Federated Learning against Backdoor Attacks under Non-iids via Buffering**|Xingyu Lyu et.al.|[2503.23511](http://arxiv.org/abs/2503.23511)|null|
|**2025-03-30**|**Federated Self-Supervised Learning for One-Shot Cross-Modal and Cross-Imaging Technique Segmentation**|Siladittya Manna et.al.|[2503.23507](http://arxiv.org/abs/2503.23507)|null|
|**2025-03-30**|**A Systematic Decade Review of Trip Route Planning with Travel Time Estimation based on User Preferences and Behavior**|Nikil Jayasuriya et.al.|[2503.23486](http://arxiv.org/abs/2503.23486)|null|
|**2025-03-30**|**FedCAPrivacy: Privacy-Preserving Heterogeneous Federated Learning with Anonymous Adaptive Clustering**|Yunan Wei et.al.|[2503.23292](http://arxiv.org/abs/2503.23292)|null|
|**2025-03-30**|**Two Heads Are Better than One: Model-Weight and Latent-Space Analysis for Federated Learning on Non-iid Data against Poisoning Attacks**|Xingyu Lyu et.al.|[2503.23288](http://arxiv.org/abs/2503.23288)|null|
|**2025-03-29**|**Multi-Agent Reinforcement Learning for Graph Discovery in D2D-Enabled Federated Learning**|Satyavrat Wagle et.al.|[2503.23218](http://arxiv.org/abs/2503.23218)|null|
|**2025-03-29**|**Enhancing Federated Learning Through Secure Cluster-Weighted Client Aggregation**|Kanishka Ranaweera et.al.|[2503.22971](http://arxiv.org/abs/2503.22971)|null|
|**2025-03-28**|**FLIP: Towards Comprehensive and Reliable Evaluation of Federated Prompt Learning**|Dongping Liao et.al.|[2503.22263](http://arxiv.org/abs/2503.22263)|**[link](https://github.com/0-ml/flip)**|
|**2025-03-28**|**Route-and-Aggregate Decentralized Federated Learning Under Communication Errors**|Weicai Li et.al.|[2503.22186](http://arxiv.org/abs/2503.22186)|null|
|**2025-03-28**|**Federated Intrusion Detection System Based on Unsupervised Machine Learning**|Maxime Gourceyraud et.al.|[2503.22065](http://arxiv.org/abs/2503.22065)|null|
|**2025-03-27**|**Energy Minimization for Participatory Federated Learning in IoT Analyzed via Game Theory**|Alessandro Buratto et.al.|[2503.21722](http://arxiv.org/abs/2503.21722)|null|
|**2025-03-27**|**Provable Reduction in Communication Rounds for Non-Smooth Convex Federated Learning**|Karlo Palenzuela et.al.|[2503.21627](http://arxiv.org/abs/2503.21627)|null|
|**2025-03-27**|**Improving $(α, f)$ -Byzantine Resilience in Federated Learning via layerwise aggregation and cosine distance**|Mario García-Márquez et.al.|[2503.21244](http://arxiv.org/abs/2503.21244)|**[link](https://github.com/ari-dasci/S-layerwise_cosine_aggregation)**|
|**2025-03-27**|**Resource-Efficient Federated Fine-Tuning Large Language Models for Heterogeneous Data**|Jun Liu et.al.|[2503.21213](http://arxiv.org/abs/2503.21213)|null|
|**2025-03-27**|**Multi-Objective Optimization for Privacy-Utility Balance in Differentially Private Federated Learning**|Kanishka Ranaweera et.al.|[2503.21159](http://arxiv.org/abs/2503.21159)|null|
|**2025-03-27**|**Federated Learning with Differential Privacy: An Utility-Enhanced Approach**|Kanishka Ranaweera et.al.|[2503.21154](http://arxiv.org/abs/2503.21154)|null|
|**2025-03-26**|**TS-Inverse: A Gradient Inversion Attack Tailored for Federated Time Series Forecasting Models**|Caspar Meijer et.al.|[2503.20952](http://arxiv.org/abs/2503.20952)|**[link](https://github.com/capsar/ts-inverse)**|
|**2025-03-26**|**Robust Federated Learning Against Poisoning Attacks: A GAN-Based Defense Framework**|Usama Zafar et.al.|[2503.20884](http://arxiv.org/abs/2503.20884)|**[link](https://github.com/SciML-FL/gan-filter)**|
|**2025-03-27**|**An Empirical Study of the Impact of Federated Learning on Machine Learning Model Accuracy**|Haotian Yang et.al.|[2503.20768](http://arxiv.org/abs/2503.20768)|null|
|**2025-03-26**|**Convergence Theory of Flexible ALADIN for Distributed Optimization**|Xu Du et.al.|[2503.20716](http://arxiv.org/abs/2503.20716)|null|
|**2025-03-26**|**ProFed: a Benchmark for Proximity-based non-IID Federated Learning**|Davide Domini et.al.|[2503.20618](http://arxiv.org/abs/2503.20618)|null|
|**2025-03-26**|**AIGC-assisted Federated Learning for Edge Intelligence: Architecture Design, Research Challenges and Future Directions**|Xianke Qiang et.al.|[2503.20166](http://arxiv.org/abs/2503.20166)|null|
|**2025-03-26**|**Unlocking the Value of Decentralized Data: A Federated Dual Learning Approach for Model Aggregation**|Junyi Zhu et.al.|[2503.20138](http://arxiv.org/abs/2503.20138)|null|
|**2025-03-25**|**From Interpretation to Correction: A Decentralized Optimization Framework for Exact Convergence in Federated Learning**|Bicheng Ying et.al.|[2503.20117](http://arxiv.org/abs/2503.20117)|null|
|**2025-03-25**|**Federated Learning: A new frontier in the exploration of multi-institutional medical imaging data**|Dominika Ciupek et.al.|[2503.20107](http://arxiv.org/abs/2503.20107)|null|
|**2025-03-25**|**RCC-PFL: Robust Client Clustering under Noisy Labels in Personalized Federated Learning**|Abdulmoneam Ali et.al.|[2503.19886](http://arxiv.org/abs/2503.19886)|null|
|**2025-03-25**|**AIGC-assisted Federated Learning for Vehicular Edge Intelligence: Vehicle Selection, Resource Allocation and Model Augmentation**|Xianke Qiang et.al.|[2503.19676](http://arxiv.org/abs/2503.19676)|null|
|**2025-03-25**|**FedMM-X: A Trustworthy and Interpretable Framework for Federated Multi-Modal Learning in Dynamic Environments**|Sree Bhargavi Balija et.al.|[2503.19564](http://arxiv.org/abs/2503.19564)|null|
|**2025-03-25**|**Noise Resilient Over-The-Air Federated Learning In Heterogeneous Wireless Networks**|Zubair Shaban et.al.|[2503.19549](http://arxiv.org/abs/2503.19549)|null|
|**2025-03-25**|**Social Network User Profiling for Anomaly Detection Based on Graph Neural Networks**|Yiwei Zhang et.al.|[2503.19380](http://arxiv.org/abs/2503.19380)|null|
|**2025-03-23**|**FedSKD: Aggregation-free Model-heterogeneous Federated Learning using Multi-dimensional Similarity Knowledge Distillation**|Ziqiao Weng et.al.|[2503.18981](http://arxiv.org/abs/2503.18981)|null|
|**2025-03-24**|**Streaming Federated Learning with Markovian Data**|Tan-Khiem Huynh et.al.|[2503.18807](http://arxiv.org/abs/2503.18807)|null|
|**2025-03-24**|**Distributionally Robust Federated Learning: An ADMM Algorithm**|Wen Bai et.al.|[2503.18436](http://arxiv.org/abs/2503.18436)|null|
|**2025-03-24**|**Byzantine-Resilient Over-the-Air Federated Learning under Zero-Trust Architecture**|Jiacheng Yao et.al.|[2503.18284](http://arxiv.org/abs/2503.18284)|null|
|**2025-03-23**|**Dynamic Allocation Hypernetwork with Adaptive Model Recalibration for FCL**|Xiaoming Qi et.al.|[2503.18064](http://arxiv.org/abs/2503.18064)|**[link](https://github.com/jinlab-imvr/feddah)**|
|**2025-03-22**|**Sense4FL: Vehicular Crowdsensing Enhanced Federated Learning for Autonomous Driving**|Yanan Ma et.al.|[2503.17697](http://arxiv.org/abs/2503.17697)|null|
|**2025-03-22**|**Quantized Analog Beamforming Enabled Multi-task Federated Learning Over-the-air**|Jiacheng Yao et.al.|[2503.17649](http://arxiv.org/abs/2503.17649)|null|
|**2025-03-21**|**LoGoFair: Post-Processing for Local and Global Fairness in Federated Learning**|Li Zhang et.al.|[2503.17231](http://arxiv.org/abs/2503.17231)|**[link](https://github.com/liizhang/LoGofair)**|
|**2025-03-21**|**A Thorough Assessment of the Non-IID Data Impact in Federated Learning**|Daniel M. Jimenez-Gutierrez et.al.|[2503.17070](http://arxiv.org/abs/2503.17070)|null|
|**2025-03-20**|**Fed-NDIF: A Noise-Embedded Federated Diffusion Model For Low-Count Whole-Body PET Denoising**|Yinchi Zhou et.al.|[2503.16635](http://arxiv.org/abs/2503.16635)|null|
|**2025-03-20**|**RESFL: An Uncertainty-Aware Framework for Responsible Federated Learning by Balancing Privacy, Fairness and Utility in Autonomous Vehicles**|Dawood Wasif et.al.|[2503.16251](http://arxiv.org/abs/2503.16251)|null|
|**2025-03-20**|**Empirical Analysis of Privacy-Fairness-Accuracy Trade-offs in Federated Learning: A Step Towards Responsible AI**|Dawood Wasif et.al.|[2503.16233](http://arxiv.org/abs/2503.16233)|null|
|**2025-03-20**|**Federated Quantum-Train Long Short-Term Memory for Gravitational Wave Signal**|Chen-Yu Liu et.al.|[2503.16049](http://arxiv.org/abs/2503.16049)|null|
|**2025-03-20**|**FedSAF: A Federated Learning Framework for Enhanced Gastric Cancer Detection and Privacy Preservation**|Yuxin Miao et.al.|[2503.15870](http://arxiv.org/abs/2503.15870)|null|
|**2025-03-20**|**FedAWA: Adaptive Optimization of Aggregation Weights in Federated Learning Using Client Vectors**|Changlong Shi et.al.|[2503.15842](http://arxiv.org/abs/2503.15842)|null|
|**2025-03-20**|**Energy-Efficient Federated Learning and Migration in Digital Twin Edge Networks**|Yuzhi Zhou et.al.|[2503.15822](http://arxiv.org/abs/2503.15822)|null|
|**2025-03-20**|**Communication Efficient Federated Learning with Linear Convergence on Heterogeneous Data**|Jie Liu et.al.|[2503.15804](http://arxiv.org/abs/2503.15804)|null|
|**2025-03-19**|**Reducing Communication Overhead in Federated Learning for Network Anomaly Detection with Adaptive Client Selection**|William Marfo et.al.|[2503.15448](http://arxiv.org/abs/2503.15448)|null|
|**2025-03-19**|**Federated Continual 3D Segmentation With Single-round Communication**|Can Peng et.al.|[2503.15414](http://arxiv.org/abs/2503.15414)|null|
|**2025-03-19**|**FedSCA: Federated Tuning with Similarity-guided Collaborative Aggregation for Heterogeneous Medical Image Segmentation**|Yumin Zhang et.al.|[2503.15390](http://arxiv.org/abs/2503.15390)|null|
|**2025-03-19**|**FedBEns: One-Shot Federated Learning based on Bayesian Ensemble**|Jacopo Talpini et.al.|[2503.15367](http://arxiv.org/abs/2503.15367)|null|
|**2025-03-19**|**Online federated learning framework for classification**|Wenxing Guo et.al.|[2503.15210](http://arxiv.org/abs/2503.15210)|null|
|**2025-03-19**|**Global Group Fairness in Federated Learning via Function Tracking**|Yves Rychener et.al.|[2503.15163](http://arxiv.org/abs/2503.15163)|null|
|**2025-03-19**|**UltraFlwr -- An Efficient Federated Medical and Surgical Object Detection Framework**|Yang Li et.al.|[2503.15161](http://arxiv.org/abs/2503.15161)|**[link](https://github.com/kcl-bmeis/ultraflwr)**|
|**2025-03-19**|**FedLWS: Federated Learning with Adaptive Layer-wise Weight Shrinking**|Changlong Shi et.al.|[2503.15111](http://arxiv.org/abs/2503.15111)|**[link](https://github.com/ChanglongShi/FedLWS)**|
|**2025-03-19**|**OFL: Opportunistic Federated Learning for Resource-Heterogeneous and Privacy-Aware Devices**|Yunlong Mao et.al.|[2503.15015](http://arxiv.org/abs/2503.15015)|null|
|**2025-03-19**|**pFedFair: Towards Optimal Group Fairness-Accuracy Trade-off in Heterogeneous Federated Learning**|Haoyu Lei et.al.|[2503.14925](http://arxiv.org/abs/2503.14925)|null|
|**2025-03-19**|**Technical Report: Aggregation on Learnable Manifolds for Asynchronous Federated Optimization**|Archie Licudi et.al.|[2503.14396](http://arxiv.org/abs/2503.14396)|null|
|**2025-03-18**|**Entente: Cross-silo Intrusion Detection on Network Log Graphs with Federated Learning**|Jiacen Xu et.al.|[2503.14284](http://arxiv.org/abs/2503.14284)|null|
|**2025-03-18**|**Trading-off Accuracy and Communication Cost in Federated Learning**|Mattia Jacopo Villani et.al.|[2503.14246](http://arxiv.org/abs/2503.14246)|null|
|**2025-03-18**|**Semantic Communication in Dynamic Channel Scenarios: Collaborative Optimization of Dual-Pipeline Joint Source-Channel Coding and Personalized Federated Learning**|Xingrun Yan et.al.|[2503.14084](http://arxiv.org/abs/2503.14084)|null|
|**2025-03-18**|**LLM-Empowered IoT for 6G Networks: Architecture, Challenges, and Solutions**|Xiaopei Chen et.al.|[2503.13819](http://arxiv.org/abs/2503.13819)|null|
|**2025-03-17**|**FedVSR: Towards Model-Agnostic Federated Learning in Video Super-Resolution**|Ali Mollaahmadi Dehaghi et.al.|[2503.13745](http://arxiv.org/abs/2503.13745)|**[link](https://github.com/alimd94/fedvsr)**|
|**2025-03-17**|**SDFLMQ: A Semi-Decentralized Federated Learning Framework over MQTT**|Amir Ali-Pour et.al.|[2503.13624](http://arxiv.org/abs/2503.13624)|null|
|**2025-03-17**|**Fed-Joint: Joint Modeling of Nonlinear Degradation Signals and Failure Events for Remaining Useful Life Prediction using Federated Learning**|Cheoljoon Jeong et.al.|[2503.13404](http://arxiv.org/abs/2503.13404)|null|
|**2025-03-17**|**Zero-Knowledge Proof-Based Consensus for Blockchain-Secured Federated Learning**|Tianxing Fu et.al.|[2503.13255](http://arxiv.org/abs/2503.13255)|null|
|**2025-03-17**|**Federated Mixture-of-Expert for Non-Overlapped Cross-Domain Sequential Recommendation**|Yu Liu et.al.|[2503.13254](http://arxiv.org/abs/2503.13254)|null|
|**2025-03-17**|**Mind the Gap: Confidence Discrepancy Can Guide Federated Semi-Supervised Learning Across Pseudo-Mismatch**|Yijie Liu et.al.|[2503.13227](http://arxiv.org/abs/2503.13227)|**[link](https://github.com/jay-codeman/sage)**|
|**2025-03-17**|**GC-Fed: Gradient Centralized Federated Learning with Partial Client Participation**|Jungwon Seo et.al.|[2503.13180](http://arxiv.org/abs/2503.13180)|**[link](https://github.com/thejungwon/gc-fed)**|
|**2025-03-17**|**PAUSE: Low-Latency and Privacy-Aware Active User Selection for Federated Learning**|Ori Peleg et.al.|[2503.13173](http://arxiv.org/abs/2503.13173)|**[link](https://github.com/oritalp/PAUSE)**|
|**2025-03-17**|**Federated Learning with Domain Shift Eraser**|Zheng Wang et.al.|[2503.13063](http://arxiv.org/abs/2503.13063)|null|
|**2025-03-17**|**FedSDP: Explainable Differential Privacy in Federated Learning via Shapley Values**|Yunbo Li et.al.|[2503.12958](http://arxiv.org/abs/2503.12958)|null|
|**2025-03-17**|**Federated Continual Instruction Tuning**|Haiyang Guo et.al.|[2503.12897](http://arxiv.org/abs/2503.12897)|null|
|**2025-03-18**|**A Linearized Alternating Direction Multiplier Method for Federated Matrix Completion Problems**|Patrick Hytla et.al.|[2503.12733](http://arxiv.org/abs/2503.12733)|null|
|**2025-03-13**|**Exploring the Vulnerabilities of Federated Learning: A Deep Dive into Gradient Inversion Attacks**|Pengxin Guo et.al.|[2503.11514](http://arxiv.org/abs/2503.11514)|**[link](https://github.com/1wrx1/GIA)**|
|**2025-03-14**|**Federated Koopman-Reservoir Learning for Large-Scale Multivariate Time-Series Anomaly Detection**|Long Tan Le et.al.|[2503.11255](http://arxiv.org/abs/2503.11255)|null|
|**2025-03-14**|**Enabling Weak Client Participation via On-device Knowledge Distillation in Heterogenous Federated Learning**|Jihyun Lim et.al.|[2503.11151](http://arxiv.org/abs/2503.11151)|null|
|**2025-03-14**|**Layer-wise Update Aggregation with Recycling for Communication-Efficient Federated Learning**|Jisoo Kim et.al.|[2503.11146](http://arxiv.org/abs/2503.11146)|null|
|**2025-03-14**|**FedOSAA: Improving Federated Learning with One-Step Anderson Acceleration**|Xue Feng et.al.|[2503.10961](http://arxiv.org/abs/2503.10961)|null|
|**2025-03-13**|**Byzantine-Resilient Federated Learning via Distributed Optimization**|Yufei Xia et.al.|[2503.10792](http://arxiv.org/abs/2503.10792)|null|
|**2025-03-13**|**FedPCA: Noise-Robust Fair Federated Learning via Performance-Capacity Analysis**|Nannan Wu et.al.|[2503.10567](http://arxiv.org/abs/2503.10567)|null|
|**2025-03-14**|**dFLMoE: Decentralized Federated Learning via Mixture of Experts for Medical Data Analysis**|Luyuan Xie et.al.|[2503.10412](http://arxiv.org/abs/2503.10412)|null|
|**2025-03-13**|**A Multi-Modal Federated Learning Framework for Remote Sensing Image Classification**|Barış Büyüktaş et.al.|[2503.10262](http://arxiv.org/abs/2503.10262)|null|
|**2025-03-13**|**Moss: Proxy Model-based Full-Weight Aggregation in Federated Learning with Heterogeneous Models**|Yifeng Cai et.al.|[2503.10218](http://arxiv.org/abs/2503.10218)|null|
|**2025-03-13**|**One-Shot Federated Unsupervised Domain Adaptation with Scaled Entropy Attention and Multi-Source Smoothed Pseudo Labeling**|Ali Abedi et.al.|[2503.10020](http://arxiv.org/abs/2503.10020)|null|
|**2025-03-13**|**PluralLLM: Pluralistic Alignment in LLMs via Federated Learning**|Mahmoud Srewa et.al.|[2503.09925](http://arxiv.org/abs/2503.09925)|null|
|**2025-03-12**|**A Comprehensive Review on Understanding the Decentralized and Collaborative Approach in Machine Learning**|Sarwar Saif et.al.|[2503.09833](http://arxiv.org/abs/2503.09833)|null|
|**2025-03-12**|**Fair Federated Medical Image Classification Against Quality Shift via Inter-Client Progressive State Matching**|Nannan Wu et.al.|[2503.09587](http://arxiv.org/abs/2503.09587)|**[link](https://github.com/wnn2000/ffl4mia)**|
|**2025-03-12**|**Mitigating Membership Inference Vulnerability in Personalized Federated Learning**|Kangsoo Jung et.al.|[2503.09414](http://arxiv.org/abs/2503.09414)|null|
|**2025-03-12**|**Robust Asymmetric Heterogeneous Federated Learning with Corrupted Clients**|Xiuwen Fang et.al.|[2503.09206](http://arxiv.org/abs/2503.09206)|**[link](https://github.com/fangxiuwen/rahfl)**|
|**2025-03-12**|**Differential Privacy Personalized Federated Learning Based on Dynamically Sparsified Client Updates**|Chuanyin Wang et.al.|[2503.09192](http://arxiv.org/abs/2503.09192)|null|
|**2025-03-12**|**Efficient UAV Swarm-Based Multi-Task Federated Learning with Dynamic Task Knowledge Sharing**|Yubo Yang et.al.|[2503.09144](http://arxiv.org/abs/2503.09144)|null|
|**2025-03-12**|**Drift-Aware Federated Learning: A Causal Perspective**|Yunjie Fang et.al.|[2503.09116](http://arxiv.org/abs/2503.09116)|null|
|**2025-03-12**|**Incentive Analysis for Agent Participation in Federated Learning**|Lihui Yi et.al.|[2503.09039](http://arxiv.org/abs/2503.09039)|null|
|**2025-03-12**|**Not All Edges are Equally Robust: Evaluating the Robustness of Ranking-Based Federated Learning**|Zirui Gong et.al.|[2503.08976](http://arxiv.org/abs/2503.08976)|null|
|**2025-03-11**|**Smoothing ADMM for Non-convex and Non-smooth Hierarchical Federated Learning**|Reza Mirzaeifard et.al.|[2503.08869](http://arxiv.org/abs/2503.08869)|null|
|**2025-03-11**|**Extra Clients at No Extra Cost: Overcome Data Heterogeneity in Federated Learning with Filter Decomposition**|Wei Chen et.al.|[2503.08652](http://arxiv.org/abs/2503.08652)|null|
|**2025-03-11**|**Regularized Federated Methods with Universal Guarantees for Simple Bilevel Optimization**|Mohammadjavad Ebrahimi et.al.|[2503.08634](http://arxiv.org/abs/2503.08634)|null|
|**2025-03-11**|**Prototype-based Heterogeneous Federated Learning for Blade Icing Detection in Wind Turbines with Class Imbalanced Data**|Lele Qi et.al.|[2503.08325](http://arxiv.org/abs/2503.08325)|null|
|**2025-03-11**|**Will LLMs Scaling Hit the Wall? Breaking Barriers via Distributed Resources on Massive Edge Devices**|Tao Shen et.al.|[2503.08223](http://arxiv.org/abs/2503.08223)|null|
|**2025-03-11**|**Scaling Probabilistic Circuits via Data Partitioning**|Jonas Seng et.al.|[2503.08141](http://arxiv.org/abs/2503.08141)|**[link](https://github.com/J0nasSeng/federated-spn)**|
|**2025-03-12**|**PRISM: Privacy-Preserving Improved Stochastic Masking for Federated Generative Models**|Kyeongkook Seo et.al.|[2503.08085](http://arxiv.org/abs/2503.08085)|**[link](https://github.com/tjrudrnr2/PRISM_ICLR25)**|
|**2025-03-11**|**Detecting Backdoor Attacks in Federated Learning via Direction Alignment Inspection**|Jiahao Xu et.al.|[2503.07978](http://arxiv.org/abs/2503.07978)|**[link](https://github.com/jiiahaoxu/alignins)**|
|**2025-03-10**|**Right Reward Right Time for Federated Learning**|Thanh Linh Nguyen et.al.|[2503.07869](http://arxiv.org/abs/2503.07869)|null|
|**2025-03-10**|**Sublinear Algorithms for Wasserstein and Total Variation Distances: Applications to Fairness and Privacy Auditing**|Debabrota Basu et.al.|[2503.07775](http://arxiv.org/abs/2503.07775)|null|
|**2025-03-10**|**Scaffold with Stochastic Gradients: New Analysis with Linear Speed-Up**|Paul Mangold et.al.|[2503.07594](http://arxiv.org/abs/2503.07594)|**[link](https://github.com/pmangold/scaffold-speed-up)**|
|**2025-03-10**|**Federated Learning in NTNs: Design, Architecture and Challenges**|Amin Farajzadeh et.al.|[2503.07272](http://arxiv.org/abs/2503.07272)|null|
|**2025-03-10**|**An Analytics-Driven Approach to Enhancing Supply Chain Visibility with Graph Neural Networks and Federated Learning**|Ge Zheng et.al.|[2503.07231](http://arxiv.org/abs/2503.07231)|null|
|**2025-03-10**|**FedRand: Enhancing Privacy in Federated Learning with Randomized LoRA Subparameter Updates**|Sangwoo Park et.al.|[2503.07216](http://arxiv.org/abs/2503.07216)|null|
|**2025-03-10**|**A Failure-Free and Efficient Discrete Laplace Distribution for Differential Privacy in MPC**|Ivan Tjuawinata et.al.|[2503.07048](http://arxiv.org/abs/2503.07048)|null|
|**2025-03-10**|**CAPT: Class-Aware Prompt Tuning for Federated Long-Tailed Learning with Vision-Language Model**|Shihao Hou et.al.|[2503.06993](http://arxiv.org/abs/2503.06993)|null|
|**2025-03-10**|**Capture Global Feature Statistics for One-Shot Federated Learning**|Zenghao Guan et.al.|[2503.06962](http://arxiv.org/abs/2503.06962)|**[link](https://github.com/yuqin-g/fedcgs)**|
|**2025-03-10**|**You Are Your Own Best Teacher: Achieving Centralized-level Performance in Federated Learning under Heterogeneous and Long-tailed Data**|Shanshan Yan et.al.|[2503.06916](http://arxiv.org/abs/2503.06916)|null|
|**2025-03-09**|**BTFL: A Bayesian-based Test-Time Generalization Method for Internal and External Data Distributions in Federated learning**|Yu Zhou et.al.|[2503.06633](http://arxiv.org/abs/2503.06633)|**[link](https://github.com/zhouyucs/btfl)**|
|**2025-03-09**|**BDPFL: Backdoor Defense for Personalized Federated Learning via Explainable Distillation**|Chengcheng Zhu et.al.|[2503.06554](http://arxiv.org/abs/2503.06554)|null|
|**2025-03-09**|**HFedCKD: Toward Robust Heterogeneous Federated Learning via Data-free Knowledge Distillation and Two-way Contrast**|Yiting Zheng et.al.|[2503.06511](http://arxiv.org/abs/2503.06511)|null|
|**2025-03-07**|**NoT: Federated Unlearning via Weight Negation**|Yasser H. Khalil et.al.|[2503.05657](http://arxiv.org/abs/2503.05657)|null|
|**2025-03-07**|**Practical Federated Learning without a Server**|Akash Dhasade et.al.|[2503.05509](http://arxiv.org/abs/2503.05509)|**[link](https://github.com/sacs-epfl/plexus)**|
|**2025-03-07**|**Personalized Federated Learning via Learning Dynamic Graphs**|Ziran Zhou et.al.|[2503.05474](http://arxiv.org/abs/2503.05474)|null|
|**2025-03-07**|**Uncertainty-Aware Explainable Federated Learning**|Yanci Zhang et.al.|[2503.05194](http://arxiv.org/abs/2503.05194)|null|
|**2025-03-07**|**FedMABench: Benchmarking Mobile Agents on Decentralized Heterogeneous User Data**|Wenhao Wang et.al.|[2503.05143](http://arxiv.org/abs/2503.05143)|**[link](https://github.com/wwh0411/fedmabench)**|
|**2025-03-06**|**Incentivizing Multi-Tenant Split Federated Learning for Foundation Models at the Network Edge**|Songyuan Li et.al.|[2503.04971](http://arxiv.org/abs/2503.04971)|null|
|**2025-03-07**|**Fundamental Limits of Hierarchical Secure Aggregation with Cyclic User Association**|Xiang Zhang et.al.|[2503.04564](http://arxiv.org/abs/2503.04564)|null|
|**2025-03-06**|**Federated Dynamic Modeling and Learning for Spatiotemporal Data Forecasting**|Thien Pham et.al.|[2503.04528](http://arxiv.org/abs/2503.04528)|null|
|**2025-03-06**|**Runtime Backdoor Detection for Federated Learning via Representational Dissimilarity Analysis**|Xiyue Zhang et.al.|[2503.04473](http://arxiv.org/abs/2503.04473)|null|
|**2025-03-06**|**Privacy Preserving and Robust Aggregation for Cross-Silo Federated Learning in Non-IID Settings**|Marco Arazzi et.al.|[2503.04451](http://arxiv.org/abs/2503.04451)|null|
|**2025-03-06**|**InFL-UX: A Toolkit for Web-Based Interactive Federated Learning**|Tim Maurer et.al.|[2503.04318](http://arxiv.org/abs/2503.04318)|**[link](https://github.com/tmaurer42/interactive-fl-poc)**|
|**2025-03-06**|**One-Shot Clustering for Federated Learning**|Maciej Krzysztof Zuziak et.al.|[2503.04231](http://arxiv.org/abs/2503.04231)|null|
|**2025-03-06**|**LiteChain: A Lightweight Blockchain for Verifiable and Scalable Federated Learning in Massive Edge Networks**|Handi Chen et.al.|[2503.04140](http://arxiv.org/abs/2503.04140)|null|
|**2025-03-06**|**FLAME: A Federated Learning Approach for Multi-Modal RF Fingerprinting**|Kiarash Kianfar et.al.|[2503.04136](http://arxiv.org/abs/2503.04136)|null|
|**2025-03-06**|**Generalization in Federated Learning: A Conditional Mutual Information Framework**|Ziqiao Wang et.al.|[2503.04091](http://arxiv.org/abs/2503.04091)|null|
|**2025-03-06**|**Brain Tumor Detection in MRI Based on Federated Learning with YOLOv11**|Sheikh Moonwara Anjum Monisha et.al.|[2503.04087](http://arxiv.org/abs/2503.04087)|null|
|**2025-03-05**|**Towards Trustworthy Federated Learning**|Alina Basharat et.al.|[2503.03684](http://arxiv.org/abs/2503.03684)|null|
|**2025-03-05**|**Federated Learning for Predicting Mild Cognitive Impairment to Dementia Conversion**|Gaurang Sharma et.al.|[2503.03489](http://arxiv.org/abs/2503.03489)|null|
|**2025-03-05**|**Privacy is All You Need: Revolutionizing Wearable Health Data with Advanced PETs**|Karthik Barma et.al.|[2503.03428](http://arxiv.org/abs/2503.03428)|null|
|**2025-03-05**|**Quantum-Inspired Privacy-Preserving Federated Learning Framework for Secure Dementia Classification**|Gazi Tanbhir et.al.|[2503.03267](http://arxiv.org/abs/2503.03267)|null|
|**2025-03-05**|**PriFFT: Privacy-preserving Federated Fine-tuning of Large Language Models via Function Secret Sharing**|Zhichao You et.al.|[2503.03146](http://arxiv.org/abs/2503.03146)|null|
|**2025-03-05**|**Knowledge Augmentation in Federation: Rethinking What Collaborative Learning Can Bring Back to Decentralized Data**|Wentai Wu et.al.|[2503.03140](http://arxiv.org/abs/2503.03140)|null|
|**2025-03-05**|**Convergence Analysis of Federated Learning Methods Using Backward Error Analysis**|Jinwoo Lim et.al.|[2503.03139](http://arxiv.org/abs/2503.03139)|null|
|**2025-03-05**|**WarmFed: Federated Learning with Warm-Start for Globalization and Personalization Via Personalized Diffusion Models**|Tao Feng et.al.|[2503.03110](http://arxiv.org/abs/2503.03110)|null|
|**2025-03-04**|**Federated Learning Meets Fluid Antenna: Towards Robust and Scalable Edge Intelligence**|Sangjun Park et.al.|[2503.03054](http://arxiv.org/abs/2503.03054)|null|
|**2025-03-04**|**Leveraging Randomness in Model and Data Partitioning for Privacy Amplification**|Andy Dong et.al.|[2503.03043](http://arxiv.org/abs/2503.03043)|null|
|**2025-03-04**|**Federated Learning for Privacy-Preserving Feedforward Control in Multi-Agent Systems**|Jakob Weber et.al.|[2503.02693](http://arxiv.org/abs/2503.02693)|**[link](https://github.com/j-cap/FL-based-neural-FF-control)**|
|**2025-03-04**|**Federated nnU-Net for Privacy-Preserving Medical Image Segmentation**|Grzegorz Skorupko et.al.|[2503.02549](http://arxiv.org/abs/2503.02549)|**[link](https://github.com/faildeny/fednnunet)**|
|**2025-03-04**|**AugFL: Augmenting Federated Learning with Pretrained Models**|Sheng Yue et.al.|[2503.02154](http://arxiv.org/abs/2503.02154)|**[link](https://github.com/zerui981105/augfl)**|
|**2025-03-03**|**A Lightweight and Secure Deep Learning Model for Privacy-Preserving Federated Learning in Intelligent Enterprises**|Reza Fotohi et.al.|[2503.02017](http://arxiv.org/abs/2503.02017)|**[link](https://github.com/rezafotohi/FedAnilPlus)**|
|**2025-03-03**|**GRAIN: Exact Graph Reconstruction from Gradients**|Maria Drencheva et.al.|[2503.01838](http://arxiv.org/abs/2503.01838)|null|
|**2025-03-03**|**FLAME: A Federated Learning Benchmark for Robotic Manipulation**|Santiago Bou Betran et.al.|[2503.01729](http://arxiv.org/abs/2503.01729)|null|
|**2025-03-03**|**Heterogeneity Matters even More in Distributed Learning: Study from Generalization Perspective**|Masoud Kavian et.al.|[2503.01598](http://arxiv.org/abs/2503.01598)|null|
|**2025-03-03**|**MoCFL: Mobile Cluster Federated Learning Framework for Highly Dynamic Network**|Kai Fang et.al.|[2503.01557](http://arxiv.org/abs/2503.01557)|null|
|**2025-03-03**|**MAB-Based Channel Scheduling for Asynchronous Federated Learning in Non-Stationary Environments**|Zhiyin Li et.al.|[2503.01324](http://arxiv.org/abs/2503.01324)|null|
|**2025-03-02**|**Patient-Level Anatomy Meets Scanning-Level Physics: Personalized Federated Low-Dose CT Denoising Empowered by Large Language Model**|Ziyuan Yang et.al.|[2503.00908](http://arxiv.org/abs/2503.00908)|null|
|**2025-02-28**|**QFAL: Quantum Federated Adversarial Learning**|Walid El Maouaki et.al.|[2502.21171](http://arxiv.org/abs/2502.21171)|null|
|**2025-02-28**|**FedDyMem: Efficient Federated Learning with Dynamic Memory and Memory-Reduce for Unsupervised Image Anomaly Detection**|Silin Chen et.al.|[2502.21012](http://arxiv.org/abs/2502.21012)|null|
|**2025-02-28**|**Managing Federated Learning on Decentralized Infrastructures as a Reputation-based Collaborative Workflow**|Yuandou Wang et.al.|[2502.20882](http://arxiv.org/abs/2502.20882)|null|
|**2025-02-28**|**Unlearning through Knowledge Overwriting: Reversible Federated Unlearning via Selective Sparse Adapter**|Zhengyi Zhong et.al.|[2502.20709](http://arxiv.org/abs/2502.20709)|null|
|**2025-02-28**|**FedConv: A Learning-on-Model Paradigm for Heterogeneous Federated Clients**|Leming Shen et.al.|[2502.20639](http://arxiv.org/abs/2502.20639)|**[link](https://github.com/lemingshen/FedConv)**|
|**2025-02-27**|**DPZV: Resource Efficient ZO Optimization For Differentially Private VFL**|Jianing Zhang et.al.|[2502.20565](http://arxiv.org/abs/2502.20565)|null|
|**2025-02-27**|**GreenDFL: a Framework for Assessing the Sustainability of Decentralized Federated Learning Systems**|Chao Feng et.al.|[2502.20242](http://arxiv.org/abs/2502.20242)|null|
|**2025-02-27**|**Can Textual Gradient Work in Federated Learning?**|Minghui Chen et.al.|[2502.19980](http://arxiv.org/abs/2502.19980)|**[link](https://github.com/ubc-tea/FedTextGrad)**|
|**2025-02-27**|**Revisit the Stability of Vanilla Federated Learning Under Diverse Conditions**|Youngjoon Lee et.al.|[2502.19849](http://arxiv.org/abs/2502.19849)|null|
|**2025-02-27**|**Probabilistic Federated Prompt-Tuning with Non-IID and Imbalanced Data**|Pei-Yau Weng et.al.|[2502.19752](http://arxiv.org/abs/2502.19752)|null|
|**2025-02-26**|**FedCDC: A Collaborative Framework for Data Consumers in Federated Learning Market**|Zhuan Shi et.al.|[2502.19109](http://arxiv.org/abs/2502.19109)|null|
|**2025-02-26**|**Robust Over-the-Air Computation with Type-Based Multiple Access**|Marc Martinez-Gost et.al.|[2502.19014](http://arxiv.org/abs/2502.19014)|null|
|**2025-02-26**|**CLLoRA: An Approach to Measure the Effects of the Context Length for LLM Fine-Tuning**|Ping Zhang et.al.|[2502.18910](http://arxiv.org/abs/2502.18910)|null|
|**2025-02-25**|**Differentially Private Federated Learning With Time-Adaptive Privacy Spending**|Shahrzad Kiani et.al.|[2502.18706](http://arxiv.org/abs/2502.18706)|null|
|**2025-02-25**|**H-FLTN: A Privacy-Preserving Hierarchical Framework for Electric Vehicle Spatio-Temporal Charge Prediction**|Robert Marlin et.al.|[2502.18697](http://arxiv.org/abs/2502.18697)|null|
|**2025-02-25**|**Personalized Federated Learning for Egocentric Video Gaze Estimation with Comprehensive Parameter Frezzing**|Yuhu Feng et.al.|[2502.18123](http://arxiv.org/abs/2502.18123)|null|
|**2025-02-25**|**The Built-In Robustness of Decentralized Federated Averaging to Bad Data**|Samuele Sabella et.al.|[2502.18097](http://arxiv.org/abs/2502.18097)|null|
|**2025-02-25**|**Design and implementation of a distributed security threat detection system integrating federated learning and multimodal LLM**|Yuqing Wang et.al.|[2502.17763](http://arxiv.org/abs/2502.17763)|null|
|**2025-02-25**|**FinP: Fairness-in-Privacy in Federated Learning by Addressing Disparities in Privacy Risk**|Tianyu Zhao et.al.|[2502.17748](http://arxiv.org/abs/2502.17748)|null|
|**2025-02-24**|**Robust Federated Learning with Global Sensitivity Estimation for Financial Risk Management**|Lei Zhao et.al.|[2502.17694](http://arxiv.org/abs/2502.17694)|null|
|**2025-02-24**|**FedSV: Byzantine-Robust Federated Learning via Shapley Value**|Khaoula Otmani et.al.|[2502.17526](http://arxiv.org/abs/2502.17526)|null|
|**2025-02-24**|**Robust Federated Learning in Unreliable Wireless Networks: A Client Selection Approach**|Yanmeng Wang et.al.|[2502.17260](http://arxiv.org/abs/2502.17260)|null|
|**2025-02-24**|**Electrical Load Forecasting over Multihop Smart Metering Networks with Federated Learning**|Ratun Rahman et.al.|[2502.17226](http://arxiv.org/abs/2502.17226)|null|
|**2025-02-24**|**Forgetting Any Data at Any Time: A Theoretically Certified Unlearning Framework for Vertical Federated Learning**|Linian Wang et.al.|[2502.17081](http://arxiv.org/abs/2502.17081)|**[link](https://github.com/wangln19/vertical-federated-unlearning)**|
|**2025-02-24**|**FedBM: Stealing Knowledge from Pre-trained Language Models for Heterogeneous Federated Learning**|Meilu Zhu et.al.|[2502.16832](http://arxiv.org/abs/2502.16832)|**[link](https://github.com/cuhk-aim-group/fedbm)**|
|**2025-02-24**|**VGFL-SA: Vertical Graph Federated Learning Structure Attack Based on Contrastive Learning**|Yang Chen et.al.|[2502.16793](http://arxiv.org/abs/2502.16793)|null|
|**2025-02-23**|**FedDA-TSformer: Federated Domain Adaptation with Vision TimeSformer for Left Ventricle Segmentation on Gated Myocardial Perfusion SPECT Image**|Yehong Huang et.al.|[2502.16709](http://arxiv.org/abs/2502.16709)|null|
|**2025-02-23**|**Toward Responsible Federated Large Language Models: Leveraging a Safety Filter and Constitutional AI**|Eunchung Noh et.al.|[2502.16691](http://arxiv.org/abs/2502.16691)|null|
|**2025-02-23**|**Multi-Target Federated Backdoor Attack Based on Feature Aggregation**|Lingguag Hao et.al.|[2502.16545](http://arxiv.org/abs/2502.16545)|null|
|**2025-02-23**|**TrustChain: A Blockchain Framework for Auditing and Verifying Aggregators in Decentralized Federated Learning**|Ehsan Hallaji et.al.|[2502.16406](http://arxiv.org/abs/2502.16406)|null|
|**2025-02-23**|**FedNIA: Noise-Induced Activation Analysis for Mitigating Data Poisoning in FL**|Ehsan Hallaji et.al.|[2502.16396](http://arxiv.org/abs/2502.16396)|null|
|**2025-02-20**|**Distributed U-net model and Image Segmentation for Lung Cancer Detection**|Tianzuo Hu et.al.|[2502.14928](http://arxiv.org/abs/2502.14928)|null|
|**2025-02-21**|**Vision Foundation Models in Medical Image Analysis: Advances and Challenges**|Pengchen Liang et.al.|[2502.14584](http://arxiv.org/abs/2502.14584)|null|
|**2025-02-20**|**FUIA: Model Inversion Attack against Federated Unlearning**|Lei Zhou et.al.|[2502.14558](http://arxiv.org/abs/2502.14558)|null|
|**2025-02-20**|**PQBFL: A Post-Quantum Blockchain-based Protocol for Federated Learning**|Hadi GHaravi et.al.|[2502.14464](http://arxiv.org/abs/2502.14464)|null|
|**2025-02-20**|**VFL-RPS: Relevant Participant Selection in Vertical Federated Learning**|Afsana Khan et.al.|[2502.14375](http://arxiv.org/abs/2502.14375)|null|
|**2025-02-20**|**A Note on Efficient Privacy-Preserving Similarity Search for Encrypted Vectors**|Dongfang Zhao et.al.|[2502.14291](http://arxiv.org/abs/2502.14291)|null|
|**2025-02-20**|**Accurate Forgetting for Heterogeneous Federated Continual Learning**|Abudukelimu Wuerkaixi et.al.|[2502.14205](http://arxiv.org/abs/2502.14205)|**[link](https://github.com/zaocan666/af-fcl)**|
|**2025-02-20**|**Federated Fine-Tuning of Large Language Models: Kahneman-Tversky vs. Direct Preference Optimization**|Fernando Spadea et.al.|[2502.14187](http://arxiv.org/abs/2502.14187)|null|
|**2025-02-20**|**Blockchain-based Framework for Scalable and Incentivized Federated Learning**|Bijun Wu et.al.|[2502.14170](http://arxiv.org/abs/2502.14170)|null|
|**2025-02-19**|**Homophily Heterogeneity Matters in Graph Federated Learning: A Spectrum Sharing and Complementing Perspective**|Wentao Yu et.al.|[2502.13732](http://arxiv.org/abs/2502.13732)|null|
|**2025-02-19**|**Smoothed Normalization for Efficient Distributed Private Optimization**|Egor Shulgin et.al.|[2502.13482](http://arxiv.org/abs/2502.13482)|null|
|**2025-02-18**|**FedHC: A Hierarchical Clustered Federated Learning Framework for Satellite Networks**|Zhuocheng Liu et.al.|[2502.12783](http://arxiv.org/abs/2502.12783)|null|
|**2025-02-18**|**Federated Variational Inference for Bayesian Mixture Models**|Jackie Rao et.al.|[2502.12684](http://arxiv.org/abs/2502.12684)|null|
|**2025-02-14**|**ClusMFL: A Cluster-Enhanced Framework for Modality-Incomplete Multimodal Federated Learning in Brain Imaging Analysis**|Xinpeng Wang et.al.|[2502.12180](http://arxiv.org/abs/2502.12180)|null|
|**2025-02-14**|**Ten Challenging Problems in Federated Foundation Models**|Tao Fan et.al.|[2502.12176](http://arxiv.org/abs/2502.12176)|null|
|**2025-02-17**|**FedEAT: A Robustness Optimization Framework for Federated LLMs**|Yahao Pang et.al.|[2502.11863](http://arxiv.org/abs/2502.11863)|null|
|**2025-02-17**|**Double Momentum and Error Feedback for Clipping with Fast Rates and Differential Privacy**|Rustem Islamov et.al.|[2502.11682](http://arxiv.org/abs/2502.11682)|null|
|**2025-02-14**|**Federated Learning-Driven Cybersecurity Framework for IoT Networks with Privacy-Preserving and Real-Time Threat Detection Capabilities**|Milad Rahmati et.al.|[2502.10599](http://arxiv.org/abs/2502.10599)|null|
|**2025-02-14**|**Efficient Zero-Order Federated Finetuning of Language Models for Resource-Constrained Devices**|Mohamed Aboelenien Ahmed et.al.|[2502.10239](http://arxiv.org/abs/2502.10239)|null|
|**2025-02-14**|**RoadFed: A Multimodal Federated Learning System for Improving Road Safety**|Yachao Yuan et.al.|[2502.09978](http://arxiv.org/abs/2502.09978)|null|
|**2025-02-13**|**Fine-Tuning Foundation Models with Federated Learning for Privacy Preserving Medical Time Series Forecasting**|Mahad Ali et.al.|[2502.09744](http://arxiv.org/abs/2502.09744)|null|
|**2025-02-13**|**Towards Seamless Hierarchical Federated Learning under Intermittent Client Participation: A Stagewise Decision-Making Methodology**|Minghong Wu et.al.|[2502.09303](http://arxiv.org/abs/2502.09303)|null|
|**2025-02-13**|**Use of Air Quality Sensor Network Data for Real-time Pollution-Aware POI Suggestion**|Giuseppe Fasano et.al.|[2502.09155](http://arxiv.org/abs/2502.09155)|**[link](https://github.com/airtownapp/airtown-application)**|
|**2025-02-13**|**Vertical Federated Continual Learning via Evolving Prototype Knowledge**|Shuo Wang et.al.|[2502.09152](http://arxiv.org/abs/2502.09152)|null|
|**2025-02-13**|**One-shot Federated Learning Methods: A Practical Guide**|Xiang Liu et.al.|[2502.09104](http://arxiv.org/abs/2502.09104)|null|
|**2025-02-13**|**RLSA-PFL: Robust Lightweight Secure Aggregation with Model Inconsistency Detection in Privacy-Preserving Federated Learning**|Nazatul H. Sultan et.al.|[2502.08989](http://arxiv.org/abs/2502.08989)|null|
|**2025-02-12**|**PLayer-FL: A Principled Approach to Personalized Layer-wise Cross-Silo Federated Learning**|Ahmed Elhussein et.al.|[2502.08829](http://arxiv.org/abs/2502.08829)|**[link](https://github.com/gaiters-aerials/player_fl)**|
|**2025-02-12**|**FBFL: A Field-Based Coordination Approach for Data Heterogeneity in Federated Learning**|Davide Domini et.al.|[2502.08577](http://arxiv.org/abs/2502.08577)|**[link](https://github.com/davidedomini/experiments-2025-lmcs-field-based-fl)**|
|**2025-02-12**|**Representation Learning to Advance Multi-institutional Studies with Electronic Health Record Data**|Doudou Zhou et.al.|[2502.08547](http://arxiv.org/abs/2502.08547)|null|
|**2025-02-12**|**FedMHO: Heterogeneous One-Shot Federated Learning Towards Resource-Constrained Edge Devices**|Dezhong Yao et.al.|[2502.08518](http://arxiv.org/abs/2502.08518)|**[link](https://github.com/YXShi2000/FedMHO)**|
|**2025-02-12**|**One-Shot Federated Learning with Classifier-Free Diffusion Models**|Obaidullah Zaland et.al.|[2502.08488](http://arxiv.org/abs/2502.08488)|null|
|**2025-02-12**|**Optimizing Asynchronous Federated Learning: A Delicate Trade-Off Between Model-Parameter Staleness and Update Frequency**|Abdelkrim Alahyane et.al.|[2502.08206](http://arxiv.org/abs/2502.08206)|null|
|**2025-02-12**|**Vertical Federated Learning in Practice: The Good, the Bad, and the Ugly**|Zhaomin Wu et.al.|[2502.08160](http://arxiv.org/abs/2502.08160)|null|
|**2025-02-12**|**Local Differential Privacy is Not Enough: A Sample Reconstruction Attack against Federated Learning with Local Differential Privacy**|Zhichao You et.al.|[2502.08151](http://arxiv.org/abs/2502.08151)|null|
|**2025-02-12**|**SLVR: Securely Leveraging Client Validation for Robust Federated Learning**|Jihye Choi et.al.|[2502.08055](http://arxiv.org/abs/2502.08055)|null|
|**2025-02-11**|**Initialization Matters: Unraveling the Impact of Pre-Training on Federated Learning**|Divyansh Jhunjhunwala et.al.|[2502.08024](http://arxiv.org/abs/2502.08024)|null|
|**2025-02-11**|**An Interactive Framework for Implementing Privacy-Preserving Federated Learning: Experiments on Large Language Models**|Kasra Ahmadi et.al.|[2502.08008](http://arxiv.org/abs/2502.08008)|**[link](https://github.com/KasraAhmadi/FL-Privacy-LLM)**|
|**2025-02-11**|**PFedDST: Personalized Federated Learning with Decentralized Selection Training**|Mengchen Fan et.al.|[2502.07750](http://arxiv.org/abs/2502.07750)|null|
|**2025-02-11**|**FedAPA: Server-side Gradient-Based Adaptive Personalized Aggregation for Federated Learning on Heterogeneous Data**|Yuxia Sun et.al.|[2502.07456](http://arxiv.org/abs/2502.07456)|null|
|**2025-02-10**|**Federated Continual Learning: Concepts, Challenges, and Solutions**|Parisa Hamedi et.al.|[2502.07059](http://arxiv.org/abs/2502.07059)|null|
|**2025-02-10**|**Federated Sinkhorn**|Jeremy Kulcsar et.al.|[2502.07021](http://arxiv.org/abs/2502.07021)|null|
|**2025-02-10**|**DROP: Poison Dilution via Knowledge Distillation for Federated Learning**|Georgios Syros et.al.|[2502.07011](http://arxiv.org/abs/2502.07011)|**[link](https://github.com/gsiros/drop)**|
|**2025-02-10**|**Krum Federated Chain (KFC): Using blockchain to defend against adversarial attacks in Federated Learning**|Mario García-Márquez et.al.|[2502.06917](http://arxiv.org/abs/2502.06917)|**[link](https://github.com/ari-dasci/S-kfc)**|
|**2025-02-10**|**Analytic Personalized Federated Meta-Learning**|Shunxian Gu et.al.|[2502.06915](http://arxiv.org/abs/2502.06915)|null|
|**2025-02-10**|**A Fair Federated Learning Framework for Collaborative Network Traffic Prediction and Resource Allocation**|Saroj Kumar Panda et.al.|[2502.06743](http://arxiv.org/abs/2502.06743)|null|
|**2025-02-10**|**Many-Task Federated Fine-Tuning via Unified Task Vectors**|Vasileios Tsouvalas et.al.|[2502.06376](http://arxiv.org/abs/2502.06376)|null|
|**2025-02-10**|**Fine-tuning Multimodal Transformers on Edge: A Parallel Split Learning Approach**|Timo Fudala et.al.|[2502.06355](http://arxiv.org/abs/2502.06355)|null|
|**2025-02-10**|**Delay Optimization of a Federated Learning-based UAV-aided IoT network**|Hossein Mohammadi Firouzjaei et.al.|[2502.06284](http://arxiv.org/abs/2502.06284)|null|
|**2025-02-10**|**Fine-Tuning Federated Learning-Based Intrusion Detection Systems for Transportation IoT**|Robert Akinie et.al.|[2502.06099](http://arxiv.org/abs/2502.06099)|null|
|**2025-02-08**|**Federated Learning with Reservoir State Analysis for Time Series Anomaly Detection**|Keigo Nogami et.al.|[2502.05679](http://arxiv.org/abs/2502.05679)|**[link](https://github.com/Key5n/IncFed-MDRS)**|
|**2025-02-08**|**Dual Defense: Enhancing Privacy and Mitigating Poisoning Attacks in Federated Learning**|Runhua Xu et.al.|[2502.05547](http://arxiv.org/abs/2502.05547)|**[link](https://github.com/irxyzzz/DualDefense)**|
|**2025-02-08**|**Coalition Formation for Heterogeneous Federated Learning Enabled Channel Estimation in RIS-assisted Cell-free MIMO**|Nan Qi et.al.|[2502.05538](http://arxiv.org/abs/2502.05538)|null|
|**2025-02-07**|**Using Federated Machine Learning in Predictive Maintenance of Jet Engines**|Asaph Matheus Barbosa et.al.|[2502.05321](http://arxiv.org/abs/2502.05321)|null|
|**2025-02-07**|**Principles and Components of Federated Learning Architectures**|Sarwar Saif et.al.|[2502.05273](http://arxiv.org/abs/2502.05273)|null|
|**2025-02-07**|**Mitigating Unintended Memorization with LoRA in Federated Learning for LLMs**|Thierry Bossy et.al.|[2502.05087](http://arxiv.org/abs/2502.05087)|**[link](https://github.com/tuneinsight/federated-llms)**|
|**2025-02-07**|**Federated Learning for Anomaly Detection in Energy Consumption Data: Assessing the Vulnerability to Adversarial Attacks**|Yohannis Kifle Telila et.al.|[2502.05041](http://arxiv.org/abs/2502.05041)|null|
|**2025-02-07**|**Exploit Gradient Skewness to Circumvent Byzantine Defenses for Federated Learning**|Yuchen Liu et.al.|[2502.04890](http://arxiv.org/abs/2502.04890)|null|
|**2025-02-07**|**DMPA: Model Poisoning Attacks on Decentralized Federated Learning for Model Differences**|Chao Feng et.al.|[2502.04771](http://arxiv.org/abs/2502.04771)|null|
|**2025-02-07**|**Graph Federated Learning Based Proactive Content Caching in Edge Computing**|Rui Wang et.al.|[2502.04760](http://arxiv.org/abs/2502.04760)|null|
|**2025-02-07**|**LATTEO: A Framework to Support Learning Asynchronously Tempered with Trusted Execution and Obfuscation**|Abhinav Kumar et.al.|[2502.04601](http://arxiv.org/abs/2502.04601)|null|
|**2025-02-06**|**Private Federated Learning In Real World Application -- A Case Study**|An Ji et.al.|[2502.04565](http://arxiv.org/abs/2502.04565)|null|
|**2025-02-06**|**Generative Autoregressive Transformers for Model-Agnostic Federated MRI Reconstruction**|Valiyeh A. Nezhad et.al.|[2502.04521](http://arxiv.org/abs/2502.04521)|null|
|**2025-02-06**|**FedOptimus: Optimizing Vertical Federated Learning for Scalability and Efficiency**|Nikita Shrivastava et.al.|[2502.04243](http://arxiv.org/abs/2502.04243)|null|
|**2025-02-06**|**The Gradient Puppeteer: Adversarial Domination in Gradient Leakage Attacks through Model Poisoning**|Kunlan Xiang et.al.|[2502.04106](http://arxiv.org/abs/2502.04106)|null|
|**2025-02-06**|**Comparing privacy notions for protection against reconstruction attacks in machine learning**|Sayan Biswas et.al.|[2502.04045](http://arxiv.org/abs/2502.04045)|null|
|**2025-02-06**|**Non-convex composite federated learning with heterogeneous data**|Jiaojiao Zhang et.al.|[2502.03958](http://arxiv.org/abs/2502.03958)|null|
|**2025-02-06**|**Privacy Risks in Health Big Data: A Systematic Literature Review**|Zhang Si Yuan et.al.|[2502.03811](http://arxiv.org/abs/2502.03811)|null|
|**2025-02-06**|**SoK: Benchmarking Poisoning Attacks and Defenses in Federated Learning**|Heyi Zhang et.al.|[2502.03801](http://arxiv.org/abs/2502.03801)|**[link](https://github.com/vio1etus/flpoison)**|
|**2025-02-05**|**Interaction-Aware Gaussian Weighting for Clustered Federated Learning**|Alessandro Licciardi et.al.|[2502.03340](http://arxiv.org/abs/2502.03340)|null|
|**2025-02-05**|**The Other Side of the Coin: Unveiling the Downsides of Model Aggregation in Federated Learning from a Layer-peeled Perspective**|Guogang Zhu et.al.|[2502.03231](http://arxiv.org/abs/2502.03231)|null|
|**2025-02-05**|**Multi-objective methods in Federated Learning: A survey and taxonomy**|Maria Hartmann et.al.|[2502.03108](http://arxiv.org/abs/2502.03108)|null|
|**2025-02-05**|**E-3SFC: Communication-Efficient Federated Learning with Double-way Features Synthesizing**|Yuhao Zhou et.al.|[2502.03092](http://arxiv.org/abs/2502.03092)|**[link](https://github.com/Soptq/e-3sfc)**|
|**2025-02-05**|**Differentially-Private Multi-Tier Federated Learning: A Formal Analysis and Evaluation**|Evan Chen et.al.|[2502.02877](http://arxiv.org/abs/2502.02877)|null|
|**2025-02-05**|**Vertical Federated Learning for Failure-Cause Identification in Disaggregated Microwave Networks**|Fatih Temiz et.al.|[2502.02874](http://arxiv.org/abs/2502.02874)|null|
|**2025-02-04**|**Federated Low-Rank Tensor Estimation for Multimodal Image Reconstruction**|Anh Van Nguyen et.al.|[2502.02761](http://arxiv.org/abs/2502.02761)|null|
|**2025-02-04**|**Parameter Tracking in Federated Learning with Adaptive Optimization**|Evan Chen. Jianing Zhang et.al.|[2502.02727](http://arxiv.org/abs/2502.02727)|null|
|**2025-02-04**|**SMTFL: Secure Model Training to Untrusted Participants in Federated Learning**|Zhihui Zhao et.al.|[2502.02038](http://arxiv.org/abs/2502.02038)|null|
|**2025-02-04**|**Improving Wireless Federated Learning via Joint Downlink-Uplink Beamforming over Analog Transmission**|Chong Zhang et.al.|[2502.02034](http://arxiv.org/abs/2502.02034)|null|
|**2025-02-03**|**A Privacy-Preserving Domain Adversarial Federated learning for multi-site brain functional connectivity analysis**|Yipu Zhang et.al.|[2502.01885](http://arxiv.org/abs/2502.01885)|null|
|**2025-02-03**|**Beyond the Crawl: Unmasking Browser Fingerprinting in Real User Interactions**|Meenatchi Sundaram Muthu Selva Annamalai et.al.|[2502.01608](http://arxiv.org/abs/2502.01608)|**[link](https://github.com/spalabucr/beyond-the-crawl)**|
|**2025-02-03**|**Federated Detection of Open Charge Point Protocol 1.6 Cyberattacks**|Christos Dalamagkas et.al.|[2502.01569](http://arxiv.org/abs/2502.01569)|null|
|**2025-02-03**|**FedGES: A Federated Learning Approach for BN Structure Learning**|Pablo Torrijos et.al.|[2502.01538](http://arxiv.org/abs/2502.01538)|null|
|**2025-02-03**|**Federated Learning with Discriminative Naive Bayes Classifier**|Pablo Torrijos et.al.|[2502.01532](http://arxiv.org/abs/2502.01532)|null|
|**2025-02-03**|**Metric Privacy in Federated Learning for Medical Imaging: Improving Convergence and Preventing Client Inference Attacks**|Judith Sáinz-Pardo Díaz et.al.|[2502.01352](http://arxiv.org/abs/2502.01352)|null|
|**2025-02-03**|**A Framework for Double-Blind Federated Adaptation of Foundation Models**|Nurbek Tastan et.al.|[2502.01289](http://arxiv.org/abs/2502.01289)|null|
|**2025-02-03**|**Tackling Feature and Sample Heterogeneity in Decentralized Multi-Task Learning: A Sheaf-Theoretic Approach**|Chaouki Ben Issaid et.al.|[2502.01145](http://arxiv.org/abs/2502.01145)|null|
|**2025-01-31**|**S-VOTE: Similarity-based Voting for Client Selection in Decentralized Federated Learning**|Pedro Miguel Sánchez Sánchez et.al.|[2501.19279](http://arxiv.org/abs/2501.19279)|null|
|**2025-01-31**|**FedRTS: Federated Robust Pruning via Combinatorial Thompson Sampling**|Hong Huang et.al.|[2501.19122](http://arxiv.org/abs/2501.19122)|null|
|**2025-01-31**|**FL-APU: A Software Architecture to Ease Practical Implementation of Cross-Silo Federated Learning**|F. Stricker et.al.|[2501.19091](http://arxiv.org/abs/2501.19091)|null|
|**2025-01-31**|**Continuous-Time Analysis of Federated Averaging**|Tom Overman et.al.|[2501.18870](http://arxiv.org/abs/2501.18870)|null|
|**2025-01-30**|**Targeted Data Fusion for Causal Survival Analysis Under Distribution Shift**|Yi Liu et.al.|[2501.18798](http://arxiv.org/abs/2501.18798)|null|
|**2025-01-30**|**SAFL: Structure-Aware Personalized Federated Learning via Client-Specific Clustering and SCSI-Guided Model Pruning**|Nan Li et.al.|[2501.18659](http://arxiv.org/abs/2501.18659)|null|
|**2025-01-30**|**Exploring Potential Prompt Injection Attacks in Federated Military LLMs and Their Mitigation**|Youngjoon Lee et.al.|[2501.18416](http://arxiv.org/abs/2501.18416)|null|
|**2025-01-30**|**Update Estimation and Scheduling for Over-the-Air Federated Learning with Energy Harvesting Devices**|Furkan Bagci et.al.|[2501.18298](http://arxiv.org/abs/2501.18298)|null|
|**2025-01-30**|**Advancing Personalized Federated Learning: Integrative Approaches with AI for Enhanced Privacy and Customization**|Kevin Cooper et.al.|[2501.18174](http://arxiv.org/abs/2501.18174)|null|
|**2025-01-29**|**Power-Efficient Over-the-Air Aggregation with Receive Beamforming for Federated Learning**|Faeze Moradi Kalarde et.al.|[2501.18058](http://arxiv.org/abs/2501.18058)|null|
|**2025-01-29**|**Federated Learning With Individualized Privacy Through Client Sampling**|Lucas Lange et.al.|[2501.17634](http://arxiv.org/abs/2501.17634)|**[link](https://github.com/luckyos-code/flidp)**|
|**2025-01-29**|**A Survey on Cluster-based Federated Learning**|Omar El-Rifai et.al.|[2501.17512](http://arxiv.org/abs/2501.17512)|null|
|**2025-01-29**|**Poisoning Attacks and Defenses to Federated Unlearning**|Wenbin Wang et.al.|[2501.17396](http://arxiv.org/abs/2501.17396)|null|
|**2025-01-29**|**Byzantine-Robust Federated Learning over Ring-All-Reduce Distributed Computing**|Minghong Fang et.al.|[2501.17392](http://arxiv.org/abs/2501.17392)|null|
|**2025-01-29**|**Do We Really Need to Design New Byzantine-robust Aggregation Rules?**|Minghong Fang et.al.|[2501.17381](http://arxiv.org/abs/2501.17381)|null|
|**2025-01-28**|**Connecting Federated ADMM to Bayes**|Siddharth Swaroop et.al.|[2501.17325](http://arxiv.org/abs/2501.17325)|null|
|**2025-01-28**|**FedEFM: Federated Endovascular Foundation Model with Unseen Data**|Tuong Do et.al.|[2501.16992](http://arxiv.org/abs/2501.16992)|null|
|**2025-01-28**|**Heterogeneity-aware Personalized Federated Learning via Adaptive Dual-Agent Reinforcement Learning**|Xi Chen et.al.|[2501.16966](http://arxiv.org/abs/2501.16966)|null|
|**2025-01-28**|**Federated Learning Strategies for Coordinated Beamforming in Multicell ISAC**|Lai Jiang et.al.|[2501.16951](http://arxiv.org/abs/2501.16951)|null|
|**2025-01-28**|**Meta-Federated Learning: A Novel Approach for Real-Time Traffic Flow Management**|Bob Johnson et.al.|[2501.16758](http://arxiv.org/abs/2501.16758)|null|
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
|**2024-12-20**|**fluke: Federated Learning Utility frameworK for Experimentation and research**|Mirko Polato et.al.|[2412.15728](http://arxiv.org/abs/2412.15728)|**[link](https://github.com/makgyver/fluke)**|
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
|**2024-12-18**|**On the Robustness of Distributed Machine Learning against Transfer Attacks**|Sébastien Andreina et.al.|[2412.14080](http://arxiv.org/abs/2412.14080)|**[link](https://github.com/RUB-InfSec/distributed_learning_robustness)**|
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
|**2024-12-10**|**Optimizing Personalized Federated Learning through Adaptive Layer-Wise Learning**|Weihang Chen et.al.|[2412.07062](http://arxiv.org/abs/2412.07062)|**[link](https://github.com/lancasterJie/FLAYER)**|
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
|**2024-11-26**|**Distributed Sign Momentum with Local Steps for Training Transformers**|Shuhua Yu et.al.|[2411.17866](http://arxiv.org/abs/2411.17866)|**[link](https://github.com/shuhuayu/dist-sign-momentum)**|
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
|**2024-11-20**|**On-device Content-based Recommendation with Single-shot Embedding Pruning: A Cooperative Game Perspective**|Hung Vinh Tran et.al.|[2411.13052](http://arxiv.org/abs/2411.13052)|**[link](https://github.com/chenxing1999/shaver)**|
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
|**2024-11-15**|**FedAli: Personalized Federated Learning with Aligned Prototypes through Optimal Transport**|Sannara Ek et.al.|[2411.10595](http://arxiv.org/abs/2411.10595)|**[link](https://github.com/getalp/FedAli)**|
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

<p align=right>(<a href=#updated-on-20250404>back to top</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[contributors-url]: https://github.com/Vincentqyw/cv-arxiv-daily/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[forks-url]: https://github.com/Vincentqyw/cv-arxiv-daily/network/members
[stars-shield]: https://img.shields.io/github/stars/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[stars-url]: https://github.com/Vincentqyw/cv-arxiv-daily/stargazers
[issues-shield]: https://img.shields.io/github/issues/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[issues-url]: https://github.com/Vincentqyw/cv-arxiv-daily/issues

