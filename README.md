[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## Updated on 2024.10.25
> Usage instructions: [here](./docs/README.md#usage)

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href=#agent>agent</a></li>
    <li><a href=#llm>llm</a></li>
    <li><a href=#wireless-network>Wireless Network</a></li>
    <li><a href=#wireless-communications>Wireless Communications</a></li>
    <li><a href=#wireless-intelligence>Wireless Intelligence</a></li>
    <li><a href=#communication-intelligence>Communication Intelligence</a></li>
    <li><a href=#rag>RAG</a></li>
    <li><a href=#text2sql>text2sql</a></li>
    <li><a href=#aiops>AIOps</a></li>
    <li><a href=#ppc>PPC</a></li>
    <li><a href=#moe>moe</a></li>
    <li><a href=#ssms>SSMs</a></li>
  </ol>
</details>

## agent

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-24**|**An LLM Agent for Automatic Geospatial Data Analysis**|Yuxing Chen et.al.|[2410.18792](http://arxiv.org/abs/2410.18792)|null|大型语言模型（LLM）被用于数据科学代码生成任务，但在处理复杂顺序任务时经常遇到逻辑错误。将它们应用于地理空间数据处理尤其具有挑战性，因为难以整合复杂的数据结构和空间约束、有效利用多样化的函数调用，以及倾向于虚构较少使用的地理空间库。为了解决这些问题，我们引入了GeoAgent，这是一个新的交互式框架，旨在帮助LLM更有效地处理地理空间数据处理。GeoAgent首次将代码解释器、静态分析和检索增强生成（RAG）技术集成到蒙特卡洛树搜索（MCTS）算法中，为地理空间数据处理提供了一种新方法。此外，我们贡献了一个专门为评估基于LLM的方法在地理空间任务中的表现而设计的新基准。该基准利用了多种Python库，并包括单轮和多轮任务，如数据获取、数据分析和可视化。通过在各种地理空间上下文中提供全面的评估，该基准为开发基于LLM的方法在地理空间数据分析任务中设定了新的标准。我们的研究结果表明，仅依靠LLM的知识不足以准确完成地理空间任务编程，这需要连贯的多步骤过程和多次函数调用。与基线LLM相比，所提出的GeoAgent表现出色，在函数调用和任务完成方面取得了显著改进。此外，这些结果为未来基于LLM代理在自动地理空间数据分析任务编程的发展提供了宝贵见解。|
|**2024-10-24**|**PRACT: Optimizing Principled Reasoning and Acting of LLM Agent**|Zhiwei Liu et.al.|[2410.18528](http://arxiv.org/abs/2410.18528)|null|我们提出了一个名为原则性推理与行动（PRAct）的新框架，这是一种从轨迹数据中学习和执行动作原则的方法。我们的方法核心是利用来自反思与优化引擎的文本梯度来推导这些动作原则。为了使动作原则适应特定任务需求，我们提出了一种新的优化框架——反思原则优化（RPO）。在执行后，RPO使用一个反思器来批评当前的动作原则，并使用一个优化器相应地更新这些原则。我们在两种场景下开发了RPO框架：Reward-RPO，它使用环境奖励进行反思；Self-RPO，它在没有外部奖励的情况下进行自我反思。此外，还引入了两种RPO方法，RPO-Traj 和 RPO-Batch，以适应不同的设置。四个环境中的实验结果表明，利用RPO框架的PRAct代理能够有效地学习并应用动作原则以提高性能。|
|**2024-10-23**|**GraphTeam: Facilitating Large Language Model-based Graph Analysis via Multi-Agent Collaboration**|Xin Li et.al.|[2410.18032](http://arxiv.org/abs/2410.18032)|**[link](https://github.com/bupt-gamma/graphteam)**|**图在现实世界场景中被广泛用于建模关系数据，例如社交网络和城市计算。现有的基于大语言模型（LLM）的图分析方法要么将图神经网络（GNN）集成到特定的机器学习任务中，限制了其可迁移性；要么仅依赖于LLM的内部推理能力，导致性能不佳。为了解决这些局限性，我们利用了最近在基于LLM的代理上的进展，这些代理已经展示了利用外部知识或工具解决问题的能力。通过模拟人类解决问题的策略，如类比和协作，我们提出了一种基于LLM的多代理系统GraphTeam，用于图分析。GraphTeam由来自三个模块的五个基于LLM的代理组成，具有不同专长的代理可以相互协作以解决复杂问题。具体来说，(1) 输入-输出规范化模块：问题代理从原始问题中提取并精炼四个关键参数，促进对问题的理解，答案代理则整理结果以满足输出要求；(2) 外部知识检索模块：我们首先构建了一个包含相关文档和经验信息的知识库，然后搜索代理为每个问题检索最相关的条目。(3) 问题解决模块：根据从搜索代理获取的信息，编码代理通过编程使用已建立的算法生成解决方案；如果编码代理无法工作，则推理代理将直接计算结果而无需编程。在六个图分析基准上的广泛实验表明，GraphTeam在准确性方面平均比最佳基线提高了25.85%。代码和数据可在https://github.com/BUPT-GAMMA/GraphTeam获得。**|
|**2024-10-23**|**MiniFed : Integrating LLM-based Agentic-Workflow for Simulating FOMC Meeting**|Sungil Seok et.al.|[2410.18012](http://arxiv.org/abs/2410.18012)|null|在美国，联邦基金利率对国内外金融市场都起着重要作用。然而，研究主要集中在联邦基金利率调整的影响上，而非决策过程本身。最近在大型语言模型（LLM）方面的进展提供了一种可能的方法来重构负责设定联邦基金利率的联邦公开市场委员会（FOMC）会议。在本文中，我们提出了一个五阶段的FOMC会议模拟框架MiniFed，该框架使用LLM代理来模拟现实世界中的FOMC会议成员，并优化FOMC结构。这一框架有效地重振了FOMC会议流程，并促进了联邦基金利率的预测。实验结果表明，我们提出的MiniFed框架不仅在联邦基金利率预测方面达到了高精度，而且其行为与现实中对应人物的行为一致。鉴于很少有研究关注于利用LLM代理来模拟大规模现实世界的会议，我们的工作可以为未来的发展提供一个基准。|
|**2024-10-22**|**SELA: Tree-Search Enhanced LLM Agents for Automated Machine Learning**|Yizhou Chi et.al.|[2410.17238](http://arxiv.org/abs/2410.17238)|**[link](https://github.com/geekan/metagpt)**|**自动化机器学习（AutoML）方法包括优化固定模型选择和集成管道的传统方法，以及能够自主构建管道的新型基于大语言模型（LLM）的框架。尽管基于LLM的代理在自动化机器学习任务方面显示出潜力，但它们往往生成低多样性和次优代码，即使经过多次迭代也是如此。为克服这些限制，我们引入了树搜索增强的LLM代理（SELA），这是一种创新的基于代理的系统，它利用蒙特卡洛树搜索（MCTS）来优化AutoML过程。通过将管道配置表示为树，我们的框架使代理能够智能地进行实验，并迭代地改进其策略，从而更有效地探索机器学习解决方案空间。这种方法允许SELA根据实验反馈发现最优路径，提高解决方案的整体质量。通过对20个机器学习数据集的广泛评估，我们将传统和基于代理的AutoML方法进行了比较，结果表明SELA在所有数据集中对每个基线的胜率达到了65%到80%。这些结果突显了基于代理策略在AutoML中的巨大潜力，为解决复杂的机器学习挑战提供了新的视角。**|
|**2024-10-22**|**EnvBridge: Bridging Diverse Environments with Cross-Environment Knowledge Transfer for Embodied AI**|Tomoyuki Kagaya et.al.|[2410.16919](http://arxiv.org/abs/2410.16919)|null|近年来，大型语言模型（LLM）展现出了高推理能力，引起了人们对其在各种决策过程中的应用的关注。其中，LLM 作为代理在机器人操作中的应用尤其具有前景。最近的研究表明，LLM 可以生成文本计划或控制代码来操控机器人，提供了极大的灵活性和交互能力。然而，这些方法在不同环境下的灵活性和适用性方面仍面临挑战，限制了它们的自主适应能力。当前的方法通常分为两类：一类依赖于特定环境的策略训练，这限制了其可迁移性；另一类基于固定提示生成代码动作，在面对新环境时性能会下降。这些局限性显著制约了代理在机器人操作任务中的泛化能力。为了解决这些问题，我们提出了一种名为 EnvBridge 的新方法。该方法涉及从源环境到目标环境的成功机器人控制代码的保留和转移。EnvBridge 通过利用多个环境的洞察力，提高了代理在不同设置下的适应性和性能。值得注意的是，我们的方法缓解了环境约束，为机器人操作任务提供了一个更灵活、更具泛化性的解决方案。我们使用机器人操作基准 RLBench、MetaWorld 和 CALVIN 验证了方法的有效性。实验结果表明，LLM 代理可以成功利用多样化的知识来源解决复杂任务。因此，我们的方法显著增强了机器人操作代理在多样化环境中的规划适应性和鲁棒性。|
|**2024-10-22**|**CoPS: Empowering LLM Agents with Provable Cross-Task Experience Sharing**|Chen Yang et.al.|[2410.16670](http://arxiv.org/abs/2410.16670)|**[link](https://github.com/uclaml/cops)**|**在代理系统中，大型语言模型（LLMs）显著推进了序列推理的发展，但现有方法仍存在局限性。基于反思的推理仅依赖于预训练模型中的知识，在新场景下的表现受限；而基于经验辅助的推理通常依赖外部经验，并且缺乏选择代表性经验的明确原则。为解决这些局限性，我们提出了CoPS（跨任务经验共享），这是一种通用算法，通过跨任务的经验共享和选择来增强序列推理能力。具体而言，CoPS利用代理在先前任务上的经验，通过一种可证明的悲观策略选择分布匹配的经验，以最大化效用并最小化由于分布偏移带来的风险。在Alfworld、Webshop和HotPotQA等基准测试上的广泛实验结果表明，CoPS始终优于最先进基线，并具有适合资源受限场景的卓越样本效率。理论上，我们展示了该算法的性能既取决于预训练LLM的质量，也取决于代理的任务依赖试验分布与LLM生成的分布之间的匹配程度。我们的工作弥合了现有序列推理范式之间的差距，验证了利用跨任务经验的有效性，为提高代理在多样化任务中的泛化能力和适应性提供了启示。我们的代码可在https://github.com/uclaml/COPS获取。**|
|**2024-10-22**|**Adsorb-Agent: Autonomous Identification of Stable Adsorption Configurations via Large Language Model Agent**|Janghoon Ock et.al.|[2410.16658](http://arxiv.org/abs/2410.16658)|null|吸附能是催化中的一个关键反应性描述符，能够有效地筛选潜在的催化剂。然而，确定吸附能需要比较多种吸附物-催化剂构型的能量，由于可能的构型数量庞大，这在计算上是非常耗费资源的。当前的算法通常通过枚举吸附位点和构型来进行，而没有充分利用理论见解来指导初始设置。在这项工作中，我们介绍了Adsorb-Agent，这是一种大型语言模型（LLM）代理，旨在以最少的人工干预高效地推导出特定系统的稳定吸附构型。Adsorb-Agent利用内置的知识和涌现的推理能力，显著减少了所需的初始构型数量，同时提高了预测最低吸附能的准确性。我们使用两个示例系统NNH-CuPd3 (111) 和 NNH-Mo3Pd (111) 对氮还原反应（NRR）进行了性能展示，NRR是一种可持续的哈伯-博施过程替代方案。Adsorb-Agent 通过识别更少的初始设置下的低能量构型，优于传统的“启发式”和“随机”算法，降低了计算成本并提高了准确性。这突显了其加速催化剂发现的潜力。|
|**2024-10-23**|**IBGP: Imperfect Byzantine Generals Problem for Zero-Shot Robustness in Communicative Multi-Agent Systems**|Yihuan Mao et.al.|[2410.16237](http://arxiv.org/abs/2410.16237)|null|随着大型语言模型（LLM）代理越来越多地融入我们的基础设施，它们的稳健协调和消息同步变得至关重要。拜占庭将军问题（BGP）是构建在敌对攻击下具有弹性的多代理系统（MAS）的关键模型。它描述了系统中存在身份不明的恶意代理的情况——在我们的背景下，这种情况可能是由于LLM代理的幻觉或外部攻击造成的。在BGP中，整个系统的目的是就采取的行动达成一致。传统的BGP要求所有代理之间达成全局共识；然而，在实际场景中，全局共识并不总是必要的，甚至可能是低效的。因此，迫切需要探索一个与MAS中观察到的局部协调模式相一致的改进版BGP。在我们的研究中，我们把这个改进版本称为不完美BGP（IBGP），旨在解决这一差异。为了解决这个问题，我们提出了一种框架，该框架利用共识协议在一般的MAS设置中提供可证明的针对通信攻击的弹性以及对变化环境的适应性，这已经通过实证结果得到验证。此外，我们还展示了一个传感器网络环境中的案例研究，以说明我们协议的实际应用。|
|**2024-10-21**|**NetSafe: Exploring the Topological Safety of Multi-agent Networks**|Miao Yu et.al.|[2410.15686](http://arxiv.org/abs/2410.15686)|null|大型语言模型（LLM）为多智能体网络中的节点赋予了智能，在学术界和工业界的应用日益广泛。然而，如何防止这些网络生成恶意信息的问题仍未得到探索，而以往针对单一LLM安全性的研究难以直接应用到此问题上。在本文中，我们从拓扑角度聚焦于多智能体网络的安全性，探讨哪些拓扑属性有助于构建更安全的网络。为此，我们提出了一种通用框架NetSafe以及一种迭代RelCom交互机制，以统一现有的多样化基于LLM的智能体框架，为广义上的拓扑安全性研究奠定基础。我们识别出当多智能体网络受到涉及错误信息、偏见和有害信息攻击时出现的一些关键现象，将其称为“智能体幻觉”和“聚合安全性”。此外，我们发现高度互联的网络更容易受到对抗性攻击的影响，在星形图拓扑结构中任务性能下降了29.7%。我们的静态度量指标比传统的图论度量指标更接近现实世界中的动态评估结果，表明与攻击者平均距离更大的网络表现出更高的安全性。总之，本工作引入了一个关于基于LLM的多智能体网络安全性的新拓扑视角，并揭示了一些未被报道的现象，为未来研究探索此类网络的安全性开辟了道路。|
|**2024-10-20**|**Who is Undercover? Guiding LLMs to Explore Multi-Perspective Team Tactic in the Game**|Ruiqi Dong et.al.|[2410.15311](http://arxiv.org/abs/2410.15311)|null|
|**2024-10-20**|**When Machine Unlearning Meets Retrieval-Augmented Generation (RAG): Keep Secret or Forget Knowledge?**|Shang Wang et.al.|[2410.15267](http://arxiv.org/abs/2410.15267)|null|
|**2024-10-19**|**SPA-Bench: A Comprehensive Benchmark for SmartPhone Agent Evaluation**|Jingxuan Chen et.al.|[2410.15164](http://arxiv.org/abs/2410.15164)|null|
|**2024-10-22**|**Imprompter: Tricking LLM Agents into Improper Tool Use**|Xiaohan Fu et.al.|[2410.14923](http://arxiv.org/abs/2410.14923)|**[link](https://github.com/Reapor-Yurnero/imprompter)**|
|**2024-10-18**|**When LLMs Go Online: The Emerging Threat of Web-Enabled LLMs**|Hanna Kim et.al.|[2410.14569](http://arxiv.org/abs/2410.14569)|null|
|**2024-10-18**|**Do LLMs "know" internally when they follow instructions?**|Juyeon Heo et.al.|[2410.14516](http://arxiv.org/abs/2410.14516)|null|
|**2024-10-18**|**CoMAL: Collaborative Multi-Agent Large Language Models for Mixed-Autonomy Traffic**|Huaiyuan Yao et.al.|[2410.14368](http://arxiv.org/abs/2410.14368)|**[link](https://github.com/hyan-yao/comal)**|
|**2024-10-22**|**Good Parenting is all you need -- Multi-agentic LLM Hallucination Mitigation**|Ted Kwartler et.al.|[2410.14262](http://arxiv.org/abs/2410.14262)|null|
|**2024-10-18**|**Agents4PLC: Automating Closed-loop PLC Code Generation and Verification in Industrial Control Systems using LLM-based Agents**|Zihan Liu et.al.|[2410.14209](http://arxiv.org/abs/2410.14209)|null|
|**2024-10-18**|**Rationale Behind Essay Scores: Enhancing S-LLM's Multi-Trait Essay Scoring with Rationale Generated by LLMs**|SeongYeub Chu et.al.|[2410.14202](http://arxiv.org/abs/2410.14202)|null|
|**2024-10-18**|**SRAP-Agent: Simulating and Optimizing Scarce Resource Allocation Policy with LLM-based Agent**|Jiarui Ji et.al.|[2410.14152](http://arxiv.org/abs/2410.14152)|null|
|**2024-10-17**|**From Barriers to Tactics: A Behavioral Science-Informed Agentic Workflow for Personalized Nutrition Coaching**|Eric Yang et.al.|[2410.14041](http://arxiv.org/abs/2410.14041)|null|
|**2024-10-17**|**AgentOccam: A Simple Yet Strong Baseline for LLM-Based Web Agents**|Ke Yang et.al.|[2410.13825](http://arxiv.org/abs/2410.13825)|null|
|**2024-10-17**|**Rapid and Automated Alloy Design with Graph Neural Network-Powered LLM-Driven Multi-Agent Systems**|Alireza Ghafarollahi et.al.|[2410.13768](http://arxiv.org/abs/2410.13768)|null|
|**2024-10-17**|**MeNTi: Bridging Medical Calculator and LLM Agent with Nested Tool Calling**|Yakun Zhu et.al.|[2410.13610](http://arxiv.org/abs/2410.13610)|null|
|**2024-10-17**|**Chain of Ideas: Revolutionizing Research in Novel Idea Development with LLM Agents**|Long Li et.al.|[2410.13185](http://arxiv.org/abs/2410.13185)|**[link](https://github.com/damo-nlp-sg/coi-agent)**|
|**2024-10-16**|**Robust RL with LLM-Driven Data Synthesis and Policy Adaptation for Autonomous Driving**|Sihao Wu et.al.|[2410.12568](http://arxiv.org/abs/2410.12568)|null|
|**2024-10-16**|**SAC-GLAM: Improving Online RL for LLM agents with Soft Actor-Critic and Hindsight Relabeling**|Loris Gaven et.al.|[2410.12481](http://arxiv.org/abs/2410.12481)|null|
|**2024-10-16**|**Proactive Agent: Shifting LLM Agents from Reactive Responses to Active Assistance**|Yaxi Lu et.al.|[2410.12361](http://arxiv.org/abs/2410.12361)|null|
|**2024-10-16**|**Enhancing LLM Agents for Code Generation with Possibility and Pass-rate Prioritized Experience Replay**|Yuyang Chen et.al.|[2410.12236](http://arxiv.org/abs/2410.12236)|null|
|**2024-10-15**|**Empowering Users in Digital Privacy Management through Interactive LLM-Based Agents**|Bolun Sun et.al.|[2410.11906](http://arxiv.org/abs/2410.11906)|null|
|**2024-10-15**|**HR-Agent: A Task-Oriented Dialogue (TOD) LLM Agent Tailored for HR Applications**|Weijie Xu et.al.|[2410.11239](http://arxiv.org/abs/2410.11239)|null|
|**2024-10-14**|**Denial-of-Service Poisoning Attacks against Large Language Models**|Kuofeng Gao et.al.|[2410.10760](http://arxiv.org/abs/2410.10760)|**[link](https://github.com/sail-sg/p-dos)**|
|**2024-10-14**|**FairMindSim: Alignment of Behavior, Emotion, and Belief in Humans and LLM Agents Amid Ethical Dilemmas**|Yu Lei et.al.|[2410.10398](http://arxiv.org/abs/2410.10398)|null|
|**2024-10-14**|**Beyond-RAG: Question Identification and Answer Generation in Real-Time Conversations**|Garima Agrawal et.al.|[2410.10136](http://arxiv.org/abs/2410.10136)|null|
|**2024-10-13**|**Adaptive Reasoning and Acting in Medical Language Agents**|Abhishek Dutta et.al.|[2410.10020](http://arxiv.org/abs/2410.10020)|null|
|**2024-10-13**|**Dynamic and Textual Graph Generation Via Large-Scale LLM-based Agent Simulation**|Jiarui Ji et.al.|[2410.09824](http://arxiv.org/abs/2410.09824)|null|
|**2024-10-13**|**Agentic Information Retrieval**|Weinan Zhang et.al.|[2410.09713](http://arxiv.org/abs/2410.09713)|null|
|**2024-10-12**|**LLM-SmartAudit: Advanced Smart Contract Vulnerability Detection**|Zhiyuan Wei et.al.|[2410.09381](http://arxiv.org/abs/2410.09381)|**[link](https://github.com/LLMAudit/LLMSmartAuditTool)**|
|**2024-10-11**|**PEAR: A Robust and Flexible Automation Framework for Ptychography Enabled by Multiple Large Language Model Agents**|Xiangyu Yin et.al.|[2410.09034](http://arxiv.org/abs/2410.09034)|null|
|**2024-10-14**|**AgentHarm: A Benchmark for Measuring Harmfulness of LLM Agents**|Maksym Andriushchenko et.al.|[2410.09024](http://arxiv.org/abs/2410.09024)|null|
|**2024-10-11**|**The Dynamics of Social Conventions in LLM populations: Spontaneous Emergence, Collective Biases and Tipping Points**|Ariel Flint Ashery et.al.|[2410.08948](http://arxiv.org/abs/2410.08948)|null|
|**2024-10-10**|**Benchmarking Agentic Workflow Generation**|Shuofei Qiao et.al.|[2410.07869](http://arxiv.org/abs/2410.07869)|**[link](https://github.com/zjunlp/worfbench)**|
|**2024-10-10**|**AgentBank: Towards Generalized LLM Agents via Fine-Tuning on 50000+ Interaction Trajectories**|Yifan Song et.al.|[2410.07706](http://arxiv.org/abs/2410.07706)|null|
|**2024-10-11**|**WALL-E: World Alignment by Rule Learning Improves World Model-based LLM Agents**|Siyu Zhou et.al.|[2410.07484](http://arxiv.org/abs/2410.07484)|**[link](https://github.com/elated-sawyer/WALL-E)**|
|**2024-10-09**|**I Want to Break Free! Anti-Social Behavior and Persuasion Ability of LLMs in Multi-Agent Settings with Social Hierarchy**|Gian Maria Campedelli et.al.|[2410.07109](http://arxiv.org/abs/2410.07109)|**[link](https://github.com/mobs-fbk/llm_interaction_simulator)**|
|**2024-10-09**|**Reproducing and Extending Experiments in Behavioral Strategy with Large Language Models**|Daniel Albert et.al.|[2410.06932](http://arxiv.org/abs/2410.06932)|null|
|**2024-10-08**|**AgentSquare: Automatic LLM Agent Search in Modular Design Space**|Yu Shang et.al.|[2410.06153](http://arxiv.org/abs/2410.06153)|**[link](https://github.com/tsinghua-fib-lab/agentsquare)**|
|**2024-10-08**|**Conversate: Supporting Reflective Learning in Interview Practice Through Interactive Simulation and Dialogic Feedback**|Taufiq Daryanto et.al.|[2410.05570](http://arxiv.org/abs/2410.05570)|null|
|**2024-10-07**|**Better than Your Teacher: LLM Agents that learn from Privileged AI Feedback**|Sanjiban Choudhury et.al.|[2410.05434](http://arxiv.org/abs/2410.05434)|null|
|**2024-10-07**|**GLEE: A Unified Framework and Benchmark for Language-based Economic Environments**|Eilam Shapira et.al.|[2410.05254](http://arxiv.org/abs/2410.05254)|**[link](https://github.com/eilamshapira/GLEE)**|
|**2024-10-09**|**GenSim: A General Social Simulation Platform with Large Language Model based Agents**|Jiakai Tang et.al.|[2410.04360](http://arxiv.org/abs/2410.04360)|**[link](https://github.com/TangJiakai/GenSim)**|
|**2024-10-04**|**Permissive Information-Flow Analysis for Large Language Models**|Shoaib Ahmed Siddiqui et.al.|[2410.03055](http://arxiv.org/abs/2410.03055)|null|
|**2024-10-03**|**AutoML-Agent: A Multi-Agent LLM Framework for Full-Pipeline AutoML**|Patara Trirat et.al.|[2410.02958](http://arxiv.org/abs/2410.02958)|null|
|**2024-10-03**|**Grounding Large Language Models In Embodied Environment With Imperfect World Models**|Haolan Liu et.al.|[2410.02742](http://arxiv.org/abs/2410.02742)|null|
|**2024-10-03**|**Agent Security Bench (ASB): Formalizing and Benchmarking Attacks and Defenses in LLM-based Agents**|Hanrong Zhang et.al.|[2410.02644](http://arxiv.org/abs/2410.02644)|**[link](https://github.com/agiresearch/asb)**|
|**2024-10-03**|**ColaCare: Enhancing Electronic Health Record Modeling through Large Language Model-Driven Multi-Agent Collaboration**|Zixiang Wang et.al.|[2410.02551](http://arxiv.org/abs/2410.02551)|null|
|**2024-10-03**|**ELLMA-T: an Embodied LLM-agent for Supporting English Language Learning in Social VR**|Mengxu Pan et.al.|[2410.02406](http://arxiv.org/abs/2410.02406)|null|
|**2024-10-03**|**A LLM-Powered Automatic Grading Framework with Human-Level Guidelines Optimization**|Yucheng Chu et.al.|[2410.02165](http://arxiv.org/abs/2410.02165)|null|
|**2024-10-02**|**Zodiac: A Cardiologist-Level LLM Framework for Multi-Agent Diagnostics**|Yuan Zhou et.al.|[2410.02026](http://arxiv.org/abs/2410.02026)|null|
|**2024-10-02**|**Moral Alignment for LLM Agents**|Elizaveta Tennant et.al.|[2410.01639](http://arxiv.org/abs/2410.01639)|null|
|**2024-10-03**|**RGD: Multi-LLM Based Agent Debugger via Refinement and Generation Guidance**|Haolin Jin et.al.|[2410.01242](http://arxiv.org/abs/2410.01242)|null|
|**2024-10-01**|**Dynamic Planning for LLM-based Graphical User Interface Automation**|Shaoqing Zhang et.al.|[2410.00467](http://arxiv.org/abs/2410.00467)|**[link](https://github.com/sqzhang-lazy/d-pot)**|
|**2024-09-30**|**MemSim: A Bayesian Simulator for Evaluating Memory of LLM-based Personal Assistants**|Zeyu Zhang et.al.|[2409.20163](http://arxiv.org/abs/2409.20163)|**[link](https://github.com/nuster1128/memsim)**|
|**2024-10-01**|**TRANSAGENT: An LLM-Based Multi-Agent System for Code Translation**|Zhiqiang Yuan et.al.|[2409.19894](http://arxiv.org/abs/2409.19894)|null|
|**2024-09-26**|**From News to Forecast: Integrating Event Analysis in LLM-Based Time Series Forecasting with Reflection**|Xinlei Wang et.al.|[2409.17515](http://arxiv.org/abs/2409.17515)|**[link](https://github.com/ameliawong1996/From_News_to_Forecast)**|
|**2024-09-25**|**AAPM: Large Language Model Agent-based Asset Pricing Models**|Junyan Cheng et.al.|[2409.17266](http://arxiv.org/abs/2409.17266)|**[link](https://github.com/chengjunyan1/aapm)**|
|**2024-09-25**|**Turn Every Application into an Agent: Towards Efficient Human-Agent-Computer Interaction with API-First LLM-Based Agents**|Junting Lu et.al.|[2409.17140](http://arxiv.org/abs/2409.17140)|null|
|**2024-09-24**|**MultiTalk: Introspective and Extrospective Dialogue for Human-Environment-LLM Alignment**|Venkata Naren Devarakonda et.al.|[2409.16455](http://arxiv.org/abs/2409.16455)|null|
|**2024-09-23**|**Safe Guard: an LLM-agent for Real-time Voice-based Hate Speech Detection in Social Virtual Reality**|Yiwen Xu et.al.|[2409.15623](http://arxiv.org/abs/2409.15623)|null|
|**2024-09-25**|**Towards a Realistic Long-Term Benchmark for Open-Web Research Agents**|Peter Mühlbacher et.al.|[2409.14913](http://arxiv.org/abs/2409.14913)|null|
|**2024-09-23**|**Interpreting Multi-band Galaxy Observations with Large Language Model-Based Agents**|Zechang Sun et.al.|[2409.14807](http://arxiv.org/abs/2409.14807)|null|
|**2024-09-22**|**Enhancing LLM-based Autonomous Driving Agents to Mitigate Perception Attacks**|Ruoyu Song et.al.|[2409.14488](http://arxiv.org/abs/2409.14488)|null|
|**2024-09-20**|**Enhancing Fault Localization Through Ordered Code Analysis with LLM Agents and Self-Reflection**|Md Nakhla Rafi et.al.|[2409.13642](http://arxiv.org/abs/2409.13642)|null|
|**2024-09-23**|**AQA: Adaptive Question Answering in a Society of LLMs via Contextual Multi-Armed Bandit**|Mohanna Hoveyda et.al.|[2409.13447](http://arxiv.org/abs/2409.13447)|null|
|**2024-09-17**|**LLM-Agent-UMF: LLM-based Agent Unified Modeling Framework for Seamless Integration of Multi Active/Passive Core-Agents**|Amine B. Hassouna et.al.|[2409.11393](http://arxiv.org/abs/2409.11393)|null|
|**2024-09-17**|**Hackphyr: A Local Fine-Tuned LLM Agent for Network Security Environments**|Maria Rigaki et.al.|[2409.11276](http://arxiv.org/abs/2409.11276)|null|
|**2024-09-14**|**On the limits of agency in agent-based models**|Ayush Chopra et.al.|[2409.10568](http://arxiv.org/abs/2409.10568)|**[link](https://github.com/agenttorch/agenttorch)**|
|**2024-09-19**|**Instigating Cooperation among LLM Agents Using Adaptive Information Modulation**|Qiliang Chen et.al.|[2409.10372](http://arxiv.org/abs/2409.10372)|null|
|**2024-09-17**|**Large Language Model Based Generative Error Correction: A Challenge and Baselines for Speech Recognition, Speaker Tagging, and Emotion Recognition**|Chao-Han Huck Yang et.al.|[2409.09785](http://arxiv.org/abs/2409.09785)|null|
|**2024-09-15**|**RethinkMCTS: Refining Erroneous Thoughts in Monte Carlo Tree Search for Code Generation**|Qingyao Li et.al.|[2409.09584](http://arxiv.org/abs/2409.09584)|null|
|**2024-09-14**|**Enhancing Decision-Making for LLM Agents via Step-Level Q-Value Models**|Yuanzhao Zhai et.al.|[2409.09345](http://arxiv.org/abs/2409.09345)|null|
|**2024-09-14**|**Python Symbolic Execution with LLM-powered Code Generation**|Wenhan Wang et.al.|[2409.09271](http://arxiv.org/abs/2409.09271)|null|
|**2024-09-23**|**Agents in Software Engineering: Survey, Landscape, and Vision**|Yanlin Wang et.al.|[2409.09030](http://arxiv.org/abs/2409.09030)|**[link](https://github.com/deepsoftwareanalytics/awesome-agent4se)**|
|**2024-09-13**|**AI-LieDar: Examine the Trade-off Between Utility and Truthfulness in LLM Agents**|Zhe Su et.al.|[2409.09013](http://arxiv.org/abs/2409.09013)|null|
|**2024-09-13**|**Safeguarding Decentralized Social Media: LLM Agents for Automating Community Rule Compliance**|Lucio La Cava et.al.|[2409.08963](http://arxiv.org/abs/2409.08963)|null|
|**2024-09-13**|**Fusing Dynamics Equation: A Social Opinions Prediction Algorithm with LLM-based Agents**|Junchi Yao et.al.|[2409.08717](http://arxiv.org/abs/2409.08717)|null|
|**2024-09-10**|**MAGDA: Multi-agent guideline-driven diagnostic assistance**|David Bani-Harouni et.al.|[2409.06351](http://arxiv.org/abs/2409.06351)|null|
|**2024-09-08**|**A Pair Programming Framework for Code Generation via Multi-Plan Exploration and Feedback-Driven Refinement**|Huan Zhang et.al.|[2409.05001](http://arxiv.org/abs/2409.05001)|**[link](https://github.com/nju-websoft/paircoder)**|
|**2024-09-06**|**Sparse Rewards Can Self-Train Dialogue Agents**|Barrett Martin Lattimer et.al.|[2409.04617](http://arxiv.org/abs/2409.04617)|**[link](https://github.com/asappresearch/josh-llm-simulation-training)**|
|**2024-09-06**|**LLM-based multi-agent poetry generation in non-cooperative environments**|Ran Zhang et.al.|[2409.03659](http://arxiv.org/abs/2409.03659)|**[link](https://github.com/zhangr2021/Multiagent_poetry)**|
|**2024-09-05**|**Rx Strategist: Prescription Verification using LLM Agents System**|Phuc Phan Van et.al.|[2409.03440](http://arxiv.org/abs/2409.03440)|null|
|**2024-09-05**|**GraphInsight: Unlocking Insights in Large Language Models for Graph Structure Understanding**|Yukun Cao et.al.|[2409.03258](http://arxiv.org/abs/2409.03258)|null|
|**2024-09-04**|**Large Language Model-Based Agents for Software Engineering: A Survey**|Junwei Liu et.al.|[2409.02977](http://arxiv.org/abs/2409.02977)|**[link](https://github.com/fudanselab/agent4se-paper-list)**|
|**2024-09-02**|**Evolution of Social Norms in LLM Agents using Natural Language**|Ilya Horiguchi et.al.|[2409.00993](http://arxiv.org/abs/2409.00993)|null|
|**2024-09-02**|**Co-Learning: Code Learning for Multi-Agent Reinforcement Collaborative Framework with Conversational Natural Language Interfaces**|Jiapeng Yu et.al.|[2409.00985](http://arxiv.org/abs/2409.00985)|**[link](https://github.com/yuqian2003/co_learning)**|
|**2024-08-29**|**HoneyComb: A Flexible LLM-Based Agent System for Materials Science**|Huan Zhang et.al.|[2409.00135](http://arxiv.org/abs/2409.00135)|null|
|**2024-08-30**|**Tool-Assisted Agent on SQL Inspection and Refinement in Real-World Scenarios**|Zhongyuan Wang et.al.|[2408.16991](http://arxiv.org/abs/2408.16991)|null|
|**2024-08-28**|**EPO: Hierarchical LLM Agents with Environment Preference Optimization**|Qi Zhao et.al.|[2408.16090](http://arxiv.org/abs/2408.16090)|**[link](https://github.com/kevinz8866/epo)**|
|**2024-09-05**|**LogicGame: Benchmarking Rule-Based Reasoning Abilities of Large Language Models**|Jiayi Gui et.al.|[2408.15778](http://arxiv.org/abs/2408.15778)|**[link](https://github.com/hypatiaalegra/logicgame-data)**|
|**2024-08-27**|**AgentMonitor: A Plug-and-Play Framework for Predictive and Secure Multi-Agent Systems**|Chi-Min Chan et.al.|[2408.14972](http://arxiv.org/abs/2408.14972)|**[link](https://github.com/chanchimin/agentmonitor)**|
|**2024-08-26**|**LLM-3D Print: Large Language Models To Monitor and Control 3D Printing**|Yayati Jadhav et.al.|[2408.14307](http://arxiv.org/abs/2408.14307)|null|
|**2024-09-02**|**MLR-Copilot: Autonomous Machine Learning Research based on Large Language Models Agents**|Ruochen Li et.al.|[2408.14033](http://arxiv.org/abs/2408.14033)|**[link](https://github.com/du-nlp-lab/mlr-copilot)**|
|**2024-08-26**|**AgentMove: Predicting Human Mobility Anywhere Using Large Language Model based Agentic Framework**|Jie Feng et.al.|[2408.13986](http://arxiv.org/abs/2408.13986)|**[link](https://github.com/tsinghua-fib-lab/agentmove)**|
|**2024-08-23**|**Optimizing Collaboration of LLM based Agents for Finite Element Analysis**|Chuan Tian et.al.|[2408.13406](http://arxiv.org/abs/2408.13406)|null|
|**2024-09-01**|**Can LLMs Understand Social Norms in Autonomous Driving Games?**|Boxuan Wang et.al.|[2408.12680](http://arxiv.org/abs/2408.12680)|null|
|**2024-08-22**|**MDD-5k: A New Diagnostic Conversation Dataset for Mental Disorders Synthesized via Neuro-Symbolic LLM Agents**|Congchi Yin et.al.|[2408.12142](http://arxiv.org/abs/2408.12142)|**[link](https://github.com/lemonsis/mdd-5k)**|
|**2024-08-20**|**FLAME: Learning to Navigate with Multimodal LLM in Urban Environments**|Yunzhe Xu et.al.|[2408.11051](http://arxiv.org/abs/2408.11051)|**[link](https://github.com/xyz9911/FLAME)**|
|**2024-08-20**|**Athena: Safe Autonomous Agents with Verbal Contrastive Learning**|Tanmana Sadhu et.al.|[2408.11021](http://arxiv.org/abs/2408.11021)|null|
|**2024-08-24**|**IDEA:Enhancing the Rule Learning Ability of Language Agents through Induction, Deduction, and Abduction**|Kaiyu He et.al.|[2408.10455](http://arxiv.org/abs/2408.10455)|null|
|**2024-08-20**|**MegaAgent: A Practical Framework for Autonomous Cooperation in Large-Scale LLM Agent Systems**|Qian Wang et.al.|[2408.09955](http://arxiv.org/abs/2408.09955)|null|
|**2024-08-19**|**GoNoGo: An Efficient LLM-based Multi-Agent System for Streamlining Automotive Software Release Decision-Making**|Arsham Gholamzadeh Khoee et.al.|[2408.09785](http://arxiv.org/abs/2408.09785)|null|
|**2024-08-18**|**HiAgent: Hierarchical Working Memory Management for Solving Long-Horizon Agent Tasks with Large Language Model**|Mengkang Hu et.al.|[2408.09559](http://arxiv.org/abs/2408.09559)|**[link](https://github.com/hiagent2024/hiagent)**|
|**2024-08-15**|**EmBARDiment: an Embodied AI Agent for Productivity in XR**|Riccardo Bovo et.al.|[2408.08158](http://arxiv.org/abs/2408.08158)|null|
|**2024-08-15**|**Text2BIM: Generating Building Models Using a Large Language Model-based Multi-Agent Framework**|Changyu Du et.al.|[2408.08054](http://arxiv.org/abs/2408.08054)|null|
|**2024-08-13**|**Agent Q: Advanced Reasoning and Learning for Autonomous AI Agents**|Pranav Putta et.al.|[2408.07199](http://arxiv.org/abs/2408.07199)|null|
|**2024-08-13**|**Diversity Empowers Intelligence: Integrating Expertise of Software Engineering Agents**|Kexun Zhang et.al.|[2408.07060](http://arxiv.org/abs/2408.07060)|null|
|**2024-08-12**|**Hierarchical in-Context Reinforcement Learning with Hindsight Modular Reflections for Planning**|Chuanneng Sun et.al.|[2408.06520](http://arxiv.org/abs/2408.06520)|null|
|**2024-08-12**|**Can We Rely on LLM Agents to Draft Long-Horizon Plans? Let's Take TravelPlanner as an Example**|Yanan Chen et.al.|[2408.06318](http://arxiv.org/abs/2408.06318)|null|
|**2024-08-13**|**DataNarrative: Automated Data-Driven Storytelling with Visualizations and Texts**|Mohammed Saidul Islam et.al.|[2408.05346](http://arxiv.org/abs/2408.05346)|**[link](https://github.com/saidul-islam98/DataNarrative)**|
|**2024-08-08**|**Perceive, Reflect, and Plan: Designing LLM Agent for Goal-Directed City Navigation without Instructions**|Qingbin Zeng et.al.|[2408.04168](http://arxiv.org/abs/2408.04168)|**[link](https://github.com/hiyouga/llama-factory)**|
|**2024-08-11**|**CodexGraph: Bridging Large Language Models and Code Repositories via Code Graph Databases**|Xiangyan Liu et.al.|[2408.03910](http://arxiv.org/abs/2408.03910)|**[link](https://github.com/modelscope/modelscope-agent)**|
|**2024-08-07**|**Large Language Models for Base Station Siting: Intelligent Deployment based on Prompt or Agent**|Yanhu Wang et.al.|[2408.03631](http://arxiv.org/abs/2408.03631)|null|
|**2024-08-05**|**Evaluating and Enhancing LLMs Agent based on Theory of Mind in Guandan: A Multi-Player Cooperative Game under Imperfect Information**|Yauwai Yim et.al.|[2408.02559](http://arxiv.org/abs/2408.02559)|null|
|**2024-08-05**|**From LLMs to LLM-based Agents for Software Engineering: A Survey of Current, Challenges and Future**|Haolin Jin et.al.|[2408.02479](http://arxiv.org/abs/2408.02479)|null|
|**2024-05-16**|**When LLMs step into the 3D World: A Survey and Meta-Analysis of 3D Tasks via Multi-modal Large Language Models**|Xianzheng Ma et.al.|[2405.10255](http://arxiv.org/abs/2405.10255)|**[link](https://github.com/activevisionlab/awesome-llm-3d)**|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## llm

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-24**|**Unbounded: A Generative Infinite Game of Character Life Simulation**|Jialu Li et.al.|[2410.18975](http://arxiv.org/abs/2410.18975)|null|我们引入了生成式无限游戏的概念，这是一种通过使用生成模型超越传统有限、硬编码系统边界的视频游戏。受詹姆斯·P·卡斯关于有限与无限游戏区别的启发，我们利用最近在生成式人工智能领域的进展，创造了《无界》：一个完全封装在生成模型中的角色生活模拟游戏。具体来说，《无界》从沙盒生活模拟游戏中汲取灵感，允许玩家在一个虚拟世界中通过喂养、玩耍和引导来与自主的虚拟角色互动——其中一些开放式的机制是由大型语言模型（LLM）生成的，部分机制可以是涌现出来的。为了开发《无界》，我们在LLM和视觉生成领域提出了技术创新。特别地，我们展示了：(1) 一种专门精简的大规模语言模型（LLM），能够实时动态地生成游戏机制、叙事和角色互动；(2) 一种新的动态区域图像提示适配器（IP-Adapter），用于视觉模型中，确保角色在多个环境下的视觉生成既一致又灵活。我们通过对系统的定性和定量分析进行了评估，显示在角色生活模拟、用户指令遵循、叙事连贯性以及角色和环境的视觉一致性方面，相比传统的相关方法有了显著改进。|
|**2024-10-24**|**Does Data Contamination Detection Work (Well) for LLMs? A Survey and Evaluation on Detection Assumptions**|Yujuan Fu et.al.|[2410.18966](http://arxiv.org/abs/2410.18966)|null|大型语言模型（LLMs）在各种基准测试中表现出色，显示出作为通用任务解决者的潜力。然而，由于LLMs通常是在大量数据上进行训练的，在其评估过程中一个重要的问题是数据污染，即训练数据与评估数据集之间的重叠会导致性能评估虚高。虽然已经开发了多种方法来识别数据污染，但这些方法依赖于特定的假设，而这些假设可能在不同场景下并不普遍适用。为了填补这一空白，我们系统地回顾了47篇关于数据污染检测的论文，对其中的假设进行了分类，并评估了这些假设是否得到了严格的验证。我们确定并分析了八类假设，并将其中三类作为案例研究进行了测试。我们的分析表明，在对用于预训练LLMs的实例进行分类时，基于这三种假设的检测方法的表现接近随机猜测，这表明当前的LLMs学习的是数据分布而不是记忆单个实例。总体而言，这项工作强调了方法明确陈述其基本假设并在各种场景下验证其有效性的必要性。|
|**2024-10-24**|**OSCAR: Operating System Control via State-Aware Reasoning and Re-Planning**|Xiaoqiang Wang et.al.|[2410.18963](http://arxiv.org/abs/2410.18963)|null|大型语言模型（LLM）和大型多模态模型（LMM）在自动化复杂任务如网页浏览和游戏方面展现了巨大潜力。然而，它们在多样化应用中的泛化能力仍然有限，限制了更广泛的应用。为了解决这一挑战，我们提出了OSCAR：基于状态感知推理和重规划的操作系统控制。OSCAR是一个通用代理，旨在通过标准化的控制方式（例如鼠标和键盘输入），同时处理屏幕图像以执行用户命令，自主地导航和与各种桌面和移动应用程序交互。OSCAR将人类指令转换成可执行的Python代码，实现对图形用户界面（GUI）的精确控制。为了提高稳定性和适应性，OSCAR作为一个状态机运行，配备错误处理机制和动态任务重规划功能，使其能够高效地根据实时反馈和异常情况进行调整。我们在多样化的基准测试中展示了OSCAR的有效性，这些测试涵盖了桌面和移动平台，在这些测试中，它将复杂的工作流程简化为简单的自然语言命令，显著提高了用户的生产力。我们的代码将在发表时开源。|
|**2024-10-24**|**Bridge-Coder: Unlocking LLMs' Potential to Overcome Language Gaps in Low-Resource Code**|Jipeng Zhang et.al.|[2410.18957](http://arxiv.org/abs/2410.18957)|null|大型语言模型（LLMs）在生成高资源编程语言（如Python）的代码方面表现出强大的能力，但在低资源编程语言（如Racket或D）上表现不佳。这种性能差距加深了数字鸿沟，阻碍了使用低资源编程语言的开发者从LLM的进步中同等受益，并加剧了在代表性不足的编程社区中的创新差异。尽管为低资源编程语言生成额外训练数据是一个有前景的方法，但它面临两个主要挑战：人工标注劳动密集且成本高昂，而由LLM生成的低资源编程语言代码质量往往较差。这个问题的根本原因在于自然语言到编程语言之间的差距（NL-PL Gap），特别是在低资源编程语言中，由于对齐数据有限，这一差距尤为明显。在这项工作中，我们提出了一种名为Bridge-Coder的新方法，该方法利用LLM的内在能力来提高其在低资源编程语言上的表现。我们的方法包括两个关键阶段：桥接生成，通过利用LLM的一般知识理解、高资源编程语言的熟练程度以及上下文学习能力来创建高质量的数据集；然后是桥接对齐，逐步改进自然语言指令与低资源编程语言之间的对齐。实验结果表明，在多个低资源编程语言上，Bridge-Coder显著提升了模型的表现，证明了我们方法的有效性和泛化性。此外，我们还对方法的关键组成部分进行了详细分析，为未来解决低资源编程语言相关挑战的工作提供了有价值的见解。|
|**2024-10-24**|**BioMistral-NLU: Towards More Generalizable Medical Language Understanding through Instruction Tuning**|Yujuan Velvin Fu et.al.|[2410.18955](http://arxiv.org/abs/2410.18955)|null|大型语言模型（如ChatGPT）通过在大量多样化的指令跟随语料库上进行微调，可以泛化到新任务。然而，这些经过指令微调的大型语言模型在需要领域知识、细粒度文本理解和结构化数据提取的专业医疗自然语言理解（NLU）任务中往往表现不佳。为了解决这个问题，我们：(1) 提出了一种统一的提示格式，用于7个重要的NLU任务，(2) 整理了一个指令微调数据集MNLU-Instruct，利用了多种现有的开源医疗NLU语料库，(3) 通过在MNLU-Instruct上对BioMistral进行微调，开发了具有泛化能力的医疗NLU模型BioMistral-NLU。我们在零样本设置下，在来自两个广泛采用的医疗NLU基准——生物医学语言理解评估（BLUE）和生物医学语言理解和推理基准（BLURB）中的6个重要NLU任务上评估了BioMistral-NLU。实验表明，我们的BioMistral-NLU优于原始的BioMistral以及专有大语言模型ChatGPT和GPT-4。我们的与数据集无关的提示策略和跨多样化NLU任务的指令微调步骤增强了大语言模型在多样化医疗NLU任务上的泛化能力。消融实验表明，即使总的训练实例数量保持不变，通过更广泛的任务进行指令微调也能增强下游的零样本泛化性能。|
|**2024-10-24**|**Dynamic Vocabulary Pruning in Early-Exit LLMs**|Jort Vincenti et.al.|[2410.18952](http://arxiv.org/abs/2410.18952)|**[link](https://github.com/matteonulli/vocabulary_pruning)**|**增加大型语言模型（LLM）的规模已被证明可以提高性能。然而，这会导致推理速度变慢且成本更高。提前退出是一种有望提高LLM推理效率的方法，它允许在中间层进行下一个词的预测。然而，现代LLM中的大词汇量使得退出决策所需的置信度估计计算变得非常昂贵，从而降低了效率增益。为了解决这个问题，我们提出在测试时对每个词动态剪枝词汇表。具体来说，在初始层之一对词汇表进行剪枝，然后在整个前向传递过程中使用较小的词汇表。我们的实验表明，这种后处理动态词汇剪枝方法提高了提前退出LLM中置信度估计的效率，同时保持了竞争力。**|
|**2024-10-24**|**From Blind Solvers to Logical Thinkers: Benchmarking LLMs' Logical Integrity on Faulty Mathematical Problems**|A M Muntasir Rahman et.al.|[2410.18921](http://arxiv.org/abs/2410.18921)|null|考虑这个数学问题：“莉莉昨天从她最好的朋友那里收到了3块饼干，并且早餐吃了5块。今天，她的朋友又给了她3块饼干。莉莉现在有多少块饼干？”许多大型语言模型（LLM）在以往的研究中通过使用方程“3 - 5 + 3”计算出答案“1”。然而，从人类的角度来看，我们认识到这个问题的固有缺陷：如果莉莉最初只有3块饼干，她不可能吃掉5块。这种差异引发了一个关键问题：当前的LLM仅仅是盲目解题者，仅应用数学运算而不进行更深层次的推理，还是能够识别逻辑不一致性的逻辑思考者？为了探讨这个问题，我们提出了一个基准数据集FaultyMath，其中包括多种类型的错误数学问题：i) 多个数学类别，如代数、几何、数论等；ii) 不同难度级别；iii) 错误来源多样——从违反常识和表述模糊到数学矛盾等。我们对包括开源、闭源和专门针对数学的模型在内的广泛LLM进行了评估，评估维度包括：(i) 模型在没有明确提示的情况下检测错误数学问题的准确性如何？(ii) 当提供关于问题有效性的提示时（无论是正确的还是误导性的），LLM在多大程度上能适应成为可靠的逻辑思考者？(iii) 当LLM识别出一个数学问题是错误的时候，它们生成的解释有多可信？通过广泛的实验和详细的分析，我们的结果表明，现有的LLM大多表现为盲目解题者，在作为逻辑思考者所需的推理能力方面存在不足。|
|**2024-10-24**|**A Survey on Speech Large Language Models**|Jing Peng et.al.|[2410.18908](http://arxiv.org/abs/2410.18908)|null|大型语言模型（LLMs）表现出强大的上下文理解和卓越的多任务性能。因此，研究人员一直在寻求将LLMs集成到广义的口语理解（SLU）领域中。与传统的通过自动语音识别（ASR）生成文本后再级联使用LLMs的方法不同，新的努力集中在设计以音频特征提取-多模态信息融合-LLM推理（语音LLMs）为中心的架构上。这种方法能够实现更丰富的音频特征提取，同时促进音频和文本模态的端到端融合，从而从音频数据中获得更深的理解和推理能力。本文阐述了语音LLMs的发展，深入分析了系统架构和训练策略。通过广泛的研究和一系列针对性实验，论文评估了语音LLMs在丰富音频转录方面的进步及其在SLU领域内跨任务整合的潜力。此外，它还指出了实验过程中发现的关键挑战，例如在某些条件下LLMs的休眠问题。论文进一步探讨了语音LLMs的训练策略，基于这些发现提出了潜在解决方案，并为该领域的未来研究以及LLMs在多模态场景中的应用提供了有价值的见解和参考。|
|**2024-10-24**|**PRISM: A Methodology for Auditing Biases in Large Language Models**|Leif Azzopardi et.al.|[2410.18906](http://arxiv.org/abs/2410.18906)|**[link](https://github.com/cis-phawm/prism)**|**审计大型语言模型（LLMs）以发现其偏见和偏好是创建负责任的人工智能（AI）中出现的一个新挑战。虽然已经提出了多种方法来引出这些模型的偏好，但LLM训练者也采取了对策，使得LLMs隐藏、混淆或直接拒绝披露它们在某些主题上的立场。本文介绍了PRISM，这是一种灵活的基于询问的方法，用于审计LLMs——该方法试图通过任务驱动的询问提示间接引出这些立场，而不是直接询问所述偏好。为了展示该方法的实用性，我们将PRISM应用于政治罗盘测试，评估了来自七个提供者的二十一个LLMs的政治倾向。我们展示了这些模型默认上倾向于经济左翼和社会自由主义（与先前的工作一致）。我们还展示了这些模型愿意表达的立场空间——一些模型受到更多限制且不那么顺从，而另一些则更加中立和客观。总之，PRISM可以更可靠地探测和审计LLMs，以理解它们的偏好、偏见和约束。**|
|**2024-10-24**|**LLMs for Extremely Low-Resource Finno-Ugric Languages**|Taido Purason et.al.|[2410.18902](http://arxiv.org/abs/2410.18902)|null|大型语言模型（LLM）的发展主要集中在资源丰富的语言上，导致资源较少的语言，如芬兰-乌戈尔语系中的语言，严重代表性不足。本文通过关注沃罗语、利沃尼亚语和科米语来解决这一差距。我们涵盖了从数据收集到指令微调和评估的几乎整个LLM创建周期。我们的贡献包括开发多语言基础模型和指令微调模型；创建评估基准，包括smugri-MT-bench多轮对话基准；并进行人工评估。我们希望这项工作能够促进语言多样性，确保资源较少的语言也能从自然语言处理的进步中受益。|
|**2024-10-23**|**LongRAG: A Dual-Perspective Retrieval-Augmented Generation Paradigm for Long-Context Question Answering**|Qingfei Zhao et.al.|[2410.18050](http://arxiv.org/abs/2410.18050)|**[link](https://github.com/qingfei1/longrag)**|
|**2024-10-23**|**Key Algorithms for Keyphrase Generation: Instruction-Based LLMs for Russian Scientific Keyphrases**|Anna Glazkova et.al.|[2410.18040](http://arxiv.org/abs/2410.18040)|null|
|**2024-10-23**|**MiniFed : Integrating LLM-based Agentic-Workflow for Simulating FOMC Meeting**|Sungil Seok et.al.|[2410.18012](http://arxiv.org/abs/2410.18012)|null|
|**2024-10-23**|**ExpertFlow: Optimized Expert Activation and Token Allocation for Efficient Mixture-of-Experts Inference**|Xin He et.al.|[2410.17954](http://arxiv.org/abs/2410.17954)|null|
|**2024-10-23**|**SimRAG: Self-Improving Retrieval-Augmented Generation for Adapting Large Language Models to Specialized Domains**|Ran Xu et.al.|[2410.17952](http://arxiv.org/abs/2410.17952)|null|
|**2024-10-23**|**Benchmarking Floworks against OpenAI & Anthropic: A Novel Framework for Enhanced LLM Function Calling**|Nirav Bhan et.al.|[2410.17950](http://arxiv.org/abs/2410.17950)|null|
|**2024-10-23**|**Guide for Defense (G4D): Dynamic Guidance for Robust and Balanced Defense in Large Language Models**|He Cao et.al.|[2410.17922](http://arxiv.org/abs/2410.17922)|null|
|**2024-10-23**|**R-CoT: Reverse Chain-of-Thought Problem Generation for Geometric Reasoning in Large Multimodal Models**|Linger Deng et.al.|[2410.17885](http://arxiv.org/abs/2410.17885)|**[link](https://github.com/dle666/r-cot)**|
|**2024-10-23**|**AdaRankGrad: Adaptive Gradient-Rank and Moments for Memory-Efficient LLMs Training and Fine-Tuning**|Yehonathan Refael et.al.|[2410.17881](http://arxiv.org/abs/2410.17881)|null|
|**2024-10-23**|**Understanding Layer Significance in LLM Alignment**|Guangyuan Shi et.al.|[2410.17875](http://arxiv.org/abs/2410.17875)|null|
|**2024-10-22**|**Large Language Models Empowered Personalized Web Agents**|Hongru Cai et.al.|[2410.17236](http://arxiv.org/abs/2410.17236)|null|
|**2024-10-22**|**Fine-Tuning Large Language Models to Appropriately Abstain with Semantic Entropy**|Benedict Aaron Tjandra et.al.|[2410.17234](http://arxiv.org/abs/2410.17234)|null|
|**2024-10-22**|**Few-shot In-Context Preference Learning Using Large Language Models**|Chao Yu et.al.|[2410.17233](http://arxiv.org/abs/2410.17233)|null|
|**2024-10-22**|**Context-aware Prompt Tuning: Advancing In-Context Learning with Adversarial Methods**|Tsachi Blau et.al.|[2410.17222](http://arxiv.org/abs/2410.17222)|null|
|**2024-10-22**|**Exploring Possibilities of AI-Powered Legal Assistance in Bangladesh through Large Language Modeling**|Azmine Toushik Wasi et.al.|[2410.17210](http://arxiv.org/abs/2410.17210)|**[link](https://github.com/ciol-researchlab/ukil)**|
|**2024-10-22**|**VoiceBench: Benchmarking LLM-Based Voice Assistants**|Yiming Chen et.al.|[2410.17196](http://arxiv.org/abs/2410.17196)|**[link](https://github.com/matthewcym/voicebench)**|
|**2024-10-22**|**Improving Pinterest Search Relevance Using Large Language Models**|Han Wang et.al.|[2410.17152](http://arxiv.org/abs/2410.17152)|null|
|**2024-10-22**|**Can General-Purpose Large Language Models Generalize to English-Thai Machine Translation ?**|Jirat Chiaranaipanich et.al.|[2410.17145](http://arxiv.org/abs/2410.17145)|null|
|**2024-10-22**|**Towards Automated Penetration Testing: Introducing LLM Benchmark, Analysis, and Improvements**|Isamu Isozaki et.al.|[2410.17141](http://arxiv.org/abs/2410.17141)|null|
|**2024-10-22**|**Exploring RL-based LLM Training for Formal Language Tasks with Programmed Rewards**|Alexander G. Padula et.al.|[2410.17126](http://arxiv.org/abs/2410.17126)|**[link](https://github.com/padlex/reinforcement-learning-from-explicitly-programmed-reward-signals)**|
|**2024-10-21**|**Reflection-Bench: probing AI intelligence with reflection**|Lingyu Li et.al.|[2410.16270](http://arxiv.org/abs/2410.16270)|**[link](https://github.com/yabyum/reflectionbench)**|
|**2024-10-21**|**Elucidating the design space of language models for image generation**|Xuantong Liu et.al.|[2410.16257](http://arxiv.org/abs/2410.16257)|**[link](https://github.com/Pepper-lll/LMforImageGeneration)**|
|**2024-10-21**|**CompassJudger-1: All-in-one Judge Model Helps Model Evaluation and Evolution**|Maosong Cao et.al.|[2410.16256](http://arxiv.org/abs/2410.16256)|**[link](https://github.com/open-compass/compassjudger)**|
|**2024-10-21**|**Can Knowledge Editing Really Correct Hallucinations?**|Baixiang Huang et.al.|[2410.16251](http://arxiv.org/abs/2410.16251)|**[link](https://github.com/llm-editing/HalluEditBench)**|
|**2024-10-21**|**Analyzing Context Contributions in LLM-based Machine Translation**|Emmanouil Zaranis et.al.|[2410.16246](http://arxiv.org/abs/2410.16246)|null|
|**2024-10-21**|**IBGP: Imperfect Byzantine Generals Problem for Zero-Shot Robustness in Communicative Multi-Agent Systems**|Yihuan Mao et.al.|[2410.16237](http://arxiv.org/abs/2410.16237)|null|
|**2024-10-21**|**LLaVA-KD: A Framework of Distilling Multimodal Large Language Models**|Yuxuan Cai et.al.|[2410.16236](http://arxiv.org/abs/2410.16236)|**[link](https://github.com/Fantasyele/LLaVA-KD)**|
|**2024-10-21**|**Building A Coding Assistant via the Retrieval-Augmented Language Model**|Xinze Li et.al.|[2410.16229](http://arxiv.org/abs/2410.16229)|**[link](https://github.com/NEUIR/CONAN)**|
|**2024-10-21**|**Pre-training Distillation for Large Language Models: A Design Space Exploration**|Hao Peng et.al.|[2410.16215](http://arxiv.org/abs/2410.16215)|null|
|**2024-10-21**|**Comprehensive benchmarking of large language models for RNA secondary structure prediction**|L. I. Zablocki et.al.|[2410.16212](http://arxiv.org/abs/2410.16212)|**[link](https://github.com/sinc-lab/rna-llm-folding)**|
|**2024-10-18**|**Are AI Detectors Good Enough? A Survey on Quality of Datasets With Machine-Generated Texts**|German Gritsai et.al.|[2410.14677](http://arxiv.org/abs/2410.14677)|null|
|**2024-10-18**|**SudoLM: Learning Access Control of Parametric Knowledge with Authorization Alignment**|Qin Liu et.al.|[2410.14676](http://arxiv.org/abs/2410.14676)|null|
|**2024-10-18**|**Enhancing Large Language Models' Situated Faithfulness to External Contexts**|Yukun Huang et.al.|[2410.14675](http://arxiv.org/abs/2410.14675)|**[link](https://github.com/kkkevinkkkkk/situated_faithfulness)**|
|**2024-10-18**|**A Large Language Model-Driven Reward Design Framework via Dynamic Feedback for Reinforcement Learning**|Shengjie Sun et.al.|[2410.14660](http://arxiv.org/abs/2410.14660)|null|
|**2024-10-18**|**EvoPress: Towards Optimal Dynamic Model Compression via Evolutionary Search**|Oliver Sieberling et.al.|[2410.14649](http://arxiv.org/abs/2410.14649)|**[link](https://github.com/ist-daslab/evopress)**|
|**2024-10-18**|**Distance between Relevant Information Pieces Causes Bias in Long-Context LLMs**|Runchu Tian et.al.|[2410.14641](http://arxiv.org/abs/2410.14641)|**[link](https://github.com/Rachum-thu/LongPiBench)**|
|**2024-10-18**|**GenEOL: Harnessing the Generative Power of LLMs for Training-Free Sentence Embeddings**|Raghuveer Thirukovalluru et.al.|[2410.14635](http://arxiv.org/abs/2410.14635)|null|
|**2024-10-18**|**DiSCo Meets LLMs: A Unified Approach for Sparse Retrieval and Contextual Distillation in Conversational Search**|Simon Lupart et.al.|[2410.14609](http://arxiv.org/abs/2410.14609)|null|
|**2024-10-18**|**Teaching Models to Balance Resisting and Accepting Persuasion**|Elias Stengel-Eskin et.al.|[2410.14596](http://arxiv.org/abs/2410.14596)|**[link](https://github.com/esteng/persuasion_balanced_training)**|
|**2024-10-18**|**Do LLMs estimate uncertainty well in instruction-following?**|Juyeon Heo et.al.|[2410.14582](http://arxiv.org/abs/2410.14582)|null|
|**2024-10-17**|**How Numerical Precision Affects Mathematical Reasoning Capabilities of LLMs**|Guhao Feng et.al.|[2410.13857](http://arxiv.org/abs/2410.13857)|null|
|**2024-10-17**|**Retrospective Learning from Interactions**|Zizhao Chen et.al.|[2410.13852](http://arxiv.org/abs/2410.13852)|null|
|**2024-10-17**|**SimLayerKV: A Simple Framework for Layer-Level KV Cache Reduction**|Xuan Zhang et.al.|[2410.13846](http://arxiv.org/abs/2410.13846)|**[link](https://github.com/sail-sg/simlayerkv)**|
|**2024-10-17**|**Active-Dormant Attention Heads: Mechanistically Demystifying Extreme-Token Phenomena in LLMs**|Tianyu Guo et.al.|[2410.13835](http://arxiv.org/abs/2410.13835)|null|
|**2024-10-17**|**AgentOccam: A Simple Yet Strong Baseline for LLM-Based Web Agents**|Ke Yang et.al.|[2410.13825](http://arxiv.org/abs/2410.13825)|null|
|**2024-10-18**|**Harnessing Webpage UIs for Text-Rich Visual Understanding**|Junpeng Liu et.al.|[2410.13824](http://arxiv.org/abs/2410.13824)|null|
|**2024-10-18**|**BenTo: Benchmark Task Reduction with In-Context Transferability**|Hongyu Zhao et.al.|[2410.13804](http://arxiv.org/abs/2410.13804)|**[link](https://github.com/tianyi-lab/bento)**|
|**2024-10-17**|**Modeling Future Conversation Turns to Teach LLMs to Ask Clarifying Questions**|Michael J. Q. Zhang et.al.|[2410.13788](http://arxiv.org/abs/2410.13788)|null|
|**2024-10-17**|**PopAlign: Diversifying Contrasting Patterns for a More Comprehensive Alignment**|Zekun Moore Wang et.al.|[2410.13785](http://arxiv.org/abs/2410.13785)|null|
|**2024-10-17**|**Aggregation Artifacts in Subjective Tasks Collapse Large Language Models' Posteriors**|Georgios Chochlakis et.al.|[2410.13776](http://arxiv.org/abs/2410.13776)|null|
|**2024-10-16**|**Meta-Chunking: Learning Efficient Text Segmentation via Logical Perception**|Jihao Zhao et.al.|[2410.12788](http://arxiv.org/abs/2410.12788)|**[link](https://github.com/IAAR-Shanghai/Meta-Chunking)**|
|**2024-10-16**|**In-Context Learning Enables Robot Action Prediction in LLMs**|Yida Yin et.al.|[2410.12782](http://arxiv.org/abs/2410.12782)|null|
|**2024-10-17**|**CREAM: Consistency Regularized Self-Rewarding Language Models**|Zhaoyang Wang et.al.|[2410.12735](http://arxiv.org/abs/2410.12735)|null|
|**2024-10-16**|**FusionLLM: A Decentralized LLM Training System on Geo-distributed GPUs with Adaptive Compression**|Zhenheng Tang et.al.|[2410.12707](http://arxiv.org/abs/2410.12707)|null|
|**2024-10-16**|**Embedding an Ethical Mind: Aligning Text-to-Image Synthesis via Lightweight Value Optimization**|Xingqi Wang et.al.|[2410.12700](http://arxiv.org/abs/2410.12700)|**[link](https://github.com/achernarwang/LiVO)**|
|**2024-10-16**|**Automatic Mapping of Anatomical Landmarks from Free-Text Using Large Language Models: Insights from Llama-2**|Mohamad Abdi et.al.|[2410.12686](http://arxiv.org/abs/2410.12686)|null|
|**2024-10-16**|**Evaluating Morphological Compositional Generalization in Large Language Models**|Mete Ismayilzada et.al.|[2410.12656](http://arxiv.org/abs/2410.12656)|null|
|**2024-10-16**|**Weak-to-Strong Generalization beyond Accuracy: a Pilot Study in Safety, Toxicity, and Legal Reasoning**|Ruimeng Ye et.al.|[2410.12621](http://arxiv.org/abs/2410.12621)|**[link](https://github.com/yeruimeng/wts)**|
|**2024-10-16**|**Exploring Model Kinship for Merging Large Language Models**|Yedi Hu et.al.|[2410.12613](http://arxiv.org/abs/2410.12613)|**[link](https://github.com/zjunlp/ModelKinship)**|
|**2024-10-16**|**Not All Votes Count! Programs as Verifiers Improve Self-Consistency of Language Models for Math Reasoning**|Vernon Y. H. Toh et.al.|[2410.12608](http://arxiv.org/abs/2410.12608)|null|
|**2024-10-15**|**SGEdit: Bridging LLM with Text2Image Generative Model for Scene Graph-based Image Editing**|Zhiyuan Zhang et.al.|[2410.11815](http://arxiv.org/abs/2410.11815)|null|
|**2024-10-15**|**NesTools: A Dataset for Evaluating Nested Tool Learning Abilities of Large Language Models**|Han Han et.al.|[2410.11805](http://arxiv.org/abs/2410.11805)|null|
|**2024-10-15**|**Selection-p: Self-Supervised Task-Agnostic Prompt Compression for Faithfulness and Transferability**|Tsz Ting Chung et.al.|[2410.11786](http://arxiv.org/abs/2410.11786)|null|
|**2024-10-15**|**G-Designer: Architecting Multi-agent Communication Topologies via Graph Neural Networks**|Guibin Zhang et.al.|[2410.11782](http://arxiv.org/abs/2410.11782)|null|
|**2024-10-15**|**Language Models Encode Numbers Using Digit Representations in Base 10**|Amit Arnold Levy et.al.|[2410.11781](http://arxiv.org/abs/2410.11781)|**[link](https://github.com/amitlevy/base10)**|
|**2024-10-15**|**Layer-wise Importance Matters: Less Memory for Better Performance in Parameter-efficient Fine-tuning of Large Language Models**|Kai Yao et.al.|[2410.11772](http://arxiv.org/abs/2410.11772)|**[link](https://github.com/kaiseem/ist)**|
|**2024-10-15**|**Personas with Attitudes: Controlling LLMs for Diverse Data Annotation**|Leon Fröhling et.al.|[2410.11745](http://arxiv.org/abs/2410.11745)|**[link](https://github.com/frohleon/personas-with-attitudes)**|
|**2024-10-15**|**DySpec: Faster Speculative Decoding with Dynamic Token Tree Structure**|Yunfan Xiong et.al.|[2410.11744](http://arxiv.org/abs/2410.11744)|null|
|**2024-10-15**|**Light-Weight Fault Tolerant Attention for Large Language Model Training**|Yuhang Liang et.al.|[2410.11720](http://arxiv.org/abs/2410.11720)|null|
|**2024-10-15**|**Converging to a Lingua Franca: Evolution of Linguistic Regions and Semantics Alignment in Multilingual Large Language Models**|Hongchuan Zeng et.al.|[2410.11718](http://arxiv.org/abs/2410.11718)|null|
|**2024-10-14**|**DuoAttention: Efficient Long-Context LLM Inference with Retrieval and Streaming Heads**|Guangxuan Xiao et.al.|[2410.10819](http://arxiv.org/abs/2410.10819)|**[link](https://github.com/mit-han-lab/duo-attention)**|
|**2024-10-14**|**Your Mixture-of-Experts LLM Is Secretly an Embedding Model For Free**|Ziyue Li et.al.|[2410.10814](http://arxiv.org/abs/2410.10814)|**[link](https://github.com/tianyi-lab/moe-embedding)**|
|**2024-10-14**|**LongMemEval: Benchmarking Chat Assistants on Long-Term Interactive Memory**|Di Wu et.al.|[2410.10813](http://arxiv.org/abs/2410.10813)|**[link](https://github.com/xiaowu0162/longmemeval)**|
|**2024-10-14**|**Mix Data or Merge Models? Optimizing for Diverse Multi-Task Learning**|Aakanksha et.al.|[2410.10801](http://arxiv.org/abs/2410.10801)|null|
|**2024-10-14**|**Focused ReAct: Improving ReAct through Reiterate and Early Stop**|Shuoqiu Li et.al.|[2410.10779](http://arxiv.org/abs/2410.10779)|null|
|**2024-10-14**|**AFlow: Automating Agentic Workflow Generation**|Jiayi Zhang et.al.|[2410.10762](http://arxiv.org/abs/2410.10762)|**[link](https://github.com/geekan/metagpt)**|
|**2024-10-14**|**SplitLLM: Collaborative Inference of LLMs for Model Placement and Throughput Optimization**|Akrit Mudvari et.al.|[2410.10759](http://arxiv.org/abs/2410.10759)|null|
|**2024-10-14**|**Use Random Selection for Now: Investigation of Few-Shot Selection Strategies in LLM-based Text Augmentation for Classification**|Jan Cegin et.al.|[2410.10756](http://arxiv.org/abs/2410.10756)|**[link](https://github.com/kinit-sk/selec-strats-for-aug)**|
|**2024-10-14**|**NT-LLM: A Novel Node Tokenizer for Integrating Graph Structure into Large Language Models**|Yanbiao Ji et.al.|[2410.10743](http://arxiv.org/abs/2410.10743)|null|
|**2024-10-14**|**SensorBench: Benchmarking LLMs in Coding-Based Sensor Processing**|Pengrui Quan et.al.|[2410.10741](http://arxiv.org/abs/2410.10741)|**[link](https://github.com/nesl/llm_sensor_processing)**|
|**2024-10-11**|**AttnGCG: Enhancing Jailbreaking Attacks on LLMs with Attention Manipulation**|Zijun Wang et.al.|[2410.09040](http://arxiv.org/abs/2410.09040)|**[link](https://github.com/ucsc-vlaa/attngcg-attack)**|
|**2024-10-11**|**SimpleStrat: Diversifying Language Model Generation with Stratification**|Justin Wong et.al.|[2410.09038](http://arxiv.org/abs/2410.09038)|null|
|**2024-10-11**|**Mentor-KD: Making Small Language Models Better Multi-step Reasoners**|Hojae Lee et.al.|[2410.09037](http://arxiv.org/abs/2410.09037)|**[link](https://github.com/2hojae/mentor-kd)**|
|**2024-10-11**|**PEAR: A Robust and Flexible Automation Framework for Ptychography Enabled by Multiple Large Language Model Agents**|Xiangyu Yin et.al.|[2410.09034](http://arxiv.org/abs/2410.09034)|null|
|**2024-10-11**|**The Impact of Visual Information in Chinese Characters: Evaluating Large Models' Ability to Recognize and Utilize Radicals**|Xiaofeng Wu et.al.|[2410.09013](http://arxiv.org/abs/2410.09013)|null|
|**2024-10-11**|**Software Engineering and Foundation Models: Insights from Industry Blogs Using a Jury of Foundation Models**|Hao Li et.al.|[2410.09012](http://arxiv.org/abs/2410.09012)|**[link](https://github.com/sailresearch/fmse-blogs)**|
|**2024-10-11**|**SuperCorrect: Supervising and Correcting Language Models with Error-Driven Insights**|Ling Yang et.al.|[2410.09008](http://arxiv.org/abs/2410.09008)|**[link](https://github.com/yangling0818/supercorrect-llm)**|
|**2024-10-11**|**From Interaction to Impact: Towards Safer AI Agents Through Understanding and Evaluating UI Operation Impacts**|Zhuohao Jerry Zhang et.al.|[2410.09006](http://arxiv.org/abs/2410.09006)|null|
|**2024-10-11**|**Science is Exploration: Computational Frontiers for Conceptual Metaphor Theory**|Rebecca M. M. Hicke et.al.|[2410.08991](http://arxiv.org/abs/2410.08991)|**[link](https://github.com/rmatouschekh/science-is-exploration)**|
|**2024-10-11**|**SubZero: Random Subspace Zeroth-Order Optimization for Memory-Efficient LLM Fine-Tuning**|Ziming Yu et.al.|[2410.08989](http://arxiv.org/abs/2410.08989)|**[link](https://github.com/zimingyy/subzero)**|
|**2024-10-10**|**Mono-InternVL: Pushing the Boundaries of Monolithic Multimodal Large Language Models with Endogenous Visual Pre-training**|Gen Luo et.al.|[2410.08202](http://arxiv.org/abs/2410.08202)|null|
|**2024-10-10**|**From Exploration to Mastery: Enabling LLMs to Master Tools via Self-Driven Interactions**|Changle Qu et.al.|[2410.08197](http://arxiv.org/abs/2410.08197)|**[link](https://github.com/quchangle1/DRAFT)**|
|**2024-10-10**|**GenARM: Reward Guided Generation with Autoregressive Reward Model for Test-time Alignment**|Yuancheng Xu et.al.|[2410.08193](http://arxiv.org/abs/2410.08193)|null|
|**2024-10-10**|**DelTA: An Online Document-Level Translation Agent Based on Multi-Level Memory**|Yutong Wang et.al.|[2410.08143](http://arxiv.org/abs/2410.08143)|**[link](https://github.com/yutongwang1216/docmtagent)**|
|**2024-10-10**|**Think Beyond Size: Dynamic Prompting for More Effective Reasoning**|Kamesh R et.al.|[2410.08130](http://arxiv.org/abs/2410.08130)|null|
|**2024-10-10**|**Mars: Situated Inductive Reasoning in an Open-World Environment**|Xiaojuan Tang et.al.|[2410.08126](http://arxiv.org/abs/2410.08126)|null|
|**2024-10-10**|**Optima: Optimizing Effectiveness and Efficiency for LLM-Based Multi-Agent System**|Weize Chen et.al.|[2410.08115](http://arxiv.org/abs/2410.08115)|null|
|**2024-10-10**|**A Closer Look at Machine Unlearning for Large Language Models**|Xiaojian Yuan et.al.|[2410.08109](http://arxiv.org/abs/2410.08109)|**[link](https://github.com/sail-sg/closer-look-llm-unlearning)**|
|**2024-10-10**|**What Makes Large Language Models Reason in (Multi-Turn) Code Generation?**|Kunhao Zheng et.al.|[2410.08105](http://arxiv.org/abs/2410.08105)|null|
|**2024-10-10**|**Multi-Agent Collaborative Data Selection for Efficient LLM Pretraining**|Tianyi Bai et.al.|[2410.08102](http://arxiv.org/abs/2410.08102)|**[link](https://github.com/beccabai/multi-agent-data-selection)**|
|**2024-10-09**|**Astute RAG: Overcoming Imperfect Retrieval Augmentation and Knowledge Conflicts for Large Language Models**|Fei Wang et.al.|[2410.07176](http://arxiv.org/abs/2410.07176)|null|
|**2024-10-09**|**Do better language models have crisper vision?**|Jona Ruthardt et.al.|[2410.07173](http://arxiv.org/abs/2410.07173)|null|
|**2024-10-09**|**Deciphering Cross-Modal Alignment in Large Vision-Language Models with Modality Integration Rate**|Qidong Huang et.al.|[2410.07167](http://arxiv.org/abs/2410.07167)|**[link](https://github.com/shikiw/modality-integration-rate)**|
|**2024-10-09**|**Embodied Agent Interface: Benchmarking LLMs for Embodied Decision Making**|Manling Li et.al.|[2410.07166](http://arxiv.org/abs/2410.07166)|**[link](https://github.com/embodied-agent-interface/embodied-agent-interface)**|
|**2024-10-09**|**Simplicity Prevails: Rethinking Negative Preference Optimization for LLM Unlearning**|Chongyu Fan et.al.|[2410.07163](http://arxiv.org/abs/2410.07163)|**[link](https://github.com/OPTML-Group/Unlearn-Simple)**|
|**2024-10-09**|**Mental Disorders Detection in the Era of Large Language Models**|Gleb Kuzmin et.al.|[2410.07129](http://arxiv.org/abs/2410.07129)|null|
|**2024-10-09**|**I Want to Break Free! Anti-Social Behavior and Persuasion Ability of LLMs in Multi-Agent Settings with Social Hierarchy**|Gian Maria Campedelli et.al.|[2410.07109](http://arxiv.org/abs/2410.07109)|**[link](https://github.com/mobs-fbk/llm_interaction_simulator)**|
|**2024-10-09**|**Unleashing Multi-Hop Reasoning Potential in Large Language Models through Repetition of Misordered Context**|Sangwon Yu et.al.|[2410.07103](http://arxiv.org/abs/2410.07103)|null|
|**2024-10-09**|**Stanceformer: Target-Aware Transformer for Stance Detection**|Krishna Garg et.al.|[2410.07083](http://arxiv.org/abs/2410.07083)|null|
|**2024-10-09**|**Let's Ask GNN: Empowering Large Language Model for Graph In-Context Learning**|Zhengyu Hu et.al.|[2410.07074](http://arxiv.org/abs/2410.07074)|null|
|**2024-10-07**|**Data Advisor: Dynamic Data Curation for Safety Alignment of Large Language Models**|Fei Wang et.al.|[2410.05269](http://arxiv.org/abs/2410.05269)|null|
|**2024-10-07**|**PrefixQuant: Static Quantization Beats Dynamic through Prefixed Outliers in LLMs**|Mengzhao Chen et.al.|[2410.05265](http://arxiv.org/abs/2410.05265)|**[link](https://github.com/chenmnz/prefixquant)**|
|**2024-10-07**|**TurtleBench: Evaluating Top Language Models via Real-World Yes/No Puzzles**|Qingchen Yu et.al.|[2410.05262](http://arxiv.org/abs/2410.05262)|**[link](https://github.com/mazzzystar/TurtleBench)**|
|**2024-10-07**|**GLEE: A Unified Framework and Benchmark for Language-based Economic Environments**|Eilam Shapira et.al.|[2410.05254](http://arxiv.org/abs/2410.05254)|**[link](https://github.com/eilamshapira/GLEE)**|
|**2024-10-07**|**Causal Micro-Narratives**|Mourad Heddaya et.al.|[2410.05252](http://arxiv.org/abs/2410.05252)|null|
|**2024-10-07**|**SFTMix: Elevating Language Model Instruction Tuning with Mixup Recipe**|Yuxin Xiao et.al.|[2410.05248](http://arxiv.org/abs/2410.05248)|null|
|**2024-10-07**|**GSM-Symbolic: Understanding the Limitations of Mathematical Reasoning in Large Language Models**|Iman Mirzadeh et.al.|[2410.05229](http://arxiv.org/abs/2410.05229)|null|
|**2024-10-07**|**Cookbook: A framework for improving LLM generative abilities via programmatic data generating templates**|Avanika Narayan et.al.|[2410.05224](http://arxiv.org/abs/2410.05224)|null|
|**2024-10-07**|**Precise Model Benchmarking with Only a Few Observations**|Riccardo Fogliato et.al.|[2410.05222](http://arxiv.org/abs/2410.05222)|null|
|**2024-10-07**|**Density estimation with LLMs: a geometric investigation of in-context learning trajectories**|Toni J. B. Liu et.al.|[2410.05218](http://arxiv.org/abs/2410.05218)|null|
|**2024-10-04**|**Enhance Reasoning by Learning from Mistakes: Peer-Review Knowledge Distillation from Multiple Large Language Models**|Zhuochun Li et.al.|[2410.03663](http://arxiv.org/abs/2410.03663)|null|
|**2024-10-04**|**RAFT: Realistic Attacks to Fool Text Detectors**|James Wang et.al.|[2410.03658](http://arxiv.org/abs/2410.03658)|**[link](https://github.com/jameslwang/raft)**|
|**2024-10-04**|**Aligning LLMs with Individual Preferences via Interaction**|Shujin Wu et.al.|[2410.03642](http://arxiv.org/abs/2410.03642)|**[link](https://github.com/shujinwu-0814/aloe)**|
|**2024-10-04**|**Large Language Model Performance Benchmarking on Mobile Platforms: A Thorough Evaluation**|Jie Xiao et.al.|[2410.03613](http://arxiv.org/abs/2410.03613)|null|
|**2024-10-04**|**TICKing All the Boxes: Generated Checklists Improve LLM Evaluation and Generation**|Jonathan Cook et.al.|[2410.03608](http://arxiv.org/abs/2410.03608)|null|
|**2024-10-04**|**Efficiently Identifying Watermarked Segments in Mixed-Source Texts**|Xuandong Zhao et.al.|[2410.03600](http://arxiv.org/abs/2410.03600)|null|
|**2024-10-04**|**Towards Linguistically-Aware and Language-Independent Tokenization for Large Language Models (LLMs)**|Abrar Rahman et.al.|[2410.03568](http://arxiv.org/abs/2410.03568)|null|
|**2024-10-04**|**Structure-Enhanced Protein Instruction Tuning: Towards General-Purpose Protein Understanding**|Wei Wu et.al.|[2410.03553](http://arxiv.org/abs/2410.03553)|null|
|**2024-10-04**|**Steering Large Language Models between Code Execution and Textual Reasoning**|Yongchao Chen et.al.|[2410.03524](http://arxiv.org/abs/2410.03524)|null|
|**2024-10-04**|**A Probabilistic Perspective on Unlearning and Alignment for Large Language Models**|Yan Scholten et.al.|[2410.03523](http://arxiv.org/abs/2410.03523)|null|
|**2024-10-03**|**Loong: Generating Minute-level Long Videos with Autoregressive Language Models**|Yuqing Wang et.al.|[2410.02757](http://arxiv.org/abs/2410.02757)|null|
|**2024-10-03**|**Training Language Models on Synthetic Edit Sequences Improves Code Synthesis**|Ulyana Piterbarg et.al.|[2410.02749](http://arxiv.org/abs/2410.02749)|**[link](https://github.com/upiterbarg/lintseq)**|
|**2024-10-03**|**CriSPO: Multi-Aspect Critique-Suggestion-guided Automatic Prompt Optimization for Text Generation**|Han He et.al.|[2410.02748](http://arxiv.org/abs/2410.02748)|null|
|**2024-10-03**|**MA-RLHF: Reinforcement Learning from Human Feedback with Macro Actions**|Yekun Chai et.al.|[2410.02743](http://arxiv.org/abs/2410.02743)|null|
|**2024-10-03**|**Grounding Large Language Models In Embodied Environment With Imperfect World Models**|Haolan Liu et.al.|[2410.02742](http://arxiv.org/abs/2410.02742)|null|
|**2024-10-03**|**Salient Information Prompting to Steer Content in Prompt-based Abstractive Summarization**|Lei Xu et.al.|[2410.02741](http://arxiv.org/abs/2410.02741)|null|
|**2024-10-03**|**Adaptive Inference-Time Compute: LLMs Can Predict if They Can Do Better, Even Mid-Generation**|Rohin Manvi et.al.|[2410.02725](http://arxiv.org/abs/2410.02725)|null|
|**2024-10-03**|**Large Language Models as Markov Chains**|Oussama Zekri et.al.|[2410.02724](http://arxiv.org/abs/2410.02724)|null|
|**2024-10-03**|**Domain-Specific Retrieval-Augmented Generation Using Vector Stores, Knowledge Graphs, and Tensor Factorization**|Ryan C. Barron et.al.|[2410.02721](http://arxiv.org/abs/2410.02721)|null|
|**2024-10-03**|**LLMs Know More Than They Show: On the Intrinsic Representation of LLM Hallucinations**|Hadas Orgad et.al.|[2410.02707](http://arxiv.org/abs/2410.02707)|**[link](https://github.com/technion-cs-nlp/llmsknow)**|
|**2024-10-02**|**Locret: Enhancing Eviction in Long-Context LLM Inference with Trained Retaining Heads**|Yuxiang Huang et.al.|[2410.01805](http://arxiv.org/abs/2410.01805)|**[link](https://github.com/huangyuxiang03/Locret)**|
|**2024-10-02**|**When a language model is optimized for reasoning, does it still show embers of autoregression? An analysis of OpenAI o1**|R. Thomas McCoy et.al.|[2410.01792](http://arxiv.org/abs/2410.01792)|null|
|**2024-10-02**|**OmniGenBench: Automating Large-scale in-silico Benchmarking for Genomic Foundation Models**|Heng Yang et.al.|[2410.01784](http://arxiv.org/abs/2410.01784)|**[link](https://github.com/yangheng95/OmniGenomeBench)**|
|**2024-10-02**|**Open-RAG: Enhanced Retrieval-Augmented Reasoning with Open-Source Large Language Models**|Shayekh Bin Islam et.al.|[2410.01782](http://arxiv.org/abs/2410.01782)|**[link](https://github.com/ShayekhBinIslam/openrag)**|
|**2024-10-02**|**Quantifying Generalization Complexity for Large Language Models**|Zhenting Qi et.al.|[2410.01769](http://arxiv.org/abs/2410.01769)|**[link](https://github.com/zhentingqi/scylla)**|
|**2024-10-02**|**Visual Perception in Text Strings**|Qi Jia et.al.|[2410.01733](http://arxiv.org/abs/2410.01733)|**[link](https://github.com/JiaQiSJTU/VisionInText)**|
|**2024-10-02**|**Automated Knowledge Concept Annotation and Question Representation Learning for Knowledge Tracing**|Yilmazcan Ozyurt et.al.|[2410.01727](http://arxiv.org/abs/2410.01727)|**[link](https://github.com/oezyurty/kcqrl)**|
|**2024-10-02**|**Auto-Demo Prompting: Leveraging Generated Outputs as Demonstrations for Enhanced Batch Prompting**|Longyu Feng et.al.|[2410.01724](http://arxiv.org/abs/2410.01724)|null|
|**2024-10-02**|**Towards a Theoretical Understanding of Synthetic Data in LLM Post-Training: A Reverse-Bottleneck Perspective**|Zeyu Gan et.al.|[2410.01720](http://arxiv.org/abs/2410.01720)|**[link](https://github.com/zygan1999/towards-a-theoretical-understanding-of-synthetic-data-in-llm-post-training)**|
|**2024-10-02**|**Interpretable Contrastive Monte Carlo Tree Search Reasoning**|Zitian Gao et.al.|[2410.01707](http://arxiv.org/abs/2410.01707)|**[link](https://github.com/zitian-gao/sc-mcts)**|
|**2024-09-30**|**Propose, Assess, Search: Harnessing LLMs for Goal-Oriented Planning in Instructional Videos**|Md Mohaiminul Islam et.al.|[2409.20557](http://arxiv.org/abs/2409.20557)|null|
|**2024-09-30**|**LLM Hallucinations in Practical Code Generation: Phenomena, Mechanism, and Mitigation**|Ziyao Zhang et.al.|[2409.20550](http://arxiv.org/abs/2409.20550)|null|
|**2024-09-30**|**Robi Butler: Remote Multimodal Interactions with Household Robot Assistant**|Anxing Xiao et.al.|[2409.20548](http://arxiv.org/abs/2409.20548)|null|
|**2024-09-30**|**Uncertainty-Informed Screening for Safer Solvents Used in the Synthesis of Perovskite via Language Models**|Arpan Mukherjee et.al.|[2409.20512](http://arxiv.org/abs/2409.20512)|null|
|**2024-09-30**|**COLLAGE: Collaborative Human-Agent Interaction Generation using Hierarchical Latent Diffusion and Language Models**|Divyanshu Daiya et.al.|[2409.20502](http://arxiv.org/abs/2409.20502)|null|
|**2024-10-01**|**Instance-adaptive Zero-shot Chain-of-Thought Prompting**|Xiaosong Yuan et.al.|[2409.20441](http://arxiv.org/abs/2409.20441)|null|
|**2024-09-30**|**Wait, but Tylenol is Acetaminophen... Investigating and Improving Language Models' Ability to Resist Requests for Misinformation**|Shan Chen et.al.|[2409.20385](http://arxiv.org/abs/2409.20385)|null|
|**2024-09-30**|**The Perfect Blend: Redefining RLHF with Mixture of Judges**|Tengyu Xu et.al.|[2409.20370](http://arxiv.org/abs/2409.20370)|null|
|**2024-09-30**|**VideoINSTA: Zero-shot Long Video Understanding via Informative Spatial-Temporal Reasoning with LLMs**|Ruotong Liao et.al.|[2409.20365](http://arxiv.org/abs/2409.20365)|null|
|**2024-09-30**|**Efficient Driving Behavior Narration and Reasoning on Edge Device Using Large Language Models**|Yizhou Huang et.al.|[2409.20364](http://arxiv.org/abs/2409.20364)|null|
|**2024-09-27**|**LML: Language Model Learning a Dataset for Data-Augmented Prediction**|Praneeth Vadlapati et.al.|[2409.18957](http://arxiv.org/abs/2409.18957)|**[link](https://github.com/pro-genai/lml-dap)**|
|**2024-09-27**|**From Seconds to Hours: Reviewing MultiModal Large Language Models on Comprehensive Long Video Understanding**|Heqing Zou et.al.|[2409.18938](http://arxiv.org/abs/2409.18938)|null|
|**2024-09-27**|**AIPatient: Simulating Patients with EHRs and LLM Powered Agentic Workflow**|Huizi Yu et.al.|[2409.18924](http://arxiv.org/abs/2409.18924)|null|
|**2024-09-27**|**Soft Measures for Extracting Causal Collective Intelligence**|Maryam Berijanian et.al.|[2409.18911](http://arxiv.org/abs/2409.18911)|**[link](https://github.com/kuldeep7688/soft-measures-causal-intelligence)**|
|**2024-09-27**|**IDGen: Item Discrimination Induced Prompt Generation for LLM Evaluation**|Fan Lin et.al.|[2409.18892](http://arxiv.org/abs/2409.18892)|**[link](https://github.com/DUTlf/IDGen)**|
|**2024-09-27**|**Mitigating Selection Bias with Node Pruning and Auxiliary Options**|Hyeong Kyu Choi et.al.|[2409.18857](http://arxiv.org/abs/2409.18857)|null|
|**2024-09-27**|**LLMs4Synthesis: Leveraging Large Language Models for Scientific Synthesis**|Hamed Babaei Giglou et.al.|[2409.18812](http://arxiv.org/abs/2409.18812)|**[link](https://github.com/HamedBabaei/LLMs4Synthesis)**|
|**2024-09-27**|**Open-Nav: Exploring Zero-Shot Vision-and-Language Navigation in Continuous Environment with Open-Source LLMs**|Yanyuan Qiao et.al.|[2409.18794](http://arxiv.org/abs/2409.18794)|null|
|**2024-09-27**|**A Survey on the Honesty of Large Language Models**|Siheng Li et.al.|[2409.18786](http://arxiv.org/abs/2409.18786)|**[link](https://github.com/sihengli99/llm-honesty-survey)**|
|**2024-09-27**|**"Why" Has the Least Side Effect on Model Editing**|Tsung-Hsuan Pan et.al.|[2409.18679](http://arxiv.org/abs/2409.18679)|null|
|**2024-09-26**|**EgoLM: Multi-Modal Language Model of Egocentric Motions**|Fangzhou Hong et.al.|[2409.18127](http://arxiv.org/abs/2409.18127)|null|
|**2024-09-26**|**Infering Alt-text For UI Icons With Large Language Models During App Development**|Sabrina Haque et.al.|[2409.18060](http://arxiv.org/abs/2409.18060)|null|
|**2024-09-26**|**DualAD: Dual-Layer Planning for Reasoning in Autonomous Driving**|Dingrui Wang et.al.|[2409.18053](http://arxiv.org/abs/2409.18053)|null|
|**2024-09-26**|**Compositional Hardness of Code in Large Language Models -- A Probabilistic Perspective**|Yotam Wolf et.al.|[2409.18028](http://arxiv.org/abs/2409.18028)|null|
|**2024-09-26**|**Role-RL: Online Long-Context Processing with Role Reinforcement Learning for Distinct LLMs in Their Optimal Roles**|Lewei He et.al.|[2409.18014](http://arxiv.org/abs/2409.18014)|null|
|**2024-09-26**|**Multilingual Evaluation of Long Context Retrieval and Reasoning**|Ameeta Agrawal et.al.|[2409.18006](http://arxiv.org/abs/2409.18006)|null|
|**2024-09-26**|**Enhancing Tourism Recommender Systems for Sustainable City Trips Using Retrieval-Augmented Generation**|Ashmi Banerjee et.al.|[2409.18003](http://arxiv.org/abs/2409.18003)|null|
|**2024-09-26**|**Extracting Affect Aggregates from Longitudinal Social Media Data with Temporal Adapters for Large Language Models**|Georg Ahnert et.al.|[2409.17990](http://arxiv.org/abs/2409.17990)|**[link](https://github.com/dess-mannheim/temporal-adapters)**|
|**2024-09-26**|**LLM4Brain: Training a Large Language Model for Brain Video Understanding**|Ruizhe Zheng et.al.|[2409.17987](http://arxiv.org/abs/2409.17987)|null|
|**2024-09-26**|**BEATS: Optimizing LLM Mathematical Capabilities with BackVerify and Adaptive Disambiguate based Efficient Tree Search**|Linzhuang Sun et.al.|[2409.17972](http://arxiv.org/abs/2409.17972)|**[link](https://github.com/Aurora-slz/BEATS)**|
|**2024-09-18**|**To CoT or not to CoT? Chain-of-thought helps mainly on math and symbolic reasoning**|Zayne Sprague et.al.|[2409.12183](http://arxiv.org/abs/2409.12183)|null|
|**2024-09-18**|**Finetuning Language Models to Emit Linguistic Expressions of Uncertainty**|Arslan Chaudhry et.al.|[2409.12180](http://arxiv.org/abs/2409.12180)|null|
|**2024-09-18**|**Decoding Style: Efficient Fine-Tuning of LLMs for Image-Guided Outfit Recommendation with Preference**|Najmeh Forouzandehmehr et.al.|[2409.12150](http://arxiv.org/abs/2409.12150)|null|
|**2024-09-18**|**MAgICoRe: Multi-Agent, Iterative, Coarse-to-Fine Refinement for Reasoning**|Justin Chih-Yao Chen et.al.|[2409.12147](http://arxiv.org/abs/2409.12147)|**[link](https://github.com/dinobby/magicore)**|
|**2024-09-18**|**MoRAG -- Multi-Fusion Retrieval Augmented Generation for Human Motion**|Kalakonda Sai Shashank et.al.|[2409.12140](http://arxiv.org/abs/2409.12140)|null|
|**2024-09-18**|**Low Frame-rate Speech Codec: a Codec Designed for Fast High-quality Speech LLM Training and Inference**|Edresson Casanova et.al.|[2409.12117](http://arxiv.org/abs/2409.12117)|null|
|**2024-09-18**|**Measuring Human and AI Values based on Generative Psychometrics with Large Language Models**|Haoran Ye et.al.|[2409.12106](http://arxiv.org/abs/2409.12106)|**[link](https://github.com/value4ai/gpv)**|
|**2024-09-19**|**Using Large Language Models to Generate Clinical Trial Tables and Figures**|Yumeng Yang et.al.|[2409.12046](http://arxiv.org/abs/2409.12046)|null|
|**2024-09-18**|**ChefFusion: Multimodal Foundation Model Integrating Recipe and Food Image Generation**|Peiyu Li et.al.|[2409.12010](http://arxiv.org/abs/2409.12010)|**[link](https://github.com/peiyu-georgia-li/cheffusion-multimodal-foundation-model-integrating-recipe-and-food-image-generation)**|
|**2024-09-18**|**Sampling Latent Material-Property Information From LLM-Derived Embedding Representations**|Luke P. J. Gilligan et.al.|[2409.11971](http://arxiv.org/abs/2409.11971)|null|
|**2024-09-17**|**NVLM: Open Frontier-Class Multimodal LLMs**|Wenliang Dai et.al.|[2409.11402](http://arxiv.org/abs/2409.11402)|null|
|**2024-09-17**|**Says Who? Effective Zero-Shot Annotation of Focalization**|Rebecca M. M. Hicke et.al.|[2409.11390](http://arxiv.org/abs/2409.11390)|null|
|**2024-09-17**|**Multi-OCT-SelfNet: Integrating Self-Supervised Learning with Multi-Source Data Fusion for Enhanced Multi-Class Retinal Disease Classification**|Fatema-E- Jannat et.al.|[2409.11375](http://arxiv.org/abs/2409.11375)|null|
|**2024-09-17**|**CoCA: Regaining Safety-awareness of Multimodal Large Language Models with Constitutional Calibration**|Jiahui Gao et.al.|[2409.11365](http://arxiv.org/abs/2409.11365)|null|
|**2024-09-17**|**AI Suggestions Homogenize Writing Toward Western Styles and Diminish Cultural Nuances**|Dhruv Agarwal et.al.|[2409.11360](http://arxiv.org/abs/2409.11360)|null|
|**2024-09-17**|**THaMES: An End-to-End Tool for Hallucination Mitigation and Evaluation in Large Language Models**|Mengfei Liang et.al.|[2409.11353](http://arxiv.org/abs/2409.11353)|null|
|**2024-09-17**|**Leveraging Distillation Techniques for Document Understanding: A Case Study with FLAN-T5**|Marcel Lamott et.al.|[2409.11282](http://arxiv.org/abs/2409.11282)|null|
|**2024-09-17**|**P-RAG: Progressive Retrieval Augmented Generation For Planning on Embodied Everyday Task**|Weiye Xu et.al.|[2409.11279](http://arxiv.org/abs/2409.11279)|null|
|**2024-09-17**|**Hackphyr: A Local Fine-Tuned LLM Agent for Network Security Environments**|Maria Rigaki et.al.|[2409.11276](http://arxiv.org/abs/2409.11276)|null|
|**2024-09-17**|**Task Arithmetic for Language Expansion in Speech Translation**|Yao-Fei Cheng et.al.|[2409.11274](http://arxiv.org/abs/2409.11274)|null|
|**2024-09-16**|**RetrievalAttention: Accelerating Long-Context LLM Inference via Vector Retrieval**|Di Liu et.al.|[2409.10516](http://arxiv.org/abs/2409.10516)|**[link](https://github.com/jzbjyb/reatt)**|
|**2024-09-16**|**Context-aware Code Segmentation for C-to-Rust Translation using Large Language Models**|Momoko Shiraishi et.al.|[2409.10506](http://arxiv.org/abs/2409.10506)|null|
|**2024-09-16**|**DILA: Dictionary Label Attention for Mechanistic Interpretability in High-dimensional Multi-label Medical Coding Prediction**|John Wu et.al.|[2409.10504](http://arxiv.org/abs/2409.10504)|null|
|**2024-09-16**|**Causal Language Modeling Can Elicit Search and Reasoning Capabilities on Logic Puzzles**|Kulin Shah et.al.|[2409.10502](http://arxiv.org/abs/2409.10502)|**[link](https://github.com/kulinshah98/llm-reasoning-logic-puzzles)**|
|**2024-09-16**|**Code Vulnerability Detection: A Comparative Analysis of Emerging Large Language Models**|Shaznin Sultana et.al.|[2409.10490](http://arxiv.org/abs/2409.10490)|null|
|**2024-09-16**|**XLM for Autonomous Driving Systems: A Comprehensive Review**|Sonda Fourati et.al.|[2409.10484](http://arxiv.org/abs/2409.10484)|null|
|**2024-09-16**|**LLM as BT-Planner: Leveraging LLMs for Behavior Tree Generation in Robot Task Planning**|Jicong Ao et.al.|[2409.10444](http://arxiv.org/abs/2409.10444)|null|
|**2024-09-17**|**Learnings from a Large-Scale Deployment of an LLM-Powered Expert-in-the-Loop Healthcare Chatbot**|Bhuvan Sachdeva et.al.|[2409.10354](http://arxiv.org/abs/2409.10354)|null|
|**2024-09-16**|**The 20 questions game to distinguish large language models**|Gurvan Richardeau et.al.|[2409.10338](http://arxiv.org/abs/2409.10338)|null|
|**2024-09-16**|**ReflectDiffu: Reflect between Emotion-intent Contagion and Mimicry for Empathetic Response Generation via a RL-Diffusion Framework**|Jiahao Yuan et.al.|[2409.10289](http://arxiv.org/abs/2409.10289)|**[link](https://github.com/Jiahao-Yuan/ReflectDiffu)**|
|**2024-09-13**|**Agents in Software Engineering: Survey, Landscape, and Vision**|Yanxian Huang et.al.|[2409.09030](http://arxiv.org/abs/2409.09030)|**[link](https://github.com/deepsoftwareanalytics/awesome-agent4se)**|
|**2024-09-13**|**Contri(e)ve: Context + Retrieve for Scholarly Question Answering**|Kanchan Shivashankar et.al.|[2409.09010](http://arxiv.org/abs/2409.09010)|null|
|**2024-09-13**|**Emerging Reliance Behaviors in Human-AI Text Generation: Hallucinations, Data Quality Assessment, and Cognitive Forcing Functions**|Zahra Ashktorab et.al.|[2409.08937](http://arxiv.org/abs/2409.08937)|null|
|**2024-09-13**|**LLM-based Weak Supervision Framework for Query Intent Classification in Video Search**|Farnoosh Javadi et.al.|[2409.08931](http://arxiv.org/abs/2409.08931)|null|
|**2024-09-13**|**AnyBipe: An End-to-End Framework for Training and Deploying Bipedal Robots Guided by Large Language Models**|Yifei Yao et.al.|[2409.08904](http://arxiv.org/abs/2409.08904)|**[link](https://github.com/sjtu-mvasl-robotics/AnyBipe)**|
|**2024-09-13**|**Exploring Graph Structure Comprehension Ability of Multimodal Large Language Models: Case Studies**|Zhiqiang Zhong et.al.|[2409.08864](http://arxiv.org/abs/2409.08864)|null|
|**2024-09-13**|**FP-VEC: Fingerprinting Large Language Models via Efficient Vector Addition**|Zhenhua Xu et.al.|[2409.08846](http://arxiv.org/abs/2409.08846)|null|
|**2024-09-13**|**AIPO: Improving Training Objective for Iterative Preference Optimization**|Yaojie Shen et.al.|[2409.08845](http://arxiv.org/abs/2409.08845)|**[link](https://github.com/bytedance/aipo)**|
|**2024-09-13**|**A RAG Approach for Generating Competency Questions in Ontology Engineering**|Xueli Pan et.al.|[2409.08820](http://arxiv.org/abs/2409.08820)|null|
|**2024-09-13**|**Your Weak LLM is Secretly a Strong Teacher for Alignment**|Leitian Tao et.al.|[2409.08813](http://arxiv.org/abs/2409.08813)|null|
|**2024-09-12**|**Windows Agent Arena: Evaluating Multi-Modal OS Agents at Scale**|Rogerio Bonatti et.al.|[2409.08264](http://arxiv.org/abs/2409.08264)|**[link](https://github.com/microsoft/windowsagentarena)**|
|**2024-09-12**|**OmniQuery: Contextually Augmenting Captured Multimodal Memory to Enable Personal Question Answering**|Jiahao Nick Li et.al.|[2409.08250](http://arxiv.org/abs/2409.08250)|null|
|**2024-09-12**|**LLM Honeypot: Leveraging Large Language Models as Advanced Interactive Honeypot Systems**|Hakan T. Otal et.al.|[2409.08234](http://arxiv.org/abs/2409.08234)|**[link](https://github.com/ai-in-complex-systems-lab/llm-honeypot)**|
|**2024-09-12**|**Fine-tuning Large Language Models for Entity Matching**|Aaron Steiner et.al.|[2409.08185](http://arxiv.org/abs/2409.08185)|**[link](https://github.com/wbsg-uni-mannheim/tailormatch)**|
|**2024-09-12**|**Faster Speech-LLaMA Inference with Multi-token Prediction**|Desh Raj et.al.|[2409.08148](http://arxiv.org/abs/2409.08148)|null|
|**2024-09-12**|**The CLC-UKET Dataset: Benchmarking Case Outcome Prediction for the UK Employment Tribunal**|Huiyuan Xie et.al.|[2409.08098](http://arxiv.org/abs/2409.08098)|null|
|**2024-09-12**|**Securing Large Language Models: Addressing Bias, Misinformation, and Prompt Attacks**|Benji Peng et.al.|[2409.08087](http://arxiv.org/abs/2409.08087)|null|
|**2024-09-12**|**TravelAgent: An AI Assistant for Personalized Travel Planning**|Aili Chen et.al.|[2409.08069](http://arxiv.org/abs/2409.08069)|null|
|**2024-09-12**|**An Evaluation Framework for Attributed Information Retrieval using Large Language Models**|Hanane Djeddal et.al.|[2409.08014](http://arxiv.org/abs/2409.08014)|**[link](https://github.com/hanane-djeddal/attributed-ir)**|
|**2024-09-12**|**WirelessAgent: Large Language Model Agents for Intelligent Wireless Networks**|Jingwen Tong et.al.|[2409.07964](http://arxiv.org/abs/2409.07964)|**[link](https://github.com/weiiguo/wireless-agent)**|
|**2024-09-11**|**"My Grade is Wrong!": A Contestable AI Framework for Interactive Feedback in Evaluating Student Essays**|Shengxin Hong et.al.|[2409.07453](http://arxiv.org/abs/2409.07453)|null|
|**2024-09-11**|**SUPER: Evaluating Agents on Setting Up and Executing Tasks from Research Repositories**|Ben Bogin et.al.|[2409.07440](http://arxiv.org/abs/2409.07440)|**[link](https://github.com/allenai/super-benchmark)**|
|**2024-09-11**|**CLNX: Bridging Code and Natural Language for C/C++ Vulnerability-Contributing Commits Identification**|Zeqing Qin et.al.|[2409.07407](http://arxiv.org/abs/2409.07407)|null|
|**2024-09-11**|**AdaCAD: Adaptively Decoding to Balance Conflicts between Contextual and Parametric Knowledge**|Han Wang et.al.|[2409.07394](http://arxiv.org/abs/2409.07394)|**[link](https://github.com/hannight/adacad)**|
|**2024-09-11**|**Demo: SGCode: A Flexible Prompt-Optimizing System for Secure Generation of Code**|Khiem Ton et.al.|[2409.07368](http://arxiv.org/abs/2409.07368)|null|
|**2024-09-11**|**Think Together and Work Better: Combining Humans' and LLMs' Think-Aloud Outcomes for Effective Text Evaluation**|SeongYeub Chu et.al.|[2409.07355](http://arxiv.org/abs/2409.07355)|**[link](https://github.com/BBeeChu/InteractEval)**|
|**2024-09-11**|**MEDIC: Towards a Comprehensive Framework for Evaluating LLMs in Clinical Applications**|Praveen K Kanithi et.al.|[2409.07314](http://arxiv.org/abs/2409.07314)|null|
|**2024-09-11**|**STORE: Streamlining Semantic Tokenization and Generative Recommendation with A Single LLM**|Qijiong Liu et.al.|[2409.07276](http://arxiv.org/abs/2409.07276)|null|
|**2024-09-11**|**MiniDrive: More Efficient Vision-Language Models with Multi-Level 2D Features as Text Tokens for Autonomous Driving**|Enming Zhang et.al.|[2409.07267](http://arxiv.org/abs/2409.07267)|**[link](https://github.com/emzucas/minidrive)**|
|**2024-09-11**|**PiTe: Pixel-Temporal Alignment for Large Video-Language Model**|Yang Liu et.al.|[2409.07239](http://arxiv.org/abs/2409.07239)|**[link](https://github.com/yliu-cs/pite)**|
|**2024-09-10**|**E2LLM: Encoder Elongated Large Language Models for Long-Context Understanding and Reasoning**|Zihan Liao et.al.|[2409.06679](http://arxiv.org/abs/2409.06679)|null|
|**2024-09-10**|**LLaMA-Omni: Seamless Speech Interaction with Large Language Models**|Qingkai Fang et.al.|[2409.06666](http://arxiv.org/abs/2409.06666)|**[link](https://github.com/ictnlp/llama-omni)**|
|**2024-09-10**|**Human Perception of LLM-generated Text Content in Social Media Environments**|Kristina Radivojevic et.al.|[2409.06653](http://arxiv.org/abs/2409.06653)|null|
|**2024-09-10**|**Optimal Workload Placement on Multi-Instance GPUs**|Bekir Turkkan et.al.|[2409.06646](http://arxiv.org/abs/2409.06646)|null|
|**2024-09-10**|**MoWE-Audio: Multitask AudioLLMs with Mixture of Weak Encoders**|Wenyu Zhang et.al.|[2409.06635](http://arxiv.org/abs/2409.06635)|null|
|**2024-09-10**|**A Practice of Post-Training on Llama-3 70B with Optimal Selection of Additional Language Mixture Ratio**|Ningyuan Xi et.al.|[2409.06624](http://arxiv.org/abs/2409.06624)|null|
|**2024-09-10**|**Alleviating Hallucinations in Large Language Models with Scepticism Modeling**|Yetao Wu et.al.|[2409.06601](http://arxiv.org/abs/2409.06601)|null|
|**2024-09-10**|**GroUSE: A Benchmark to Evaluate Evaluators in Grounded Question Answering**|Sacha Muller et.al.|[2409.06595](http://arxiv.org/abs/2409.06595)|**[link](https://github.com/illuin-tech/grouse)**|
|**2024-09-10**|**MAPS: Energy-Reliability Tradeoff Management in Autonomous Vehicles Through LLMs Penetrated Science**|Mahdieh Aliazam et.al.|[2409.06558](http://arxiv.org/abs/2409.06558)|null|
|**2024-09-10**|**Questioning Internal Knowledge Structure of Large Language Models Through the Lens of the Olympic Games**|Juhwan Choi et.al.|[2409.06518](http://arxiv.org/abs/2409.06518)|**[link](https://github.com/c-juhwan/olympics_analysis)**|
|**2024-09-09**|**Are Large Language Models a Threat to Programming Platforms? An Exploratory Study**|Md Mustakim Billah et.al.|[2409.05824](http://arxiv.org/abs/2409.05824)|null|
|**2024-09-09**|**Benchmarking Chinese Knowledge Rectification in Large Language Models**|Tianhe Lu et.al.|[2409.05806](http://arxiv.org/abs/2409.05806)|**[link](https://github.com/zjunlp/easyedit)**|
|**2024-09-09**|**Model Input Verification of Large Scale Simulations**|Rumyana Neykova et.al.|[2409.05768](http://arxiv.org/abs/2409.05768)|null|
|**2024-09-09**|**A Novel Idea Generation Tool using a Structured Conversational AI (CAI) System**|B. Sankar et.al.|[2409.05747](http://arxiv.org/abs/2409.05747)|null|
|**2024-09-09**|**A System and Benchmark for LLM-based Q\&A on Heterogeneous Data**|Achille Fokoue et.al.|[2409.05735](http://arxiv.org/abs/2409.05735)|null|
|**2024-09-09**|**Towards Democratizing Multilingual Large Language Models For Medicine Through A Two-Stage Instruction Fine-tuning Approach**|Meng Zhou et.al.|[2409.05732](http://arxiv.org/abs/2409.05732)|null|
|**2024-09-09**|**The Influence of Task and Group Disparities over Users' Attitudes Toward Using Large Language Models for Psychotherapy**|Qihang He et.al.|[2409.05703](http://arxiv.org/abs/2409.05703)|null|
|**2024-09-10**|**MemoRAG: Moving towards Next-Gen RAG Via Memory-Inspired Knowledge Discovery**|Hongjin Qian et.al.|[2409.05591](http://arxiv.org/abs/2409.05591)|**[link](https://github.com/qhjqhj00/memorag)**|
|**2024-09-09**|**CauseJudger: Identifying the Cause with LLMs for Abductive Logical Reasoning**|Jinwei He et.al.|[2409.05559](http://arxiv.org/abs/2409.05559)|null|
|**2024-09-09**|**SciAgents: Automating scientific discovery through multi-agent intelligent graph reasoning**|Alireza Ghafarollahi et.al.|[2409.05556](http://arxiv.org/abs/2409.05556)|**[link](https://github.com/lamm-mit/SciAgentsDiscovery)**|
|**2024-09-06**|**RLPF: Reinforcement Learning from Prediction Feedback for User Summarization with LLMs**|Jiaxing Wu et.al.|[2409.04421](http://arxiv.org/abs/2409.04421)|null|
|**2024-09-06**|**Learning vs Retrieval: The Role of In-Context Examples in Regression with LLMs**|Aliakbar Nafar et.al.|[2409.04318](http://arxiv.org/abs/2409.04318)|**[link](https://github.com/HLR/LvsR-LLM)**|
|**2024-09-06**|**Advancing Automated Knowledge Transfer in Evolutionary Multitasking via Large Language Models**|Yuxiao Huang et.al.|[2409.04270](http://arxiv.org/abs/2409.04270)|null|
|**2024-09-06**|**Combining LLMs and Knowledge Graphs to Reduce Hallucinations in Question Answering**|Larissa Pusch et.al.|[2409.04181](http://arxiv.org/abs/2409.04181)|null|
|**2024-09-06**|**From Calculation to Adjudication: Examining LLM judges on Mathematical Reasoning Tasks**|Andreas Stephan et.al.|[2409.04168](http://arxiv.org/abs/2409.04168)|null|
|**2024-09-06**|**Can OpenSource beat ChatGPT? -- A Comparative Study of Large Language Models for Text-to-Code Generation**|Luis Mayer et.al.|[2409.04164](http://arxiv.org/abs/2409.04164)|null|
|**2024-09-06**|**Multi-Programming Language Ensemble for Code Generation in Large Language Model**|Tengfei Xue et.al.|[2409.04114](http://arxiv.org/abs/2409.04114)|**[link](https://github.com/ninjatech-ai/mple)**|
|**2024-09-06**|**Can LLMs Generate Novel Research Ideas? A Large-Scale Human Study with 100+ NLP Researchers**|Chenglei Si et.al.|[2409.04109](http://arxiv.org/abs/2409.04109)|**[link](https://github.com/NoviScl/AI-Researcher)**|
|**2024-09-06**|**AnyMatch -- Efficient Zero-Shot Entity Matching with a Small Language Model**|Zeyu Zhang et.al.|[2409.04073](http://arxiv.org/abs/2409.04073)|**[link](https://github.com/Jantory/anymatch)**|
|**2024-09-06**|**Refining Wikidata Taxonomy using Large Language Models**|Yiwen Peng et.al.|[2409.04056](http://arxiv.org/abs/2409.04056)|**[link](https://github.com/peng-yiwen/WiKC)**|
|**2024-09-05**|**Attention Heads of Large Language Models: A Survey**|Zifan Zheng et.al.|[2409.03752](http://arxiv.org/abs/2409.03752)|**[link](https://github.com/iaar-shanghai/awesome-attention-heads)**|
|**2024-09-05**|**LLM-CI: Assessing Contextual Integrity Norms in Language Models**|Yan Shvartzshnaider et.al.|[2409.03735](http://arxiv.org/abs/2409.03735)|null|
|**2024-09-05**|**Planning In Natural Language Improves LLM Search For Code Generation**|Evan Wang et.al.|[2409.03733](http://arxiv.org/abs/2409.03733)|**[link](https://github.com/scaleapi/plansearch)**|
|**2024-09-06**|**RAG based Question-Answering for Contextual Response Prediction System**|Sriram Veturi et.al.|[2409.03708](http://arxiv.org/abs/2409.03708)|null|
|**2024-09-05**|**TRACE-cs: Trustworthy Reasoning for Contrastive Explanations in Course Scheduling Problems**|Stylianos Loukas Vasileiou et.al.|[2409.03671](http://arxiv.org/abs/2409.03671)|null|
|**2024-09-05**|**The representation landscape of few-shot learning and fine-tuning in large language models**|Diego Doimo et.al.|[2409.03662](http://arxiv.org/abs/2409.03662)|**[link](https://github.com/diegodoimo/geometry_icl_finetuning)**|
|**2024-09-06**|**LLM-based multi-agent poetry generation in non-cooperative environments**|Ran Zhang et.al.|[2409.03659](http://arxiv.org/abs/2409.03659)|**[link](https://github.com/zhangr2021/Multiagent_poetry)**|
|**2024-09-05**|**From MOOC to MAIC: Reshaping Online Teaching and Learning through LLM-driven Agents**|Jifan Yu et.al.|[2409.03512](http://arxiv.org/abs/2409.03512)|null|
|**2024-09-05**|**LLM-based event abstraction and integration for IoT-sourced logs**|Mohsen Shirali et.al.|[2409.03478](http://arxiv.org/abs/2409.03478)|**[link](https://github.com/mfanisani/LLM4IoT)**|
|**2024-09-05**|**How Much Data is Enough Data? Fine-Tuning Large Language Models for In-House Translation: Performance Evaluation Across Multiple Dataset Sizes**|Inacio Vieira et.al.|[2409.03454](http://arxiv.org/abs/2409.03454)|null|
|**2024-09-05**|**LongCite: Enabling LLMs to Generate Fine-grained Citations in Long-context QA**|Jiajie Zhang et.al.|[2409.02897](http://arxiv.org/abs/2409.02897)|**[link](https://github.com/THUDM/LongCite)**|
|**2024-09-04**|**CMM-Math: A Chinese Multimodal Math Dataset To Evaluate and Enhance the Mathematics Reasoning of Large Multimodal Models**|Wentao Liu et.al.|[2409.02834](http://arxiv.org/abs/2409.02834)|null|
|**2024-09-04**|**Design Contradictions: Help or Hindrance?**|Aron E. Owen et.al.|[2409.02823](http://arxiv.org/abs/2409.02823)|null|
|**2024-09-04**|**Language Understanding as a Constraint on Consensus Size in LLM Societies**|Giordano De Marzo et.al.|[2409.02822](http://arxiv.org/abs/2409.02822)|null|
|**2024-09-04**|**Towards a Unified View of Preference Learning for Large Language Models: A Survey**|Bofei Gao et.al.|[2409.02795](http://arxiv.org/abs/2409.02795)|**[link](https://github.com/kbsdjames/awesome-llm-preference-learning)**|
|**2024-09-05**|**Pooling And Attention: What Are Effective Designs For LLM-Based Embedding Models?**|Yixuan Tang et.al.|[2409.02727](http://arxiv.org/abs/2409.02727)|**[link](https://github.com/yixuantt/poolingandattn)**|
|**2024-09-04**|**Alignment-Aware Model Extraction Attacks on Large Language Models**|Zi Liang et.al.|[2409.02718](http://arxiv.org/abs/2409.02718)|**[link](https://github.com/liangzid/alignmentextraction)**|
|**2024-09-04**|**Creating a Gen-AI based Track and Trace Assistant MVP (SuperTracy) for PostNL**|Mohammad Reshadati et.al.|[2409.02711](http://arxiv.org/abs/2409.02711)|null|
|**2024-09-04**|**LLM-Assisted Visual Analytics: Opportunities and Challenges**|Maeve Hutchinson et.al.|[2409.02691](http://arxiv.org/abs/2409.02691)|null|
|**2024-09-04**|**Deconfounded Causality-aware Parameter-Efficient Fine-Tuning for Problem-Solving Improvement of LLMs**|Ruoyu Wang et.al.|[2409.02686](http://arxiv.org/abs/2409.02686)|null|
|**2024-08-30**|**SYNTHEVAL: Hybrid Behavioral Testing of NLP Models with Synthetic CheckLists**|Raoyuan Zhao et.al.|[2408.17437](http://arxiv.org/abs/2408.17437)|**[link](https://github.com/loreley99/syntheval_checklist)**|
|**2024-08-30**|**Advancing Multi-talker ASR Performance with Large Language Models**|Mohan Shi et.al.|[2408.17431](http://arxiv.org/abs/2408.17431)|null|
|**2024-08-30**|**Getting Inspiration for Feature Elicitation: App Store- vs. LLM-based Approach**|Jialiang Wei et.al.|[2408.17404](http://arxiv.org/abs/2408.17404)|**[link](https://github.com/jl-wei/feature-inspiration)**|
|**2024-08-30**|**NDP: Next Distribution Prediction as a More Broad Target**|Junhao Ruan et.al.|[2408.17377](http://arxiv.org/abs/2408.17377)|null|
|**2024-08-30**|**Assessing Generative Language Models in Classification Tasks: Performance and Self-Evaluation Capabilities in the Environmental and Climate Change Domain**|Francesca Grasso et.al.|[2408.17362](http://arxiv.org/abs/2408.17362)|**[link](https://github.com/stefanolocci/LLMClassification)**|
|**2024-08-30**|**Bridging Domain Knowledge and Process Discovery Using Large Language Models**|Ali Norouzifar et.al.|[2408.17316](http://arxiv.org/abs/2408.17316)|**[link](https://github.com/alinorouzifar/imr-llm)**|
|**2024-08-30**|**VisionTS: Visual Masked Autoencoders Are Free-Lunch Zero-Shot Time Series Forecasters**|Mouxiang Chen et.al.|[2408.17253](http://arxiv.org/abs/2408.17253)|**[link](https://github.com/keytoyze/visionts)**|
|**2024-08-30**|**Codec Does Matter: Exploring the Semantic Shortcoming of Codec for Audio Language Model**|Zhen Ye et.al.|[2408.17175](http://arxiv.org/abs/2408.17175)|**[link](https://github.com/zhenye234/xcodec)**|
|**2024-08-30**|**Reasoning AI Performance Degradation in 6G Networks with Large Language Models**|Liming Huang et.al.|[2408.17097](http://arxiv.org/abs/2408.17097)|null|
|**2024-08-30**|**From Text to Emotion: Unveiling the Emotion Annotation Capabilities of LLMs**|Minxue Niu et.al.|[2408.17026](http://arxiv.org/abs/2408.17026)|**[link](https://github.com/chailab-umich/GPT-4-Emotion-Annotation)**|
|**2024-08-29**|**How Far Can Cantonese NLP Go? Benchmarking Cantonese Capabilities of Large Language Models**|Jiyue Jiang et.al.|[2408.16756](http://arxiv.org/abs/2408.16756)|**[link](https://github.com/jiangjyjy/yue-benchmark)**|
|**2024-08-29**|**Theoretical and Methodological Framework for Studying Texts Produced by Large Language Models**|Jiří Milička et.al.|[2408.16740](http://arxiv.org/abs/2408.16740)|null|
|**2024-08-29**|**GradBias: Unveiling Word Influence on Bias in Text-to-Image Generative Models**|Moreno D'Incà et.al.|[2408.16700](http://arxiv.org/abs/2408.16700)|**[link](https://github.com/moreno98/gradbias)**|
|**2024-08-29**|**Examination of Code generated by Large Language Models**|Robin Beer et.al.|[2408.16601](http://arxiv.org/abs/2408.16601)|**[link](https://github.com/t-muras/ai-code-analysis)**|
|**2024-08-29**|**Enhancing Dialogue Generation in Werewolf Game Through Situation Analysis and Persuasion Strategies**|Zhiyang Qi et.al.|[2408.16586](http://arxiv.org/abs/2408.16586)|null|
|**2024-08-29**|**LLMs vs Established Text Augmentation Techniques for Classification: When do the Benefits Outweight the Costs?**|Jan Cegin et.al.|[2408.16502](http://arxiv.org/abs/2408.16502)|null|
|**2024-08-29**|**A Survey on Evaluating Large Language Models in Code Generation Tasks**|Liguo Chen et.al.|[2408.16498](http://arxiv.org/abs/2408.16498)|null|
|**2024-08-29**|**Self-Alignment: Improving Alignment of Cultural Values in LLMs via In-Context Learning**|Rochelle Choenni et.al.|[2408.16482](http://arxiv.org/abs/2408.16482)|null|
|**2024-08-29**|**Human and LLM-Based Voice Assistant Interaction: An Analytical Framework for User Verbal and Nonverbal Behaviors**|Szeyi Chan et.al.|[2408.16465](http://arxiv.org/abs/2408.16465)|null|
|**2024-08-29**|**Instruction-tuned Large Language Models for Machine Translation in the Medical Domain**|Miguel Rios et.al.|[2408.16440](http://arxiv.org/abs/2408.16440)|null|
|**2024-08-28**|**BattleAgentBench: A Benchmark for Evaluating Cooperation and Competition Capabilities of Language Models in Multi-Agent Systems**|Wei Wang et.al.|[2408.15971](http://arxiv.org/abs/2408.15971)|null|
|**2024-08-28**|**More Text, Less Point: Towards 3D Data-Efficient Point-Language Understanding**|Yuan Tang et.al.|[2408.15966](http://arxiv.org/abs/2408.15966)|**[link](https://github.com/tangyuan96/greenplm)**|
|**2024-08-28**|**Atari-GPT: Investigating the Capabilities of Multimodal Large Language Models as Low-Level Policies for Atari Games**|Nicholas R. Waytowich et.al.|[2408.15950](http://arxiv.org/abs/2408.15950)|null|
|**2024-08-28**|**Leveraging Open Knowledge for Advancing Task Expertise in Large Language Models**|Yuncheng Yang et.al.|[2408.15915](http://arxiv.org/abs/2408.15915)|**[link](https://github.com/yaphabates/rocket)**|
|**2024-08-28**|**LLM-Based Multi-Hop Question Answering with Knowledge Graph Integration in Evolving Environments**|Ruirui Chen et.al.|[2408.15903](http://arxiv.org/abs/2408.15903)|null|
|**2024-08-28**|**Bias in LLMs as Annotators: The Effect of Party Cues on Labelling Decision by Large Language Models**|Sebastian Vallejo Vera et.al.|[2408.15895](http://arxiv.org/abs/2408.15895)|null|
|**2024-08-28**|**Persuasion Games using Large Language Models**|Ganesh Prasath Ramani et.al.|[2408.15879](http://arxiv.org/abs/2408.15879)|null|
|**2024-08-28**|**Scaling Up Summarization: Leveraging Large Language Models for Long Text Extractive Summarization**|Léo Hemamou et.al.|[2408.15801](http://arxiv.org/abs/2408.15801)|null|
|**2024-08-28**|**Efficient LLM Scheduling by Learning to Rank**|Yichao Fu et.al.|[2408.15792](http://arxiv.org/abs/2408.15792)|**[link](https://github.com/hao-ai-lab/vllm-ltr)**|
|**2024-08-28**|**Interactive Agents: Simulating Counselor-Client Psychological Counseling via Role-Playing LLM-to-LLM Interactions**|Huachuan Qiu et.al.|[2408.15787](http://arxiv.org/abs/2408.15787)|**[link](https://github.com/qiuhuachuan/interactive-agents)**|
|**2024-08-27**|**Generative Verifiers: Reward Modeling as Next-Token Prediction**|Lunjun Zhang et.al.|[2408.15240](http://arxiv.org/abs/2408.15240)|null|
|**2024-08-27**|**LLM Defenses Are Not Robust to Multi-Turn Human Jailbreaks Yet**|Nathaniel Li et.al.|[2408.15221](http://arxiv.org/abs/2408.15221)|null|
|**2024-08-27**|**Investigating Coverage Criteria in Large Language Models: An In-Depth Study Through Jailbreak Attacks**|Shide Zhou et.al.|[2408.15207](http://arxiv.org/abs/2408.15207)|null|
|**2024-08-27**|**Can Unconfident LLM Annotations Be Used for Confident Conclusions?**|Kristina Gligorić et.al.|[2408.15204](http://arxiv.org/abs/2408.15204)|**[link](https://github.com/kristinagligoric/confidence-driven-inference)**|
|**2024-08-27**|**X-Reflect: Cross-Reflection Prompting for Multimodal Recommendation**|Hanjia Lyu et.al.|[2408.15172](http://arxiv.org/abs/2408.15172)|null|
|**2024-08-27**|**Measuring text summarization factuality using atomic facts entailment metrics in the context of retrieval augmented generation**|N. E. Kriman et.al.|[2408.15171](http://arxiv.org/abs/2408.15171)|null|
|**2024-08-27**|**BaichuanSEED: Sharing the Potential of ExtensivE Data Collection and Deduplication by Introducing a Competitive Large Language Model Baseline**|Guosheng Dong et.al.|[2408.15079](http://arxiv.org/abs/2408.15079)|null|
|**2024-08-27**|**Constraining Participation: Affordances of Feedback Features in Interfaces to Large Language Models**|Ned Cooper et.al.|[2408.15066](http://arxiv.org/abs/2408.15066)|null|
|**2024-08-28**|**DocLayLLM: An Efficient and Effective Multi-modal Extension of Large Language Models for Text-rich Document Understanding**|Wenhui Liao et.al.|[2408.15045](http://arxiv.org/abs/2408.15045)|null|
|**2024-08-28**|**A Survey of Large Language Models for European Languages**|Wazir Ali et.al.|[2408.15040](http://arxiv.org/abs/2408.15040)|null|
|**2024-08-27**|**Step-by-Step Unmasking for Parameter-Efficient Fine-tuning of Large Language Models**|Aradhye Agarwal et.al.|[2408.14470](http://arxiv.org/abs/2408.14470)|**[link](https://github.com/Aradhye2002/selective-peft-toolkit)**|
|**2024-08-26**|**Explicit Inductive Inference using Large Language Models**|Tianyang Liu et.al.|[2408.14467](http://arxiv.org/abs/2408.14467)|null|
|**2024-08-26**|**MEDSAGE: Enhancing Robustness of Medical Dialogue Summarization to ASR Errors with LLM-generated Synthetic Dialogues**|Kuluhan Binici et.al.|[2408.14418](http://arxiv.org/abs/2408.14418)|null|
|**2024-08-26**|**Language-specific Calibration for Pruning Multilingual Language Models**|Simon Kurz et.al.|[2408.14398](http://arxiv.org/abs/2408.14398)|null|
|**2024-08-26**|**Reprogramming Foundational Large Language Models(LLMs) for Enterprise Adoption for Spatio-Temporal Forecasting Applications: Unveiling a New Era in Copilot-Guided Cross-Modal Time Series Representation Learning**|Sakhinana Sagar Srinivas et.al.|[2408.14387](http://arxiv.org/abs/2408.14387)|null|
|**2024-08-26**|**Probing Causality Manipulation of Large Language Models**|Chenyang Zhang et.al.|[2408.14380](http://arxiv.org/abs/2408.14380)|**[link](https://github.com/tongjinlp/llm-causality-probing)**|
|**2024-08-26**|**SWE-bench-java: A GitHub Issue Resolving Benchmark for Java**|Daoguang Zan et.al.|[2408.14354](http://arxiv.org/abs/2408.14354)|**[link](https://github.com/multi-swe-bench/multi-swe-bench-env)**|
|**2024-08-26**|**Assessing Contamination in Large Language Models: Introducing the LogProber method**|Nicolas Yax et.al.|[2408.14352](http://arxiv.org/abs/2408.14352)|null|
|**2024-08-27**|**Foundation Models for Music: A Survey**|Yinghao Ma et.al.|[2408.14340](http://arxiv.org/abs/2408.14340)|**[link](https://github.com/nicolaus625/fm4music)**|
|**2024-08-26**|**Claim Verification in the Age of Large Language Models: A Survey**|Alphaeus Dmonte et.al.|[2408.14317](http://arxiv.org/abs/2408.14317)|null|
|**2024-08-23**|**DOMAINEVAL: An Auto-Constructed Benchmark for Multi-Domain Code Generation**|Qiming Zhu et.al.|[2408.13204](http://arxiv.org/abs/2408.13204)|null|
|**2024-08-23**|**Can LLM be a Good Path Planner based on Prompt Engineering? Mitigating the Hallucination for Path Planning**|Hourui Deng et.al.|[2408.13184](http://arxiv.org/abs/2408.13184)|null|
|**2024-08-23**|**IntelliCare: Improving Healthcare Analysis with Variance-Controlled Patient-Level Knowledge from Large Language Models**|Zhihao Yu et.al.|[2408.13073](http://arxiv.org/abs/2408.13073)|**[link](https://github.com/yzhHoward/IntelliCare)**|
|**2024-08-23**|**Guiding IoT-Based Healthcare Alert Systems with Large Language Models**|Yulan Gao et.al.|[2408.13071](http://arxiv.org/abs/2408.13071)|null|
|**2024-08-23**|**In-Context Learning with Reinforcement Learning for Incomplete Utterance Rewriting**|Haowei Du et.al.|[2408.13028](http://arxiv.org/abs/2408.13028)|null|
|**2024-08-23**|**Systematic Evaluation of LLM-as-a-Judge in LLM Alignment Tasks: Explainable Metrics and Diverse Prompt Templates**|Hui Wei et.al.|[2408.13006](http://arxiv.org/abs/2408.13006)|**[link](https://github.com/shenghh2015/llm-judge-eval)**|
|**2024-08-23**|**CRUXEval-X: A Benchmark for Multilingual Code Reasoning, Understanding and Execution**|Ruiyang Xu et.al.|[2408.13001](http://arxiv.org/abs/2408.13001)|null|
|**2024-08-23**|**Open Llama2 Model for the Lithuanian Language**|Artūras Nakvosas et.al.|[2408.12963](http://arxiv.org/abs/2408.12963)|null|
|**2024-08-23**|**Multimodal Contrastive In-Context Learning**|Yosuke Miyanishi et.al.|[2408.12959](http://arxiv.org/abs/2408.12959)|null|
|**2024-08-23**|**E-code: Mastering Efficient Code Generation through Pretrained Models and Expert Encoder Group**|Yue Pan et.al.|[2408.12948](http://arxiv.org/abs/2408.12948)|null|
|**2024-08-22**|**Controllable Text Generation for Large Language Models: A Survey**|Xun Liang et.al.|[2408.12599](http://arxiv.org/abs/2408.12599)|**[link](https://github.com/iaar-shanghai/ctgsurvey)**|
|**2024-08-22**|**RuleAlign: Making Large Language Models Better Physicians with Diagnostic Rule Alignment**|Xiaohan Wang et.al.|[2408.12579](http://arxiv.org/abs/2408.12579)|null|
|**2024-08-22**|**Towards Evaluating and Building Versatile Large Language Models for Medicine**|Chaoyi Wu et.al.|[2408.12547](http://arxiv.org/abs/2408.12547)|**[link](https://github.com/magic-ai4med/meds-ins)**|
|**2024-08-22**|**MEDCO: Medical Education Copilots Based on A Multi-Agent Framework**|Hao Wei et.al.|[2408.12496](http://arxiv.org/abs/2408.12496)|null|
|**2024-08-22**|**GenderCARE: A Comprehensive Framework for Assessing and Reducing Gender Bias in Large Language Models**|Kunsheng Tang et.al.|[2408.12494](http://arxiv.org/abs/2408.12494)|**[link](https://github.com/kstanghere/gendercare-ccs24)**|
|**2024-08-22**|**Frame Order Matters: A Temporal Sequence-Aware Model for Few-Shot Action Recognition**|Bozheng Li et.al.|[2408.12475](http://arxiv.org/abs/2408.12475)|null|
|**2024-08-22**|**DLCRec: A Novel Approach for Managing Diversity in LLM-Based Recommender Systems**|Jiaju Chen et.al.|[2408.12470](http://arxiv.org/abs/2408.12470)|null|
|**2024-08-22**|**Envisioning Class Entity Reasoning by Large Language Models for Few-shot Learning**|Mushui Liu et.al.|[2408.12469](http://arxiv.org/abs/2408.12469)|null|
|**2024-08-22**|**Enhancing Multi-hop Reasoning through Knowledge Erasure in Large Language Model Editing**|Mengqi Zhang et.al.|[2408.12456](http://arxiv.org/abs/2408.12456)|null|
|**2024-08-22**|**A Comparative Analysis of Faithfulness Metrics and Humans in Citation Evaluation**|Weijia Zhang et.al.|[2408.12398](http://arxiv.org/abs/2408.12398)|null|
|**2024-08-21**|**SEA: Supervised Embedding Alignment for Token-Level Visual-Textual Integration in MLLMs**|Yuanyang Yin et.al.|[2408.11813](http://arxiv.org/abs/2408.11813)|null|
|**2024-08-21**|**Story3D-Agent: Exploring 3D Storytelling Visualization with Large Language Models**|Yuzhou Huang et.al.|[2408.11801](http://arxiv.org/abs/2408.11801)|null|
|**2024-08-21**|**PermitQA: A Benchmark for Retrieval Augmented Generation in Wind Siting and Permitting domain**|Rounak Meyur et.al.|[2408.11800](http://arxiv.org/abs/2408.11800)|null|
|**2024-08-21**|**EE-MLLM: A Data-Efficient and Compute-Efficient Multimodal Large Language Model**|Feipeng Ma et.al.|[2408.11795](http://arxiv.org/abs/2408.11795)|null|
|**2024-08-21**|**Leveraging Chemistry Foundation Models to Facilitate Structure Focused Retrieval Augmented Generation in Multi-Agent Workflows for Catalyst and Materials Design**|Nathaniel H. Park et.al.|[2408.11793](http://arxiv.org/abs/2408.11793)|null|
|**2024-08-21**|**Critique-out-Loud Reward Models**|Zachary Ankner et.al.|[2408.11791](http://arxiv.org/abs/2408.11791)|**[link](https://github.com/zankner/cloud)**|
|**2024-08-21**|**Personality Alignment of Large Language Models**|Minjun Zhu et.al.|[2408.11779](http://arxiv.org/abs/2408.11779)|**[link](https://github.com/zhu-minjun/palign)**|
|**2024-08-21**|**Leveraging Fine-Tuned Retrieval-Augmented Generation with Long-Context Support: For 3GPP Standards**|Omar Erak et.al.|[2408.11775](http://arxiv.org/abs/2408.11775)|**[link](https://github.com/Nouf-Alabbasi/oKUmura_AI_Telecom_challenge)**|
|**2024-08-21**|**Against All Odds: Overcoming Typology, Script, and Language Confusion in Multilingual Embedding Inversion Attacks**|Yiyi Chen et.al.|[2408.11749](http://arxiv.org/abs/2408.11749)|**[link](https://github.com/siebeniris/vec2text_exp)**|
|**2024-08-21**|**Mixed Sparsity Training: Achieving 4 $\times$ FLOP Reduction for Transformer Pretraining**|Pihe Hu et.al.|[2408.11746](http://arxiv.org/abs/2408.11746)|null|
|**2024-08-20**|**Revisiting VerilogEval: Newer LLMs, In-Context Learning, and Specification-to-RTL Tasks**|Nathaniel Pinckney et.al.|[2408.11053](http://arxiv.org/abs/2408.11053)|**[link](https://github.com/nvlabs/verilog-eval)**|
|**2024-08-20**|**FLAME: Learning to Navigate with Multimodal LLM in Urban Environments**|Yunzhe Xu et.al.|[2408.11051](http://arxiv.org/abs/2408.11051)|**[link](https://github.com/xyz9911/FLAME)**|
|**2024-08-21**|**MagicDec: Breaking the Latency-Throughput Tradeoff for Long Context Generation with Speculative Decoding**|Jian Chen et.al.|[2408.11049](http://arxiv.org/abs/2408.11049)|**[link](https://github.com/infini-ai-lab/magicdec)**|
|**2024-08-20**|**Reconciling Methodological Paradigms: Employing Large Language Models as Novice Qualitative Research Assistants in Talent Management Research**|Sreyoshi Bhaduri et.al.|[2408.11043](http://arxiv.org/abs/2408.11043)|null|
|**2024-08-20**|**Athena: Safe Autonomous Agents with Verbal Contrastive Learning**|Tanmana Sadhu et.al.|[2408.11021](http://arxiv.org/abs/2408.11021)|null|
|**2024-08-20**|**While GitHub Copilot Excels at Coding, Does It Ensure Responsible Output?**|Wen Cheng et.al.|[2408.11006](http://arxiv.org/abs/2408.11006)|**[link](https://github.com/sensente/security-attacks-on-lccts)**|
|**2024-08-20**|**CTP-LLM: Clinical Trial Phase Transition Prediction Using Large Language Models**|Michael Reinisch et.al.|[2408.10995](http://arxiv.org/abs/2408.10995)|null|
|**2024-08-20**|**Dr.Academy: A Benchmark for Evaluating Questioning Capability in Education for Large Language Models**|Yuyan Chen et.al.|[2408.10947](http://arxiv.org/abs/2408.10947)|null|
|**2024-08-20**|**HiRED: Attention-Guided Token Dropping for Efficient Inference of High-Resolution Vision-Language Models in Resource-Constrained Environments**|Kazi Hasan Ibn Arif et.al.|[2408.10945](http://arxiv.org/abs/2408.10945)|**[link](https://github.com/hasanar1f/hired)**|
|**2024-08-20**|**SysBench: Can Large Language Models Follow System Messages?**|Yanzhao Qin et.al.|[2408.10943](http://arxiv.org/abs/2408.10943)|**[link](https://github.com/pku-baichuan-mlsystemlab/sysbench)**|
|**2024-08-19**|**Demystifying the Communication Characteristics for Distributed Transformer Models**|Quentin Anthony et.al.|[2408.10197](http://arxiv.org/abs/2408.10197)|null|
|**2024-08-19**|**Customizing Language Models with Instance-wise LoRA for Sequential Recommendation**|Xiaoyu Kong et.al.|[2408.10159](http://arxiv.org/abs/2408.10159)|null|
|**2024-08-19**|**Multilingual Needle in a Haystack: Investigating Long-Context Behavior of Multilingual Large Language Models**|Amey Hengle et.al.|[2408.10151](http://arxiv.org/abs/2408.10151)|**[link](https://github.com/AmeyHengle/multilingual-needle-in-a-haystack)**|
|**2024-08-19**|**Instruction Finetuning for Leaderboard Generation from Empirical AI Research**|Salomon Kabongo et.al.|[2408.10141](http://arxiv.org/abs/2408.10141)|null|
|**2024-08-19**|**Molecular Graph Representation Learning Integrating Large Language Models with Domain-specific Small Models**|Tianyu Zhang et.al.|[2408.10124](http://arxiv.org/abs/2408.10124)|**[link](https://github.com/zhangtia16/molgraph-lardo)**|
|**2024-08-19**|**ARMADA: Attribute-Based Multimodal Data Augmentation**|Xiaomeng Jin et.al.|[2408.10086](http://arxiv.org/abs/2408.10086)|null|
|**2024-08-19**|**Privacy Checklist: Privacy Violation Detection Grounding on Contextual Integrity Theory**|Haoran Li et.al.|[2408.10053](http://arxiv.org/abs/2408.10053)|null|
|**2024-08-19**|**TBA: Faster Large Language Model Training Using SSD-Based Activation Offloading**|Kun Wu et.al.|[2408.10013](http://arxiv.org/abs/2408.10013)|null|
|**2024-08-20**|**Application of Large Language Models in Automated Question Generation: A Case Study on ChatGLM's Structured Questions for National Teacher Certification Exams**|Ling He et.al.|[2408.09982](http://arxiv.org/abs/2408.09982)|null|
|**2024-08-19**|**Edge-Cloud Collaborative Motion Planning for Autonomous Driving with Large Language Models**|Jiao Chen et.al.|[2408.09972](http://arxiv.org/abs/2408.09972)|null|
|**2024-08-19**|**PEDAL: Enhancing Greedy Decoding with Large Language Models using Diverse Exemplars**|Sumanth Prabhu et.al.|[2408.08869](http://arxiv.org/abs/2408.08869)|null|
|**2024-08-16**|**Visual Agents as Fast and Slow Thinkers**|Guangyan Sun et.al.|[2408.08862](http://arxiv.org/abs/2408.08862)|**[link](https://github.com/guangyans/sys2-llava)**|
|**2024-08-16**|**ECG-Chat: A Large ECG-Language Model for Cardiac Disease Diagnosis**|Yubao Zhao et.al.|[2408.08849](http://arxiv.org/abs/2408.08849)|null|
|**2024-08-16**|**PsychoLex: Unveiling the Psychological Mind of Large Language Models**|Mohammad Amin Abbasi et.al.|[2408.08848](http://arxiv.org/abs/2408.08848)|null|
|**2024-08-16**|**FLEXTAF: Enhancing Table Reasoning with Flexible Tabular Formats**|Xuanliang Zhang et.al.|[2408.08841](http://arxiv.org/abs/2408.08841)|**[link](https://github.com/zhxlia/FLEXTAF)**|
|**2024-08-16**|**Artificial Intelligence and Strategic Decision-Making: Evidence from Entrepreneurs and Investors**|Felipe A. Csaszar et.al.|[2408.08811](http://arxiv.org/abs/2408.08811)|null|
|**2024-08-19**|**Constructing Domain-Specific Evaluation Sets for LLM-as-a-judge**|Ravi Raju et.al.|[2408.08808](http://arxiv.org/abs/2408.08808)|null|
|**2024-08-16**|**EmoDynamiX: Emotional Support Dialogue Strategy Prediction by Modelling MiXed Emotions and Discourse Dynamics**|Chenwei Wan et.al.|[2408.08782](http://arxiv.org/abs/2408.08782)|**[link](https://github.com/cw-wan/EmoDynamiX-v2)**|
|**2024-08-16**|**Large Language Models Might Not Care What You Are Saying: Prompt Format Beats Descriptions**|Chenming Tang et.al.|[2408.08780](http://arxiv.org/abs/2408.08780)|null|
|**2024-08-16**|**DAC: Decomposed Automation Correction for Text-to-SQL**|Dingzirui Wang et.al.|[2408.08779](http://arxiv.org/abs/2408.08779)|**[link](https://github.com/zirui-HIT/DAC)**|
|**2024-08-15**|**Can Large Language Models Understand Symbolic Graphics Programs?**|Zeju Qiu et.al.|[2408.08313](http://arxiv.org/abs/2408.08313)|null|
|**2024-08-15**|**ScalingFilter: Assessing Data Quality through Inverse Utilization of Scaling Laws**|Ruihang Li et.al.|[2408.08310](http://arxiv.org/abs/2408.08310)|null|
|**2024-08-15**|**Benchmarking the Capabilities of Large Language Models in Transportation System Engineering: Accuracy, Consistency, and Reasoning Behaviors**|Usman Syed et.al.|[2408.08302](http://arxiv.org/abs/2408.08302)|null|
|**2024-08-15**|**HELP: Hierarchical Embeddings-based Log Parsing**|Andy Xu et.al.|[2408.08300](http://arxiv.org/abs/2408.08300)|null|
|**2024-08-15**|**The ShareLM Collection and Plugin: Contributing Human-Model Chats for the Benefit of the Community**|Shachar Don-Yehiya et.al.|[2408.08291](http://arxiv.org/abs/2408.08291)|null|
|**2024-08-15**|**Autonomous Behavior Planning For Humanoid Loco-manipulation Through Grounded Language Model**|Jin Wang et.al.|[2408.08282](http://arxiv.org/abs/2408.08282)|null|
|**2024-08-15**|**BAM! Just Like That: Simple and Efficient Parameter Upcycling for Mixture of Experts**|Qizhen Zhang et.al.|[2408.08274](http://arxiv.org/abs/2408.08274)|null|
|**2024-08-15**|**DaRec: A Disentangled Alignment Framework for Large Language Model and Recommender System**|Xihong Yang et.al.|[2408.08231](http://arxiv.org/abs/2408.08231)|null|
|**2024-08-15**|**RED-CT: A Systems Design Methodology for Using LLM-labeled Data to Train and Deploy Edge Classifiers for Computational Social Science**|David Farr et.al.|[2408.08217](http://arxiv.org/abs/2408.08217)|null|
|**2024-08-15**|**Does Reasoning Emerge? Examining the Probabilities of Causation in Large Language Models**|Javier González et.al.|[2408.08210](http://arxiv.org/abs/2408.08210)|null|
|**2024-08-14**|**The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models**|Karime Maamari et.al.|[2408.07702](http://arxiv.org/abs/2408.07702)|null|
|**2024-08-15**|**Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories, Applications and Opportunities**|Enneng Yang et.al.|[2408.07666](http://arxiv.org/abs/2408.07666)|**[link](https://github.com/ennengyang/awesome-model-merging-methods-theories-applications)**|
|**2024-08-14**|**Spoken Stereoset: On Evaluating Social Bias Toward Speaker in Speech Large Language Models**|Yi-Cheng Lin et.al.|[2408.07665](http://arxiv.org/abs/2408.07665)|**[link](https://github.com/dlion168/spoken_stereoset)**|
|**2024-08-14**|**Alignment-Enhanced Decoding:Defending via Token-Level Adaptive Refining of Probability Distributions**|Quan Liu et.al.|[2408.07663](http://arxiv.org/abs/2408.07663)|**[link](https://github.com/gigabaozi/aed)**|
|**2024-08-14**|**WeKnow-RAG: An Adaptive Approach for Retrieval-Augmented Generation Integrating Web Search and Knowledge Graphs**|Weijian Xie et.al.|[2408.07611](http://arxiv.org/abs/2408.07611)|null|
|**2024-08-14**|**Transformers and Large Language Models for Efficient Intrusion Detection Systems: A Comprehensive Survey**|Hamza Kheddar et.al.|[2408.07583](http://arxiv.org/abs/2408.07583)|null|
|**2024-08-15**|**MathScape: Evaluating MLLMs in multimodal Math Scenarios through a Hierarchical Benchmark**|Minxuan Zhou et.al.|[2408.07543](http://arxiv.org/abs/2408.07543)|**[link](https://github.com/PKU-Baichuan-MLSystemLab/MathScape)**|
|**2024-08-15**|**Usefulness of data flow diagrams and large language models for security threat validation: a registered report**|Winnie Bahati Mbaka et.al.|[2408.07537](http://arxiv.org/abs/2408.07537)|null|
|**2024-08-14**|**Development of a Multi-Agent Clinical Decision Support System for Korean Triage and Acuity Scale (KTAS)-Based Triage and Treatment Planning in Emergency Departments**|Seungjun Han et.al.|[2408.07531](http://arxiv.org/abs/2408.07531)|null|
|**2024-08-14**|**Large Language Models Know What Makes Exemplary Contexts**|Quanyu Long et.al.|[2408.07505](http://arxiv.org/abs/2408.07505)|null|
|**2024-05-16**|**When LLMs step into the 3D World: A Survey and Meta-Analysis of 3D Tasks via Multi-modal Large Language Models**|Xianzheng Ma et.al.|[2405.10255](http://arxiv.org/abs/2405.10255)|**[link](https://github.com/activevisionlab/awesome-llm-3d)**|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## Wireless Network

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-08-19**|**PEDAL: Enhancing Greedy Decoding with Large Language Models using Diverse Exemplars**|Sumanth Prabhu et.al.|[2408.08869](http://arxiv.org/abs/2408.08869)|null|
|**2024-08-16**|**PsychoLex: Unveiling the Psychological Mind of Large Language Models**|Mohammad Amin Abbasi et.al.|[2408.08848](http://arxiv.org/abs/2408.08848)|null|
|**2024-08-16**|**FLEXTAF: Enhancing Table Reasoning with Flexible Tabular Formats**|Xuanliang Zhang et.al.|[2408.08841](http://arxiv.org/abs/2408.08841)|**[link](https://github.com/zhxlia/FLEXTAF)**|
|**2024-08-16**|**Artificial Intelligence and Strategic Decision-Making: Evidence from Entrepreneurs and Investors**|Felipe A. Csaszar et.al.|[2408.08811](http://arxiv.org/abs/2408.08811)|null|
|**2024-08-19**|**Constructing Domain-Specific Evaluation Sets for LLM-as-a-judge**|Ravi Raju et.al.|[2408.08808](http://arxiv.org/abs/2408.08808)|null|
|**2024-08-16**|**EmoDynamiX: Emotional Support Dialogue Strategy Prediction by Modelling MiXed Emotions and Discourse Dynamics**|Chenwei Wan et.al.|[2408.08782](http://arxiv.org/abs/2408.08782)|**[link](https://github.com/cw-wan/EmoDynamiX-v2)**|
|**2024-08-16**|**Evaluating the Evaluator: Measuring LLMs' Adherence to Task Evaluation Instructions**|Bhuvanashree Murugadoss et.al.|[2408.08781](http://arxiv.org/abs/2408.08781)|null|
|**2024-08-16**|**Large Language Models Might Not Care What You Are Saying: Prompt Format Beats Descriptions**|Chenming Tang et.al.|[2408.08780](http://arxiv.org/abs/2408.08780)|null|
|**2024-08-16**|**DAC: Decomposed Automation Correction for Text-to-SQL**|Dingzirui Wang et.al.|[2408.08779](http://arxiv.org/abs/2408.08779)|**[link](https://github.com/zirui-HIT/DAC)**|
|**2024-08-16**|**Lower Layer Matters: Alleviating Hallucination via Multi-Layer Fusion Contrastive Decoding with Truthfulness Refocused**|Dingwei Chen et.al.|[2408.08769](http://arxiv.org/abs/2408.08769)|null|
|**2024-08-15**|**Can Large Language Models Understand Symbolic Graphics Programs?**|Zeju Qiu et.al.|[2408.08313](http://arxiv.org/abs/2408.08313)|null|
|**2024-08-15**|**Benchmarking the Capabilities of Large Language Models in Transportation System Engineering: Accuracy, Consistency, and Reasoning Behaviors**|Usman Syed et.al.|[2408.08302](http://arxiv.org/abs/2408.08302)|null|
|**2024-08-15**|**HELP: Hierarchical Embeddings-based Log Parsing**|Andy Xu et.al.|[2408.08300](http://arxiv.org/abs/2408.08300)|null|
|**2024-08-15**|**Autonomous Behavior Planning For Humanoid Loco-manipulation Through Grounded Language Model**|Jin Wang et.al.|[2408.08282](http://arxiv.org/abs/2408.08282)|null|
|**2024-08-15**|**DaRec: A Disentangled Alignment Framework for Large Language Model and Recommender System**|Xihong Yang et.al.|[2408.08231](http://arxiv.org/abs/2408.08231)|null|
|**2024-08-15**|**RED-CT: A Systems Design Methodology for Using LLM-labeled Data to Train and Deploy Edge Classifiers for Computational Social Science**|David Farr et.al.|[2408.08217](http://arxiv.org/abs/2408.08217)|null|
|**2024-08-16**|**Covert Bias: The Severity of Social Views' Unalignment in Language Models Towards Implicit and Explicit Opinion**|Abeer Aldayel et.al.|[2408.08212](http://arxiv.org/abs/2408.08212)|null|
|**2024-08-15**|**Does Reasoning Emerge? Examining the Probabilities of Causation in Large Language Models**|Javier González et.al.|[2408.08210](http://arxiv.org/abs/2408.08210)|null|
|**2024-08-15**|**LLM4DSR: Leveraing Large Language Model for Denoising Sequential Recommendation**|Bohao Wang et.al.|[2408.08208](http://arxiv.org/abs/2408.08208)|null|
|**2024-08-15**|**Scaling Up Natural Language Understanding for Multi-Robots Through the Lens of Hierarchy**|Shaojun Xu et.al.|[2408.08188](http://arxiv.org/abs/2408.08188)|null|
|**2024-08-14**|**The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models**|Karime Maamari et.al.|[2408.07702](http://arxiv.org/abs/2408.07702)|null|
|**2024-08-15**|**Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories, Applications and Opportunities**|Enneng Yang et.al.|[2408.07666](http://arxiv.org/abs/2408.07666)|**[link](https://github.com/ennengyang/awesome-model-merging-methods-theories-applications)**|
|**2024-08-14**|**Spoken Stereoset: On Evaluating Social Bias Toward Speaker in Speech Large Language Models**|Yi-Cheng Lin et.al.|[2408.07665](http://arxiv.org/abs/2408.07665)|**[link](https://github.com/dlion168/spoken_stereoset)**|
|**2024-08-14**|**Alignment-Enhanced Decoding:Defending via Token-Level Adaptive Refining of Probability Distributions**|Quan Liu et.al.|[2408.07663](http://arxiv.org/abs/2408.07663)|**[link](https://github.com/gigabaozi/aed)**|
|**2024-08-14**|**WeKnow-RAG: An Adaptive Approach for Retrieval-Augmented Generation Integrating Web Search and Knowledge Graphs**|Weijian Xie et.al.|[2408.07611](http://arxiv.org/abs/2408.07611)|null|
|**2024-08-14**|**Optimizing UAV Trajectory for Emergency Response Operations under Real 3D Environments: Integrating Priority Levels and LoS Constraints**|Mohammad Taghi Dabiri et.al.|[2408.07589](http://arxiv.org/abs/2408.07589)|null|
|**2024-08-14**|**Transformers and Large Language Models for Efficient Intrusion Detection Systems: A Comprehensive Survey**|Hamza Kheddar et.al.|[2408.07583](http://arxiv.org/abs/2408.07583)|null|
|**2024-08-15**|**MathScape: Evaluating MLLMs in multimodal Math Scenarios through a Hierarchical Benchmark**|Minxuan Zhou et.al.|[2408.07543](http://arxiv.org/abs/2408.07543)|**[link](https://github.com/PKU-Baichuan-MLSystemLab/MathScape)**|
|**2024-08-15**|**Usefulness of data flow diagrams and large language models for security threat validation: a registered report**|Winnie Bahati Mbaka et.al.|[2408.07537](http://arxiv.org/abs/2408.07537)|null|
|**2024-08-14**|**Development of a Multi-Agent Clinical Decision Support System for Korean Triage and Acuity Scale (KTAS)-Based Triage and Treatment Planning in Emergency Departments**|Seungjun Han et.al.|[2408.07531](http://arxiv.org/abs/2408.07531)|null|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## Wireless Communications

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-08-19**|**PEDAL: Enhancing Greedy Decoding with Large Language Models using Diverse Exemplars**|Sumanth Prabhu et.al.|[2408.08869](http://arxiv.org/abs/2408.08869)|null|
|**2024-08-16**|**PsychoLex: Unveiling the Psychological Mind of Large Language Models**|Mohammad Amin Abbasi et.al.|[2408.08848](http://arxiv.org/abs/2408.08848)|null|
|**2024-08-16**|**FLEXTAF: Enhancing Table Reasoning with Flexible Tabular Formats**|Xuanliang Zhang et.al.|[2408.08841](http://arxiv.org/abs/2408.08841)|**[link](https://github.com/zhxlia/FLEXTAF)**|
|**2024-08-16**|**Intra-symbol Differential Amplitude Shift Keying-aided Blind Detector for Ambient Backscatter Communication Systems**|Shuaijun Ma et.al.|[2408.08833](http://arxiv.org/abs/2408.08833)|null|
|**2024-08-16**|**Artificial Intelligence and Strategic Decision-Making: Evidence from Entrepreneurs and Investors**|Felipe A. Csaszar et.al.|[2408.08811](http://arxiv.org/abs/2408.08811)|null|
|**2024-08-19**|**Constructing Domain-Specific Evaluation Sets for LLM-as-a-judge**|Ravi Raju et.al.|[2408.08808](http://arxiv.org/abs/2408.08808)|null|
|**2024-08-16**|**Xpikeformer: Hybrid Analog-Digital Hardware Acceleration for Spiking Transformers**|Zihang Song et.al.|[2408.08794](http://arxiv.org/abs/2408.08794)|null|
|**2024-08-16**|**EmoDynamiX: Emotional Support Dialogue Strategy Prediction by Modelling MiXed Emotions and Discourse Dynamics**|Chenwei Wan et.al.|[2408.08782](http://arxiv.org/abs/2408.08782)|**[link](https://github.com/cw-wan/EmoDynamiX-v2)**|
|**2024-08-16**|**Evaluating the Evaluator: Measuring LLMs' Adherence to Task Evaluation Instructions**|Bhuvanashree Murugadoss et.al.|[2408.08781](http://arxiv.org/abs/2408.08781)|null|
|**2024-08-16**|**Large Language Models Might Not Care What You Are Saying: Prompt Format Beats Descriptions**|Chenming Tang et.al.|[2408.08780](http://arxiv.org/abs/2408.08780)|null|
|**2024-08-15**|**Can Large Language Models Understand Symbolic Graphics Programs?**|Zeju Qiu et.al.|[2408.08313](http://arxiv.org/abs/2408.08313)|null|
|**2024-08-15**|**Benchmarking the Capabilities of Large Language Models in Transportation System Engineering: Accuracy, Consistency, and Reasoning Behaviors**|Usman Syed et.al.|[2408.08302](http://arxiv.org/abs/2408.08302)|null|
|**2024-08-15**|**HELP: Hierarchical Embeddings-based Log Parsing**|Andy Xu et.al.|[2408.08300](http://arxiv.org/abs/2408.08300)|null|
|**2024-08-15**|**Autonomous Behavior Planning For Humanoid Loco-manipulation Through Grounded Language Model**|Jin Wang et.al.|[2408.08282](http://arxiv.org/abs/2408.08282)|null|
|**2024-08-15**|**DaRec: A Disentangled Alignment Framework for Large Language Model and Recommender System**|Xihong Yang et.al.|[2408.08231](http://arxiv.org/abs/2408.08231)|null|
|**2024-08-15**|**RED-CT: A Systems Design Methodology for Using LLM-labeled Data to Train and Deploy Edge Classifiers for Computational Social Science**|David Farr et.al.|[2408.08217](http://arxiv.org/abs/2408.08217)|null|
|**2024-08-16**|**Covert Bias: The Severity of Social Views' Unalignment in Language Models Towards Implicit and Explicit Opinion**|Abeer Aldayel et.al.|[2408.08212](http://arxiv.org/abs/2408.08212)|null|
|**2024-08-15**|**Does Reasoning Emerge? Examining the Probabilities of Causation in Large Language Models**|Javier González et.al.|[2408.08210](http://arxiv.org/abs/2408.08210)|null|
|**2024-08-15**|**LLM4DSR: Leveraing Large Language Model for Denoising Sequential Recommendation**|Bohao Wang et.al.|[2408.08208](http://arxiv.org/abs/2408.08208)|null|
|**2024-08-15**|**Scaling Up Natural Language Understanding for Multi-Robots Through the Lens of Hierarchy**|Shaojun Xu et.al.|[2408.08188](http://arxiv.org/abs/2408.08188)|null|
|**2024-08-14**|**The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models**|Karime Maamari et.al.|[2408.07702](http://arxiv.org/abs/2408.07702)|null|
|**2024-08-15**|**Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories, Applications and Opportunities**|Enneng Yang et.al.|[2408.07666](http://arxiv.org/abs/2408.07666)|**[link](https://github.com/ennengyang/awesome-model-merging-methods-theories-applications)**|
|**2024-08-14**|**Spoken Stereoset: On Evaluating Social Bias Toward Speaker in Speech Large Language Models**|Yi-Cheng Lin et.al.|[2408.07665](http://arxiv.org/abs/2408.07665)|**[link](https://github.com/dlion168/spoken_stereoset)**|
|**2024-08-14**|**Alignment-Enhanced Decoding:Defending via Token-Level Adaptive Refining of Probability Distributions**|Quan Liu et.al.|[2408.07663](http://arxiv.org/abs/2408.07663)|**[link](https://github.com/gigabaozi/aed)**|
|**2024-08-14**|**WeKnow-RAG: An Adaptive Approach for Retrieval-Augmented Generation Integrating Web Search and Knowledge Graphs**|Weijian Xie et.al.|[2408.07611](http://arxiv.org/abs/2408.07611)|null|
|**2024-08-14**|**Transformers and Large Language Models for Efficient Intrusion Detection Systems: A Comprehensive Survey**|Hamza Kheddar et.al.|[2408.07583](http://arxiv.org/abs/2408.07583)|null|
|**2024-08-15**|**MathScape: Evaluating MLLMs in multimodal Math Scenarios through a Hierarchical Benchmark**|Minxuan Zhou et.al.|[2408.07543](http://arxiv.org/abs/2408.07543)|**[link](https://github.com/PKU-Baichuan-MLSystemLab/MathScape)**|
|**2024-08-15**|**Usefulness of data flow diagrams and large language models for security threat validation: a registered report**|Winnie Bahati Mbaka et.al.|[2408.07537](http://arxiv.org/abs/2408.07537)|null|
|**2024-08-14**|**Development of a Multi-Agent Clinical Decision Support System for Korean Triage and Acuity Scale (KTAS)-Based Triage and Treatment Planning in Emergency Departments**|Seungjun Han et.al.|[2408.07531](http://arxiv.org/abs/2408.07531)|null|
|**2024-08-14**|**Large Language Models Know What Makes Exemplary Contexts**|Quanyu Long et.al.|[2408.07505](http://arxiv.org/abs/2408.07505)|null|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## Wireless Intelligence

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-08-19**|**PEDAL: Enhancing Greedy Decoding with Large Language Models using Diverse Exemplars**|Sumanth Prabhu et.al.|[2408.08869](http://arxiv.org/abs/2408.08869)|null|
|**2024-08-16**|**PsychoLex: Unveiling the Psychological Mind of Large Language Models**|Mohammad Amin Abbasi et.al.|[2408.08848](http://arxiv.org/abs/2408.08848)|null|
|**2024-08-16**|**FLEXTAF: Enhancing Table Reasoning with Flexible Tabular Formats**|Xuanliang Zhang et.al.|[2408.08841](http://arxiv.org/abs/2408.08841)|**[link](https://github.com/zhxlia/FLEXTAF)**|
|**2024-08-16**|**Artificial Intelligence and Strategic Decision-Making: Evidence from Entrepreneurs and Investors**|Felipe A. Csaszar et.al.|[2408.08811](http://arxiv.org/abs/2408.08811)|null|
|**2024-08-19**|**Constructing Domain-Specific Evaluation Sets for LLM-as-a-judge**|Ravi Raju et.al.|[2408.08808](http://arxiv.org/abs/2408.08808)|null|
|**2024-08-16**|**EmoDynamiX: Emotional Support Dialogue Strategy Prediction by Modelling MiXed Emotions and Discourse Dynamics**|Chenwei Wan et.al.|[2408.08782](http://arxiv.org/abs/2408.08782)|**[link](https://github.com/cw-wan/EmoDynamiX-v2)**|
|**2024-08-16**|**Evaluating the Evaluator: Measuring LLMs' Adherence to Task Evaluation Instructions**|Bhuvanashree Murugadoss et.al.|[2408.08781](http://arxiv.org/abs/2408.08781)|null|
|**2024-08-16**|**Large Language Models Might Not Care What You Are Saying: Prompt Format Beats Descriptions**|Chenming Tang et.al.|[2408.08780](http://arxiv.org/abs/2408.08780)|null|
|**2024-08-16**|**DAC: Decomposed Automation Correction for Text-to-SQL**|Dingzirui Wang et.al.|[2408.08779](http://arxiv.org/abs/2408.08779)|**[link](https://github.com/zirui-HIT/DAC)**|
|**2024-08-16**|**Lower Layer Matters: Alleviating Hallucination via Multi-Layer Fusion Contrastive Decoding with Truthfulness Refocused**|Dingwei Chen et.al.|[2408.08769](http://arxiv.org/abs/2408.08769)|null|
|**2024-08-15**|**Can Large Language Models Understand Symbolic Graphics Programs?**|Zeju Qiu et.al.|[2408.08313](http://arxiv.org/abs/2408.08313)|null|
|**2024-08-15**|**Benchmarking the Capabilities of Large Language Models in Transportation System Engineering: Accuracy, Consistency, and Reasoning Behaviors**|Usman Syed et.al.|[2408.08302](http://arxiv.org/abs/2408.08302)|null|
|**2024-08-15**|**HELP: Hierarchical Embeddings-based Log Parsing**|Andy Xu et.al.|[2408.08300](http://arxiv.org/abs/2408.08300)|null|
|**2024-08-15**|**Autonomous Behavior Planning For Humanoid Loco-manipulation Through Grounded Language Model**|Jin Wang et.al.|[2408.08282](http://arxiv.org/abs/2408.08282)|null|
|**2024-08-15**|**DaRec: A Disentangled Alignment Framework for Large Language Model and Recommender System**|Xihong Yang et.al.|[2408.08231](http://arxiv.org/abs/2408.08231)|null|
|**2024-08-15**|**RED-CT: A Systems Design Methodology for Using LLM-labeled Data to Train and Deploy Edge Classifiers for Computational Social Science**|David Farr et.al.|[2408.08217](http://arxiv.org/abs/2408.08217)|null|
|**2024-08-16**|**Covert Bias: The Severity of Social Views' Unalignment in Language Models Towards Implicit and Explicit Opinion**|Abeer Aldayel et.al.|[2408.08212](http://arxiv.org/abs/2408.08212)|null|
|**2024-08-15**|**Does Reasoning Emerge? Examining the Probabilities of Causation in Large Language Models**|Javier González et.al.|[2408.08210](http://arxiv.org/abs/2408.08210)|null|
|**2024-08-15**|**LLM4DSR: Leveraing Large Language Model for Denoising Sequential Recommendation**|Bohao Wang et.al.|[2408.08208](http://arxiv.org/abs/2408.08208)|null|
|**2024-08-15**|**Scaling Up Natural Language Understanding for Multi-Robots Through the Lens of Hierarchy**|Shaojun Xu et.al.|[2408.08188](http://arxiv.org/abs/2408.08188)|null|
|**2024-08-14**|**The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models**|Karime Maamari et.al.|[2408.07702](http://arxiv.org/abs/2408.07702)|null|
|**2024-08-15**|**Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories, Applications and Opportunities**|Enneng Yang et.al.|[2408.07666](http://arxiv.org/abs/2408.07666)|**[link](https://github.com/ennengyang/awesome-model-merging-methods-theories-applications)**|
|**2024-08-14**|**Spoken Stereoset: On Evaluating Social Bias Toward Speaker in Speech Large Language Models**|Yi-Cheng Lin et.al.|[2408.07665](http://arxiv.org/abs/2408.07665)|**[link](https://github.com/dlion168/spoken_stereoset)**|
|**2024-08-14**|**Alignment-Enhanced Decoding:Defending via Token-Level Adaptive Refining of Probability Distributions**|Quan Liu et.al.|[2408.07663](http://arxiv.org/abs/2408.07663)|**[link](https://github.com/gigabaozi/aed)**|
|**2024-08-14**|**WeKnow-RAG: An Adaptive Approach for Retrieval-Augmented Generation Integrating Web Search and Knowledge Graphs**|Weijian Xie et.al.|[2408.07611](http://arxiv.org/abs/2408.07611)|null|
|**2024-08-14**|**Transformers and Large Language Models for Efficient Intrusion Detection Systems: A Comprehensive Survey**|Hamza Kheddar et.al.|[2408.07583](http://arxiv.org/abs/2408.07583)|null|
|**2024-08-15**|**MathScape: Evaluating MLLMs in multimodal Math Scenarios through a Hierarchical Benchmark**|Minxuan Zhou et.al.|[2408.07543](http://arxiv.org/abs/2408.07543)|**[link](https://github.com/PKU-Baichuan-MLSystemLab/MathScape)**|
|**2024-08-15**|**Usefulness of data flow diagrams and large language models for security threat validation: a registered report**|Winnie Bahati Mbaka et.al.|[2408.07537](http://arxiv.org/abs/2408.07537)|null|
|**2024-08-14**|**Development of a Multi-Agent Clinical Decision Support System for Korean Triage and Acuity Scale (KTAS)-Based Triage and Treatment Planning in Emergency Departments**|Seungjun Han et.al.|[2408.07531](http://arxiv.org/abs/2408.07531)|null|
|**2024-08-14**|**Large Language Models Know What Makes Exemplary Contexts**|Quanyu Long et.al.|[2408.07505](http://arxiv.org/abs/2408.07505)|null|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## Communication Intelligence

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-09-21**|**LLM Agents as 6G Orchestrator: A Paradigm for Task-Oriented Physical-Layer Automation**|Zhuoran Xiao et.al.|[2410.03688](http://arxiv.org/abs/2410.03688)|null|生成式预训练模型的快速发展正在推动技术进步从基础应用（如聊天机器人）向更复杂的基于代理的系统转变。将6G系统与大型语言模型（LLM）代理和数字孪生（DT）相结合，具有巨大的潜力和必要性，以管理具有新出现功能（如原生AI服务和感知）的高度复杂通信系统。通过6G导向的代理，基站可以理解各种动态上层任务的传输需求，自动编排最优系统工作流程。通过不断从6G DT获取反馈进行强化，代理最终可以相应地提高实际系统的性能。与为通用应用设计的现有LLM代理不同，6G导向的代理旨在利用大量的额外专业知识进行高度严谨和精确的规划，这不可避免地需要从模型训练到实施的特定系统设计。本文提出了一种构建面向任务的6G LLM代理的新综合方法。我们首先提出一个两阶段持续预训练和微调方案，以建立领域基础模型和多种专门化专家模型，以满足各种应用场景的需求。此外，还提出了一个基于语义检索的新推理框架，以利用现有的通信相关功能。物理层任务分解等示例任务的实验结果表明了所提范式的可行性和有效性。|
|**2024-08-19**|**Demystifying the Communication Characteristics for Distributed Transformer Models**|Quentin Anthony et.al.|[2408.10197](http://arxiv.org/abs/2408.10197)|null|
|**2024-08-19**|**Customizing Language Models with Instance-wise LoRA for Sequential Recommendation**|Xiaoyu Kong et.al.|[2408.10159](http://arxiv.org/abs/2408.10159)|null|
|**2024-08-19**|**Multilingual Needle in a Haystack: Investigating Long-Context Behavior of Multilingual Large Language Models**|Amey Hengle et.al.|[2408.10151](http://arxiv.org/abs/2408.10151)|**[link](https://github.com/AmeyHengle/multilingual-needle-in-a-haystack)**|
|**2024-08-19**|**Instruction Finetuning for Leaderboard Generation from Empirical AI Research**|Salomon Kabongo et.al.|[2408.10141](http://arxiv.org/abs/2408.10141)|null|
|**2024-08-19**|**Molecular Graph Representation Learning Integrating Large Language Models with Domain-specific Small Models**|Tianyu Zhang et.al.|[2408.10124](http://arxiv.org/abs/2408.10124)|**[link](https://github.com/zhangtia16/molgraph-lardo)**|
|**2024-08-19**|**ARMADA: Attribute-Based Multimodal Data Augmentation**|Xiaomeng Jin et.al.|[2408.10086](http://arxiv.org/abs/2408.10086)|null|
|**2024-08-19**|**Privacy Checklist: Privacy Violation Detection Grounding on Contextual Integrity Theory**|Haoran Li et.al.|[2408.10053](http://arxiv.org/abs/2408.10053)|null|
|**2024-08-19**|**MSDiagnosis: An EMR-based Dataset for Clinical Multi-Step Diagnosis**|Ruihui Hou et.al.|[2408.10039](http://arxiv.org/abs/2408.10039)|null|
|**2024-08-19**|**TBA: Faster Large Language Model Training Using SSD-Based Activation Offloading**|Kun Wu et.al.|[2408.10013](http://arxiv.org/abs/2408.10013)|null|
|**2024-08-19**|**Application of Large Language Models in Automated Question Generation: A Case Study on ChatGLM's Structured Questions for National Teacher Certification Exams**|Yanxin Chen et.al.|[2408.09982](http://arxiv.org/abs/2408.09982)|null|
|**2024-08-16**|**PEDAL: Enhancing Greedy Decoding with Large Language Models using Diverse Exemplars**|Sumanth Prabhu et.al.|[2408.08869](http://arxiv.org/abs/2408.08869)|null|
|**2024-08-16**|**PsychoLex: Unveiling the Psychological Mind of Large Language Models**|Mohammad Amin Abbasi et.al.|[2408.08848](http://arxiv.org/abs/2408.08848)|null|
|**2024-08-16**|**FLEXTAF: Enhancing Table Reasoning with Flexible Tabular Formats**|Xuanliang Zhang et.al.|[2408.08841](http://arxiv.org/abs/2408.08841)|**[link](https://github.com/zhxlia/FLEXTAF)**|
|**2024-08-16**|**Artificial Intelligence and Strategic Decision-Making: Evidence from Entrepreneurs and Investors**|Felipe A. Csaszar et.al.|[2408.08811](http://arxiv.org/abs/2408.08811)|null|
|**2024-08-16**|**Constructing Domain-Specific Evaluation Sets for LLM-as-a-judge**|Ravi Raju et.al.|[2408.08808](http://arxiv.org/abs/2408.08808)|null|
|**2024-08-16**|**EmoDynamiX: Emotional Support Dialogue Strategy Prediction by Modelling MiXed Emotions and Discourse Dynamics**|Chenwei Wan et.al.|[2408.08782](http://arxiv.org/abs/2408.08782)|**[link](https://github.com/cw-wan/EmoDynamiX-v2)**|
|**2024-08-16**|**Evaluating the Evaluator: Measuring LLMs' Adherence to Task Evaluation Instructions**|Bhuvanashree Murugadoss et.al.|[2408.08781](http://arxiv.org/abs/2408.08781)|null|
|**2024-08-16**|**Large Language Models Might Not Care What You Are Saying: Prompt Format Beats Descriptions**|Chenming Tang et.al.|[2408.08780](http://arxiv.org/abs/2408.08780)|null|
|**2024-08-16**|**DAC: Decomposed Automation Correction for Text-to-SQL**|Dingzirui Wang et.al.|[2408.08779](http://arxiv.org/abs/2408.08779)|**[link](https://github.com/zirui-HIT/DAC)**|
|**2024-08-16**|**Lower Layer Matters: Alleviating Hallucination via Multi-Layer Fusion Contrastive Decoding with Truthfulness Refocused**|Dingwei Chen et.al.|[2408.08769](http://arxiv.org/abs/2408.08769)|null|
|**2024-08-15**|**Can Large Language Models Understand Symbolic Graphics Programs?**|Zeju Qiu et.al.|[2408.08313](http://arxiv.org/abs/2408.08313)|null|
|**2024-08-15**|**ScalingFilter: Assessing Data Quality through Inverse Utilization of Scaling Laws**|Ruihang Li et.al.|[2408.08310](http://arxiv.org/abs/2408.08310)|null|
|**2024-08-15**|**Benchmarking the Capabilities of Large Language Models in Transportation System Engineering: Accuracy, Consistency, and Reasoning Behaviors**|Usman Syed et.al.|[2408.08302](http://arxiv.org/abs/2408.08302)|null|
|**2024-08-15**|**HELP: Hierarchical Embeddings-based Log Parsing**|Andy Xu et.al.|[2408.08300](http://arxiv.org/abs/2408.08300)|null|
|**2024-08-15**|**The ShareLM Collection and Plugin: Contributing Human-Model Chats for the Benefit of the Community**|Shachar Don-Yehiya et.al.|[2408.08291](http://arxiv.org/abs/2408.08291)|null|
|**2024-08-15**|**Autonomous Behavior Planning For Humanoid Loco-manipulation Through Grounded Language Model**|Jin Wang et.al.|[2408.08282](http://arxiv.org/abs/2408.08282)|null|
|**2024-08-15**|**BAM! Just Like That: Simple and Efficient Parameter Upcycling for Mixture of Experts**|Qizhen Zhang et.al.|[2408.08274](http://arxiv.org/abs/2408.08274)|null|
|**2024-08-15**|**DaRec: A Disentangled Alignment Framework for Large Language Model and Recommender System**|Xihong Yang et.al.|[2408.08231](http://arxiv.org/abs/2408.08231)|null|
|**2024-08-15**|**RED-CT: A Systems Design Methodology for Using LLM-labeled Data to Train and Deploy Edge Classifiers for Computational Social Science**|David Farr et.al.|[2408.08217](http://arxiv.org/abs/2408.08217)|null|
|**2024-08-16**|**Covert Bias: The Severity of Social Views' Unalignment in Language Models Towards Implicit and Explicit Opinion**|Abeer Aldayel et.al.|[2408.08212](http://arxiv.org/abs/2408.08212)|null|
|**2024-08-15**|**Does Reasoning Emerge? Examining the Probabilities of Causation in Large Language Models**|Javier González et.al.|[2408.08210](http://arxiv.org/abs/2408.08210)|null|
|**2024-08-15**|**LLM4DSR: Leveraing Large Language Model for Denoising Sequential Recommendation**|Bohao Wang et.al.|[2408.08208](http://arxiv.org/abs/2408.08208)|null|
|**2024-08-15**|**Scaling Up Natural Language Understanding for Multi-Robots Through the Lens of Hierarchy**|Shaojun Xu et.al.|[2408.08188](http://arxiv.org/abs/2408.08188)|null|
|**2024-08-14**|**The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models**|Karime Maamari et.al.|[2408.07702](http://arxiv.org/abs/2408.07702)|null|
|**2024-08-14**|**On the Parameter Selection of Phase-transmittance Radial Basis Function Neural Networks for Communication Systems**|Jonathan A. Soares et.al.|[2408.07692](http://arxiv.org/abs/2408.07692)|null|
|**2024-08-14**|**Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories, Applications and Opportunities**|Enneng Yang et.al.|[2408.07666](http://arxiv.org/abs/2408.07666)|**[link](https://github.com/ennengyang/awesome-model-merging-methods-theories-applications)**|
|**2024-08-14**|**Spoken Stereoset: On Evaluating Social Bias Toward Speaker in Speech Large Language Models**|Yi-Cheng Lin et.al.|[2408.07665](http://arxiv.org/abs/2408.07665)|**[link](https://github.com/dlion168/spoken_stereoset)**|
|**2024-08-14**|**Alignment-Enhanced Decoding:Defending via Token-Level Adaptive Refining of Probability Distributions**|Quan Liu et.al.|[2408.07663](http://arxiv.org/abs/2408.07663)|**[link](https://github.com/gigabaozi/aed)**|
|**2024-08-14**|**WeKnow-RAG: An Adaptive Approach for Retrieval-Augmented Generation Integrating Web Search and Knowledge Graphs**|Weijian Xie et.al.|[2408.07611](http://arxiv.org/abs/2408.07611)|null|
|**2024-08-14**|**Transformers and Large Language Models for Efficient Intrusion Detection Systems: A Comprehensive Survey**|Hamza Kheddar et.al.|[2408.07583](http://arxiv.org/abs/2408.07583)|null|
|**2024-08-14**|**MathScape: Evaluating MLLMs in multimodal Math Scenarios through a Hierarchical Benchmark**|Minxuan Zhou et.al.|[2408.07543](http://arxiv.org/abs/2408.07543)|**[link](https://github.com/PKU-Baichuan-MLSystemLab/MathScape)**|
|**2024-08-14**|**Usefulness of data flow diagrams and large language models for security threat validation: a registered report**|Winnie Bahati Mbaka et.al.|[2408.07537](http://arxiv.org/abs/2408.07537)|null|
|**2024-08-14**|**Development of a Multi-Agent Clinical Decision Support System for Korean Triage and Acuity Scale (KTAS)-Based Triage and Treatment Planning in Emergency Departments**|Seungjun Han et.al.|[2408.07531](http://arxiv.org/abs/2408.07531)|null|
|**2024-10-22**|**Designing Network Algorithms via Large Language Models**|Zhiyuan He et.al.|[2404.01617](http://arxiv.org/abs/2404.01617)|**[link](https://github.com/hzy46/nada)**|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## RAG

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-24**|**LoRANN: Low-Rank Matrix Factorization for Approximate Nearest Neighbor Search**|Elias Jääsaari et.al.|[2410.18926](http://arxiv.org/abs/2410.18926)|**[link](https://github.com/ejaasaari/lorann)**|**近似最近邻（ANN）搜索是许多现代机器学习流水线中的关键组成部分；最近的使用案例包括检索增强生成（RAG）和向量数据库。基于聚类的ANN算法，使用基于乘积量化（PQ）的评分计算方法，在工业规模应用中由于其可扩展性和适用于分布式及磁盘实现而经常被采用。然而，与领先的基于图的ANN算法相比，它们的查询时间较慢。在这项工作中，我们提出了一种新的监督评分计算方法，基于内积近似是一个可以由降秩回归高效解决的多变量（多输出）回归问题这一观察。实验表明，在现代高维数据集上，所提出的降秩回归（RRR）方法在查询延迟和内存使用方面均优于PQ。我们还介绍了LoRANN，这是一种利用所提出的评分计算方法的基于聚类的ANN库。LoRANN能够与领先的基于图的算法竞争，并在高维数据集上超越了最先进的GPU ANN方法。**|
|**2024-10-24**|**An LLM Agent for Automatic Geospatial Data Analysis**|Yuxing Chen et.al.|[2410.18792](http://arxiv.org/abs/2410.18792)|null|大型语言模型（LLM）正在被用于数据科学代码生成任务，但它们在处理复杂顺序任务时经常遇到逻辑错误。将这些模型应用于地理空间数据处理尤其具有挑战性，因为难以整合复杂的数据结构和空间约束、有效利用多样的函数调用，并且容易产生对较少使用的地理空间库的幻觉。为了解决这些问题，我们引入了GeoAgent，这是一种新的交互式框架，旨在帮助LLM更有效地处理地理空间数据处理。GeoAgent开创性地将代码解释器、静态分析和检索增强生成（RAG）技术集成到蒙特卡洛树搜索（MCTS）算法中，为地理空间数据处理提供了一种新方法。此外，我们还贡献了一个专门为评估基于LLM的方法在地理空间任务中的表现而设计的新基准。该基准利用了多种Python库，包括单轮和多轮任务，如数据获取、数据分析和可视化。通过在多样化的地理空间情境中进行全面评估，这一基准为开发基于LLM的方法在地理空间数据分析任务中设定了新的标准。我们的研究结果表明，仅依靠LLM的知识不足以准确完成地理空间任务编程，这需要连贯的多步骤过程和多次函数调用。与基线LLM相比，提出的GeoAgent表现出色，在函数调用和任务完成方面取得了显著改进。此外，这些结果为未来开发自动地理空间数据分析任务编程的LLM代理提供了宝贵的见解。|
|**2024-10-24**|**Bielik 7B v0.1: A Polish Language Model -- Development, Insights, and Evaluation**|Krzysztof Ociepa et.al.|[2410.18565](http://arxiv.org/abs/2410.18565)|null|我们推出了Bielik 7B v0.1，这是一个拥有70亿参数的生成式文本模型，专门用于波兰语语言处理。该模型在精心策划的波兰语文本库上进行训练，通过创新技术解决了语言模型开发中的关键挑战。这些技术包括加权指令交叉熵损失，它平衡了不同类型指令的学习，以及自适应学习率，它根据训练进展动态调整学习率。为了评估性能，我们创建了Open PL LLM排行榜和波兰MT-Bench，这是评估各种自然语言处理任务和对话能力的新框架。Bielik 7B v0.1表现出显著的改进，在RAG阅读任务中比Mistral-7B-v0.1平均得分提高了9个百分点。它在波兰MT-Bench中也表现出色，特别是在推理（6.15/10）和角色扮演（7.83/10）类别中。这一模型代表了波兰语人工智能的重大进步，为多样化的语言应用提供了强大的工具，并在该领域设定了新的基准。|
|**2024-10-24**|**Aggregated Knowledge Model: Enhancing Domain-Specific QA with Fine-Tuned and Retrieval-Augmented Generation Models**|Fengchen Liu et.al.|[2410.18344](http://arxiv.org/abs/2410.18344)|null|本文介绍了一种增强封闭领域问答系统（QA）的新方法，重点满足劳伦斯伯克利国家实验室（LBL）科学信息技术（ScienceIT）领域的特定需求。通过利用从ScienceIT文档中提取的丰富数据集，我们的研究详细比较了两个微调的大规模语言模型和五个检索增强生成（RAG）模型。通过数据处理技术，我们将文档转换为结构化的上下文-问题-答案三元组，并利用最新的大规模语言模型（AWS Bedrock、GCP PaLM2、Meta LLaMA2、OpenAI GPT-4、Google Gemini-Pro）进行数据驱动的洞察。此外，我们引入了聚合知识模型（AKM），该模型通过K-means聚类从上述七个模型中选择最具代表性的答案来综合响应。通过对这些模型在多个指标上的评估，全面展示了它们在LBL ScienceIT环境中的有效性和适用性。结果表明，结合微调和检索增强策略具有潜在优势，特别是在使用AKM时实现了显著的性能提升。本研究获得的见解可以应用于开发针对特定领域的专门QA系统。|
|**2024-10-23**|**LongRAG: A Dual-Perspective Retrieval-Augmented Generation Paradigm for Long-Context Question Answering**|Qingfei Zhao et.al.|[2410.18050](http://arxiv.org/abs/2410.18050)|**[link](https://github.com/qingfei1/longrag)**|**长上下文问答（LCQA）是一项具有挑战性的任务，旨在通过对长上下文文档的推理来提供准确的答案。现有的用于LCQA的长上下文大型语言模型（LLMs）常常遇到“中间迷失”的问题。检索增强生成（RAG）通过提供外部事实证据缓解了这一问题。然而，其分块策略破坏了全局长上下文信息，并且在长上下文中的低质量检索阻碍了LLMs识别有效的事实细节，因为存在大量噪音。为此，我们提出了LongRAG，这是一种通用的、双视角的、鲁棒的基于LLM的RAG系统范式，用于LCQA，以增强RAG对复杂长上下文知识（即全局信息和事实细节）的理解。我们将LongRAG设计为即插即用的范式，便于适应各种领域和LLMs。在三个多跳数据集上的广泛实验表明，LongRAG显著优于长上下文LLMs（提高了6.94%）、先进的RAG（提高了6.16%）以及原始RAG（提高了17.25%）。此外，我们进行了定量消融研究和多维度分析，突出了系统组件和微调策略的有效性。数据和代码可在https://github.com/QingFei1/LongRAG获取。**|
|**2024-10-23**|**SimRAG: Self-Improving Retrieval-Augmented Generation for Adapting Large Language Models to Specialized Domains**|Ran Xu et.al.|[2410.17952](http://arxiv.org/abs/2410.17952)|null|检索增强生成（RAG）通过整合外部知识来增强大型语言模型（LLM）的问题回答（QA）能力。然而，将通用的RAG系统适应于科学和医学等专业领域面临着独特的挑战，这主要是由于分布偏移以及领域特定数据的有限访问性。为了解决这个问题，我们提出了SimRAG，这是一种自我训练方法，使LLM具备问题回答和问题生成的联合能力，以实现领域适应。我们的方法首先在指令跟随、问题回答和搜索相关数据上对LLM进行微调。然后，它提示同一个LLM从未标记的语料库中生成多样化的领域相关问题，并采用额外的过滤策略保留高质量的合成示例。通过利用这些合成示例，LLM可以在领域特定的RAG任务上提高其性能。在11个数据集上的实验表明，涵盖两个骨干规模和三个领域，SimRAG相比基线方法提高了1.2%至8.6%。|
|**2024-10-23**|**Leveraging the Domain Adaptation of Retrieval Augmented Generation Models for Question Answering and Reducing Hallucination**|Salman Rakin et.al.|[2410.17783](http://arxiv.org/abs/2410.17783)|null|尽管大型语言模型在各种自然语言处理任务中取得了显著的成功，但检索增强生成模型在诸如问答等下游应用中表现出特别的有效性。最近，RAG-end2end模型进一步优化了架构，在领域适应方面实现了显著的性能提升。然而，当这些基于RAG的架构被微调应用于客户服务等专业领域以构建可靠的对话AI系统时，其有效性仍相对未被充分探索。此外，减少幻觉发生同时保持高领域的特定准确性仍然是一个关键挑战。在这篇论文中，我们通过领域适应研究了不同RAG和类似RAG架构的表现，并评估了它们根据上下文知识库生成准确且相关响应的能力。为了便于对模型进行评估，我们构建了一个名为HotelConvQA的新数据集，该数据集来源于广泛的酒店相关对话，并将所有模型在我们的领域特定数据集上进行了微调。我们还解决了先前工作中未得到适当衡量的一个重要研究空白：确定领域适应对减少不同RAG架构中幻觉的影响。我们的评估表明，通过采用领域适应，在所有指标上均获得了积极的结果，展示了在问答任务上的强大表现，并提供了关于其在减少幻觉方面的有效性的见解。我们的发现清楚地表明，领域适应不仅提高了模型在问答任务上的表现，而且显著减少了所有评估过的RAG架构中的幻觉现象。|
|**2024-10-23**|**An Adaptive Framework for Generating Systematic Explanatory Answer in Online Q&A Platforms**|Ziyang Chen et.al.|[2410.17694](http://arxiv.org/abs/2410.17694)|**[link](https://github.com/czy1999/synthrag)**|**问答系统在处理需要跨领域知识综合的复杂问题时面临挑战。虽然朴素的RAG模型在信息检索方面表现出色，但在生成全面且深入的答案方面仍显不足。为了解决这些问题，我们定义了一个开创性的任务——解释性答案生成，该任务旨在应对诸如要求信息全面性和逻辑连贯性等挑战。为了应对这些难题，我们参考了系统思维理论，提出了SynthRAG这一创新框架，以提升问答系统的性能。SynthRAG通过采用自适应提纲进行动态内容结构化、生成系统化的信息以确保详细覆盖，并产生针对特定用户查询定制的答案，从而改进了传统模型。这种结构化的方法保证了逻辑连贯性和信息的充分整合，生成既深刻又条理清晰的回答。实证评估表明，SynthRAG在处理复杂问题方面表现出色，克服了朴素RAG模型的局限性，显著提高了答案的质量和深度。此外，在知乎平台上的在线部署显示，SynthRAG生成的答案平均获得5.73个赞同票，超过了79.8%的人类贡献者的表现，突出了所提框架的实际相关性和影响力。我们的代码可从https://github.com/czy1999/SynthRAG 获取。**|
|**2024-10-23**|**Graphusion: A RAG Framework for Knowledge Graph Construction with a Global Perspective**|Rui Yang et.al.|[2410.17600](http://arxiv.org/abs/2410.17600)|null|知识图谱（KGs）在人工智能领域至关重要，并广泛应用于诸如问答（QA）等下游任务中。构建知识图谱通常需要领域专家的大量努力。最近，大型语言模型（LLMs）已被用于知识图谱构建（KGC）。然而，大多数现有方法侧重于局部视角，从单个句子或文档中提取知识三元组，缺乏将这些知识融合到全局知识图谱中的过程。本文介绍了Graphusion，这是一种从自由文本进行零样本知识图谱构建的框架。它包含三个步骤：第一步，我们使用主题建模提取一系列种子实体，以指导最终的知识图谱包含最相关的实体；第二步，我们利用大型语言模型进行候选三元组提取；第三步，我们设计了一种新颖的融合模块，提供所提取知识的全局视图，包括实体合并、冲突解决和新三元组发现。结果显示，Graphusion在实体提取和关系识别方面的得分分别为2.92分和2.37分（满分3分）。此外，我们展示了如何将Graphusion应用于自然语言处理（NLP）领域，并在一个教育场景中进行了验证。具体来说，我们引入了TutorQA，这是一个新的由专家验证的问答基准，包含六个任务和总计1,200对问答。利用Graphusion构建的知识图谱，我们在该基准上实现了显著的性能提升，例如，在子图补全任务上的准确率提高了9.2%。|
|**2024-10-22**|**IPL: Leveraging Multimodal Large Language Models for Intelligent Product Listing**|Kang Chen et.al.|[2410.16977](http://arxiv.org/abs/2410.16977)|null|与专业的商业对消费者（B2C）电商平台（如亚马逊）不同，消费者对消费者（C2C）平台（如Facebook Marketplace）主要面向通常缺乏足够电商经验的个人卖家。个人卖家往往难以撰写合适的产品描述。随着多模态大语言模型（MLLMs）的最新进展，我们尝试将这种尖端的生成式人工智能技术整合到产品发布过程中。为此，我们开发了IPL，一种智能产品列表工具，能够利用各种产品属性（如类别、品牌、颜色、状况等）来生成描述。IPL使用户只需上传待售产品的照片即可编写产品描述。更重要的是，它能够模仿我们C2C平台闲鱼的内容风格。这是通过在MLLM上进行领域特定的指令微调并采用多模态检索增强生成（RAG）过程实现的。全面的经验评估表明，IPL的基础模型在领域特定任务上的表现显著优于基线模型，并且产生的幻觉更少。IPL已经成功部署到我们的生产系统中，在该系统中72%的用户基于生成的内容发布了他们的产品列表，这些产品列表的质量评分比没有AI辅助的产品列表高出5.6%。|
|**2024-10-22**|**DNAHLM -- DNA sequence and Human Language mixed large language Model**|Wang Liang et.al.|[2410.16917](http://arxiv.org/abs/2410.16917)|**[link](https://github.com/maris205/dnahl)**|
|**2024-10-22**|**Trustworthy Alignment of Retrieval-Augmented Large Language Models via Reinforcement Learning**|Zongmeng Zhang et.al.|[2410.16843](http://arxiv.org/abs/2410.16843)|**[link](https://github.com/zmzhang2000/trustworthy-alignment)**|
|**2024-10-22**|**Distill-SynthKG: Distilling Knowledge Graph Synthesis Workflow for Improved Coverage and Efficiency**|Prafulla Kumar Choubey et.al.|[2410.16597](http://arxiv.org/abs/2410.16597)|null|
|**2024-10-22**|**ViMGuard: A Novel Multi-Modal System for Video Misinformation Guarding**|Andrew Kan et.al.|[2410.16592](http://arxiv.org/abs/2410.16592)|null|
|**2024-10-21**|**Towards a Reliable Offline Personal AI Assistant for Long Duration Spaceflight**|Oliver Bensch et.al.|[2410.16397](http://arxiv.org/abs/2410.16397)|null|
|**2024-10-21**|**Building A Coding Assistant via the Retrieval-Augmented Language Model**|Xinze Li et.al.|[2410.16229](http://arxiv.org/abs/2410.16229)|**[link](https://github.com/NEUIR/CONAN)**|
|**2024-10-21**|**Developing Retrieval Augmented Generation (RAG) based LLM Systems from PDFs: An Experience Report**|Ayman Asad Khan et.al.|[2410.15944](http://arxiv.org/abs/2410.15944)|**[link](https://github.com/gpt-laboratory/rag-llm-development-guidebook-from-pdfs)**|
|**2024-10-21**|**Using GPT Models for Qualitative and Quantitative News Analytics in the 2024 US Presidental Election Process**|Bohdan M. Pavlyshenko et.al.|[2410.15884](http://arxiv.org/abs/2410.15884)|null|
|**2024-10-21**|**RAG4ITOps: A Supervised Fine-Tunable and Comprehensive RAG Framework for IT Operations and Maintenance**|Tianyang Zhang et.al.|[2410.15805](http://arxiv.org/abs/2410.15805)|null|
|**2024-10-21**|**Improve Dense Passage Retrieval with Entailment Tuning**|Lu Dai et.al.|[2410.15801](http://arxiv.org/abs/2410.15801)|null|
|**2024-10-21**|**Who's Who: Large Language Models Meet Knowledge Conflicts in Practice**|Quang Hieu Pham et.al.|[2410.15737](http://arxiv.org/abs/2410.15737)|**[link](https://github.com/vinairesearch/whoqa)**|
|**2024-10-21**|**RAC: Efficient LLM Factuality Correction with Retrieval Augmentation**|Changmao Li et.al.|[2410.15667](http://arxiv.org/abs/2410.15667)|**[link](https://github.com/jlab-nlp/retrieval-augmented-correction)**|
|**2024-10-21**|**DRIM-ANN: An Approximate Nearest Neighbor Search Engine based on Commercial DRAM-PIMs**|Mingkai Chen et.al.|[2410.15621](http://arxiv.org/abs/2410.15621)|null|
|**2024-10-21**|**Leveraging Retrieval-Augmented Generation for Culturally Inclusive Hakka Chatbots: Design Insights and User Perceptions**|Chen-Chi Chang et.al.|[2410.15572](http://arxiv.org/abs/2410.15572)|null|
|**2024-10-20**|**Do RAG Systems Cover What Matters? Evaluating and Optimizing Responses with Sub-Question Coverage**|Kaige Xie et.al.|[2410.15531](http://arxiv.org/abs/2410.15531)|null|
|**2024-10-18**|**Real-time Fake News from Adversarial Feedback**|Sanxing Chen et.al.|[2410.14651](http://arxiv.org/abs/2410.14651)|null|
|**2024-10-18**|**Toolshed: Scale Tool-Equipped Agents with Advanced RAG-Tool Fusion and Tool Knowledge Bases**|Elias Lumer et.al.|[2410.14594](http://arxiv.org/abs/2410.14594)|null|
|**2024-10-18**|**RAG-ConfusionQA: A Benchmark for Evaluating LLMs on Confusing Questions**|Zhiyuan Peng et.al.|[2410.14567](http://arxiv.org/abs/2410.14567)|null|
|**2024-10-18**|**Backdoored Retrievers for Prompt Injection Attacks on Retrieval Augmented Generation of Large Language Models**|Cody Clop et.al.|[2410.14479](http://arxiv.org/abs/2410.14479)|null|
|**2024-10-18**|**Agents4PLC: Automating Closed-loop PLC Code Generation and Verification in Industrial Control Systems using LLM-based Agents**|Zihan Liu et.al.|[2410.14209](http://arxiv.org/abs/2410.14209)|null|
|**2024-10-18**|**Optimizing Retrieval-Augmented Generation with Elasticsearch for Enhanced Question-Answering Systems**|Jiajing Chen et.al.|[2410.14167](http://arxiv.org/abs/2410.14167)|null|
|**2024-10-17**|**Towards Cross-Cultural Machine Translation with Retrieval-Augmented Generation from Multilingual Knowledge Graphs**|Simone Conia et.al.|[2410.14057](http://arxiv.org/abs/2410.14057)|null|
|**2024-10-17**|**MIRAGE-Bench: Automatic Multilingual Benchmark Arena for Retrieval-Augmented Generation Systems**|Nandan Thakur et.al.|[2410.13716](http://arxiv.org/abs/2410.13716)|**[link](https://github.com/vectara/mirage-bench)**|
|**2024-10-17**|**HEALTH-PARIKSHA: Assessing RAG Models for Health Chatbots in Real-World Multilingual Settings**|Varun Gumma et.al.|[2410.13671](http://arxiv.org/abs/2410.13671)|null|
|**2024-10-17**|**Integrating Temporal Representations for Dynamic Memory Retrieval and Management in Large Language Models**|Yuki Hou et.al.|[2410.13553](http://arxiv.org/abs/2410.13553)|null|
|**2024-10-17**|**LLM-based Unit Test Generation via Property Retrieval**|Zhe Zhang et.al.|[2410.13542](http://arxiv.org/abs/2410.13542)|null|
|**2024-10-17**|**GeoCoder: Solving Geometry Problems by Generating Modular Code through Vision-Language Models**|Aditya Sharma et.al.|[2410.13510](http://arxiv.org/abs/2410.13510)|null|
|**2024-10-17**|**RAG-DDR: Optimizing Retrieval-Augmented Generation Using Differentiable Data Rewards**|Xinze Li et.al.|[2410.13509](http://arxiv.org/abs/2410.13509)|**[link](https://github.com/openmatch/rag-ddr)**|
|**2024-10-17**|**Probing-RAG: Self-Probing to Guide Language Models in Selective Document Retrieval**|Ingeol Baek et.al.|[2410.13339](http://arxiv.org/abs/2410.13339)|null|
|**2024-10-17**|**Comparing the Utility, Preference, and Performance of Course Material Search Functionality and Retrieval-Augmented Generation Large Language Model (RAG-LLM) AI Chatbots in Information-Seeking Tasks**|Leonardo Pasquarelli et.al.|[2410.13326](http://arxiv.org/abs/2410.13326)|null|
|**2024-10-17**|**SBI-RAG: Enhancing Math Word Problem Solving for Students through Schema-Based Instruction and Retrieval-Augmented Generation**|Prakhar Dixit et.al.|[2410.13293](http://arxiv.org/abs/2410.13293)|null|
|**2024-10-17**|**FRAG: Toward Federated Vector Database Management for Collaborative and Secure Retrieval-Augmented Generation**|Dongfang Zhao et.al.|[2410.13272](http://arxiv.org/abs/2410.13272)|null|
|**2024-10-16**|**Meta-Chunking: Learning Efficient Text Segmentation via Logical Perception**|Jihao Zhao et.al.|[2410.12788](http://arxiv.org/abs/2410.12788)|**[link](https://github.com/IAAR-Shanghai/Meta-Chunking)**|
|**2024-10-17**|**MedAide: Towards an Omni Medical Aide via Specialized LLM-based Multi-Agent Collaboration**|Jinjie Wei et.al.|[2410.12532](http://arxiv.org/abs/2410.12532)|null|
|**2024-10-17**|**Aegis:An Advanced LLM-Based Multi-Agent for Intelligent Functional Safety Engineering**|Lu Shi et.al.|[2410.12475](http://arxiv.org/abs/2410.12475)|null|
|**2024-10-16**|**Evaluation of Attribution Bias in Retrieval-Augmented Large Language Models**|Amin Abolghasemi et.al.|[2410.12380](http://arxiv.org/abs/2410.12380)|null|
|**2024-10-16**|**CoFE-RAG: A Comprehensive Full-chain Evaluation Framework for Retrieval-Augmented Generation with Enhanced Data Diversity**|Jintao Liu et.al.|[2410.12248](http://arxiv.org/abs/2410.12248)|**[link](https://github.com/Alibaba-NLP/CoFE-RAG)**|
|**2024-10-15**|**De-jargonizing Science for Journalists with GPT-4: A Pilot Study**|Sachita Nishal et.al.|[2410.12069](http://arxiv.org/abs/2410.12069)|**[link](https://github.com/ericlee878/ScienceDeJargonizer)**|
|**2024-10-15**|**Holistic Reasoning with Long-Context LMs: A Benchmark for Database Operations on Massive Textual Data**|Seiji Maekawa et.al.|[2410.11996](http://arxiv.org/abs/2410.11996)|null|
|**2024-10-15**|**Retrieval Augmented Spelling Correction for E-Commerce Applications**|Xuan Guo et.al.|[2410.11655](http://arxiv.org/abs/2410.11655)|null|
|**2024-10-16**|**Revisiting Benchmark and Assessment: An Agent-based Exploratory Dynamic Evaluation Framework for LLMs**|Wanying Wang et.al.|[2410.11507](http://arxiv.org/abs/2410.11507)|null|
|**2024-10-15**|**DynamicER: Resolving Emerging Mentions to Dynamic Entities for RAG**|Jinyoung Kim et.al.|[2410.11494](http://arxiv.org/abs/2410.11494)|null|
|**2024-10-15**|**AIC CTU system at AVeriTeC: Re-framing automated fact-checking as a simple RAG task**|Herbert Ullrich et.al.|[2410.11446](http://arxiv.org/abs/2410.11446)|**[link](https://github.com/aic-factcheck/aic_averitec)**|
|**2024-10-15**|**ReDeEP: Detecting Hallucination in Retrieval-Augmented Generation via Mechanistic Interpretability**|Zhongxiang Sun et.al.|[2410.11414](http://arxiv.org/abs/2410.11414)|null|
|**2024-10-15**|**Synthetic Interlocutors. Experiments with Generative AI to Prolong Ethnographic Encounters**|Johan Irving Søltoft et.al.|[2410.11395](http://arxiv.org/abs/2410.11395)|null|
|**2024-10-15**|**Self-adaptive Multimodal Retrieval-Augmented Generation**|Wenjia Zhai et.al.|[2410.11321](http://arxiv.org/abs/2410.11321)|**[link](https://github.com/sam-rag/sam_rag)**|
|**2024-10-15**|**SEER: Self-Aligned Evidence Extraction for Retrieval-Augmented Generation**|Xinping Zhao et.al.|[2410.11315](http://arxiv.org/abs/2410.11315)|null|
|**2024-10-15**|**On the Capacity of Citation Generation by Large Language Models**|Haosheng Qian et.al.|[2410.11217](http://arxiv.org/abs/2410.11217)|null|
|**2024-10-15**|**Athena: Retrieval-augmented Legal Judgment Prediction with Large Language Models**|Xiao Peng et.al.|[2410.11195](http://arxiv.org/abs/2410.11195)|null|
|**2024-10-14**|**When Does Perceptual Alignment Benefit Vision Representations?**|Shobhita Sundaram et.al.|[2410.10817](http://arxiv.org/abs/2410.10817)|null|
|**2024-10-14**|**VisRAG: Vision-based Retrieval-augmented Generation on Multi-modality Documents**|Shi Yu et.al.|[2410.10594](http://arxiv.org/abs/2410.10594)|**[link](https://github.com/openbmb/visrag)**|
|**2024-10-14**|**STACKFEED: Structured Textual Actor-Critic Knowledge Base Editing with FeedBack**|Naman Gupta et.al.|[2410.10584](http://arxiv.org/abs/2410.10584)|null|
|**2024-10-14**|**Model-Based Differentially Private Knowledge Transfer for Large Language Models**|Zhaomin Wu et.al.|[2410.10481](http://arxiv.org/abs/2410.10481)|null|
|**2024-10-14**|**KBLaM: Knowledge Base augmented Language Model**|Xi Wang et.al.|[2410.10450](http://arxiv.org/abs/2410.10450)|null|
|**2024-10-14**|**Parenting: Optimizing Knowledge Selection of Retrieval-Augmented Language Models with Parameter Decoupling and Tailored Tuning**|Yongxin Xu et.al.|[2410.10360](http://arxiv.org/abs/2410.10360)|null|
|**2024-10-15**|**EasyRAG: Efficient Retrieval-Augmented Generation Framework for Automated Network Operations**|Zhangchi Feng et.al.|[2410.10315](http://arxiv.org/abs/2410.10315)|**[link](https://github.com/buaadreamer/easyrag)**|
|**2024-10-14**|**FunnelRAG: A Coarse-to-Fine Progressive Retrieval Paradigm for RAG**|Xinping Zhao et.al.|[2410.10293](http://arxiv.org/abs/2410.10293)|null|
|**2024-10-14**|**Beyond-RAG: Question Identification and Answer Generation in Real-Time Conversations**|Garima Agrawal et.al.|[2410.10136](http://arxiv.org/abs/2410.10136)|null|
|**2024-10-13**|**Learning to Rank for Multiple Retrieval-Augmented Models through Iterative Utility Maximization**|Alireza Salemi et.al.|[2410.09942](http://arxiv.org/abs/2410.09942)|null|
|**2024-10-11**|**MedMobile: A mobile-sized language model with expert-level clinical capabilities**|Krithik Vishwanath et.al.|[2410.09019](http://arxiv.org/abs/2410.09019)|**[link](https://github.com/nyuolab/MedMobile)**|
|**2024-10-11**|**Retriever-and-Memory: Towards Adaptive Note-Enhanced Retrieval-Augmented Generation**|Ruobing Wang et.al.|[2410.08821](http://arxiv.org/abs/2410.08821)|**[link](https://github.com/thunlp/adaptive-note)**|
|**2024-10-11**|**StructRAG: Boosting Knowledge Intensive Reasoning of LLMs via Inference-time Hybrid Information Structurization**|Zhuoqun Li et.al.|[2410.08815](http://arxiv.org/abs/2410.08815)|null|
|**2024-10-11**|**A Methodology for Evaluating RAG Systems: A Case Study On Configuration Dependency Validation**|Sebastian Simon et.al.|[2410.08801](http://arxiv.org/abs/2410.08801)|null|
|**2024-10-11**|**Developing a Pragmatic Benchmark for Assessing Korean Legal Language Understanding in Large Language Models**|Yeeun Kim et.al.|[2410.08731](http://arxiv.org/abs/2410.08731)|**[link](https://github.com/lbox-kr/kbl)**|
|**2024-10-11**|**oRetrieval Augmented Generation for 10 Large Language Models and its Generalizability in Assessing Medical Fitness**|Yu He Ke et.al.|[2410.08431](http://arxiv.org/abs/2410.08431)|null|
|**2024-10-10**|**Do You Know What You Are Talking About? Characterizing Query-Knowledge Relevance For Reliable Retrieval Augmented Generation**|Zhuohang Li et.al.|[2410.08320](http://arxiv.org/abs/2410.08320)|null|
|**2024-10-10**|**Increasing the Difficulty of Automatically Generated Questions via Reinforcement Learning with Synthetic Preference**|William Thorne et.al.|[2410.08289](http://arxiv.org/abs/2410.08289)|null|
|**2024-10-10**|**MRAG-Bench: Vision-Centric Evaluation for Retrieval-Augmented Multimodal Models**|Wenbo Hu et.al.|[2410.08182](http://arxiv.org/abs/2410.08182)|null|
|**2024-10-10**|**TurboRAG: Accelerating Retrieval-Augmented Generation with Precomputed KV Caches for Chunked Text**|Songshuo Lu et.al.|[2410.07590](http://arxiv.org/abs/2410.07590)|**[link](https://github.com/MooreThreads/TurboRAG)**|
|**2024-10-10**|**No Free Lunch: Retrieval-Augmented Generation Undermines Fairness in LLMs, Even for Vigilant Users**|Mengxuan Hu et.al.|[2410.07589](http://arxiv.org/abs/2410.07589)|null|
|**2024-10-10**|**AI-Press: A Multi-Agent News Generating and Feedback Simulation System Powered by Large Language Models**|Xiawei Liu et.al.|[2410.07561](http://arxiv.org/abs/2410.07561)|null|
|**2024-10-10**|**KRAG Framework for Enhancing LLMs in the Legal Domain**|Nguyen Ha Thanh et.al.|[2410.07551](http://arxiv.org/abs/2410.07551)|null|
|**2024-10-10**|**News Reporter: A Multi-lingual LLM Framework for Broadcast T.V News**|Tarun Jain et.al.|[2410.07520](http://arxiv.org/abs/2410.07520)|null|
|**2024-10-09**|**Astute RAG: Overcoming Imperfect Retrieval Augmentation and Knowledge Conflicts for Large Language Models**|Fei Wang et.al.|[2410.07176](http://arxiv.org/abs/2410.07176)|null|
|**2024-10-09**|**Diamond of Thought: A Design Thinking-Based Framework for LLMs in Wearable Design**|Qiyang Miao et.al.|[2410.06972](http://arxiv.org/abs/2410.06972)|null|
|**2024-10-09**|**MedImageInsight: An Open-Source Embedding Model for General Domain Medical Imaging**|Noel C. F. Codella et.al.|[2410.06542](http://arxiv.org/abs/2410.06542)|null|
|**2024-10-09**|**Checker Bug Detection and Repair in Deep Learning Libraries**|Nima Shiri Harzevili et.al.|[2410.06440](http://arxiv.org/abs/2410.06440)|**[link](https://github.com/icsecs1992/TensorGuard)**|
|**2024-10-08**|**Less is More: Making Smaller Language Models Competent Subgraph Retrievers for Multi-hop KGQA**|Wenyu Huang et.al.|[2410.06121](http://arxiv.org/abs/2410.06121)|null|
|**2024-10-10**|**LLM-based SPARQL Query Generation from Natural Language over Federated Knowledge Graphs**|Vincent Emonet et.al.|[2410.06062](http://arxiv.org/abs/2410.06062)|null|
|**2024-10-08**|**Long-Context LLMs Meet RAG: Overcoming Challenges for Long Inputs in RAG**|Bowen Jin et.al.|[2410.05983](http://arxiv.org/abs/2410.05983)|null|
|**2024-10-08**|**Fortify Your Foundations: Practical Privacy and Security for Foundation Model Deployments In The Cloud**|Marcin Chrapek et.al.|[2410.05930](http://arxiv.org/abs/2410.05930)|null|
|**2024-10-08**|**Retrieving, Rethinking and Revising: The Chain-of-Verification Can Improve Retrieval Augmented Generation**|Bolei He et.al.|[2410.05801](http://arxiv.org/abs/2410.05801)|null|
|**2024-10-08**|**LightRAG: Simple and Fast Retrieval-Augmented Generation**|Zirui Guo et.al.|[2410.05779](http://arxiv.org/abs/2410.05779)|**[link](https://github.com/hkuds/lightrag)**|
|**2024-10-07**|**Deciphering the Interplay of Parametric and Non-parametric Memory in Retrieval-augmented Language Models**|Mehrdad Farahani et.al.|[2410.05162](http://arxiv.org/abs/2410.05162)|null|
|**2024-10-07**|**Fast State Restoration in LLM Serving with HCache**|Shiwei Gao et.al.|[2410.05004](http://arxiv.org/abs/2410.05004)|null|
|**2024-10-07**|**GARLIC: LLM-Guided Dynamic Progress Control with Hierarchical Weighted Graph for Long Document QA**|Xinyu Wang et.al.|[2410.04790](http://arxiv.org/abs/2410.04790)|null|
|**2024-10-07**|**Driving with Regulation: Interpretable Decision-Making for Autonomous Vehicles with Retrieval-Augmented Reasoning via LLM**|Tianhui Cai et.al.|[2410.04759](http://arxiv.org/abs/2410.04759)|null|
|**2024-10-07**|**LLaVA Needs More Knowledge: Retrieval Augmented Natural Language Generation with Knowledge Graph for Explaining Thoracic Pathologies**|Ameer Hamza et.al.|[2410.04749](http://arxiv.org/abs/2410.04749)|null|
|**2024-10-07**|**TableRAG: Million-Token Table Understanding with Language Models**|Si-An Chen et.al.|[2410.04739](http://arxiv.org/abs/2410.04739)|null|
|**2024-10-07**|**Knowledge Graph Based Agent for Complex, Knowledge-Intensive QA in Medicine**|Xiaorui Su et.al.|[2410.04660](http://arxiv.org/abs/2410.04660)|null|
|**2024-10-06**|**Reasoning-Enhanced Healthcare Predictions with Knowledge Graph Community Retrieval**|Pengcheng Jiang et.al.|[2410.04585](http://arxiv.org/abs/2410.04585)|**[link](https://github.com/pat-jj/KARE)**|
|**2024-10-06**|**MindScope: Exploring cognitive biases in large language models through Multi-Agent Systems**|Zhentao Xie et.al.|[2410.04452](http://arxiv.org/abs/2410.04452)|**[link](https://github.com/2279072142/mindscope)**|
|**2024-10-06**|**Inference Scaling for Long-Context Retrieval Augmented Generation**|Zhenrui Yue et.al.|[2410.04343](http://arxiv.org/abs/2410.04343)|null|
|**2024-10-04**|**Ward: Provable RAG Dataset Inference via LLM Watermarks**|Nikola Jovanović et.al.|[2410.03537](http://arxiv.org/abs/2410.03537)|null|
|**2024-10-04**|**Auto-GDA: Automatic Domain Adaptation for Efficient Grounding Verification in Retrieval Augmented Generation**|Tobias Leemann et.al.|[2410.03461](http://arxiv.org/abs/2410.03461)|null|
|**2024-10-04**|**Scalable Frame-based Construction of Sociocultural NormBases for Socially-Aware Dialogues**|Shilin Qu et.al.|[2410.03049](http://arxiv.org/abs/2410.03049)|null|
|**2024-10-03**|**Intrinsic Evaluation of RAG Systems for Deep-Logic Questions**|Junyi Hu et.al.|[2410.02932](http://arxiv.org/abs/2410.02932)|null|
|**2024-10-03**|**Streamlining Conformal Information Retrieval via Score Refinement**|Yotam Intrator et.al.|[2410.02914](http://arxiv.org/abs/2410.02914)|null|
|**2024-10-03**|**Grounding Large Language Models In Embodied Environment With Imperfect World Models**|Haolan Liu et.al.|[2410.02742](http://arxiv.org/abs/2410.02742)|null|
|**2024-10-03**|**Domain-Specific Retrieval-Augmented Generation Using Vector Stores, Knowledge Graphs, and Tensor Factorization**|Ryan C. Barron et.al.|[2410.02721](http://arxiv.org/abs/2410.02721)|null|
|**2024-10-03**|**UncertaintyRAG: Span-Level Uncertainty Enhanced Long-Context Modeling for Retrieval-Augmented Generation**|Zixuan Li et.al.|[2410.02719](http://arxiv.org/abs/2410.02719)|null|
|**2024-10-03**|**HELMET: How to Evaluate Long-Context Language Models Effectively and Thoroughly**|Howard Yen et.al.|[2410.02694](http://arxiv.org/abs/2410.02694)|**[link](https://github.com/princeton-nlp/helmet)**|
|**2024-10-03**|**Undesirable Memorization in Large Language Models: A Survey**|Ali Satvaty et.al.|[2410.02650](http://arxiv.org/abs/2410.02650)|null|
|**2024-10-03**|**Attention in Large Language Models Yields Efficient Zero-Shot Re-Rankers**|Shijie Chen et.al.|[2410.02642](http://arxiv.org/abs/2410.02642)|null|
|**2024-10-03**|**ColaCare: Enhancing Electronic Health Record Modeling through Large Language Model-Driven Multi-Agent Collaboration**|Zixiang Wang et.al.|[2410.02551](http://arxiv.org/abs/2410.02551)|null|
|**2024-10-04**|**IoT-LLM: Enhancing Real-World IoT Task Reasoning with Large Language Models**|Tuo An et.al.|[2410.02429](http://arxiv.org/abs/2410.02429)|null|
|**2024-10-03**|**How Much Can RAG Help the Reasoning of LLM?**|Jingyu Liu et.al.|[2410.02338](http://arxiv.org/abs/2410.02338)|null|
|**2024-10-03**|**Controlled Generation of Natural Adversarial Documents for Stealthy Retrieval Poisoning**|Collin Zhang et.al.|[2410.02163](http://arxiv.org/abs/2410.02163)|**[link](https://github.com/collinzrj/adversarial_decoding)**|
|**2024-10-02**|**Open-RAG: Enhanced Retrieval-Augmented Reasoning with Open-Source Large Language Models**|Shayekh Bin Islam et.al.|[2410.01782](http://arxiv.org/abs/2410.01782)|**[link](https://github.com/ShayekhBinIslam/openrag)**|
|**2024-10-02**|**Can We Further Elicit Reasoning in LLMs? Critic-Guided Planning with Retrieval-Augmentation for Solving Challenging Tasks**|Xingxuan Li et.al.|[2410.01428](http://arxiv.org/abs/2410.01428)|null|
|**2024-10-02**|**Revisiting the Index Construction of Proximity Graph-Based Approximate Nearest Neighbor Search**|Shuo Yang et.al.|[2410.01231](http://arxiv.org/abs/2410.01231)|null|
|**2024-10-02**|**BordIRlines: A Dataset for Evaluating Cross-lingual Retrieval-Augmented Generation**|Bryan Li et.al.|[2410.01171](http://arxiv.org/abs/2410.01171)|**[link](https://github.com/manestay/bordirlines)**|
|**2024-10-01**|**Quantifying reliance on external information over parametric knowledge during Retrieval Augmented Generation (RAG) using mechanistic analysis**|Reshmi Ghosh et.al.|[2410.00857](http://arxiv.org/abs/2410.00857)|null|
|**2024-10-01**|**UniAdapt: A Universal Adapter for Knowledge Calibration**|Tai D. Nguyen et.al.|[2410.00454](http://arxiv.org/abs/2410.00454)|null|
|**2024-10-01**|**Boosting the Capabilities of Compact Models in Low-Data Contexts with Large Language Models and Retrieval-Augmented Generation**|Bhargav Shandilya et.al.|[2410.00387](http://arxiv.org/abs/2410.00387)|null|
|**2024-09-30**|**LLM Hallucinations in Practical Code Generation: Phenomena, Mechanism, and Mitigation**|Ziyao Zhang et.al.|[2409.20550](http://arxiv.org/abs/2409.20550)|null|
|**2024-09-30**|**QAEncoder: Towards Aligned Representation Learning in Question Answering System**|Zhengren Wang et.al.|[2409.20434](http://arxiv.org/abs/2409.20434)|**[link](https://github.com/IAAR-Shanghai/QAEncoder)**|
|**2024-09-30**|**Reference Trustable Decoding: A Training-Free Augmentation Paradigm for Large Language Models**|Luohe Shi et.al.|[2409.20181](http://arxiv.org/abs/2409.20181)|null|
|**2024-09-30**|**BSharedRAG: Backbone Shared Retrieval-Augmented Generation for the E-commerce Domain**|Kaisi Guan et.al.|[2409.20075](http://arxiv.org/abs/2409.20075)|null|
|**2024-09-30**|**Beyond Scores: A Modular RAG-Based System for Automatic Short Answer Scoring with Feedback**|Menna Fateen et.al.|[2409.20042](http://arxiv.org/abs/2409.20042)|null|
|**2024-09-29**|**Does RAG Introduce Unfairness in LLMs? Evaluating Fairness in Retrieval-Augmented Generation Systems**|Xuyang Wu et.al.|[2409.19804](http://arxiv.org/abs/2409.19804)|null|
|**2024-09-29**|**CoTKR: Chain-of-Thought Enhanced Knowledge Rewriting for Complex Knowledge Graph Question Answering**|Yike Wu et.al.|[2409.19753](http://arxiv.org/abs/2409.19753)|**[link](https://github.com/wuyike2000/CoTKR)**|
|**2024-09-29**|**PEAR: Position-Embedding-Agnostic Attention Re-weighting Enhances Retrieval-Augmented Generation with Zero Inference Overhead**|Tao Tan et.al.|[2409.19745](http://arxiv.org/abs/2409.19745)|null|
|**2024-09-28**|**HealthQ: Unveiling Questioning Capabilities of LLM Chains in Healthcare Conversations**|Ziyu Wang et.al.|[2409.19487](http://arxiv.org/abs/2409.19487)|null|
|**2024-09-28**|**Crafting Personalized Agents through Retrieval-Augmented Generation on Editable Memory Graphs**|Zheng Wang et.al.|[2409.19401](http://arxiv.org/abs/2409.19401)|null|
|**2024-09-27**|**AIPatient: Simulating Patients with EHRs and LLM Powered Agentic Workflow**|Huizi Yu et.al.|[2409.18924](http://arxiv.org/abs/2409.18924)|null|
|**2024-09-27**|**Corpus-informed Retrieval Augmented Generation of Clarifying Questions**|Antonios Minas Krasakis et.al.|[2409.18575](http://arxiv.org/abs/2409.18575)|null|
|**2024-09-26**|**Embodied-RAG: General non-parametric Embodied Memory for Retrieval and Generation**|Quanting Xie et.al.|[2409.18313](http://arxiv.org/abs/2409.18313)|null|
|**2024-09-26**|**Data-Prep-Kit: getting your data ready for LLM application development**|David Wood et.al.|[2409.18164](http://arxiv.org/abs/2409.18164)|null|
|**2024-09-26**|**Enhancing Tourism Recommender Systems for Sustainable City Trips Using Retrieval-Augmented Generation**|Ashmi Banerjee et.al.|[2409.18003](http://arxiv.org/abs/2409.18003)|null|
|**2024-09-26**|**Efficient In-Domain Question Answering for Resource-Constrained Environments**|Isaac Chung et.al.|[2409.17648](http://arxiv.org/abs/2409.17648)|null|
|**2024-09-26**|**Enhancing Structured-Data Retrieval with GraphRAG: Soccer Data Case Study**|Zahra Sepasdar et.al.|[2409.17580](http://arxiv.org/abs/2409.17580)|null|
|**2024-09-25**|**LLaMa-SciQ: An Educational Chatbot for Answering Science MCQ**|Marc-Antoine Allard et.al.|[2409.16779](http://arxiv.org/abs/2409.16779)|null|
|**2024-09-25**|**Evaluating and Enhancing Large Language Models for Novelty Assessment in Scholarly Publications**|Ethan Lin et.al.|[2409.16605](http://arxiv.org/abs/2409.16605)|**[link](https://github.com/ethannlin/schnovel)**|
|**2024-09-24**|**REBEL: Rule-based and Experience-enhanced Learning with LLMs for Initial Task Allocation in Multi-Human Multi-Robot Teams**|Arjun Gupte et.al.|[2409.16266](http://arxiv.org/abs/2409.16266)|null|
|**2024-09-24**|**Cyber Knowledge Completion Using Large Language Models**|Braden K Webb et.al.|[2409.16176](http://arxiv.org/abs/2409.16176)|null|
|**2024-09-24**|**Controlling Risk of Retrieval-augmented Generation: A Counterfactual Prompting Framework**|Lu Chen et.al.|[2409.16146](http://arxiv.org/abs/2409.16146)|null|
|**2024-09-24**|**SwiftDossier: Tailored Automatic Dossier for Drug Discovery with LLMs and Agents**|Gabriele Fossi et.al.|[2409.15817](http://arxiv.org/abs/2409.15817)|null|
|**2024-09-24**|**AsthmaBot: Multi-modal, Multi-Lingual Retrieval Augmented Generation For Asthma Patient Support**|Adil Bahaj et.al.|[2409.15815](http://arxiv.org/abs/2409.15815)|null|
|**2024-09-18**|**MoRAG -- Multi-Fusion Retrieval Augmented Generation for Human Motion**|Kalakonda Sai Shashank et.al.|[2409.12140](http://arxiv.org/abs/2409.12140)|null|
|**2024-09-18**|**RaggeDi: Diffusion-based State Estimation of Disordered Rags, Sheets, Towels and Blankets**|Jikai Ye et.al.|[2409.11831](http://arxiv.org/abs/2409.11831)|null|
|**2024-09-17**|**Towards Fair RAG: On the Impact of Fair Ranking in Retrieval-Augmented Generation**|To Eun Kim et.al.|[2409.11598](http://arxiv.org/abs/2409.11598)|**[link](https://github.com/kimdanny/fair-rag)**|
|**2024-09-17**|**Phidias: A Generative Model for Creating 3D Content from Text, Image, and 3D Conditions with Reference-Augmented Diffusion**|Zhenwei Wang et.al.|[2409.11406](http://arxiv.org/abs/2409.11406)|null|
|**2024-09-17**|**THaMES: An End-to-End Tool for Hallucination Mitigation and Evaluation in Large Language Models**|Mengfei Liang et.al.|[2409.11353](http://arxiv.org/abs/2409.11353)|null|
|**2024-09-17**|**P-RAG: Progressive Retrieval Augmented Generation For Planning on Embodied Everyday Task**|Weiye Xu et.al.|[2409.11279](http://arxiv.org/abs/2409.11279)|null|
|**2024-09-17**|**Measuring and Enhancing Trustworthiness of LLMs in RAG through Grounded Attributions and Learning to Refuse**|Maojia Song et.al.|[2409.11242](http://arxiv.org/abs/2409.11242)|**[link](https://github.com/declare-lab/trust-align)**|
|**2024-09-17**|**SuperCoder2.0: Technical Report on Exploring the feasibility of LLMs as Autonomous Programmer**|Anmol Gautam et.al.|[2409.11190](http://arxiv.org/abs/2409.11190)|null|
|**2024-09-17**|**Investigating Context-Faithfulness in Large Language Models: The Roles of Memory Strength and Evidence Style**|Yuepei Li et.al.|[2409.10955](http://arxiv.org/abs/2409.10955)|null|
|**2024-09-18**|**Language Models and Retrieval Augmented Generation for Automated Structured Data Extraction from Diagnostic Reports**|Mohamed Sobhi Jabal et.al.|[2409.10576](http://arxiv.org/abs/2409.10576)|null|
|**2024-09-16**|**Trustworthiness in Retrieval-Augmented Generation Systems: A Survey**|Yujia Zhou et.al.|[2409.10102](http://arxiv.org/abs/2409.10102)|**[link](https://github.com/smallporridge/trustworthyrag)**|
|**2024-09-16**|**SFR-RAG: Towards Contextually Faithful LLMs**|Xuan-Phi Nguyen et.al.|[2409.09916](http://arxiv.org/abs/2409.09916)|null|
|**2024-09-14**|**Comparing Retrieval-Augmentation and Parameter-Efficient Fine-Tuning for Privacy-Preserving Personalization of Large Language Models**|Alireza Salemi et.al.|[2409.09510](http://arxiv.org/abs/2409.09510)|**[link](https://github.com/lamp-benchmark/lamp)**|
|**2024-09-14**|**Hacking, The Lazy Way: LLM Augmented Pentesting**|Dhruva Goyal et.al.|[2409.09493](http://arxiv.org/abs/2409.09493)|null|
|**2024-09-14**|**Generative AI in Data Center Networking: Fundamentals, Perspectives, and Case Study**|Yinqiu Liu et.al.|[2409.09343](http://arxiv.org/abs/2409.09343)|null|
|**2024-09-14**|**Language Models "Grok" to Copy**|Ang Lv et.al.|[2409.09281](http://arxiv.org/abs/2409.09281)|null|
|**2024-09-13**|**A RAG Approach for Generating Competency Questions in Ontology Engineering**|Xueli Pan et.al.|[2409.08820](http://arxiv.org/abs/2409.08820)|null|
|**2024-09-13**|**LA-RAG:Enhancing LLM-based ASR Accuracy with Retrieval-Augmented Generation**|Shaojun Li et.al.|[2409.08597](http://arxiv.org/abs/2409.08597)|null|
|**2024-09-13**|**Exploring Information Retrieval Landscapes: An Investigation of a Novel Evaluation Techniques and Comparative Document Splitting Methods**|Esmaeil Narimissa et.al.|[2409.08479](http://arxiv.org/abs/2409.08479)|**[link](https://github.com/EsmaeilNarimissa/RAG-Retrieval-Analysis)**|
|**2024-09-12**|**OmniQuery: Contextually Augmenting Captured Multimodal Memory to Enable Personal Question Answering**|Jiahao Nick Li et.al.|[2409.08250](http://arxiv.org/abs/2409.08250)|null|
|**2024-09-12**|**Unleashing Worms and Extracting Data: Escalating the Outcome of Attacks against RAG-based Inference in Scale and Severity Using Jailbreaking**|Stav Cohen et.al.|[2409.08045](http://arxiv.org/abs/2409.08045)|**[link](https://github.com/stavc/unleashingworms-extractingdata)**|
|**2024-09-12**|**Enabling Cost-Effective UI Automation Testing with Retrieval-Based LLMs: A Case Study in WeChat**|Sidong Feng et.al.|[2409.07829](http://arxiv.org/abs/2409.07829)|null|
|**2024-09-12**|**Experimenting with Legal AI Solutions: The Case of Question-Answering for Access to Justice**|Jonathan Li et.al.|[2409.07713](http://arxiv.org/abs/2409.07713)|null|
|**2024-09-12**|**Enhancing Q&A Text Retrieval with Ranking Models: Benchmarking, fine-tuning and deploying Rerankers for RAG**|Gabriel de Souza P. Moreira et.al.|[2409.07691](http://arxiv.org/abs/2409.07691)|null|
|**2024-09-11**|**Synthetic continued pretraining**|Zitong Yang et.al.|[2409.07431](http://arxiv.org/abs/2409.07431)|**[link](https://github.com/zitongyang/synthetic_continued_pretraining)**|
|**2024-09-11**|**Bio-Eng-LMM AI Assist chatbot: A Comprehensive Tool for Research and Education**|Ali Forootani et.al.|[2409.07110](http://arxiv.org/abs/2409.07110)|**[link](https://github.com/Ali-Forootani/multi_llm)**|
|**2024-09-10**|**GroUSE: A Benchmark to Evaluate Evaluators in Grounded Question Answering**|Sacha Muller et.al.|[2409.06595](http://arxiv.org/abs/2409.06595)|**[link](https://github.com/illuin-tech/grouse)**|
|**2024-09-10**|**Multimodal Large Language Model Driven Scenario Testing for Autonomous Vehicles**|Qiujing Lu et.al.|[2409.06450](http://arxiv.org/abs/2409.06450)|null|
|**2024-09-09**|**Retrieval Augmented Correction of Named Entity Speech Recognition Errors**|Ernest Pusateri et.al.|[2409.06062](http://arxiv.org/abs/2409.06062)|null|
|**2024-09-10**|**MemoRAG: Moving towards Next-Gen RAG Via Memory-Inspired Knowledge Discovery**|Hongjin Qian et.al.|[2409.05591](http://arxiv.org/abs/2409.05591)|**[link](https://github.com/qhjqhj00/memorag)**|
|**2024-09-08**|**OneGen: Efficient One-Pass Unified Generation and Retrieval for LLMs**|Jintian Zhang et.al.|[2409.05152](http://arxiv.org/abs/2409.05152)|**[link](https://github.com/zjunlp/onegen)**|
|**2024-09-05**|**Revolutionizing Database Q&A with Large Language Models: Comprehensive Benchmark and Evaluation**|Yihang Zheng et.al.|[2409.04475](http://arxiv.org/abs/2409.04475)|**[link](https://github.com/xmudm/dqabench)**|
|**2024-09-06**|**RAG based Question-Answering for Contextual Response Prediction System**|Sriram Veturi et.al.|[2409.03708](http://arxiv.org/abs/2409.03708)|null|
|**2024-09-05**|**GraphInsight: Unlocking Insights in Large Language Models for Graph Structure Understanding**|Yukun Cao et.al.|[2409.03258](http://arxiv.org/abs/2409.03258)|null|
|**2024-09-05**|**MARAGS: A Multi-Adapter System for Multi-Task Retrieval Augmented Generation Question Answering**|Mitchell DeHaven et.al.|[2409.03171](http://arxiv.org/abs/2409.03171)|null|
|**2024-09-04**|**Bioinformatics Retrieval Augmentation Data (BRAD) Digital Assistant**|Joshua Pickard et.al.|[2409.02864](http://arxiv.org/abs/2409.02864)|**[link](https://github.com/jpickard1/brad)**|
|**2024-09-04**|**Creating a Gen-AI based Track and Trace Assistant MVP (SuperTracy) for PostNL**|Mohammad Reshadati et.al.|[2409.02711](http://arxiv.org/abs/2409.02711)|null|
|**2024-09-04**|**Advancing Cyber Incident Timeline Analysis Through Rule Based AI and Large Language Models**|Fatma Yasmine Loumachi et.al.|[2409.02572](http://arxiv.org/abs/2409.02572)|null|
|**2024-09-04**|**Diversify-verify-adapt: Efficient and Robust Retrieval-Augmented Ambiguous Question Answering**|Yeonjun In et.al.|[2409.02361](http://arxiv.org/abs/2409.02361)|null|
|**2024-09-04**|**NUDGE: Lightweight Non-Parametric Fine-Tuning of Embeddings for Retrieval**|Sepanta Zeighami et.al.|[2409.02343](http://arxiv.org/abs/2409.02343)|**[link](https://github.com/szeighami/nudge)**|
|**2024-09-03**|**BEAVER: An Enterprise Benchmark for Text-to-SQL**|Peter Baile Chen et.al.|[2409.02038](http://arxiv.org/abs/2409.02038)|null|
|**2024-09-03**|**The Role of Large Language Models in Musicology: Are We Ready to Trust the Machines?**|Pedro Ramoneda et.al.|[2409.01864](http://arxiv.org/abs/2409.01864)|null|
|**2024-09-03**|**In Defense of RAG in the Era of Long-Context Language Models**|Tan Yu et.al.|[2409.01666](http://arxiv.org/abs/2409.01666)|null|
|**2024-09-03**|**AdaComp: Extractive Context Compression with Adaptive Predictor for Retrieval-Augmented Large Language Models**|Qianchi Zhang et.al.|[2409.01579](http://arxiv.org/abs/2409.01579)|null|
|**2024-09-03**|**Benchmarking Cognitive Domains for LLMs: Insights from Taiwanese Hakka Culture**|Chen-Chi Chang et.al.|[2409.01556](http://arxiv.org/abs/2409.01556)|null|
|**2024-09-02**|**RISSOLE: Parameter-efficient Diffusion Models via Block-wise Generation and Retrieval-Guidance**|Avideep Mukherjee et.al.|[2408.17095](http://arxiv.org/abs/2408.17095)|null|
|**2024-08-30**|**MaFeRw: Query Rewriting with Multi-Aspect Feedbacks for Retrieval-Augmented Large Language Models**|Yujing Wang et.al.|[2408.17072](http://arxiv.org/abs/2408.17072)|null|
|**2024-08-29**|**Conan-embedding: General Text Embedding with More and Better Negative Samples**|Shiyu Li et.al.|[2408.15710](http://arxiv.org/abs/2408.15710)|null|
|**2024-08-28**|**Boosting Lossless Speculative Decoding via Feature Sampling and Partial Alignment Distillation**|Lujun Gui et.al.|[2408.15562](http://arxiv.org/abs/2408.15562)|null|
|**2024-08-29**|**LRP4RAG: Detecting Hallucinations in Retrieval-Augmented Generation via Layer-wise Relevance Propagation**|Haichuan Hu et.al.|[2408.15533](http://arxiv.org/abs/2408.15533)|**[link](https://github.com/tomsawyerhu/lrp4rag)**|
|**2024-08-27**|**Into the Unknown Unknowns: Engaged Human Learning through Participation in Language Model Agent Conversations**|Yucheng Jiang et.al.|[2408.15232](http://arxiv.org/abs/2408.15232)|null|
|**2024-08-27**|**Measuring text summarization factuality using atomic facts entailment metrics in the context of retrieval augmented generation**|N. E. Kriman et.al.|[2408.15171](http://arxiv.org/abs/2408.15171)|null|
|**2024-08-27**|**Writing in the Margins: Better Inference Pattern for Long Context Retrieval**|Melisa Russak et.al.|[2408.14906](http://arxiv.org/abs/2408.14906)|**[link](https://github.com/writer/writing-in-the-margins)**|
|**2024-08-27**|**Text2SQL is Not Enough: Unifying AI and Databases with TAG**|Asim Biswal et.al.|[2408.14717](http://arxiv.org/abs/2408.14717)|**[link](https://github.com/tag-research/tag-bench)**|
|**2024-08-26**|**Retrieval Augmented Generation for Dynamic Graph Modeling**|Yuxia Wu et.al.|[2408.14523](http://arxiv.org/abs/2408.14523)|null|
|**2024-08-26**|**Probing Causality Manipulation of Large Language Models**|Chenyang Zhang et.al.|[2408.14380](http://arxiv.org/abs/2408.14380)|**[link](https://github.com/tongjinlp/llm-causality-probing)**|
|**2024-08-26**|**Claim Verification in the Age of Large Language Models: A Survey**|Alphaeus Dmonte et.al.|[2408.14317](http://arxiv.org/abs/2408.14317)|null|
|**2024-08-25**|**Biomedical Large Languages Models Seem not to be Superior to Generalist Models on Unseen Medical Data**|Felix J. Dorfner et.al.|[2408.13833](http://arxiv.org/abs/2408.13833)|null|
|**2024-08-25**|**Towards Reliable Medical Question Answering: Techniques and Challenges in Mitigating Hallucinations in Language Models**|Duy Khoa Pham et.al.|[2408.13808](http://arxiv.org/abs/2408.13808)|null|
|**2024-08-24**|**Pandora's Box or Aladdin's Lamp: A Comprehensive Analysis Revealing the Role of RAG Noise in Large Language Models**|Jinyang Wu et.al.|[2408.13533](http://arxiv.org/abs/2408.13533)|null|
|**2024-08-24**|**vitaLITy 2: Reviewing Academic Literature Using Large Language Models**|Hongye An et.al.|[2408.13450](http://arxiv.org/abs/2408.13450)|null|
|**2024-08-23**|**CodeRefine: A Pipeline for Enhancing LLM-Generated Code Implementations of Research Papers**|Ekaterina Trofimova et.al.|[2408.13366](http://arxiv.org/abs/2408.13366)|null|
|**2024-08-22**|**Graph Retrieval Augmented Trustworthiness Reasoning**|Ying Zhu et.al.|[2408.12333](http://arxiv.org/abs/2408.12333)|**[link](https://github.com/EvoNexusX/Graph-Retrieval-Augmented-Trustworthiness-Reasoning)**|
|**2024-08-22**|**LLMs are not Zero-Shot Reasoners for Biomedical Information Extraction**|Aishik Nagar et.al.|[2408.12249](http://arxiv.org/abs/2408.12249)|null|
|**2024-08-22**|**Evidence-backed Fact Checking using RAG and Few-Shot In-Context Learning with LLMs**|Ronit Singhal et.al.|[2408.12060](http://arxiv.org/abs/2408.12060)|**[link](https://github.com/ronit-singhal/evidence-backed-fact-checking-using-rag-and-few-shot-in-context-learning-with-llms)**|
|**2024-08-21**|**RAG-Optimized Tibetan Tourism LLMs: Enhancing Accuracy and Personalization**|Jinhu Qi et.al.|[2408.12003](http://arxiv.org/abs/2408.12003)|null|
|**2024-08-23**|**Ancient Wisdom, Modern Tools: Exploring Retrieval-Augmented LLMs for Ancient Indian Philosophy**|Priyanka Mandikal et.al.|[2408.11903](http://arxiv.org/abs/2408.11903)|**[link](https://github.com/priyankamandikal/vedantany-10m)**|
|**2024-08-21**|**PermitQA: A Benchmark for Retrieval Augmented Generation in Wind Siting and Permitting domain**|Rounak Meyur et.al.|[2408.11800](http://arxiv.org/abs/2408.11800)|null|
|**2024-08-21**|**Leveraging Chemistry Foundation Models to Facilitate Structure Focused Retrieval Augmented Generation in Multi-Agent Workflows for Catalyst and Materials Design**|Nathaniel H. Park et.al.|[2408.11793](http://arxiv.org/abs/2408.11793)|null|
|**2024-08-21**|**Leveraging Fine-Tuned Retrieval-Augmented Generation with Long-Context Support: For 3GPP Standards**|Omar Erak et.al.|[2408.11775](http://arxiv.org/abs/2408.11775)|**[link](https://github.com/Nouf-Alabbasi/oKUmura_AI_Telecom_challenge)**|
|**2024-08-23**|**Xinyu: An Efficient LLM-based System for Commentary Generation**|Yiquan Wu et.al.|[2408.11609](http://arxiv.org/abs/2408.11609)|null|
|**2024-08-23**|**A Quick, trustworthy spectral detection Q&A system based on the SDAAP Dataset and large language model**|Jiheng Liang et.al.|[2408.11557](http://arxiv.org/abs/2408.11557)|**[link](https://github.com/0217ljh/QA_System_For_Spectral_Analysis_With_SDAAP_Dataset)**|
|**2024-08-21**|**RAGLAB: A Modular and Research-Oriented Unified Framework for Retrieval-Augmented Generation**|Xuanwang Zhang et.al.|[2408.11381](http://arxiv.org/abs/2408.11381)|**[link](https://github.com/fate-ubw/raglab)**|
|**2024-08-20**|**Reading with Intent**|Benjamin Reichman et.al.|[2408.11189](http://arxiv.org/abs/2408.11189)|null|
|**2024-08-20**|**Reconciling Methodological Paradigms: Employing Large Language Models as Novice Qualitative Research Assistants in Talent Management Research**|Sreyoshi Bhaduri et.al.|[2408.11043](http://arxiv.org/abs/2408.11043)|null|
|**2024-08-19**|**Enhanced document retrieval with topic embeddings**|Kavsar Huseynova et.al.|[2408.10435](http://arxiv.org/abs/2408.10435)|null|
|**2024-08-19**|**LegalBench-RAG: A Benchmark for Retrieval-Augmented Generation in the Legal Domain**|Nicholas Pipitone et.al.|[2408.10343](http://arxiv.org/abs/2408.10343)|**[link](https://github.com/zeroentropy-cc/legalbenchrag)**|
|**2024-08-19**|**Demystifying the Communication Characteristics for Distributed Transformer Models**|Quentin Anthony et.al.|[2408.10197](http://arxiv.org/abs/2408.10197)|null|
|**2024-08-19**|**Customizing Language Models with Instance-wise LoRA for Sequential Recommendation**|Xiaoyu Kong et.al.|[2408.10159](http://arxiv.org/abs/2408.10159)|null|
|**2024-08-19**|**Multilingual Needle in a Haystack: Investigating Long-Context Behavior of Multilingual Large Language Models**|Amey Hengle et.al.|[2408.10151](http://arxiv.org/abs/2408.10151)|**[link](https://github.com/AmeyHengle/multilingual-needle-in-a-haystack)**|
|**2024-08-19**|**Instruction Finetuning for Leaderboard Generation from Empirical AI Research**|Salomon Kabongo et.al.|[2408.10141](http://arxiv.org/abs/2408.10141)|null|
|**2024-08-19**|**Molecular Graph Representation Learning Integrating Large Language Models with Domain-specific Small Models**|Tianyu Zhang et.al.|[2408.10124](http://arxiv.org/abs/2408.10124)|**[link](https://github.com/zhangtia16/molgraph-lardo)**|
|**2024-08-19**|**ARMADA: Attribute-Based Multimodal Data Augmentation**|Xiaomeng Jin et.al.|[2408.10086](http://arxiv.org/abs/2408.10086)|null|
|**2024-08-19**|**Privacy Checklist: Privacy Violation Detection Grounding on Contextual Integrity Theory**|Haoran Li et.al.|[2408.10053](http://arxiv.org/abs/2408.10053)|null|
|**2024-08-19**|**MSDiagnosis: An EMR-based Dataset for Clinical Multi-Step Diagnosis**|Ruihui Hou et.al.|[2408.10039](http://arxiv.org/abs/2408.10039)|null|
|**2024-08-19**|**TBA: Faster Large Language Model Training Using SSD-Based Activation Offloading**|Kun Wu et.al.|[2408.10013](http://arxiv.org/abs/2408.10013)|null|
|**2024-08-19**|**Application of Large Language Models in Automated Question Generation: A Case Study on ChatGLM's Structured Questions for National Teacher Certification Exams**|Yanxin Chen et.al.|[2408.09982](http://arxiv.org/abs/2408.09982)|null|
|**2024-08-20**|**Carbon Footprint Accounting Driven by Large Language Models and Retrieval-augmented Generation**|Haijin Wang et.al.|[2408.09713](http://arxiv.org/abs/2408.09713)|null|
|**2024-08-17**|**Developing a Llama-Based Chatbot for CI/CD Question Answering: A Case Study at Ericsson**|Daksh Chaudhary et.al.|[2408.09277](http://arxiv.org/abs/2408.09277)|null|
|**2024-08-17**|**TC-RAG:Turing-Complete RAG's Case study on Medical LLM Systems**|Xinke Jiang et.al.|[2408.09199](http://arxiv.org/abs/2408.09199)|**[link](https://github.com/artessay/sama)**|
|**2024-08-16**|**A Primer on Generative AI for Telecom: From Theory to Practice**|Xingqin Lin et.al.|[2408.09031](http://arxiv.org/abs/2408.09031)|null|
|**2024-08-16**|**Meta Knowledge for Retrieval Augmented Large Language Models**|Laurent Mombaerts et.al.|[2408.09017](http://arxiv.org/abs/2408.09017)|null|
|**2024-08-16**|**PEDAL: Enhancing Greedy Decoding with Large Language Models using Diverse Exemplars**|Sumanth Prabhu et.al.|[2408.08869](http://arxiv.org/abs/2408.08869)|null|
|**2024-08-16**|**PsychoLex: Unveiling the Psychological Mind of Large Language Models**|Mohammad Amin Abbasi et.al.|[2408.08848](http://arxiv.org/abs/2408.08848)|null|
|**2024-08-16**|**FLEXTAF: Enhancing Table Reasoning with Flexible Tabular Formats**|Xuanliang Zhang et.al.|[2408.08841](http://arxiv.org/abs/2408.08841)|**[link](https://github.com/zhxlia/FLEXTAF)**|
|**2024-08-16**|**Artificial Intelligence and Strategic Decision-Making: Evidence from Entrepreneurs and Investors**|Felipe A. Csaszar et.al.|[2408.08811](http://arxiv.org/abs/2408.08811)|null|
|**2024-08-16**|**Constructing Domain-Specific Evaluation Sets for LLM-as-a-judge**|Ravi Raju et.al.|[2408.08808](http://arxiv.org/abs/2408.08808)|null|
|**2024-08-16**|**EmoDynamiX: Emotional Support Dialogue Strategy Prediction by Modelling MiXed Emotions and Discourse Dynamics**|Chenwei Wan et.al.|[2408.08782](http://arxiv.org/abs/2408.08782)|**[link](https://github.com/cw-wan/EmoDynamiX-v2)**|
|**2024-08-16**|**Evaluating the Evaluator: Measuring LLMs' Adherence to Task Evaluation Instructions**|Bhuvanashree Murugadoss et.al.|[2408.08781](http://arxiv.org/abs/2408.08781)|null|
|**2024-08-16**|**Large Language Models Might Not Care What You Are Saying: Prompt Format Beats Descriptions**|Chenming Tang et.al.|[2408.08780](http://arxiv.org/abs/2408.08780)|null|
|**2024-08-16**|**DAC: Decomposed Automation Correction for Text-to-SQL**|Dingzirui Wang et.al.|[2408.08779](http://arxiv.org/abs/2408.08779)|**[link](https://github.com/zirui-HIT/DAC)**|
|**2024-08-16**|**Lower Layer Matters: Alleviating Hallucination via Multi-Layer Fusion Contrastive Decoding with Truthfulness Refocused**|Dingwei Chen et.al.|[2408.08769](http://arxiv.org/abs/2408.08769)|null|
|**2024-08-16**|**Extracting polygonal footprints in off-nadir images with Segment Anything Model**|Kai Li et.al.|[2408.08645](http://arxiv.org/abs/2408.08645)|null|
|**2024-08-16**|**CommunityKG-RAG: Leveraging Community Structures in Knowledge Graphs for Advanced Retrieval-Augmented Generation in Fact-Checking**|Rong-Ching Chang et.al.|[2408.08535](http://arxiv.org/abs/2408.08535)|null|
|**2024-08-16**|**MuRAR: A Simple and Effective Multimodal Retrieval and Answer Refinement Framework for Multimodal Question Answering**|Zhengyuan Zhu et.al.|[2408.08521](http://arxiv.org/abs/2408.08521)|null|
|**2024-08-15**|**W-RAG: Weakly Supervised Dense Retrieval in RAG for Open-domain Question Answering**|Jinming Nian et.al.|[2408.08444](http://arxiv.org/abs/2408.08444)|**[link](https://github.com/jmnian/weak_label_for_rag)**|
|**2024-08-15**|**Assessing and Enhancing Large Language Models in Rare Disease Question-answering**|Guanchu Wang et.al.|[2408.08422](http://arxiv.org/abs/2408.08422)|null|
|**2024-08-15**|**Can Large Language Models Understand Symbolic Graphics Programs?**|Zeju Qiu et.al.|[2408.08313](http://arxiv.org/abs/2408.08313)|null|
|**2024-08-15**|**ScalingFilter: Assessing Data Quality through Inverse Utilization of Scaling Laws**|Ruihang Li et.al.|[2408.08310](http://arxiv.org/abs/2408.08310)|null|
|**2024-08-15**|**Benchmarking the Capabilities of Large Language Models in Transportation System Engineering: Accuracy, Consistency, and Reasoning Behaviors**|Usman Syed et.al.|[2408.08302](http://arxiv.org/abs/2408.08302)|null|
|**2024-08-15**|**HELP: Hierarchical Embeddings-based Log Parsing**|Andy Xu et.al.|[2408.08300](http://arxiv.org/abs/2408.08300)|null|
|**2024-08-15**|**The ShareLM Collection and Plugin: Contributing Human-Model Chats for the Benefit of the Community**|Shachar Don-Yehiya et.al.|[2408.08291](http://arxiv.org/abs/2408.08291)|null|
|**2024-08-15**|**Autonomous Behavior Planning For Humanoid Loco-manipulation Through Grounded Language Model**|Jin Wang et.al.|[2408.08282](http://arxiv.org/abs/2408.08282)|null|
|**2024-08-15**|**BAM! Just Like That: Simple and Efficient Parameter Upcycling for Mixture of Experts**|Qizhen Zhang et.al.|[2408.08274](http://arxiv.org/abs/2408.08274)|null|
|**2024-08-15**|**DaRec: A Disentangled Alignment Framework for Large Language Model and Recommender System**|Xihong Yang et.al.|[2408.08231](http://arxiv.org/abs/2408.08231)|null|
|**2024-08-15**|**RED-CT: A Systems Design Methodology for Using LLM-labeled Data to Train and Deploy Edge Classifiers for Computational Social Science**|David Farr et.al.|[2408.08217](http://arxiv.org/abs/2408.08217)|null|
|**2024-08-16**|**Covert Bias: The Severity of Social Views' Unalignment in Language Models Towards Implicit and Explicit Opinion**|Abeer Aldayel et.al.|[2408.08212](http://arxiv.org/abs/2408.08212)|null|
|**2024-08-15**|**Does Reasoning Emerge? Examining the Probabilities of Causation in Large Language Models**|Javier González et.al.|[2408.08210](http://arxiv.org/abs/2408.08210)|null|
|**2024-08-15**|**LLM4DSR: Leveraing Large Language Model for Denoising Sequential Recommendation**|Bohao Wang et.al.|[2408.08208](http://arxiv.org/abs/2408.08208)|null|
|**2024-08-15**|**Scaling Up Natural Language Understanding for Multi-Robots Through the Lens of Hierarchy**|Shaojun Xu et.al.|[2408.08188](http://arxiv.org/abs/2408.08188)|null|
|**2024-08-14**|**The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models**|Karime Maamari et.al.|[2408.07702](http://arxiv.org/abs/2408.07702)|null|
|**2024-08-14**|**Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories, Applications and Opportunities**|Enneng Yang et.al.|[2408.07666](http://arxiv.org/abs/2408.07666)|**[link](https://github.com/ennengyang/awesome-model-merging-methods-theories-applications)**|
|**2024-08-14**|**Spoken Stereoset: On Evaluating Social Bias Toward Speaker in Speech Large Language Models**|Yi-Cheng Lin et.al.|[2408.07665](http://arxiv.org/abs/2408.07665)|**[link](https://github.com/dlion168/spoken_stereoset)**|
|**2024-08-14**|**Alignment-Enhanced Decoding:Defending via Token-Level Adaptive Refining of Probability Distributions**|Quan Liu et.al.|[2408.07663](http://arxiv.org/abs/2408.07663)|**[link](https://github.com/gigabaozi/aed)**|
|**2024-08-14**|**WeKnow-RAG: An Adaptive Approach for Retrieval-Augmented Generation Integrating Web Search and Knowledge Graphs**|Weijian Xie et.al.|[2408.07611](http://arxiv.org/abs/2408.07611)|null|
|**2024-08-14**|**Transformers and Large Language Models for Efficient Intrusion Detection Systems: A Comprehensive Survey**|Hamza Kheddar et.al.|[2408.07583](http://arxiv.org/abs/2408.07583)|null|
|**2024-08-14**|**MathScape: Evaluating MLLMs in multimodal Math Scenarios through a Hierarchical Benchmark**|Minxuan Zhou et.al.|[2408.07543](http://arxiv.org/abs/2408.07543)|**[link](https://github.com/PKU-Baichuan-MLSystemLab/MathScape)**|
|**2024-08-14**|**New Curriculum, New Chance -- Retrieval Augmented Generation for Lesson Planning in Ugandan Secondary Schools. Prototype Quality Evaluation**|Simon Kloker et.al.|[2408.07542](http://arxiv.org/abs/2408.07542)|null|
|**2024-08-14**|**Usefulness of data flow diagrams and large language models for security threat validation: a registered report**|Winnie Bahati Mbaka et.al.|[2408.07537](http://arxiv.org/abs/2408.07537)|null|
|**2024-08-14**|**Development of a Multi-Agent Clinical Decision Support System for Korean Triage and Acuity Scale (KTAS)-Based Triage and Treatment Planning in Emergency Departments**|Seungjun Han et.al.|[2408.07531](http://arxiv.org/abs/2408.07531)|null|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## text2sql

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-15**|**LR-SQL: A Supervised Fine-Tuning Method for Text2SQL Tasks under Low-Resource Scenarios**|Wen Wuzhenghong et.al.|[2410.11457](http://arxiv.org/abs/2410.11457)|**[link](https://github.com/hongwin/lr-sql)**|**大型语言模型通过监督微调在Text2SQL领域带来了革命性的变化，但一个关键的局限性被忽视了：数据库的复杂性导致上下文长度增加，从而增加了模型微调时对GPU内存的需求。为了解决这个问题，我们提出了LR-SQL。LR-SQL包括两个监督微调模型：schema_link模型和SQL_generation模型，其中schema_link模型是整个过程中的核心，用于简化整体流程。在对schema_link模型进行微调时，LR-SQL将完整的数据库分解成具有可调节数量的表的灵活组合，使模型能够从这些分散的片段中学习整个数据库内的关系。此外，为了增强模型在推理过程中感知各种离散片段之间关系的能力，LR-SQL训练了模型的链式思维能力来完成这一任务。实验结果表明，与现有的微调方法相比，LR-SQL可以将总的GPU内存使用量减少40%，而在schema_link任务中的表预测准确率仅下降2%。对于整体的Text2SQL任务，执行准确率下降了0.6%。我们的项目现已在https://github.com/hongWin/LR-SQL上可用。**|
|**2024-08-27**|**Text2SQL is Not Enough: Unifying AI and Databases with TAG**|Asim Biswal et.al.|[2408.14717](http://arxiv.org/abs/2408.14717)|**[link](https://github.com/tag-research/tag-bench)**|**能够通过自然语言查询数据库的人工智能系统有望释放巨大的价值。这类系统可以让用户同时利用语言模型的强大推理和知识能力，以及数据管理系统可扩展的计算能力。这些综合能力将使用户能够针对自定义数据源提出任意自然语言问题。然而，现有的方法和基准测试尚未充分探索这一领域。Text2SQL 方法仅关注可以通过关系代数表达的自然语言问题，这仅代表了真实用户想要提出的问题的一小部分。同样，检索增强生成（RAG）只考虑可以通过对数据库中的一个或几个数据记录进行点查找来回答的查询子集。我们提出了表增强生成（TAG），这是一种统一且通用的范式，用于回答基于数据库的自然语言问题。TAG 模型代表了之前未被探索过的语言模型与数据库之间广泛交互，并为利用语言模型在数据上的世界知识和推理能力创造了令人兴奋的研究机会。我们系统地开发了基准测试来研究 TAG 问题，并发现标准方法正确回答查询的比例不超过 20%，这证实了该领域需要进一步研究。我们在 https://github.com/TAG-Research/TAG-Bench 发布了基准测试代码。**|
|**2024-08-15**|**Can Large Language Models Understand Symbolic Graphics Programs?**|Zeju Qiu et.al.|[2408.08313](http://arxiv.org/abs/2408.08313)|null|
|**2024-08-15**|**ScalingFilter: Assessing Data Quality through Inverse Utilization of Scaling Laws**|Ruihang Li et.al.|[2408.08310](http://arxiv.org/abs/2408.08310)|null|
|**2024-08-15**|**Benchmarking the Capabilities of Large Language Models in Transportation System Engineering: Accuracy, Consistency, and Reasoning Behaviors**|Usman Syed et.al.|[2408.08302](http://arxiv.org/abs/2408.08302)|null|
|**2024-08-15**|**HELP: Hierarchical Embeddings-based Log Parsing**|Andy Xu et.al.|[2408.08300](http://arxiv.org/abs/2408.08300)|null|
|**2024-08-15**|**The ShareLM Collection and Plugin: Contributing Human-Model Chats for the Benefit of the Community**|Shachar Don-Yehiya et.al.|[2408.08291](http://arxiv.org/abs/2408.08291)|null|
|**2024-08-15**|**Autonomous Behavior Planning For Humanoid Loco-manipulation Through Grounded Language Model**|Jin Wang et.al.|[2408.08282](http://arxiv.org/abs/2408.08282)|null|
|**2024-08-15**|**BAM! Just Like That: Simple and Efficient Parameter Upcycling for Mixture of Experts**|Qizhen Zhang et.al.|[2408.08274](http://arxiv.org/abs/2408.08274)|null|
|**2024-08-15**|**DaRec: A Disentangled Alignment Framework for Large Language Model and Recommender System**|Xihong Yang et.al.|[2408.08231](http://arxiv.org/abs/2408.08231)|null|
|**2024-08-15**|**RED-CT: A Systems Design Methodology for Using LLM-labeled Data to Train and Deploy Edge Classifiers for Computational Social Science**|David Farr et.al.|[2408.08217](http://arxiv.org/abs/2408.08217)|null|
|**2024-08-15**|**Does Reasoning Emerge? Examining the Probabilities of Causation in Large Language Models**|Javier González et.al.|[2408.08210](http://arxiv.org/abs/2408.08210)|null|
|**2024-08-14**|**The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models**|Karime Maamari et.al.|[2408.07702](http://arxiv.org/abs/2408.07702)|null|
|**2024-08-14**|**Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories, Applications and Opportunities**|Enneng Yang et.al.|[2408.07666](http://arxiv.org/abs/2408.07666)|**[link](https://github.com/ennengyang/awesome-model-merging-methods-theories-applications)**|
|**2024-08-14**|**Spoken Stereoset: On Evaluating Social Bias Toward Speaker in Speech Large Language Models**|Yi-Cheng Lin et.al.|[2408.07665](http://arxiv.org/abs/2408.07665)|**[link](https://github.com/dlion168/spoken_stereoset)**|
|**2024-08-14**|**Alignment-Enhanced Decoding:Defending via Token-Level Adaptive Refining of Probability Distributions**|Quan Liu et.al.|[2408.07663](http://arxiv.org/abs/2408.07663)|**[link](https://github.com/gigabaozi/aed)**|
|**2024-08-14**|**WeKnow-RAG: An Adaptive Approach for Retrieval-Augmented Generation Integrating Web Search and Knowledge Graphs**|Weijian Xie et.al.|[2408.07611](http://arxiv.org/abs/2408.07611)|null|
|**2024-08-14**|**Transformers and Large Language Models for Efficient Intrusion Detection Systems: A Comprehensive Survey**|Hamza Kheddar et.al.|[2408.07583](http://arxiv.org/abs/2408.07583)|null|
|**2024-08-14**|**MathScape: Evaluating MLLMs in multimodal Math Scenarios through a Hierarchical Benchmark**|Minxuan Zhou et.al.|[2408.07543](http://arxiv.org/abs/2408.07543)|**[link](https://github.com/PKU-Baichuan-MLSystemLab/MathScape)**|
|**2024-08-14**|**Usefulness of data flow diagrams and large language models for security threat validation: a registered report**|Winnie Bahati Mbaka et.al.|[2408.07537](http://arxiv.org/abs/2408.07537)|null|
|**2024-08-14**|**Development of a Multi-Agent Clinical Decision Support System for Korean Triage and Acuity Scale (KTAS)-Based Triage and Treatment Planning in Emergency Departments**|Seungjun Han et.al.|[2408.07531](http://arxiv.org/abs/2408.07531)|null|
|**2024-08-14**|**Large Language Models Know What Makes Exemplary Contexts**|Quanyu Long et.al.|[2408.07505](http://arxiv.org/abs/2408.07505)|null|
|**2024-08-09**|**A Survey of NL2SQL with Large Language Models: Where are we, and where are we going?**|Xinyu Liu et.al.|[2408.05109](http://arxiv.org/abs/2408.05109)|**[link](https://github.com/hkustdial/nl2sql_handbook)**|**将用户的自然语言查询（NL）转换为SQL查询（即NL2SQL）可以显著降低访问关系数据库的障碍，并支持各种商业应用。随着大型语言模型（LLMs）的出现，NL2SQL的性能得到了极大的提升。在这篇综述中，我们全面回顾了由LLMs驱动的NL2SQL技术，涵盖了从以下四个方面看其整个生命周期：(1) 模型：处理不仅包括自然语言的歧义和不完全指定问题，还包括正确映射自然语言与数据库模式及实例的NL2SQL翻译技术；(2) 数据：从训练数据收集、由于训练数据稀缺而进行的数据合成，到NL2SQL基准测试；(3) 评估：使用不同的度量标准和粒度从多个角度评估NL2SQL方法；以及(4) 错误分析：分析NL2SQL错误以找到根本原因，并指导NL2SQL模型进化。此外，我们为开发NL2SQL解决方案提供了经验法则。最后，我们讨论了在LLMs时代NL2SQL的研究挑战和开放问题。**|
|**2024-07-21**|**Towards Automated Data Sciences with Natural Language and SageCopilot: Practices and Lessons Learned**|Yuan Liao et.al.|[2407.21040](http://arxiv.org/abs/2407.21040)|null|尽管自然语言转SQL（NL2SQL）领域在将自然语言指令转换为可执行的SQL脚本以进行数据查询和处理方面取得了显著进展，但在更广泛的数据科学管道中实现全面自动化——包括数据查询、分析、可视化和报告——仍然是一个复杂的挑战。本研究介绍了SageCopilot，这是一个先进的工业级系统，通过集成大规模语言模型（LLMs）、自主代理（AutoAgents）和语言用户界面（LUIs），实现了数据科学管道的自动化。具体来说，SageCopilot采用了两阶段设计：在线组件通过上下文学习（ICL）细化用户的输入，将其转化为可执行脚本，并运行这些脚本来生成结果报告与可视化；离线准备由在线阶段ICL请求的演示示例。一系列流行策略如思维链和提示调优被用来增强SageCopilot的性能。通过严格的测试和与基于提示解决方案的对比分析，SageCopilot已经在实际数据集上被实证验证，在生成或执行脚本以及提供带有可视化的结果方面具有优越的端到端性能。我们深入的消融研究表明了SageCopilot所使用的各个组件和策略对数据科学端到端正确性的个别贡献。|
|**2024-06-12**|**DeTriever: Decoder-representation-based Retriever for Improving NL2SQL In-Context Learning**|Yuxi Feng et.al.|[2406.07913](http://arxiv.org/abs/2406.07913)|null|虽然上下文学习（ICL）已被证明是提高大型语言模型（LLMs）在多种复杂任务中表现的有效技术，尤其是在将自然语言问题转换为结构化查询语言（NL2SQL）方面，但如何选择最有益的示例仍然是一个开放的研究问题。以往的工作通常采用现成的编码器来动态检索示例，但外部检索器与LLMs之间的表示能力存在固有差异。此外，优化示例的选择是一个非平凡的任务，因为没有直接的方法可以在不进行两两推理的情况下评估示例的相对收益。为了解决这些不足，我们提出了DeTriever，这是一种新颖的示例检索框架，它学习了LLM隐藏状态的加权组合，其中编码了丰富的语义信息。为了训练模型，我们提出了一种代理分数，该分数基于输出查询之间的相似性来估计示例的相对收益。在两个流行的NL2SQL基准测试上的实验表明，我们的方法在一击NL2SQL任务上显著优于最先进的基线。|
|**2024-07-27**|**The Dawn of Natural Language to SQL: Are We Fully Ready?**|Boyan Li et.al.|[2406.01265](http://arxiv.org/abs/2406.01265)|**[link](https://github.com/hkustdial/nl2sql360)**|**将用户的自然语言问题转换为SQL查询（即NL2SQL）显著降低了访问关系数据库的门槛。大型语言模型的出现为NL2SQL任务引入了新的范式，极大地提升了能力。然而，这引发了一个关键问题：我们是否已经完全准备好将NL2SQL模型投入生产使用？为了解答这个问题，我们提出了一个多角度的NL2SQL评估框架NL2SQL360，以帮助研究人员设计和测试新的NL2SQL方法。通过NL2SQL360，我们对领先的NL2SQL方法在不同应用场景下进行了详细比较，如不同的数据领域和SQL特性，提供了宝贵的信息来选择最适合特定需求的NL2SQL方法。此外，我们探索了NL2SQL的设计空间，利用NL2SQL360自动化地识别出一个针对用户特定需求优化的最佳NL2SQL解决方案。特别地，NL2SQL360识别出了一种有效的NL2SQL方法SuperSQL，在Spider数据集上使用执行准确度指标表现突出。值得注意的是，SuperSQL在Spider和BIRD测试集上分别达到了87%和62.66%的执行准确度，表现出色。**|
|**2024-05-01**|**ChatBI: Towards Natural Language to Complex Business Intelligence SQL**|Jinqing Lian et.al.|[2405.00527](http://arxiv.org/abs/2405.00527)|null|自然语言到SQL（NL2SQL）技术为不熟悉数据库的非专家用户提供了使用SQL进行数据分析的机会。将自然语言转换为商业智能（NL2BI）是实际生产系统中NL2SQL的一个流行实用场景。与NL2SQL相比，NL2BI引入了更多挑战。在这篇论文中，我们提出了ChatBI，这是一种全面而高效的技术，用于解决NL2BI任务。首先，我们分析了交互模式，这是NL2SQL和NL2BI在使用上一个重要的不同模块，并设计了一个更小、更便宜的模型来匹配这种交互模式。在BI场景中，表格包含大量的列，这使得依赖大型语言模型（LLMs）进行模式链接的现有NL2SQL方法由于令牌限制无法继续进行。BI场景中模糊列的较高比例也使得模式链接变得困难。ChatBI结合了数据库社区现有的视图技术，首先将模式链接问题分解为单视图选择问题，然后使用一个更小且更便宜的机器学习模型来选择具有显著减少列数的单个视图。这个单视图的列随后作为所需的列传递给LLM进行模式链接。最后，ChatBI提出了一种与现有流程不同的分阶段处理流程，使ChatBI能够更准确地生成包含复杂语义和比较关系的SQL。我们已在百度的数据平台上部署了ChatBI，并将其集成到多条产品线中进行大规模生产任务评估。所获得的结果突显了其在实用性、通用性和效率方面的优越性。同时，在我们的真实BI场景数据表和查询下，与当前主流的NL2SQL技术相比，它也取得了最佳结果。|
|**2024-03-29**|**PURPLE: Making a Large Language Model a Better SQL Writer**|Tonghui Ren et.al.|[2403.20014](http://arxiv.org/abs/2403.20014)|null|大型语言模型（LLM）技术在自然语言到SQL（NL2SQL）翻译中发挥着越来越重要的作用。通过广泛语料库训练的LLM具有强大的自然语言理解和基本的SQL生成能力，无需针对NL2SQL任务进行额外的特定调优。现有的基于LLM的NL2SQL方法试图通过增强用户意图理解来改进翻译。然而，由于缺乏组织复杂逻辑运算符组合的知识，LLM有时无法生成合适的SQL。一种有前景的方法是向LLM输入演示示例，这些示例包括来自各种数据库的已知NL2SQL翻译。LLM可以从输入的演示示例中学习如何为给定任务组织运算符组合。在本文中，我们提出了PURPLE（利用预训练模型检索提示以增强逻辑），该方法通过检索包含所需逻辑运算符组合的演示示例来提高准确性，从而指导LLM生成更好的SQL翻译。PURPLE在流行的NL2SQL基准测试Spider的验证集上实现了新的最佳性能，精确匹配准确率为80.5%，执行匹配准确率为87.8%。PURPLE在不同的基准测试、预算限制和各种LLM上保持了高准确性，显示出其鲁棒性和成本效益。|
|**2024-03-24**|**SQL-Encoder: Improving NL2SQL In-Context Learning Through a Context-Aware Encoder**|Mohammadreza Pourreza et.al.|[2403.16204](http://arxiv.org/abs/2403.16204)|null|检测查询之间的结构相似性对于在上下文学习模型中选择示例至关重要。然而，仅基于查询的自然语言表达而不考虑SQL查询来评估结构相似性是一个重大挑战。本文探讨了这种相似性度量的重要性，并提出了一种准确估计它的模型。为此，我们利用了一个包含17万问题对的数据集，精心策划以训练一个相似性预测模型。我们的综合评估表明，所提出的模型能够很好地捕捉问题之间的结构相似性，这体现在Kendall-Tau距离和precision@k指标的改进上。值得注意的是，我们的模型优于来自OpenAI和Cohere的强大竞争嵌入模型。此外，与这些竞争模型相比，我们提出的编码器在1-shot上下文学习场景中提高了NL2SQL模型的下游性能，对于GPT-3.5-turbo提升了1-2%，对于CodeLlama-7B提升了4-8%，对于CodeLlama-13B提升了2-3%。|
|**2024-06-02**|**PET-SQL: A Prompt-Enhanced Two-Round Refinement of Text-to-SQL with Cross-consistency**|Zhishuai Li et.al.|[2403.09732](http://arxiv.org/abs/2403.09732)|**[link](https://github.com/zhshlii/petsql)**|**最近在文本到SQL（Text2SQL）方面的进展强调了通过上下文学习来激发大型语言模型（LLM），取得了显著成果。然而，当处理冗长的数据库信息和复杂的用户意图时，它们仍面临挑战。本文提出了一种两阶段框架，以提高当前基于LLM的自然语言到SQL系统的性能。首先，我们引入了一种新颖的提示表示方法，称为参考增强表示，该方法包括模式信息和从表中随机抽样的单元格值，以指导LLM生成SQL查询。然后，在第一阶段，检索问题-SQL对作为少样本示例，促使LLM生成初步SQL（PreSQL）。之后，解析PreSQL中提到的实体进行模式链接，这可以显著压缩有用信息。在第二阶段，利用已链接的模式，简化提示中的模式信息，并指导LLM生成最终SQL。最后，作为后优化模块，我们建议使用不同LLM之间的交叉一致性，而不是特定LLM内的自一致性。我们的方法在Spider基准测试上达到了新的SOTA结果，执行准确率为87.6%。**|
|**2024-09-05**|**Aligning Large Language Models to a Domain-specific Graph Database for NL2GQL**|Yuanyuan Liang et.al.|[2402.16567](http://arxiv.org/abs/2402.16567)|null|
|**2024-08-06**|**Intent-Based Access Control: Using LLMs to Intelligently Manage Access Control**|Pranav Subramaniam et.al.|[2402.07332](http://arxiv.org/abs/2402.07332)|null|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## AIOps

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-08-15**|**Can Large Language Models Understand Symbolic Graphics Programs?**|Zeju Qiu et.al.|[2408.08313](http://arxiv.org/abs/2408.08313)|null|
|**2024-08-15**|**ScalingFilter: Assessing Data Quality through Inverse Utilization of Scaling Laws**|Ruihang Li et.al.|[2408.08310](http://arxiv.org/abs/2408.08310)|null|
|**2024-08-15**|**Benchmarking the Capabilities of Large Language Models in Transportation System Engineering: Accuracy, Consistency, and Reasoning Behaviors**|Usman Syed et.al.|[2408.08302](http://arxiv.org/abs/2408.08302)|null|
|**2024-08-15**|**HELP: Hierarchical Embeddings-based Log Parsing**|Andy Xu et.al.|[2408.08300](http://arxiv.org/abs/2408.08300)|null|
|**2024-08-15**|**The ShareLM Collection and Plugin: Contributing Human-Model Chats for the Benefit of the Community**|Shachar Don-Yehiya et.al.|[2408.08291](http://arxiv.org/abs/2408.08291)|null|
|**2024-08-15**|**Autonomous Behavior Planning For Humanoid Loco-manipulation Through Grounded Language Model**|Jin Wang et.al.|[2408.08282](http://arxiv.org/abs/2408.08282)|null|
|**2024-08-15**|**BAM! Just Like That: Simple and Efficient Parameter Upcycling for Mixture of Experts**|Qizhen Zhang et.al.|[2408.08274](http://arxiv.org/abs/2408.08274)|null|
|**2024-08-15**|**DaRec: A Disentangled Alignment Framework for Large Language Model and Recommender System**|Xihong Yang et.al.|[2408.08231](http://arxiv.org/abs/2408.08231)|null|
|**2024-08-15**|**RED-CT: A Systems Design Methodology for Using LLM-labeled Data to Train and Deploy Edge Classifiers for Computational Social Science**|David Farr et.al.|[2408.08217](http://arxiv.org/abs/2408.08217)|null|
|**2024-08-15**|**Does Reasoning Emerge? Examining the Probabilities of Causation in Large Language Models**|Javier González et.al.|[2408.08210](http://arxiv.org/abs/2408.08210)|null|
|**2024-08-15**|**System States Forecasting of Microservices with Dynamic Spatio-Temporal Data**|Yifei Xu et.al.|[2408.07894](http://arxiv.org/abs/2408.07894)|null|
|**2024-08-14**|**The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models**|Karime Maamari et.al.|[2408.07702](http://arxiv.org/abs/2408.07702)|null|
|**2024-08-14**|**Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories, Applications and Opportunities**|Enneng Yang et.al.|[2408.07666](http://arxiv.org/abs/2408.07666)|**[link](https://github.com/ennengyang/awesome-model-merging-methods-theories-applications)**|
|**2024-08-14**|**Spoken Stereoset: On Evaluating Social Bias Toward Speaker in Speech Large Language Models**|Yi-Cheng Lin et.al.|[2408.07665](http://arxiv.org/abs/2408.07665)|**[link](https://github.com/dlion168/spoken_stereoset)**|
|**2024-08-14**|**Alignment-Enhanced Decoding:Defending via Token-Level Adaptive Refining of Probability Distributions**|Quan Liu et.al.|[2408.07663](http://arxiv.org/abs/2408.07663)|**[link](https://github.com/gigabaozi/aed)**|
|**2024-08-14**|**WeKnow-RAG: An Adaptive Approach for Retrieval-Augmented Generation Integrating Web Search and Knowledge Graphs**|Weijian Xie et.al.|[2408.07611](http://arxiv.org/abs/2408.07611)|null|
|**2024-08-14**|**Transformers and Large Language Models for Efficient Intrusion Detection Systems: A Comprehensive Survey**|Hamza Kheddar et.al.|[2408.07583](http://arxiv.org/abs/2408.07583)|null|
|**2024-08-14**|**MathScape: Evaluating MLLMs in multimodal Math Scenarios through a Hierarchical Benchmark**|Minxuan Zhou et.al.|[2408.07543](http://arxiv.org/abs/2408.07543)|**[link](https://github.com/PKU-Baichuan-MLSystemLab/MathScape)**|
|**2024-08-14**|**Usefulness of data flow diagrams and large language models for security threat validation: a registered report**|Winnie Bahati Mbaka et.al.|[2408.07537](http://arxiv.org/abs/2408.07537)|null|
|**2024-08-14**|**Development of a Multi-Agent Clinical Decision Support System for Korean Triage and Acuity Scale (KTAS)-Based Triage and Treatment Planning in Emergency Departments**|Seungjun Han et.al.|[2408.07531](http://arxiv.org/abs/2408.07531)|null|
|**2024-08-14**|**Large Language Models Know What Makes Exemplary Contexts**|Quanyu Long et.al.|[2408.07505](http://arxiv.org/abs/2408.07505)|null|
|**2024-07-09**|**A Scenario-Oriented Benchmark for Assessing AIOps Algorithms in Microservice Management**|Yongqian Sun et.al.|[2407.14532](http://arxiv.org/abs/2407.14532)|**[link](https://github.com/microservo/hot-plugging)**|
|**2024-07-31**|**Building AI Agents for Autonomous Clouds: Challenges and Design Principles**|Manish Shetty et.al.|[2407.12165](http://arxiv.org/abs/2407.12165)|null|
|**2024-07-02**|**LogEval: A Comprehensive Benchmark Suite for Large Language Models In Log Analysis**|Tianyu Cui et.al.|[2407.01896](http://arxiv.org/abs/2407.01896)|**[link](https://github.com/LinDuoming/LogEval)**|
|**2024-06-24**|**A Survey of AIOps for Failure Management in the Era of Large Language Models**|Lingzhe Zhang et.al.|[2406.11213](http://arxiv.org/abs/2406.11213)|null|
|**2024-05-13**|**AnomalyLLM: Few-shot Anomaly Edge Detection for Dynamic Graphs using Large Language Models**|Shuo Liu et.al.|[2405.07626](http://arxiv.org/abs/2405.07626)|**[link](https://github.com/anomalyllm/anomalyllm)**|
|**2024-04-24**|**Anomaly Detection for Incident Response at Scale**|Hanzhang Wang et.al.|[2404.16887](http://arxiv.org/abs/2404.16887)|null|
|**2024-05-03**|**mABC: multi-Agent Blockchain-Inspired Collaboration for root cause analysis in micro-services architecture**|Wei Zhang et.al.|[2404.12135](http://arxiv.org/abs/2404.12135)|**[link](https://github.com/knediny/mABC)**|
|**2024-04-12**|**Efficient Interactive LLM Serving with Proxy Model-based Sequence Length Prediction**|Haoran Qiu et.al.|[2404.08509](http://arxiv.org/abs/2404.08509)|**[link](https://github.com/james-qiuhaoran/llm-serving-with-proxy-models)**|
|**2024-04-01**|**AIOps Solutions for Incident Management: Technical Guidelines and A Comprehensive Literature Review**|Youcef Remil et.al.|[2404.01363](http://arxiv.org/abs/2404.01363)|null|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## PPC

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-24**|**FedSPD: A Soft-clustering Approach for Personalized Decentralized Federated Learning**|I-Cheng Lin et.al.|[2410.18862](http://arxiv.org/abs/2410.18862)|null|联邦学习作为一种分布式客户端使用本地数据协同训练机器学习模型的框架，最近越来越受到关注。虽然传统的联邦学习依赖于中央服务器进行模型聚合，但最近的进展采用了去中心化的框架，使得客户端之间可以直接交换模型，消除了单点故障的问题。然而，现有的去中心化框架通常假设所有客户端都在训练一个共享模型。针对每个客户端的数据分布差异，个性化每个客户端的模型可以提高性能。我们提出了一种高效的去中心化个性化联邦学习算法FedSPD，并展示了它即使在低连通性网络中也能学习到准确的模型。为了提供收敛性的理论保证，我们引入了一个基于聚类的框架，该框架能够在不同数据集群上达成模型共识，同时根据各个客户端独特的数据集群混合情况进行个性化处理。这种灵活性允许根据数据分布选择性地更新模型，从而显著降低了与先前工作相比的通信成本。在真实数据集上的实验结果表明，FedSPD在低连通性网络场景下优于多种去中心化的个性化联邦学习算法变体。|
|**2024-10-24**|**Adapting MLOps for Diverse In-Network Intelligence in 6G Era: Challenges and Solutions**|Peizheng Li et.al.|[2410.18793](http://arxiv.org/abs/2410.18793)|null|无缝集成人工智能（AI）和机器学习（ML）技术与无线系统是6G智能化的关键步骤。然而，这种集成在模型功能和生命周期管理方面面临挑战。机器学习运维（MLOps）提供了一种系统化的方法来应对这些挑战。现有的在集中式平台上实施MLOps的方法往往忽视了不同学习范式和网络异构性所带来的挑战。本文提出了一种针对未来无线网络复杂性的新型MLOps方法。考虑到未来无线接入网（RAN）的独特方面，我们制定了三种操作流水线，即强化学习运维（RLOps）、联邦学习运维（FedOps）和生成式AI运维（GenOps）。这些流水线为将各种学习/推理能力无缝集成到网络中奠定了基础。我们概述了每种操作的具体挑战及提出的解决方案，以促进大规模部署AI原生的6G网络。|
|**2024-10-24**|**Classifier Clustering and Feature Alignment for Federated Learning under Distributed Concept Drift**|Junbao Chen et.al.|[2410.18478](http://arxiv.org/abs/2410.18478)|**[link](https://github.com/chen-junbao/fedccfa)**|**数据异质性是联邦学习中的一个关键挑战，已经有很多工作致力于解决这个问题。然而，带有数据异质性的分布式概念漂移，即客户端可能经历不同的概念漂移，仍然是一个未被充分探索的领域。在这项工作中，我们重点关注真实漂移，即条件分布P(Y,X)发生变化的情况。我们首先研究了分布式概念漂移如何影响模型训练，并发现局部分类器在漂移适应中起着关键作用。此外，为了解决数据异质性问题，我们在分布式概念漂移下研究了特征对齐，并发现了对特征对齐至关重要的两个因素：条件分布P(Y,X)和数据异质性的程度。基于上述发现，我们提出了FedCCFA，一种具有分类器聚类和特征对齐功能的联邦学习框架。为了增强在分布式概念漂移下的协作能力，FedCCFA在类别级别对局部分类器进行聚类，并根据聚类结果生成聚类特征锚点。借助这些锚点，FedCCFA基于标签分布P(Y)的熵自适应地对齐客户端的特征空间，从而缓解特征空间的一致性问题。我们的结果显示，在各种概念漂移设置下，FedCCFA显著优于现有方法。代码可在https://github.com/Chen-Junbao/FedCCFA获取。**|
|**2024-10-24**|**FedBaF: Federated Learning Aggregation Biased by a Foundation Model**|Jong-Ik Park et.al.|[2410.18352](http://arxiv.org/abs/2410.18352)|null|由于基础模型能够泛化到多种任务，它们现在已成为领先技术组织的主要关注点。现有的将基础模型适应于新应用的方法通常依赖于联邦学习（FL），并在使用基础模型初始化全局模型时向客户端披露基础模型的权重。虽然这些方法确保了客户端数据隐私，但它们牺牲了模型和信息安全。在本文中，我们介绍了一种名为FedBaF（基于基础模型偏置的联邦学习聚合）的新方法，该方法能够在联邦学习聚合阶段动态集成预训练的基础模型权重。与传统方法不同，FedBaF保持了基础模型的机密性，同时仍能利用其强大的能力来训练更准确的模型，尤其是在非独立同分布（non-IID）和对抗场景中。通过全面的实验，我们使用Pre-ResNet和Vision Transformer等基础模型展示了FedBaF不仅在独立同分布设置下达到了传统权重初始化方法的测试精度，甚至超越了它们高达11.4%，而在非独立同分布设置下则提高了多达15.8%。此外，当应用于基于Transformer的语言模型时，FedBaF显著降低了困惑度，最多可达39.2%。|
|**2024-10-23**|**LEGO: Language Model Building Blocks**|Shrenik Bhansali et.al.|[2410.18287](http://arxiv.org/abs/2410.18287)|null|大型语言模型（LLMs）在自然语言处理（NLP）中至关重要，但在数据收集、预训练、微调和推理方面成本高昂。针对特定任务的小型语言模型（SLMs）虽然成本较低，但缺乏鲁棒性和泛化能力。本文提出了一种名为LEGO的新技术，可以从LLM中提取SLMs并重新组合。通过使用最先进的LLM剪枝策略，我们可以创建针对任务和用户特定的SLM构建块，这些构建块在微调和推理时效率更高，同时还能保护用户数据隐私。LEGO利用联邦学习和一种新的聚合方案来重建LLM，在保持鲁棒性的同时无需高昂的成本，并且能够保护用户数据隐私。我们通过实验展示了LEGO的多功能性，证明了其能够在保持LLM鲁棒性的同时实现模型异质性并减轻数据异质性的影响。|
|**2024-10-23**|**ProFL: Performative Robust Optimal Federated Learning**|Xue Zheng et.al.|[2410.18075](http://arxiv.org/abs/2410.18075)|null|表现性预测（PP）是一个框架，用于捕捉由于机器学习模型部署而导致的训练过程中数据分布的变化。随着训练模型的使用，其生成的数据可能导致模型演变，从而偏离原始数据分布。尽管在联邦学习（FL）设置中，这种由模型引起的数据分布变化在实际应用中越来越有可能发生，但其影响尚未得到探索。虽然Jin等人（2024）最近以一种直接的方式将PP扩展到了FL，但由此产生的模型仅收敛到一个表现性稳定点，这可能远非最优。Izzo等人（2021）和Miller等人（2021）的方法可以在集中式设置中找到表现性最优点，但它们要求表现性风险是凸的且训练数据无噪声，这些假设在现实的FL系统中往往不成立。本文克服了所有这些缺点，并提出了表现性鲁棒最优联邦学习（ProFL），这是一种算法，可以从有噪声和污染的数据中在FL中找到表现性最优点。我们在Polyak-Lojasiewicz条件下进行了收敛分析，该条件适用于非凸目标。在多个数据集上的广泛实验验证了我们所提出算法的有效性。|
|**2024-10-23**|**Federated Transformer: Multi-Party Vertical Federated Learning on Practical Fuzzily Linked Data**|Zhaomin Wu et.al.|[2410.17986](http://arxiv.org/abs/2410.17986)|**[link](https://github.com/xtra-computing/fet)**|**联邦学习（FL）是一种新兴的范式，它使多个参与者能够在不共享原始数据的情况下协同训练模型。在其变体中，垂直联邦学习（VFL）在现实世界的跨组织协作中特别相关，其中不同参与者贡献了共享实例组的不同特征。在这种情况下，参与者通常使用模糊标识符进行链接，从而形成一种称为多方模糊VFL的常见做法。现有的模型通常解决的是多方VFL或两方之间的模糊VFL问题。将这些模型扩展到实际的多方模糊VFL场景通常会导致性能显著下降，并增加维护隐私的成本。为了解决这些限制，我们引入了联邦变换器（FeT），这是一种支持带有模糊标识符的多方VFL的新框架。FeT创新地将这些标识符编码为数据表示，并采用分布在不同参与者之间的变换器架构，结合三种新技术以提高性能。此外，我们开发了一种用于VFL的多方隐私框架，该框架集成了差分隐私与安全多方计算，有效保护本地表示的同时最小化相关的效用成本。我们的实验表明，在扩展到50个参与者时，FeT的准确率比基线模型高出46%。此外，在两方模糊VFL设置中，FeT在性能和隐私方面也优于最前沿的VFL模型。**|
|**2024-10-23**|**Multi-Continental Healthcare Modelling Using Blockchain-Enabled Federated Learning**|Rui Sun et.al.|[2410.17933](http://arxiv.org/abs/2410.17933)|null|在医疗领域构建人工智能（AI）模型面临的最大挑战之一是数据共享。由于医疗数据具有私密性、敏感性和异质性，收集足够的建模数据既耗时又成本高昂，有时甚至是不可能的。本文提出了一种利用来自多个大陆（欧洲、北美和亚洲）的数据集进行全球医疗建模的框架，而无需共享本地数据集，并以血糖管理作为研究模型来验证其有效性。技术上，我们实施了区块链支持的联邦学习并进行了适应性调整，使其符合医疗数据的隐私和安全要求，同时通过链上激励机制奖励诚实参与并对恶意活动进行惩罚。实验结果表明，所提出的框架是有效、高效且保护隐私的。其预测准确性远优于基于有限个人数据训练的模型，甚至与集中式数据集的结果相当或略好。这项工作为国际医疗项目的合作铺平了道路，在这些项目中，额外的数据对于减少偏见和造福人类至关重要。|
|**2024-10-23**|**Enhancing Federated Learning Convergence with Dynamic Data Queue and Data Entropy-driven Participant Selection**|Charuka Herath et.al.|[2410.17792](http://arxiv.org/abs/2410.17792)|null|联邦学习（FL）是一种在边缘设备上进行协作模型训练的去中心化方法。这种分布式模型训练方式在隐私、安全、法规遵从性和成本效率方面具有优势。本研究的重点在于解决FL中的统计复杂性问题，尤其是在本地存储的数据不是独立同分布（非IID）的情况下。我们观察到，在数据偏斜场景中，即每个边缘设备仅用一类数据进行训练时，模型准确率降低了大约10%到30%。这种降低归因于权重发散，通过计算设备级类别分布与总体分布之间的欧几里得距离来量化，从而得到偏差项（\(\delta_k\)）。作为解决方案，我们提出了一种通过在服务器上创建全局数据子集并使用动态数据队列驱动的联邦学习（DDFL）将其动态分配给各个设备的方法以改善收敛性。此外，我们利用数据熵指标来监控每轮训练过程，并合理选择参与聚合的设备。我们还提供了所提DDFL的收敛性分析，证明其在实际FL场景中的可行性，目标是实现更好的设备选择、非次优的全局模型以及更快的收敛速度。我们观察到，对于MNIST数据集，我们的方法使准确率提高了约5%，对于CIFAR-10和CIFAR-100分别提高了约18%和20%，使用了10%的全局数据子集，表现优于当前最先进的聚合算法。|
|**2024-10-23**|**Towards Active Participant-Centric Vertical Federated Learning: Some Representations May Be All You Need**|Jon Irureta et.al.|[2410.17648](http://arxiv.org/abs/2410.17648)|null|垂直联邦学习（VFL）能够在不同参与者之间进行协作模型训练，这些参与者拥有不同的特征但共享相同的样本，并且能够保护数据隐私。现有的VFL方法在处理实际数据划分时往往面临高通信成本和显著的操作复杂性问题。在这项工作中，我们提出了一种新的简化VFL方法，即以主动参与者为中心的VFL（APC-VFL），据我们所知，这是首个仅需单次通信轮次的方法，并允许主动参与者以非协作方式执行推理。该方法结合了无监督表示学习与知识蒸馏技术，在经典设置下达到了与传统基于垂直分割学习的VFL方法相当的准确率，同时将所需的通信轮次减少了高达4200倍，更具灵活性。我们的方法相比非联邦本地模型以及一种可比较的VFL提案VFedTrans也显示出改进，提供了一种高效且灵活的协作学习解决方案。|
|**2024-10-23**|**Securing Federated Learning Against Novel and Classic Backdoor Threats During Foundation Model Integration**|Xiaohuan Bi et.al.|[2410.17573](http://arxiv.org/abs/2410.17573)|null|
|**2024-10-23**|**Which Client is Reliable?: A Reliable and Personalized Prompt-based Federated Learning for Medical Image Question Answering**|He Zhu et.al.|[2410.17484](http://arxiv.org/abs/2410.17484)|null|
|**2024-10-22**|**Data Obfuscation through Latent Space Projection (LSP) for Privacy-Preserving AI Governance: Case Studies in Medical Diagnosis and Finance Fraud Detection**|Mahesh Vaijainthymala Krishnamoorthy et.al.|[2410.17459](http://arxiv.org/abs/2410.17459)|null|
|**2024-10-22**|**Meta Stackelberg Game: Robust Federated Learning against Adaptive and Mixed Poisoning Attacks**|Tao Li et.al.|[2410.17431](http://arxiv.org/abs/2410.17431)|null|
|**2024-10-22**|**Deep Learning Aided Broadcast Codes with Feedback**|Jacqueline Malayter et.al.|[2410.17404](http://arxiv.org/abs/2410.17404)|null|
|**2024-10-22**|**Beyond Yao's Millionaires: Secure Multi-Party Computation of Non-Polynomial Functions**|Seyed Reza Hoseini Najarkolaei et.al.|[2410.17000](http://arxiv.org/abs/2410.17000)|null|
|**2024-10-22**|**Federated Causal Inference: Multi-Centric ATE Estimation beyond Meta-Analysis**|Rémi Khellaf et.al.|[2410.16870](http://arxiv.org/abs/2410.16870)|null|
|**2024-10-21**|**Subword Embedding from Bytes Gains Privacy without Sacrificing Accuracy and Complexity**|Mengjiao Zhang et.al.|[2410.16410](http://arxiv.org/abs/2410.16410)|null|
|**2024-10-21**|**DMM: Distributed Matrix Mechanism for Differentially-Private Federated Learning using Packed Secret Sharing**|Alexander Bienstock et.al.|[2410.16161](http://arxiv.org/abs/2410.16161)|null|
|**2024-10-21**|**Extracting Spatiotemporal Data from Gradients with Large Language Models**|Lele Zheng et.al.|[2410.16121](http://arxiv.org/abs/2410.16121)|null|
|**2024-10-21**|**Distributed Learning for UAV Swarms**|Chen Hu et.al.|[2410.15882](http://arxiv.org/abs/2410.15882)|null|
|**2024-10-21**|**Geographical Node Clustering and Grouping to Guarantee Data IIDness in Federated Learning**|Minkwon Lee et.al.|[2410.15693](http://arxiv.org/abs/2410.15693)|null|
|**2024-10-21**|**Federated Learning with MMD-based Early Stopping for Adaptive GNSS Interference Classification**|Nishant S. Gaikwad et.al.|[2410.15681](http://arxiv.org/abs/2410.15681)|null|
|**2024-10-22**|**A Bayesian Framework for Clustered Federated Learning**|Peng Wu et.al.|[2410.15473](http://arxiv.org/abs/2410.15473)|null|
|**2024-10-20**|**Tighter Performance Theory of FedExProx**|Wojciech Anyszka et.al.|[2410.15368](http://arxiv.org/abs/2410.15368)|null|
|**2024-10-19**|**DPVS-Shapley:Faster and Universal Contribution Evaluation Component in Federated Learning**|Ketin Yin et.al.|[2410.15093](http://arxiv.org/abs/2410.15093)|null|
|**2024-10-19**|**Personalized Federated Learning with Adaptive Feature Aggregation and Knowledge Transfer**|Keting Yin et.al.|[2410.15073](http://arxiv.org/abs/2410.15073)|null|
|**2024-10-18**|**FedSpaLLM: Federated Pruning of Large Language Models**|Guangji Bai et.al.|[2410.14852](http://arxiv.org/abs/2410.14852)|null|
|**2024-10-18**|**Personalizing Low-Rank Bayesian Neural Networks Via Federated Learning**|Boning Zhang et.al.|[2410.14390](http://arxiv.org/abs/2410.14390)|null|
|**2024-10-18**|**Comparative Evaluation of Clustered Federated Learning Method**|Michael Ben Ali et.al.|[2410.14212](http://arxiv.org/abs/2410.14212)|**[link](https://github.com/leahcimali/Comparative-Evaluation-of-Clustered-Federated-Learning-Methods)**|
|**2024-10-18**|**FedMSE: Federated learning for IoT network intrusion detection**|Van Tuan Nguyen et.al.|[2410.14121](http://arxiv.org/abs/2410.14121)|**[link](https://github.com/dino-chiio/fedmse)**|
|**2024-10-18**|**A Communication and Computation Efficient Fully First-order Method for Decentralized Bilevel Optimization**|Min Wen et.al.|[2410.14115](http://arxiv.org/abs/2410.14115)|null|
|**2024-10-17**|**FedPAE: Peer-Adaptive Ensemble Learning for Asynchronous and Model-Heterogeneous Federated Learning**|Brianna Mueller et.al.|[2410.14075](http://arxiv.org/abs/2410.14075)|null|
|**2024-10-17**|**Optimal Communication and Key Rate Region for Hierarchical Secure Aggregation with User Collusion**|Xiang Zhang et.al.|[2410.14035](http://arxiv.org/abs/2410.14035)|null|
|**2024-10-17**|**Conformal Prediction for Federated Graph Neural Networks with Missing Neighbor Information**|Ömer Faruk Akgül et.al.|[2410.14010](http://arxiv.org/abs/2410.14010)|null|
|**2024-10-17**|**DPFedBank: Crafting a Privacy-Preserving Federated Learning Framework for Financial Institutions with Policy Pillars**|Peilin He et.al.|[2410.13753](http://arxiv.org/abs/2410.13753)|null|
|**2024-10-17**|**On-device Federated Learning in Smartphones for Detecting Depression from Reddit Posts**|Mustofa Ahmed et.al.|[2410.13709](http://arxiv.org/abs/2410.13709)|null|
|**2024-10-18**|**Towards Satellite Non-IID Imagery: A Spectral Clustering-Assisted Federated Learning Approach**|Luyao Zou et.al.|[2410.13602](http://arxiv.org/abs/2410.13602)|null|
|**2024-10-17**|**Towards Formal Verification of Federated Learning Orchestration Protocols on Satellites**|Miroslav Popovic et.al.|[2410.13429](http://arxiv.org/abs/2410.13429)|null|
|**2024-10-18**|**Cyber Attacks Prevention Towards Prosumer-based EV Charging Stations: An Edge-assisted Federated Prototype Knowledge Distillation Approach**|Luyao Zou et.al.|[2410.13260](http://arxiv.org/abs/2410.13260)|null|
|**2024-10-17**|**Investigating Effective Speaker Property Privacy Protection in Federated Learning for Speech Emotion Recognition**|Chao Tan et.al.|[2410.13221](http://arxiv.org/abs/2410.13221)|null|
|**2024-10-17**|**Federated scientific machine learning for approximating functions and solving differential equations with data heterogeneity**|Handi Zhang et.al.|[2410.13141](http://arxiv.org/abs/2410.13141)|null|
|**2024-10-16**|**Communication-Efficient and Tensorized Federated Fine-Tuning of Large Language Models**|Sajjad Ghiasvand et.al.|[2410.13097](http://arxiv.org/abs/2410.13097)|null|
|**2024-10-16**|**FedCAP: Robust Federated Learning via Customized Aggregation and Personalization**|Youpeng Li et.al.|[2410.13083](http://arxiv.org/abs/2410.13083)|**[link](https://github.com/youpengl/FedCAP)**|
|**2024-10-16**|**FedGTST: Boosting Global Transferability of Federated Models via Statistics Tuning**|Evelyn Ma et.al.|[2410.13045](http://arxiv.org/abs/2410.13045)|null|
|**2024-10-16**|**Vaccinating Federated Learning for Robust Modulation Classification in Distributed Wireless Networks**|Hunmin Lee et.al.|[2410.12772](http://arxiv.org/abs/2410.12772)|null|
|**2024-10-16**|**Federated Learning and Free-riding in a Competitive Market**|Jiajun Meng et.al.|[2410.12723](http://arxiv.org/abs/2410.12723)|null|
|**2024-10-16**|**Disentangling data distribution for Federated Learning**|Xinyuan Zhao et.al.|[2410.12530](http://arxiv.org/abs/2410.12530)|null|
|**2024-10-16**|**TPFL: A Trustworthy Personalized Federated Learning Framework via Subjective Logic**|Jinqian Chen et.al.|[2410.12316](http://arxiv.org/abs/2410.12316)|null|
|**2024-10-15**|**Age-of-Gradient Updates for Federated Learning over Random Access Channels**|Yu Heng Wu et.al.|[2410.11986](http://arxiv.org/abs/2410.11986)|null|
|**2024-10-15**|**Federated Learning framework for LoRaWAN-enabled IIoT communication: A case study**|Oscar Torres Sanchez et.al.|[2410.11612](http://arxiv.org/abs/2410.11612)|null|
|**2024-10-16**|**Why Go Full? Elevating Federated Learning Through Partial Network Updates**|Haolin Wang et.al.|[2410.11559](http://arxiv.org/abs/2410.11559)|**[link](https://github.com/FLAIR-Community/Fling)**|
|**2024-10-15**|**Data Quality Control in Federated Instruction-tuning of Large Language Models**|Yaxin Du et.al.|[2410.11540](http://arxiv.org/abs/2410.11540)|null|
|**2024-10-15**|**FOOGD: Federated Collaboration for Both Out-of-distribution Generalization and Detection**|Xinting Liao et.al.|[2410.11397](http://arxiv.org/abs/2410.11397)|**[link](https://github.com/xenialll/foogd-main)**|
|**2024-10-15**|**WPFed: Web-based Personalized Federation for Decentralized Systems**|Guanhua Ye et.al.|[2410.11378](http://arxiv.org/abs/2410.11378)|null|
|**2024-10-15**|**Secure Stateful Aggregation: A Practical Protocol with Applications in Differentially-Private Federated Learning**|Marshall Ball et.al.|[2410.11368](http://arxiv.org/abs/2410.11368)|null|
|**2024-10-15**|**Backdoor Attack on Vertical Federated Graph Neural Network Learning**|Jirui Yang et.al.|[2410.11290](http://arxiv.org/abs/2410.11290)|null|
|**2024-10-16**|**FedCCRL: Federated Domain Generalization with Cross-Client Representation Learning**|Xinpeng Wang et.al.|[2410.11267](http://arxiv.org/abs/2410.11267)|**[link](https://github.com/sanphouwang/fedccrl)**|
|**2024-10-15**|**Adversarially Guided Stateful Defense Against Backdoor Attacks in Federated Deep Learning**|Hassan Ali et.al.|[2410.11205](http://arxiv.org/abs/2410.11205)|**[link](https://github.com/hassanalikhatim/agsd)**|
|**2024-10-14**|**A Two-Stage Federated Learning Approach for Industrial Prognostics Using Large-Scale High-Dimensional Signals**|Yuqi Su et.al.|[2410.11101](http://arxiv.org/abs/2410.11101)|null|
|**2024-10-15**|**Mobility-Aware Federated Learning: Multi-Armed Bandit Based Selection in Vehicular Network**|Haoyu Tu et.al.|[2410.10451](http://arxiv.org/abs/2410.10451)|null|
|**2024-10-14**|**Fed-piLot: Optimizing LoRA Assignment for Efficient Federated Foundation Model Fine-Tuning**|Zikai Zhang et.al.|[2410.10200](http://arxiv.org/abs/2410.10200)|null|
|**2024-10-14**|**Mixture of Experts Made Personalized: Federated Prompt Learning for Vision-Language Models**|Jun Luo et.al.|[2410.10114](http://arxiv.org/abs/2410.10114)|null|
|**2024-10-13**|**Improving accuracy and convergence of federated learning edge computing methods for generalized DER forecasting applications in power grid**|Vineet Jagadeesan Nair et.al.|[2410.10018](http://arxiv.org/abs/2410.10018)|null|
|**2024-10-13**|**FedECADO: A Dynamical System Model of Federated Learning**|Aayushya Agarwal et.al.|[2410.09933](http://arxiv.org/abs/2410.09933)|null|
|**2024-10-13**|**Uncovering Attacks and Defenses in Secure Aggregation for Federated Deep Learning**|Yiwei Zhang et.al.|[2410.09676](http://arxiv.org/abs/2410.09676)|null|
|**2024-10-12**|**Exact Aggregation for Federated and Efficient Fine-Tuning of Foundation Models**|Raghav Singhal et.al.|[2410.09432](http://arxiv.org/abs/2410.09432)|null|
|**2024-10-11**|**Enhanced Federated Anomaly Detection Through Autoencoders Using Summary Statistics-Based Thresholding**|Sofiane Laridi et.al.|[2410.09284](http://arxiv.org/abs/2410.09284)|null|
|**2024-10-11**|**Evaluating Federated Kolmogorov-Arnold Networks on Non-IID Data**|Arthur Mendonça Sasse et.al.|[2410.08961](http://arxiv.org/abs/2410.08961)|**[link](https://github.com/artsasse/fedkan)**|
|**2024-10-11**|**The Effect of Personalization in FedProx: A Fine-grained Analysis on Statistical Accuracy and Communication Efficiency**|Xin Yu et.al.|[2410.08934](http://arxiv.org/abs/2410.08934)|null|
|**2024-10-11**|**Federated Learning in Practice: Reflections and Projections**|Katharine Daly et.al.|[2410.08892](http://arxiv.org/abs/2410.08892)|null|
|**2024-10-11**|**Unlocking FedNL: Self-Contained Compute-Optimized Implementation**|Konstantin Burlachenko et.al.|[2410.08760](http://arxiv.org/abs/2410.08760)|null|
|**2024-10-11**|**Gradients Stand-in for Defending Deep Leakage in Federated Learning**|H. Yi et.al.|[2410.08734](http://arxiv.org/abs/2410.08734)|**[link](https://github.com/Rand2AI/AdaDefense)**|
|**2024-10-11**|**DistDD: Distributed Data Distillation Aggregation through Gradient Matching**|Peiran Wang et.al.|[2410.08665](http://arxiv.org/abs/2410.08665)|null|
|**2024-10-11**|**GAI-Enabled Explainable Personalized Federated Semi-Supervised Learning**|Yubo Peng et.al.|[2410.08634](http://arxiv.org/abs/2410.08634)|null|
|**2024-10-11**|**Accelerated Distributed Stochastic Non-Convex Optimization over Time-Varying Directed Networks**|Yiyue Chen et.al.|[2410.08508](http://arxiv.org/abs/2410.08508)|null|
|**2024-10-10**|**Randomized Asymmetric Chain of LoRA: The First Meaningful Theoretical Framework for Low-Rank Adaptation**|Grigory Malinovsky et.al.|[2410.08305](http://arxiv.org/abs/2410.08305)|null|
|**2024-10-10**|**A Comprehensive Survey on Joint Resource Allocation Strategies in Federated Edge Learning**|Jingbo Zhang et.al.|[2410.07881](http://arxiv.org/abs/2410.07881)|null|
|**2024-10-10**|**Enhancing Federated Domain Adaptation with Multi-Domain Prototype-Based Federated Fine-Tuning**|Jingyuan Zhang et.al.|[2410.07738](http://arxiv.org/abs/2410.07738)|null|
|**2024-10-10**|**FedEP: Tailoring Attention to Heterogeneous Data Distribution with Entropy Pooling for Decentralized Federated Learning**|Chao Feng et.al.|[2410.07678](http://arxiv.org/abs/2410.07678)|null|
|**2024-10-10**|**Scalable and Resource-Efficient Second-Order Federated Learning via Over-the-Air Aggregation**|Abdulmomen Ghalkha et.al.|[2410.07662](http://arxiv.org/abs/2410.07662)|null|
|**2024-10-09**|**Benchmarking Data Heterogeneity Evaluation Approaches for Personalized Federated Learning**|Zhilong Li et.al.|[2410.07286](http://arxiv.org/abs/2410.07286)|**[link](https://github.com/xiaoni-61/dh-benchmark)**|
|**2024-10-09**|**Boosting the Performance of Decentralized Federated Learning via Catalyst Acceleration**|Qinglun Li et.al.|[2410.07272](http://arxiv.org/abs/2410.07272)|null|
|**2024-10-09**|**Distributionally Robust Clustered Federated Learning: A Case Study in Healthcare**|Xenia Konti et.al.|[2410.07039](http://arxiv.org/abs/2410.07039)|null|
|**2024-10-09**|**Forgetting Through Transforming: Enabling Federated Unlearning via Class-Aware Representation Transformation**|Qi Guo et.al.|[2410.06848](http://arxiv.org/abs/2410.06848)|null|
|**2024-10-09**|**PFAttack: Stealthy Attack Bypassing Group Fairness in Federated Learning**|Jiashi Gao et.al.|[2410.06509](http://arxiv.org/abs/2410.06509)|null|
|**2024-10-09**|**FedL2G: Learning to Guide Local Training in Heterogeneous Federated Learning**|Jianqing Zhang et.al.|[2410.06490](http://arxiv.org/abs/2410.06490)|**[link](https://github.com/TsingZ0/FedL2G)**|
|**2024-10-09**|**OledFL: Unleashing the Potential of Decentralized Federated Learning via Opposite Lookahead Enhancement**|Qinglun Li et.al.|[2410.06482](http://arxiv.org/abs/2410.06482)|null|
|**2024-10-08**|**Communication-Efficient Federated Group Distributionally Robust Optimization**|Zhishuai Guo et.al.|[2410.06369](http://arxiv.org/abs/2410.06369)|null|
|**2024-10-08**|**De-VertiFL: A Solution for Decentralized Vertical Federated Learning**|Alberto Huertas Celdrán et.al.|[2410.06127](http://arxiv.org/abs/2410.06127)|null|
|**2024-10-08**|**Privacy-Enhanced Over-the-Air Federated Learning via Client-Driven Power Balancing**|Bumjun Kim et.al.|[2410.05907](http://arxiv.org/abs/2410.05907)|null|
|**2024-10-10**|**Private and Communication-Efficient Federated Learning based on Differentially Private Sketches**|Meifan Zhang et.al.|[2410.05733](http://arxiv.org/abs/2410.05733)|null|
|**2024-10-10**|**KnowledgeSG: Privacy-Preserving Synthetic Text Generation with Knowledge Distillation from Server**|Wenhao Wang et.al.|[2410.05725](http://arxiv.org/abs/2410.05725)|**[link](https://github.com/wwh0411/knowledgesg)**|
|**2024-10-07**|**FRIDA: Free-Rider Detection using Privacy Attacks**|Pol G. Recasens et.al.|[2410.05020](http://arxiv.org/abs/2410.05020)|null|
|**2024-10-07**|**FedBiP: Heterogeneous One-Shot Federated Learning with Personalized Latent Diffusion Models**|Haokun Chen et.al.|[2410.04810](http://arxiv.org/abs/2410.04810)|null|
|**2024-10-07**|**Federated Learning Nodes Can Reconstruct Peers' Image Data**|Ethan Wilson et.al.|[2410.04661](http://arxiv.org/abs/2410.04661)|null|
|**2024-10-05**|**ConDa: Fast Federated Unlearning with Contribution Dampening**|Vikram S Chundawat et.al.|[2410.04144](http://arxiv.org/abs/2410.04144)|null|
|**2024-10-05**|**pFedGame -- Decentralized Federated Learning using Game Theory in Dynamic Topology**|Monik Raj Behera et.al.|[2410.04058](http://arxiv.org/abs/2410.04058)|null|
|**2024-10-04**|**A Survey on Group Fairness in Federated Learning: Challenges, Taxonomy of Solutions and Directions for Future Research**|Teresa Salazar et.al.|[2410.03855](http://arxiv.org/abs/2410.03855)|**[link](https://github.com/teresalazar13/Survey-Group-Fairness-in-Federated-Learning)**|
|**2024-10-04**|**FedStein: Enhancing Multi-Domain Federated Learning Through James-Stein Estimator**|Sunny Gupta et.al.|[2410.03499](http://arxiv.org/abs/2410.03499)|null|
|**2024-10-04**|**Collaborative and Efficient Personalization with Mixtures of Adaptors**|Abdulla Jasem Almansoori et.al.|[2410.03497](http://arxiv.org/abs/2410.03497)|null|
|**2024-10-04**|**Camel: Communication-Efficient and Maliciously Secure Federated Learning in the Shuffle Model of Differential Privacy**|Shuangqing Xu et.al.|[2410.03407](http://arxiv.org/abs/2410.03407)|**[link](https://github.com/Shuangqing-Xu/Camel)**|
|**2024-10-04**|**Influence-oriented Personalized Federated Learning**|Yue Tan et.al.|[2410.03315](http://arxiv.org/abs/2410.03315)|null|
|**2024-10-04**|**BN-SCAFFOLD: controlling the drift of Batch Normalization statistics in Federated Learning**|Gonzalo Iñaki Quintana et.al.|[2410.03281](http://arxiv.org/abs/2410.03281)|null|
|**2024-10-04**|**FedMAC: Tackling Partial-Modality Missing in Federated Learning with Cross-Modal Aggregation and Contrastive Regularization**|Manh Duong Nguyen et.al.|[2410.03070](http://arxiv.org/abs/2410.03070)|null|
|**2024-10-04**|**FedCert: Federated Accuracy Certification**|Minh Hieu Nguyen et.al.|[2410.03067](http://arxiv.org/abs/2410.03067)|**[link](https://github.com/thanhhff/FedCert)**|
|**2024-10-03**|**FedPeWS: Personalized Warmup via Subnetworks for Enhanced Heterogeneous Federated Learning**|Nurbek Tastan et.al.|[2410.03042](http://arxiv.org/abs/2410.03042)|null|
|**2024-10-03**|**Data Similarity-Based One-Shot Clustering for Multi-Task Hierarchical Federated Learning**|Abdulmoneam Ali et.al.|[2410.02733](http://arxiv.org/abs/2410.02733)|null|
|**2024-10-03**|**Personalized Quantum Federated Learning for Privacy Image Classification**|Jinjing Shi et.al.|[2410.02547](http://arxiv.org/abs/2410.02547)|null|
|**2024-10-03**|**Personalized Federated Learning for Generative AI-Assisted Semantic Communications**|Yubo Peng et.al.|[2410.02450](http://arxiv.org/abs/2410.02450)|null|
|**2024-10-03**|**Clinnova Federated Learning Proof of Concept: Key Takeaways from a Cross-border Collaboration**|Julia Alekseenko et.al.|[2410.02443](http://arxiv.org/abs/2410.02443)|null|
|**2024-10-03**|**Federated Reinforcement Learning to Optimize Teleoperated Driving Networks**|Filippo Bragato et.al.|[2410.02312](http://arxiv.org/abs/2410.02312)|null|
|**2024-10-03**|**FedScalar: A Communication efficient Federated Learning**|M. Rostami et.al.|[2410.02260](http://arxiv.org/abs/2410.02260)|null|
|**2024-10-03**|**A Survey on Point-of-Interest Recommendation: Models, Architectures, and Security**|Qianru Zhang et.al.|[2410.02191](http://arxiv.org/abs/2410.02191)|null|
|**2024-10-02**|**Frequency-Based Federated Domain Generalization for Polyp Segmentation**|Hongyi Pan et.al.|[2410.02044](http://arxiv.org/abs/2410.02044)|null|
|**2024-10-02**|**EAB-FL: Exacerbating Algorithmic Bias through Model Poisoning Attacks in Federated Learning**|Syed Irfan Ali Meerza et.al.|[2410.02042](http://arxiv.org/abs/2410.02042)|**[link](https://github.com/irfanmee/eab-fl)**|
|**2024-10-02**|**Addressing Data Heterogeneity in Federated Learning with Adaptive Normalization-Free Feature Recalibration**|Vasilis Siomos et.al.|[2410.02006](http://arxiv.org/abs/2410.02006)|null|
|**2024-10-02**|**A Novel Framework of Horizontal-Vertical Hybrid Federated Learning for EdgeIoT**|Kai Li et.al.|[2410.01644](http://arxiv.org/abs/2410.01644)|null|
|**2024-10-02**|**Personalized Federated Learning on Flowing Data Heterogeneity under Restricted Storage**|Sixing Tan et.al.|[2410.01502](http://arxiv.org/abs/2410.01502)|null|
|**2024-10-02**|**Selective Aggregation for Low-Rank Adaptation in Federated Learning**|Pengxin Guo et.al.|[2410.01463](http://arxiv.org/abs/2410.01463)|**[link](https://github.com/Pengxin-Guo/FedSA-LoRA)**|
|**2024-10-02**|**On the Convergence of FedProx with Extrapolation and Inexact Prox**|Hanmin Li et.al.|[2410.01410](http://arxiv.org/abs/2410.01410)|null|
|**2024-10-02**|**Overpredictive Signal Analytics in Federated Learning: Algorithms and Analysis**|Vijay Anavangot et.al.|[2410.01399](http://arxiv.org/abs/2410.01399)|null|
|**2024-10-02**|**FLAME: Adaptive and Reactive Concept Drift Mitigation for Federated Learning Deployments**|Ioannis Mavromatis et.al.|[2410.01386](http://arxiv.org/abs/2410.01386)|null|
|**2024-10-02**|**ParallelSFL: A Novel Split Federated Learning Framework Tackling Heterogeneity Issues**|Yunming Liao et.al.|[2410.01256](http://arxiv.org/abs/2410.01256)|null|
|**2024-10-02**|**Debiasing Federated Learning with Correlated Client Participation**|Zhenyu Sun et.al.|[2410.01209](http://arxiv.org/abs/2410.01209)|null|
|**2024-10-01**|**FedPT: Federated Proxy-Tuning of Large Language Models on Resource-Constrained Edge Devices**|Zhidong Gao et.al.|[2410.00362](http://arxiv.org/abs/2410.00362)|null|
|**2024-09-30**|**Quantized and Asynchronous Federated Learning**|Tomas Ortega et.al.|[2410.00242](http://arxiv.org/abs/2410.00242)|null|
|**2024-09-30**|**Fine-Tuning Personalization in Federated Learning to Mitigate Adversarial Clients**|Youssef Allouah et.al.|[2409.20329](http://arxiv.org/abs/2409.20329)|null|
|**2024-09-30**|**Enhancing Security Using Random Binary Weights in Privacy-Preserving Federated Learning**|Hiroto Sawada et.al.|[2409.19988](http://arxiv.org/abs/2409.19988)|null|
|**2024-09-30**|**Comments on "Privacy-Enhanced Federated Learning Against Poisoning Adversaries"**|Thomas Schneider et.al.|[2409.19964](http://arxiv.org/abs/2409.19964)|null|
|**2024-09-30**|**Leveraging Pre-trained Models for Robust Federated Learning for Kidney Stone Type Recognition**|Ivan Reyes-Amezcua et.al.|[2409.19934](http://arxiv.org/abs/2409.19934)|null|
|**2024-10-01**|**HYDRA-FL: Hybrid Knowledge Distillation for Robust and Accurate Federated Learning**|Momin Ahmad Khan et.al.|[2409.19912](http://arxiv.org/abs/2409.19912)|null|
|**2024-09-29**|**Advances in Privacy Preserving Federated Learning to Realize a Truly Learning Healthcare System**|Ravi Madduri et.al.|[2409.19756](http://arxiv.org/abs/2409.19756)|null|
|**2024-09-29**|**Tailored Federated Learning: Leveraging Direction Regulation & Knowledge Distillation**|Huidong Tang et.al.|[2409.19741](http://arxiv.org/abs/2409.19741)|null|
|**2024-09-29**|**Federated Learning from Vision-Language Foundation Models: Theoretical Analysis and Method**|Bikang Pan et.al.|[2409.19610](http://arxiv.org/abs/2409.19610)|**[link](https://github.com/PanBikang/PromptFolio)**|
|**2024-09-29**|**Infighting in the Dark: Multi-Labels Backdoor Attack in Federated Learning**|Ye Li et.al.|[2409.19601](http://arxiv.org/abs/2409.19601)|null|
|**2024-09-29**|**Fast-Convergent and Communication-Alleviated Heterogeneous Hierarchical Federated Learning in Autonomous Driving**|Wei-Bin Kou et.al.|[2409.19560](http://arxiv.org/abs/2409.19560)|null|
|**2024-09-27**|**A-FedPD: Aligning Dual-Drift is All Federated Primal-Dual Learning Needs**|Yan Sun et.al.|[2409.18915](http://arxiv.org/abs/2409.18915)|null|
|**2024-09-27**|**In-depth Analysis of Privacy Threats in Federated Learning for Medical Data**|Badhan Chandra Das et.al.|[2409.18907](http://arxiv.org/abs/2409.18907)|null|
|**2024-09-27**|**Hierarchical Federated ADMM**|Seyed Mohammad Azimi-Abarghouyi et.al.|[2409.18796](http://arxiv.org/abs/2409.18796)|null|
|**2024-09-27**|**Enhancing Spectrum Efficiency in 6G Satellite Networks: A GAIL-Powered Policy Learning via Asynchronous Federated Inverse Reinforcement Learning**|Sheikh Salman Hassan et.al.|[2409.18718](http://arxiv.org/abs/2409.18718)|null|
|**2024-09-27**|**An Enhanced Federated Prototype Learning Method under Domain Shift**|Liang Kuang et.al.|[2409.18578](http://arxiv.org/abs/2409.18578)|null|
|**2024-09-27**|**HSTFL: A Heterogeneous Federated Learning Framework for Misaligned Spatiotemporal Forecasting**|Shuowei Cai et.al.|[2409.18482](http://arxiv.org/abs/2409.18482)|null|
|**2024-09-27**|**Towards Diverse Device Heterogeneous Federated Learning via Task Arithmetic Knowledge Integration**|Mahdi Morafah et.al.|[2409.18461](http://arxiv.org/abs/2409.18461)|**[link](https://github.com/mmorafah/takfl)**|
|**2024-09-27**|**Hierarchical Federated Learning with Multi-Timescale Gradient Correction**|Wenzhi Fang et.al.|[2409.18448](http://arxiv.org/abs/2409.18448)|**[link](https://github.com/wenzhifang/mtgc)**|
|**2024-09-27**|**FedDCL: a federated data collaboration learning as a hybrid-type privacy-preserving framework based on federated learning and data collaboration**|Akira Imakura et.al.|[2409.18356](http://arxiv.org/abs/2409.18356)|null|
|**2024-09-26**|**PDFed: Privacy-Preserving and Decentralized Asynchronous Federated Learning for Diffusion Models**|Kar Balan et.al.|[2409.18245](http://arxiv.org/abs/2409.18245)|null|
|**2024-09-26**|**Federated Learning under Attack: Improving Gradient Inversion for Batch of Images**|Luiz Leite et.al.|[2409.17767](http://arxiv.org/abs/2409.17767)|null|
|**2024-09-26**|**Byzantine-Robust Aggregation for Securing Decentralized Federated Learning**|Diego Cajaraville-Aboy et.al.|[2409.17754](http://arxiv.org/abs/2409.17754)|**[link](https://github.com/diegoiclab/decentralizedfedsim)**|
|**2024-09-26**|**Dataset Distillation-based Hybrid Federated Learning on Non-IID Data**|Xiufang Shi et.al.|[2409.17517](http://arxiv.org/abs/2409.17517)|null|
|**2024-09-26**|**Does Worst-Performing Agent Lead the Pack? Analyzing Agent Dynamics in Unified Distributed SGD**|Jie Hu et.al.|[2409.17499](http://arxiv.org/abs/2409.17499)|null|
|**2024-09-26**|**Efficient Federated Learning against Heterogeneous and Non-stationary Client Unavailability**|Ming Xiang et.al.|[2409.17446](http://arxiv.org/abs/2409.17446)|null|
|**2024-09-25**|**A Hierarchical Gradient Tracking Algorithm for Mitigating Subnet-Drift in Fog Learning Networks**|Evan Chen et.al.|[2409.17430](http://arxiv.org/abs/2409.17430)|null|
|**2024-09-25**|**Immersion and Invariance-based Coding for Privacy-Preserving Federated Learning**|Haleh Hayati et.al.|[2409.17201](http://arxiv.org/abs/2409.17201)|null|
|**2024-09-25**|**Decentralized Federated Learning with Gradient Tracking over Time-Varying Directed Networks**|Duong Thuy Anh Nguyen et.al.|[2409.17189](http://arxiv.org/abs/2409.17189)|null|
|**2024-09-24**|**Flight: A FaaS-Based Framework for Complex and Hierarchical Federated Learning**|Nathaniel Hudson et.al.|[2409.16495](http://arxiv.org/abs/2409.16495)|null|
|**2024-09-24**|**Communication and Energy Efficient Federated Learning using Zero-Order Optimization Technique**|Elissa Mhanna et.al.|[2409.16456](http://arxiv.org/abs/2409.16456)|null|
|**2024-09-18**|**FedLF: Adaptive Logit Adjustment and Feature Optimization in Federated Long-Tailed Learning**|Xiuhua Lu et.al.|[2409.12105](http://arxiv.org/abs/2409.12105)|**[link](https://github.com/18sym/fedlf)**|
|**2024-09-18**|**Promise and Peril of Collaborative Code Generation Models: Balancing Effectiveness and Memorization**|Zhi Chen et.al.|[2409.12020](http://arxiv.org/abs/2409.12020)|null|
|**2024-09-17**|**Advances in APPFL: A Comprehensive and Extensible Federated Learning Framework**|Zilinghan Li et.al.|[2409.11585](http://arxiv.org/abs/2409.11585)|**[link](https://github.com/appfl/appfl)**|
|**2024-09-17**|**FedNE: Surrogate-Assisted Federated Neighbor Embedding for Dimensionality Reduction**|Ziwei Li et.al.|[2409.11509](http://arxiv.org/abs/2409.11509)|null|
|**2024-09-16**|**A Green Multi-Attribute Client Selection for Over-The-Air Federated Learning: A Grey-Wolf-Optimizer Approach**|Maryam Ben Driss et.al.|[2409.11442](http://arxiv.org/abs/2409.11442)|null|
|**2024-09-17**|**Federated Learning with Integrated Sensing, Communication, and Computation: Frameworks and Performance Analysis**|Yipeng Liang et.al.|[2409.11240](http://arxiv.org/abs/2409.11240)|null|
|**2024-09-16**|**Federated Learning for Smart Grid: A Survey on Applications and Potential Vulnerabilities**|Zikai Zhang et.al.|[2409.10764](http://arxiv.org/abs/2409.10764)|null|
|**2024-09-24**|**TPFL: Tsetlin-Personalized Federated Learning with Confidence-Based Clustering**|Rasoul Jafari Gohari et.al.|[2409.10392](http://arxiv.org/abs/2409.10392)|**[link](https://github.com/russelljeffrey/TPFL)**|
|**2024-09-15**|**Federated Learning in Adversarial Environments: Testbed Design and Poisoning Resilience in Cybersecurity**|Hao Jian Huang et.al.|[2409.09794](http://arxiv.org/abs/2409.09794)|null|
|**2024-09-15**|**From Challenges and Pitfalls to Recommendations and Opportunities: Implementing Federated Learning in Healthcare**|Ming Li et.al.|[2409.09727](http://arxiv.org/abs/2409.09727)|null|
|**2024-09-14**|**Using Synthetic Data to Mitigate Unfairness and Preserve Privacy through Single-Shot Federated Learning**|Chia-Yuan Wu et.al.|[2409.09532](http://arxiv.org/abs/2409.09532)|null|
|**2024-09-14**|**Leveraging Foundation Models for Efficient Federated Learning in Resource-restricted Edge Networks**|S. Kawa Atapour et.al.|[2409.09273](http://arxiv.org/abs/2409.09273)|null|
|**2024-09-13**|**Exploring System-Heterogeneous Federated Learning with Dynamic Model Selection**|Dixi Yao et.al.|[2409.08858](http://arxiv.org/abs/2409.08858)|null|
|**2024-09-13**|**Enhancing Privacy in ControlNet and Stable Diffusion via Split Learning**|Dixi Yao et.al.|[2409.08503](http://arxiv.org/abs/2409.08503)|null|
|**2024-09-13**|**Research on Data Right Confirmation Mechanism of Federated Learning based on Blockchain**|Xiaogang Cheng et.al.|[2409.08476](http://arxiv.org/abs/2409.08476)|null|
|**2024-09-12**|**FedProphet: Memory-Efficient Federated Adversarial Training via Theoretic-Robustness and Low-Inconsistency Cascade Learning**|Minxue Tang et.al.|[2409.08372](http://arxiv.org/abs/2409.08372)|null|
|**2024-09-12**|**Multi-Model based Federated Learning Against Model Poisoning Attack: A Deep Learning Based Model Selection for MEC Systems**|Somayeh Kianpisheh et.al.|[2409.08237](http://arxiv.org/abs/2409.08237)|null|
|**2024-09-12**|**Privacy-preserving federated prediction of pain intensity change based on multi-center survey data**|Supratim Das et.al.|[2409.07997](http://arxiv.org/abs/2409.07997)|null|
|**2024-09-12**|**Over-the-Air Federated Learning via Weighted Aggregation**|Seyed Mohammad Azimi-Abarghouyi et.al.|[2409.07822](http://arxiv.org/abs/2409.07822)|null|
|**2024-09-12**|**FedHide: Federated Learning by Hiding in the Neighbors**|Hyunsin Park et.al.|[2409.07808](http://arxiv.org/abs/2409.07808)|null|
|**2024-09-12**|**DFDG: Data-Free Dual-Generator Adversarial Distillation for One-Shot Federated Learning**|Kangyang Luo et.al.|[2409.07734](http://arxiv.org/abs/2409.07734)|null|
|**2024-09-11**|**HERL: Tiered Federated Learning with Adaptive Homomorphic Encryption using Reinforcement Learning**|Jiaxang Tang et.al.|[2409.07631](http://arxiv.org/abs/2409.07631)|null|
|**2024-09-11**|**Federated Impression for Learning with Distributed Heterogeneous Data**|Sana Ayromlou et.al.|[2409.07351](http://arxiv.org/abs/2409.07351)|**[link](https://github.com/atrin78/fedimpress)**|
|**2024-09-11**|**Exploring User-level Gradient Inversion with a Diffusion Prior**|Zhuohang Li et.al.|[2409.07291](http://arxiv.org/abs/2409.07291)|null|
|**2024-09-11**|**Federated $\mathcal{X}$ -armed Bandit with Flexible Personalisation**|Ali Arabzadeh et.al.|[2409.07251](http://arxiv.org/abs/2409.07251)|null|
|**2024-09-11**|**Riemannian Federated Learning via Averaging Gradient Stream**|Zhenwei Huang et.al.|[2409.07223](http://arxiv.org/abs/2409.07223)|null|
|**2024-09-11**|**Heterogeneity-Aware Coordination for Federated Learning via Stitching Pre-trained blocks**|Shichen Zhan et.al.|[2409.07202](http://arxiv.org/abs/2409.07202)|null|
|**2024-09-11**|**Privacy-Preserving Federated Learning with Consistency via Knowledge Distillation Using Conditional Generator**|Kangyang Luo et.al.|[2409.06955](http://arxiv.org/abs/2409.06955)|null|
|**2024-09-10**|**Applied Federated Model Personalisation in the Industrial Domain: A Comparative Study**|Ilias Siniosoglou et.al.|[2409.06904](http://arxiv.org/abs/2409.06904)|null|
|**2024-09-10**|**Personalized Federated Learning Techniques: Empirical Analysis**|Azal Ahmad Khan et.al.|[2409.06805](http://arxiv.org/abs/2409.06805)|null|
|**2024-09-10**|**Advancing Hybrid Defense for Byzantine Attacks in Federated Learning**|Kai Yue et.al.|[2409.06474](http://arxiv.org/abs/2409.06474)|null|
|**2024-09-10**|**Compute-Update Federated Learning: A Lattice Coding Approach**|Seyed Mohammad Azimi-Abarghouyi et.al.|[2409.06343](http://arxiv.org/abs/2409.06343)|null|
|**2024-09-10**|**Rate-Constrained Quantization for Communication-Efficient Federated Learning**|Shayan Mohajer Hamidi et.al.|[2409.06319](http://arxiv.org/abs/2409.06319)|null|
|**2024-09-10**|**Contrastive Federated Learning with Tabular Data Silos**|Achmad Ginanjar et.al.|[2409.06123](http://arxiv.org/abs/2409.06123)|null|
|**2024-09-09**|**MLLM-FL: Multimodal Large Language Model Assisted Federated Learning on Heterogeneous and Long-tailed Data**|Jianyi Zhang et.al.|[2409.06067](http://arxiv.org/abs/2409.06067)|null|
|**2024-09-09**|**FLoRA: Federated Fine-Tuning Large Language Models with Heterogeneous Low-Rank Adaptations**|Ziyao Wang et.al.|[2409.05976](http://arxiv.org/abs/2409.05976)|**[link](https://github.com/atp-1010/federatedllm)**|
|**2024-09-09**|**pFedGPA: Diffusion-based Generative Parameter Aggregation for Personalized Federated Learning**|Jiahao Lai et.al.|[2409.05701](http://arxiv.org/abs/2409.05701)|null|
|**2024-09-09**|**FedBrain-Distill: Communication-Efficient Federated Brain Tumor Classification Using Ensemble Knowledge Distillation on Non-IID Data**|Rasoul Jafari Gohari et.al.|[2409.05359](http://arxiv.org/abs/2409.05359)|**[link](https://github.com/russelljeffrey/FedBrain-Distill)**|
|**2024-09-09**|**TriplePlay: Enhancing Federated Learning with CLIP for Non-IID Data and Resource Efficiency**|Ahmed Imteaj et.al.|[2409.05347](http://arxiv.org/abs/2409.05347)|null|
|**2024-09-09**|**Towards Practical Overlay Networks for Decentralized Federated Learning**|Yifan Hua et.al.|[2409.05331](http://arxiv.org/abs/2409.05331)|null|
|**2024-09-08**|**FedFT: Improving Communication Performance for Federated Learning with Frequency Space Transformation**|Chamath Palihawadana et.al.|[2409.05242](http://arxiv.org/abs/2409.05242)|**[link](https://github.com/chamathpali/fedft)**|
|**2024-09-08**|**Some Results on Neural Network Stability, Consistency, and Convergence: Insights into Non-IID Data, High-Dimensional Settings, and Physics-Informed Neural Networks**|Ronald Katende et.al.|[2409.05030](http://arxiv.org/abs/2409.05030)|null|
|**2024-09-08**|**DynamicFL: Federated Learning with Dynamic Communication Resource Allocation**|Qi Le et.al.|[2409.04986](http://arxiv.org/abs/2409.04986)|null|
|**2024-09-08**|**Balancing Security and Accuracy: A Novel Federated Learning Approach for Cyberattack Detection in Blockchain Networks**|Tran Viet Khoa et.al.|[2409.04972](http://arxiv.org/abs/2409.04972)|null|
|**2024-09-07**|**Fair Allocation of Bandwidth At Edge Servers For Concurrent Hierarchical Federated Learning**|Md Anwar Hossen et.al.|[2409.04921](http://arxiv.org/abs/2409.04921)|null|
|**2024-09-07**|**Unlocking the Potential of Model Calibration in Federated Learning**|Yun-Wei Chu et.al.|[2409.04901](http://arxiv.org/abs/2409.04901)|null|
|**2024-09-06**|**Active-Passive Federated Learning for Vertically Partitioned Multi-view Data**|Jiyuan Liu et.al.|[2409.04111](http://arxiv.org/abs/2409.04111)|null|
|**2024-09-06**|**Heterogeneity-Aware Cooperative Federated Edge Learning with Adaptive Computation and Communication Compression**|Zhenxiao Zhang et.al.|[2409.04022](http://arxiv.org/abs/2409.04022)|null|
|**2024-09-05**|**Can We Theoretically Quantify the Impacts of Local Updates on the Generalization Performance of Federated Learning?**|Peizhong Ju et.al.|[2409.03863](http://arxiv.org/abs/2409.03863)|null|
|**2024-09-05**|**Wind turbine condition monitoring based on intra- and inter-farm federated learning**|Albin Grataloup et.al.|[2409.03672](http://arxiv.org/abs/2409.03672)|**[link](https://github.com/EnergyWeatherAI/FL-Wind-NBM)**|
|**2024-09-05**|**VFLGAN-TS: Vertical Federated Learning-based Generative Adversarial Networks for Publication of Vertically Partitioned Time-Series Data**|Xun Yuan et.al.|[2409.03612](http://arxiv.org/abs/2409.03612)|**[link](https://github.com/YuanXun2024/VFLGAN-TS)**|
|**2024-09-05**|**Federated Prototype-based Contrastive Learning for Privacy-Preserving Cross-domain Recommendation**|Li Wang et.al.|[2409.03294](http://arxiv.org/abs/2409.03294)|null|
|**2024-09-04**|**Resilient Two-Time-Scale Local Stochastic Gradient Descent for Byzantine Federated Learning**|Amit Dutta et.al.|[2409.03092](http://arxiv.org/abs/2409.03092)|null|
|**2024-09-04**|**Federated Quantum-Train with Batched Parameter Generation**|Chen-Yu Liu et.al.|[2409.02763](http://arxiv.org/abs/2409.02763)|null|
|**2024-09-04**|**A Joint Time and Energy-Efficient Federated Learning-based Computation Offloading Method for Mobile Edge Computing**|Anwesha Mukherjee et.al.|[2409.02548](http://arxiv.org/abs/2409.02548)|null|
|**2024-09-04**|**CoAst: Validation-Free Contribution Assessment for Federated Learning based on Cross-Round Valuation**|Hao Wu et.al.|[2409.02495](http://arxiv.org/abs/2409.02495)|null|
|**2024-09-04**|**Robust Federated Finetuning of Foundation Models via Alternating Minimization of LoRA**|Shuangyi Chen et.al.|[2409.02346](http://arxiv.org/abs/2409.02346)|null|
|**2024-09-03**|**Collaboratively Learning Federated Models from Noisy Decentralized Data**|Haoyuan Li et.al.|[2409.02189](http://arxiv.org/abs/2409.02189)|null|
|**2024-09-03**|**Personalized Federated Learning via Active Sampling**|Alexander Jung et.al.|[2409.02064](http://arxiv.org/abs/2409.02064)|null|
|**2024-09-03**|**FedMinds: Privacy-Preserving Personalized Brain Visual Decoding**|Guangyin Bao et.al.|[2409.02044](http://arxiv.org/abs/2409.02044)|null|
|**2024-09-03**|**Securing Federated Learning in Robot Swarms using Blockchain Technology**|Alexandre Pacheco et.al.|[2409.01900](http://arxiv.org/abs/2409.01900)|null|
|**2024-09-03**|**Federated Prediction-Powered Inference from Decentralized Data**|Ping Luo et.al.|[2409.01730](http://arxiv.org/abs/2409.01730)|null|
|**2024-09-05**|**ACCESS-FL: Agile Communication and Computation for Efficient Secure Aggregation in Stable Federated Learning Networks**|Niousha Nazemi et.al.|[2409.01722](http://arxiv.org/abs/2409.01722)|**[link](https://github.com/SeeAccessFL/ACCESS-FL)**|
|**2024-08-30**|**Democratizing AI in Africa: FL for Low-Resource Edge Devices**|Jorge Fabila et.al.|[2408.17216](http://arxiv.org/abs/2408.17216)|null|
|**2024-08-30**|**Towards Hyper-parameter-free Federated Learning**|Geetika et.al.|[2408.17145](http://arxiv.org/abs/2408.17145)|**[link](https://github.com/zk23du/fedli)**|
|**2024-08-30**|**FissionVAE: Federated Non-IID Image Generation with Latent Space and Decoder Decomposition**|Chen Hu et.al.|[2408.17090](http://arxiv.org/abs/2408.17090)|**[link](https://github.com/rand2ai/fissionvae)**|
|**2024-08-28**|**ModalityMirror: Improving Audio Classification in Modality Heterogeneity Federated Learning with Multimodal Distillation**|Tiantian Feng et.al.|[2408.15803](http://arxiv.org/abs/2408.15803)|null|
|**2024-08-28**|**Convergent Differential Privacy Analysis for General Federated Learning: the f-DP Perspective**|Yan Sun et.al.|[2408.15621](http://arxiv.org/abs/2408.15621)|null|
|**2024-08-28**|**Exploring Selective Layer Fine-Tuning in Federated Learning**|Yuchang Sun et.al.|[2408.15600](http://arxiv.org/abs/2408.15600)|null|
|**2024-08-29**|**VFLIP: A Backdoor Defense for Vertical Federated Learning via Identification and Purification**|Yungi Cho et.al.|[2408.15591](http://arxiv.org/abs/2408.15591)|**[link](https://github.com/blingcho/vflip-esorics24)**|
|**2024-08-27**|**Bandwidth-Aware and Overlap-Weighted Compression for Communication-Efficient Federated Learning**|Zichen Tang et.al.|[2408.14736](http://arxiv.org/abs/2408.14736)|null|
|**2024-08-27**|**PPVF: An Efficient Privacy-Preserving Online Video Fetching Framework with Correlated Differential Privacy**|Xianzhi Zhang et.al.|[2408.14735](http://arxiv.org/abs/2408.14735)|null|
|**2024-08-26**|**Federated User Preference Modeling for Privacy-Preserving Cross-Domain Recommendation**|Li Wang et.al.|[2408.14689](http://arxiv.org/abs/2408.14689)|**[link](https://github.com/lili1013/fupm)**|
|**2024-08-26**|**Hyperdimensional Computing Empowered Federated Foundation Model over Wireless Networks for Metaverse**|Yahao Ding et.al.|[2408.14416](http://arxiv.org/abs/2408.14416)|null|
|**2024-08-26**|**Resource Efficient Asynchronous Federated Learning for Digital Twin Empowered IoT Network**|Shunfeng Chu et.al.|[2408.14298](http://arxiv.org/abs/2408.14298)|null|
|**2024-08-26**|**Celtibero: Robust Layered Aggregation for Federated Learning**|Borja Molina-Coronado et.al.|[2408.14240](http://arxiv.org/abs/2408.14240)|null|
|**2024-08-26**|**Neighborhood and Global Perturbations Supported SAM in Federated Learning: From Local Tweaks To Global Awareness**|Boyuan Li et.al.|[2408.14144](http://arxiv.org/abs/2408.14144)|null|
|**2024-08-26**|**Decentralized Federated Learning with Model Caching on Mobile Agents**|Xiaoyu Wang et.al.|[2408.14001](http://arxiv.org/abs/2408.14001)|null|
|**2024-08-25**|**FedGlu: A personalized federated learning-based glucose forecasting algorithm for improved performance in glycemic excursion regions**|Darpit Dave et.al.|[2408.13926](http://arxiv.org/abs/2408.13926)|null|
|**2024-08-25**|**Sample-Independent Federated Learning Backdoor Attack**|Weida Xu et.al.|[2408.13849](http://arxiv.org/abs/2408.13849)|null|
|**2024-08-25**|**SAB:A Stealing and Robust Backdoor Attack based on Steganographic Algorithm against Federated Learning**|Weida Xu et.al.|[2408.13773](http://arxiv.org/abs/2408.13773)|null|
|**2024-08-24**|**Submodular Maximization Approaches for Equitable Client Selection in Federated Learning**|Andrés Catalino Castillo Jiménez et.al.|[2408.13683](http://arxiv.org/abs/2408.13683)|null|
|**2024-08-24**|**Towards Case-based Interpretability for Medical Federated Learning**|Laura Latorre et.al.|[2408.13626](http://arxiv.org/abs/2408.13626)|null|
|**2024-08-23**|**Social Welfare Maximization for Federated Learning with Network Effects**|Xiang Li et.al.|[2408.13223](http://arxiv.org/abs/2408.13223)|null|
|**2024-08-23**|**Improving the Classification Effect of Clinical Images of Diseases for Multi-Source Privacy Protection**|Tian Bowen et.al.|[2408.13038](http://arxiv.org/abs/2408.13038)|null|
|**2024-08-23**|**A Web-Based Solution for Federated Learning with LLM-Based Automation**|Chamith Mawela et.al.|[2408.13010](http://arxiv.org/abs/2408.13010)|null|
|**2024-08-23**|**Enhancing Vehicle Environmental Awareness via Federated Learning and Automatic Labeling**|Chih-Yu Lin et.al.|[2408.12769](http://arxiv.org/abs/2408.12769)|null|
|**2024-08-22**|**Tackling Data Heterogeneity in Federated Learning via Loss Decomposition**|Shuang Zeng et.al.|[2408.12300](http://arxiv.org/abs/2408.12300)|**[link](https://github.com/zeng-shuang/fedld)**|
|**2024-08-22**|**Weight Scope Alignment: A Frustratingly Easy Method for Model Merging**|Yichu Xu et.al.|[2408.12237](http://arxiv.org/abs/2408.12237)|null|
|**2024-08-22**|**Empowering Over-the-Air Personalized Federated Learning via RIS**|Wei Shi et.al.|[2408.12162](http://arxiv.org/abs/2408.12162)|null|
|**2024-08-22**|**Understanding Data Reconstruction Leakage in Federated Learning from a Theoretical Perspective**|Zifan Wang et.al.|[2408.12119](http://arxiv.org/abs/2408.12119)|null|
|**2024-08-21**|**Federated Diabetes Prediction in Canadian Adults Using Real-world Cross-Province Primary Care Data**|Guojun Tang et.al.|[2408.12029](http://arxiv.org/abs/2408.12029)|null|
|**2024-08-21**|**RFID based Health Adherence Medicine Case Using Fair Federated Learning**|Ali Kamrani khodaei et.al.|[2408.11782](http://arxiv.org/abs/2408.11782)|**[link](https://github.com/MibclAric/Smart-Pill-Case)**|
|**2024-08-21**|**FedGS: Federated Gradient Scaling for Heterogeneous Medical Image Segmentation**|Philip Schutte et.al.|[2408.11701](http://arxiv.org/abs/2408.11701)|**[link](https://github.com/trustworthy-ai-uu-nki/federated-learning-disentanglement)**|
|**2024-08-21**|**Technical Report: Coopetition in Heterogeneous Cross-Silo Federated Learning**|Chao Huang et.al.|[2408.11355](http://arxiv.org/abs/2408.11355)|null|
|**2024-08-21**|**FedMoE: Personalized Federated Learning via Heterogeneous Mixture of Experts**|Hanzi Mei et.al.|[2408.11304](http://arxiv.org/abs/2408.11304)|null|
|**2024-08-21**|**The Key of Parameter Skew in Federated Learning**|Sifan Wang et.al.|[2408.11278](http://arxiv.org/abs/2408.11278)|null|
|**2024-08-20**|**NeuLite: Memory-Efficient Federated Learning via Elastic Progressive Training**|Yebo Wu et.al.|[2408.10826](http://arxiv.org/abs/2408.10826)|null|
|**2024-08-20**|**Security Assessment of Hierarchical Federated Deep Learning**|D Alqattan et.al.|[2408.10752](http://arxiv.org/abs/2408.10752)|**[link](https://github.com/dalqattan/sechfl)**|
|**2024-08-20**|**Federated Clustering: An Unsupervised Cluster-Wise Training for Decentralized Data Distributions**|Mirko Nardi et.al.|[2408.10664](http://arxiv.org/abs/2408.10664)|null|
|**2024-08-19**|**Differentially Private Stochastic Gradient Descent with Fixed-Size Minibatches: Tighter RDP Guarantees with or without Replacement**|Jeremiah Birrell et.al.|[2408.10456](http://arxiv.org/abs/2408.10456)|**[link](https://github.com/star-ailab/FSRDP)**|
|**2024-08-19**|**Federated Learning of Large ASR Models in the Real World**|Yonghui Xiao et.al.|[2408.10443](http://arxiv.org/abs/2408.10443)|null|
|**2024-08-19**|**Federated Frank-Wolfe Algorithm**|Ali Dadras et.al.|[2408.10090](http://arxiv.org/abs/2408.10090)|**[link](https://github.com/sourasb05/Federated-Frank-Wolfe)**|
|**2024-08-19**|**Towards Robust Federated Image Classification: An Empirical Study of Weight Selection Strategies in Manufacturing**|Vinit Hegiste et.al.|[2408.10024](http://arxiv.org/abs/2408.10024)|null|
|**2024-08-19**|**Sequential Federated Learning in Hierarchical Architecture on Non-IID Datasets**|Xingrun Yan et.al.|[2408.09762](http://arxiv.org/abs/2408.09762)|null|
|**2024-08-18**|**Addressing Heterogeneity in Federated Learning: Challenges and Solutions for a Shared Production Environment**|Tatjana Legler et.al.|[2408.09556](http://arxiv.org/abs/2408.09556)|null|
|**2024-08-20**|**Seamless Integration: Sampling Strategies in Federated Learning Systems**|Tatjana Legler et.al.|[2408.09545](http://arxiv.org/abs/2408.09545)|null|
|**2024-08-18**|**Byzantine-resilient Federated Learning Employing Normalized Gradients on Non-IID Datasets**|Shiyuan Zuo et.al.|[2408.09539](http://arxiv.org/abs/2408.09539)|null|
|**2024-08-18**|**Orchestrating Federated Learning in Space-Air-Ground Integrated Networks: Adaptive Data Offloading and Seamless Handover**|Dong-Jun Han et.al.|[2408.09522](http://arxiv.org/abs/2408.09522)|null|
|**2024-08-18**|**Mitigating Noise Detriment in Differentially Private Federated Learning with Model Pre-training**|Huitong Jin et.al.|[2408.09478](http://arxiv.org/abs/2408.09478)|null|
|**2024-08-18**|**Federated Graph Learning with Structure Proxy Alignment**|Xingbo Fu et.al.|[2408.09393](http://arxiv.org/abs/2408.09393)|**[link](https://github.com/xbfu/fedspray)**|
|**2024-08-17**|**FEDMEKI: A Benchmark for Scaling Medical Foundation Models via Federated Knowledge Injection**|Jiaqi Wang et.al.|[2408.09227](http://arxiv.org/abs/2408.09227)|**[link](https://github.com/psudslab/FEDMEKI)**|
|**2024-08-16**|**A Hassle-free Algorithm for Private Learning in Practice: Don't Use Tree Aggregation, Use BLTs**|H. Brendan McMahan et.al.|[2408.08868](http://arxiv.org/abs/2408.08868)|null|
|**2024-08-16**|**A Novel Buffered Federated Learning Framework for Privacy-Driven Anomaly Detection in IIoT**|Samira Kamali Poorazad et.al.|[2408.08722](http://arxiv.org/abs/2408.08722)|null|
|**2024-08-16**|**RBLA: Rank-Based-LoRA-Aggregation for Fine-tuning Heterogeneous Models in FLaaS**|Shuaijun Chen et.al.|[2408.08699](http://arxiv.org/abs/2408.08699)|null|
|**2024-08-16**|**A Multivocal Literature Review on Privacy and Fairness in Federated Learning**|Beatrice Balbierer et.al.|[2408.08666](http://arxiv.org/abs/2408.08666)|null|
|**2024-08-16**|**Mitigating Backdoor Attacks in Federated Learning via Flipping Weight Updates of Low-Activation Input Neurons**|Binbin Ding et.al.|[2408.08655](http://arxiv.org/abs/2408.08655)|null|
|**2024-08-16**|**The Power of Bias: Optimizing Client Selection in Federated Learning with Heterogeneous Differential Privacy**|Jiating Ma et.al.|[2408.08642](http://arxiv.org/abs/2408.08642)|null|
|**2024-08-15**|**A Robust Multi-Stage Intrusion Detection System for In-Vehicle Network Security using Hierarchical Federated Learning**|Muzun Althunayyan et.al.|[2408.08433](http://arxiv.org/abs/2408.08433)|null|
|**2024-08-15**|**Random Gradient Masking as a Defensive Measure to Deep Leakage in Federated Learning**|Joon Kim et.al.|[2408.08430](http://arxiv.org/abs/2408.08430)|null|
|**2024-08-15**|**Federated Fairness Analytics: Quantifying Fairness in Federated Learning**|Oscar Dilley et.al.|[2408.08214](http://arxiv.org/abs/2408.08214)|**[link](https://github.com/oscardilley/federated-fairness)**|
|**2024-08-15**|**Communication-robust and Privacy-safe Distributed Estimation for Heterogeneous Community-level Behind-the-meter Solar Power Generation**|Jinglei Feng et.al.|[2408.08107](http://arxiv.org/abs/2408.08107)|null|
|**2024-08-15**|**Addressing Skewed Heterogeneity via Federated Prototype Rectification with Personalization**|Shunxin Guo et.al.|[2408.07966](http://arxiv.org/abs/2408.07966)|null|
|**2024-08-14**|**Enhancing Equitable Access to AI in Housing and Homelessness System of Care through Federated Learning**|Musa Taib et.al.|[2408.07845](http://arxiv.org/abs/2408.07845)|null|
|**2024-08-14**|**FedQUIT: On-Device Federated Unlearning via a Quasi-Competent Virtual Teacher**|Alessio Mora et.al.|[2408.07587](http://arxiv.org/abs/2408.07587)|null|
|**2024-08-13**|**FedMADE: Robust Federated Learning for Intrusion Detection in IoT Networks Using a Dynamic Aggregation Method**|Shihua Sun et.al.|[2408.07152](http://arxiv.org/abs/2408.07152)|null|
|**2024-08-12**|**OFL-W3: A One-shot Federated Learning System on Web 3.0**|Linshan Jiang et.al.|[2408.07096](http://arxiv.org/abs/2408.07096)|null|
|**2024-08-13**|**Heterogeneity: An Open Challenge for Federated On-board Machine Learning**|Maria Hartmann et.al.|[2408.06903](http://arxiv.org/abs/2408.06903)|null|
|**2024-08-13**|**Voltran: Unlocking Trust and Confidentiality in Decentralized Federated Learning Aggregation**|Hao Wang et.al.|[2408.06885](http://arxiv.org/abs/2408.06885)|null|
|**2024-08-13**|**Prioritizing Modalities: Flexible Importance Scheduling in Federated Multimodal Learning**|Jieming Bian et.al.|[2408.06549](http://arxiv.org/abs/2408.06549)|null|
|**2024-08-14**|**Decentralized Health Intelligence Network (DHIN)**|Abraham Nash et.al.|[2408.06240](http://arxiv.org/abs/2408.06240)|null|
|**2024-08-12**|**Lancelot: Towards Efficient and Privacy-Preserving Byzantine-Robust Federated Learning within Fully Homomorphic Encryption**|Siyang Jiang et.al.|[2408.06197](http://arxiv.org/abs/2408.06197)|null|
|**2024-08-12**|**Centralized and Federated Heart Disease Classification Models Using UCI Dataset and their Shapley-value Based Interpretability**|Mario Padilla Rodriguez et.al.|[2408.06183](http://arxiv.org/abs/2408.06183)|**[link](https://github.com/padillma1/heart-disease-classification-on-uci-dataset-and-shapley-interpretability-analysis)**|
|**2024-08-12**|**Understanding Byzantine Robustness in Federated Learning with A Black-box Server**|Fangyuan Zhao et.al.|[2408.06042](http://arxiv.org/abs/2408.06042)|**[link](https://github.com/alibaba/federatedscope)**|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## moe

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-23**|**Robust and Explainable Depression Identification from Speech Using Vowel-Based Ensemble Learning Approaches**|Kexin Feng et.al.|[2410.18298](http://arxiv.org/abs/2410.18298)|null|本研究探讨了用于从语音中识别抑郁症的可解释机器学习算法。基于抑郁症影响运动控制和元音生成的语音产生证据，使用预训练的基于元音的嵌入来整合具有语义意义的语言单位。随后，采用集成学习方法将问题分解为由特定抑郁症状和严重程度水平表征的组成部分。研究探索了两种方法：一种是“自下而上”的方法，用8个模型预测个体患者健康问卷-8 (PHQ-8) 项目的得分；另一种是使用专家混合模型（MoE）的“自上而下”方法，该模型配备了一个路由模块来评估抑郁严重程度。这两种方法的表现与最先进的基线相当，展示了其稳健性并减少了对数据集均值/中位数的敏感性。讨论了系统可解释性的优势，强调其在协助临床医生进行抑郁症诊断和筛查方面的潜力。|
|**2024-10-23**|**MiLoRA: Efficient Mixture of Low-Rank Adaptation for Large Language Models Fine-tuning**|Jingfan Zhang et.al.|[2410.18035](http://arxiv.org/abs/2410.18035)|null|低秩适应（LoRA）及其混合专家（MOE）变体是高效的参数高效微调（PEFT）方法。然而，它们在多租户环境中由于在Transformer层的多个线性模块中添加了LoRA模块和MOE路由器而引入了显著的延迟。为了解决这个问题，我们提出了一种新颖且高效的LoRA变体——混合低秩适应（MiLoRA）。MiLoRA与之前的MOE风格的LoRA方法不同，它将每个LoRA模块视为一个专家，并采用一种提示感知的路由机制。该机制在生成第一个新令牌之前计算一次专家路由结果，并在后续令牌中重用这些结果，从而减少延迟。在常识推理任务、数学推理任务以及广泛使用的LLM评估基准上的大量实验和分析表明，MiLoRA在可调参数预算相当的情况下始终优于强大的PEFT基线。此外，与之前的基于LoRA的方法相比，MiLoRA在多租户环境中显著降低了延迟。|
|**2024-10-23**|**ExpertFlow: Optimized Expert Activation and Token Allocation for Efficient Mixture-of-Experts Inference**|Xin He et.al.|[2410.17954](http://arxiv.org/abs/2410.17954)|null|稀疏混合专家（MoE）模型虽然在性能上优于密集型大型语言模型（LLM），但在推理过程中由于其高内存需求而面临显著的部署挑战。现有的卸载技术通常涉及在GPU和CPU之间交换激活和空闲的专家，但这些技术往往因僵化的专家缓存机制而受限。这些机制无法适应动态路由，导致缓存利用率低下，或者预测训练成本过高。为了解决这些特定于推理的挑战，我们引入了ExpertFlow，这是一个专门设计用于通过适应灵活路由并实现CPU和GPU之间的高效专家调度来提高推理效率的综合系统，从而减少开销并提升系统性能。我们的方法核心是一种基于预测路由路径的卸载机制，该机制利用轻量级预测器在计算开始前准确预测路由路径。这种主动策略允许实时纠正专家缓存中的错误，显著提高了缓存命中率，并减少了专家转移的频率，从而最小化了I/O开销。此外，我们还实现了一种动态令牌调度策略，通过重新排列不同批次中的输入令牌来优化MoE推理。这种方法不仅减少了每批次激活的专家数量，还提高了计算效率。大量实验表明，与基线方法相比，ExpertFlow能够节省高达93.72%的GPU内存，并将推理速度提高2到10倍，突显了其作为资源受限推理场景中强大解决方案的有效性和实用性。|
|**2024-10-22**|**Optimizing Mixture-of-Experts Inference Time Combining Model Deployment and Communication Scheduling**|Jialong Li et.al.|[2410.17043](http://arxiv.org/abs/2410.17043)|null|随着机器学习模型在规模和复杂性上的增加，其计算需求成为一个重要的障碍。混合专家（MoE）模型通过选择性地激活相关专家来缓解这一问题。尽管如此，MoE模型仍然受到全对全操作导致的高通信开销、同步通信约束导致的低GPU利用率以及异构GPU环境带来的复杂性的限制。本文介绍了Aurora，它通过对模型部署和全对全通信调度进行优化来解决这些挑战。Aurora通过策略性地排序令牌传输，在全对全通信中实现了最小的通信时间。它通过将不同模型的专家共置于同一设备上，提高了GPU利用率，避免了同步全对全通信的局限性。我们在四种常见的GPU集群设置下从理论上分析了Aurora的优化策略：独占与共置模型在GPU上，以及同构与异构GPU。Aurora为其中三种情况提供了最优解，而对于剩下的NP难问题，它提供了一个多项式时间内的次优解，其性能仅比最优解下降1.07倍。Aurora是首个通过优化模型部署和通信调度来减少各种场景下MoE推理时间的方法。评估表明，Aurora显著加速了推理过程，在同构集群中实现了最高2.38倍的速度提升，在异构环境中达到了3.54倍的速度提升。此外，与现有方法相比，Aurora将GPU利用率提高了最多1.5倍。|
|**2024-10-22**|**CartesianMoE: Boosting Knowledge Sharing among Experts via Cartesian Product Routing in Mixture-of-Experts**|Zhenpeng Su et.al.|[2410.16077](http://arxiv.org/abs/2410.16077)|null|最近，由于大型语言模型（LLM）在各种下游任务中的出色表现，它们受到了社区的广泛关注。根据著名的扩展定律，扩大密集型LLM的规模可以增强其能力，但也会显著增加计算复杂度。混合专家（MoE）模型通过允许模型规模增长而不大幅提高训练或推理成本来解决这个问题。然而，MoE模型面临着专家之间知识共享的挑战，这使得它们的性能对路由准确性较为敏感。为了解决这一问题，之前的工作引入了共享专家，并以“加法”的方式将其输出与前K个被路由专家的输出相结合。在这篇论文中，受到集体矩阵分解学习数据间共享知识的启发，我们提出了CartesianMoE，它以更像“乘法”的方式实现了专家之间更有效的知识共享。广泛的实验结果表明，无论是在困惑度还是下游任务性能方面，CartesianMoE都优于之前的MoE模型。此外，我们还发现CartesianMoE实现了更好的专家路由鲁棒性。|
|**2024-10-21**|**Generalizing Motion Planners with Mixture of Experts for Autonomous Driving**|Qiao Sun et.al.|[2410.15774](http://arxiv.org/abs/2410.15774)|**[link](https://github.com/tsinghua-mars-lab/statetransformer)**|**大型真实驾驶数据集激发了对自动驾驶数据驱动运动规划器各个方面的大量研究，包括数据增强、模型架构、奖励设计、训练策略和规划器流水线。这些规划器在复杂和少量样本情况下比先前的方法具有更好的泛化能力。然而，实验结果表明，由于设计过于复杂或训练范式的问题，许多方法在规划性能上的泛化能力有限。在本文中，我们回顾并基准测试了以往关注泛化能力的方法。实验结果表明，随着模型适当扩展，许多设计元素变得冗余。我们介绍了StateTransformer-2（STR2），这是一种可扩展的仅解码器运动规划器，它使用视觉变换器（ViT）编码器和混合专家（MoE）因果变换器架构。MoE骨干通过训练过程中的专家路由解决了模态崩溃和奖励平衡问题。在NuPlan数据集上进行的广泛实验表明，我们的方法在不同测试集和闭环仿真中比以往的方法具有更好的泛化能力。此外，我们在数十亿个真实城市驾驶场景上评估了其可扩展性，展示了随着数据量和模型规模的增长，准确性的持续提升。**|
|**2024-10-21**|**ViMoE: An Empirical Study of Designing Vision Mixture-of-Experts**|Xumeng Han et.al.|[2410.15732](http://arxiv.org/abs/2410.15732)|null|混合专家（MoE）模型体现了分而治之的概念，是一种有前景的方法，可以增加模型容量，并在多个领域展示了出色的可扩展性。在这篇论文中，我们将MoE结构集成到经典的视觉Transformer（ViT）中，并将其命名为ViMoE，通过图像分类的综合研究探索了将MoE应用于视觉领域的潜力。然而，我们观察到性能对MoE层的配置非常敏感，如果没有精心设计，很难获得最优结果。根本原因是不适当的MoE层会导致不可靠的路由，并阻碍专家有效地获取有用的知识。为了解决这个问题，我们引入了一个共享专家来学习和捕捉共同信息，作为一种构建稳定ViMoE的有效方式。此外，我们展示了如何分析专家路由行为，揭示哪些MoE层能够专门处理特定信息，哪些不能。这为保留关键层同时去除冗余提供了指导，从而使ViMoE变得更加高效而不牺牲准确性。我们希望这项工作能为视觉MoE模型的设计提供新的见解，并为未来的研究提供有价值的实证指导。|
|**2024-10-20**|**Unveiling and Consulting Core Experts in Retrieval-Augmented MoE-based LLMs**|Xin Zhou et.al.|[2410.15438](http://arxiv.org/abs/2410.15438)|null|检索增强生成（RAG）显著提高了大型语言模型（LLMs）解决知识密集型任务的能力。虽然现有研究通过检索更高质量的文档或设计特定于RAG的LLMs来提高RAG性能，但LLMs内部机制对RAG系统有效性的影响仍然未得到充分探索。在本文中，我们旨在研究基于混合专家（MoE）的流行LLMs中的这些内部机制，并展示如何通过检查这些LLMs中的专家激活情况来改进RAG。我们的受控实验揭示了几个核心专家群体主要负责与RAG相关的行为。这些核心专家的激活可以表明模型倾向于使用外部/内部知识，并调整其行为。例如，我们识别出一些核心专家能够（1）指示模型内部知识是否足够，（2）评估检索到的文档质量，以及（3）提高模型利用上下文的能力。基于这些发现，我们提出了一些通过专家激活来提高RAG效率和有效性的策略。在不同数据集和基于MoE的LLMs上的实验结果表明了我们方法的有效性。|
|**2024-10-20**|**LoRA-IR: Taming Low-Rank Experts for Efficient All-in-One Image Restoration**|Yuang Ai et.al.|[2410.15385](http://arxiv.org/abs/2410.15385)|**[link](https://github.com/shallowdream204/lora-ir)**|**基于提示的全功能图像恢复（IR）框架通过将特定退化的信息纳入提示模块中，已经取得了显著的性能。然而，处理在现实世界场景中遇到的复杂多样的退化仍然是一个重大挑战。为了解决这一挑战，我们提出了LoRA-IR，这是一个灵活的框架，它通过动态利用紧凑的低秩专家来促进高效的全功能图像恢复。具体来说，LoRA-IR包括两个训练阶段：退化引导的预训练和参数高效的微调。在预训练阶段，我们通过引入一个简单的机制来增强预训练的CLIP模型，使其能够扩展到更高的分辨率，从而提取出鲁棒的退化表示，这些表示可以自适应地引导IR网络。在微调阶段，我们使用低秩适应（LoRA）来改进预训练的IR网络。基于混合专家（MoE）架构，LoRA-IR通过一个退化引导的路由器动态集成多个低秩恢复专家。这种动态集成机制大大增强了我们的模型对复杂现实世界场景中多样化和未知退化的适应能力。广泛的实验表明，LoRA-IR在14个图像恢复任务和29个基准测试上达到了最先进的性能。代码和预训练模型将在以下网址提供：https://github.com/shallowdream204/LoRA-IR。**|
|**2024-10-19**|**MENTOR: Mixture-of-Experts Network with Task-Oriented Perturbation for Visual Reinforcement Learning**|Suning Huang et.al.|[2410.14972](http://arxiv.org/abs/2410.14972)|null|视觉深度强化学习（RL）使机器人能够从视觉输入中学习处理非结构化任务的技能。然而，当前算法由于样本效率低，限制了其实际应用。在这项工作中，我们提出了MENTOR方法，该方法改进了RL代理的架构和优化。具体来说，MENTOR用混合专家（MoE）骨干网络替代了标准的多层感知器（MLP），通过利用模块化的专家学习来避免梯度冲突，增强了代理处理复杂任务的能力。此外，MENTOR引入了一种面向任务的扰动机制，启发式地采样包含任务相关信息的扰动候选，从而实现更针对性和有效的优化。MENTOR在三个仿真领域——DeepMind控制套件、Meta-World和Adroit上优于最先进的方法。此外，在包括插钉、电缆布线和桌面高尔夫在内的三个具有挑战性的现实世界机器人操作任务上，MENTOR平均达到了83%的成功率，这显著超过了当前最强无模型视觉RL算法32%的成功率。这些结果强调了提高样本效率对于推动视觉RL应用于现实世界机器人技术的重要性。实验视频可在https://suninghuang19.github.io/mentor_page获取。|
|**2024-10-16**|**EPS-MoE: Expert Pipeline Scheduler for Cost-Efficient MoE Inference**|Yulei Qian et.al.|[2410.12247](http://arxiv.org/abs/2410.12247)|null|
|**2024-10-15**|**MoE-Pruner: Pruning Mixture-of-Experts Large Language Model using the Hints from Its Router**|Yanyue Xie et.al.|[2410.12013](http://arxiv.org/abs/2410.12013)|null|
|**2024-10-15**|**MoH: Multi-Head Attention as Mixture-of-Head Attention**|Peng Jin et.al.|[2410.11842](http://arxiv.org/abs/2410.11842)|**[link](https://github.com/skyworkai/moh)**|
|**2024-10-15**|**Transformer Layer Injection: A Novel Approach for Efficient Upscaling of Large Language Models**|James Vo et.al.|[2410.11654](http://arxiv.org/abs/2410.11654)|null|
|**2024-10-16**|**Quadratic Gating Functions in Mixture of Experts: A Statistical Insight**|Pedram Akbarian et.al.|[2410.11222](http://arxiv.org/abs/2410.11222)|null|
|**2024-10-16**|**Your Mixture-of-Experts LLM Is Secretly an Embedding Model For Free**|Ziyue Li et.al.|[2410.10814](http://arxiv.org/abs/2410.10814)|**[link](https://github.com/tianyi-lab/moe-embedding)**|
|**2024-10-14**|**Efficiently Democratizing Medical LLMs for 50 Languages via a Mixture of Language Family Experts**|Guorui Zheng et.al.|[2410.10626](http://arxiv.org/abs/2410.10626)|**[link](https://github.com/freedomintelligence/apollomoe)**|
|**2024-10-14**|**Learning to Ground VLMs without Forgetting**|Aritra Bhowmik et.al.|[2410.10491](http://arxiv.org/abs/2410.10491)|null|
|**2024-10-14**|**Moirai-MoE: Empowering Time Series Foundation Models with Sparse Mixture of Experts**|Xu Liu et.al.|[2410.10469](http://arxiv.org/abs/2410.10469)|null|
|**2024-10-15**|**Ada-K Routing: Boosting the Efficiency of MoE-based LLMs**|Tongtian Yue et.al.|[2410.10456](http://arxiv.org/abs/2410.10456)|null|
|**2024-10-16**|**Mixture of Experts Made Personalized: Federated Prompt Learning for Vision-Language Models**|Jun Luo et.al.|[2410.10114](http://arxiv.org/abs/2410.10114)|null|
|**2024-10-14**|**AlphaLoRA: Assigning LoRA Experts Based on Layer Training Quality**|Peijun Qing et.al.|[2410.10054](http://arxiv.org/abs/2410.10054)|**[link](https://github.com/morelife2017/alphalora)**|
|**2024-10-13**|**MoIN: Mixture of Introvert Experts to Upcycle an LLM**|Ajinkya Tejankar et.al.|[2410.09687](http://arxiv.org/abs/2410.09687)|null|
|**2024-10-11**|**Semi-Supervised Learning of Noisy Mixture of Experts Models**|Oh-Ran Kwon et.al.|[2410.09039](http://arxiv.org/abs/2410.09039)|null|
|**2024-10-10**|**SLIM: Let LLM Learn More and Forget Less with Soft LoRA and Identity Mixture**|Jiayi Han et.al.|[2410.07739](http://arxiv.org/abs/2410.07739)|null|
|**2024-10-10**|**Upcycling Large Language Models into Mixture of Experts**|Ethan He et.al.|[2410.07524](http://arxiv.org/abs/2410.07524)|null|
|**2024-10-09**|**MoE++: Accelerating Mixture-of-Experts Methods with Zero-Computation Experts**|Peng Jin et.al.|[2410.07348](http://arxiv.org/abs/2410.07348)|**[link](https://github.com/skyworkai/moe-plus-plus)**|
|**2024-10-04**|**A Dynamic Approach to Stock Price Prediction: Comparing RNN and Mixture of Experts Models Across Different Volatility Profiles**|Diego Vallarino et.al.|[2410.07234](http://arxiv.org/abs/2410.07234)|null|
|**2024-10-08**|**Scaling Laws Across Model Architectures: A Comparative Analysis of Dense and MoE Models in Large Language Models**|Siqi Wang et.al.|[2410.05661](http://arxiv.org/abs/2410.05661)|null|
|**2024-10-06**|**Realizing Video Summarization from the Path of Language-based Semantic Understanding**|Kuan-Chen Mu et.al.|[2410.04511](http://arxiv.org/abs/2410.04511)|null|
|**2024-10-09**|**Structure-Enhanced Protein Instruction Tuning: Towards General-Purpose Protein Understanding**|Wei Wu et.al.|[2410.03553](http://arxiv.org/abs/2410.03553)|null|
|**2024-10-04**|**Exploring the Benefit of Activation Sparsity in Pre-training**|Zhengyan Zhang et.al.|[2410.03440](http://arxiv.org/abs/2410.03440)|**[link](https://github.com/thunlp/moefication)**|
|**2024-10-03**|**MLP-KAN: Unifying Deep Representation and Function Learning**|Yunhong He et.al.|[2410.03027](http://arxiv.org/abs/2410.03027)|**[link](https://github.com/dlyuangod/mlp-kan)**|
|**2024-10-03**|**On Expert Estimation in Hierarchical Mixture of Experts: Beyond Softmax Gating Functions**|Huy Nguyen et.al.|[2410.02935](http://arxiv.org/abs/2410.02935)|null|
|**2024-10-03**|**Efficient Residual Learning with Mixture-of-Experts for Universal Dexterous Grasping**|Ziye Huang et.al.|[2410.02475](http://arxiv.org/abs/2410.02475)|null|
|**2024-10-04**|**Searching for Efficient Linear Layers over a Continuous Space of Structured Matrices**|Andres Potapczynski et.al.|[2410.02117](http://arxiv.org/abs/2410.02117)|**[link](https://github.com/andpotap/einsum-search)**|
|**2024-10-04**|**EC-DIT: Scaling Diffusion Transformers with Adaptive Expert-Choice Routing**|Haotian Sun et.al.|[2410.02098](http://arxiv.org/abs/2410.02098)|null|
|**2024-10-02**|**Open-RAG: Enhanced Retrieval-Augmented Reasoning with Open-Source Large Language Models**|Shayekh Bin Islam et.al.|[2410.01782](http://arxiv.org/abs/2410.01782)|**[link](https://github.com/ShayekhBinIslam/openrag)**|
|**2024-10-02**|**Upcycling Instruction Tuning from Dense to Mixture-of-Experts via Parameter Merging**|Tingfeng Hui et.al.|[2410.01610](http://arxiv.org/abs/2410.01610)|null|
|**2024-10-02**|**The Labyrinth of Links: Navigating the Associative Maze of Multi-modal LLMs**|Hong Li et.al.|[2410.01417](http://arxiv.org/abs/2410.01417)|null|
|**2024-10-01**|**MoS: Unleashing Parameter Efficiency of Low-Rank Adaptation with Mixture of Shards**|Sheng Wang et.al.|[2410.00938](http://arxiv.org/abs/2410.00938)|null|
|**2024-10-01**|**Robust Traffic Forecasting against Spatial Shift over Years**|Hongjun Wang et.al.|[2410.00373](http://arxiv.org/abs/2410.00373)|**[link](https://github.com/dreamzz5/st-expert)**|
|**2024-09-30**|**MM1.5: Methods, Analysis & Insights from Multimodal LLM Fine-tuning**|Haotian Zhang et.al.|[2409.20566](http://arxiv.org/abs/2409.20566)|null|
|**2024-10-02**|**Time-MoE: Billion-Scale Time Series Foundation Models with Mixture of Experts**|Xiaoming Shi et.al.|[2409.16040](http://arxiv.org/abs/2409.16040)|**[link](https://github.com/time-moe/time-moe)**|
|**2024-09-24**|**Boosting Code-Switching ASR with Mixture of Experts Enhanced Speech-Conditioned LLM**|Fengrun Zhang et.al.|[2409.15905](http://arxiv.org/abs/2409.15905)|null|
|**2024-09-24**|**Toward Mixture-of-Experts Enabled Trustworthy Semantic Communication for 6G Networks**|Jiayi He et.al.|[2409.15695](http://arxiv.org/abs/2409.15695)|null|
|**2024-09-23**|**A Gated Residual Kolmogorov-Arnold Networks for Mixtures of Experts**|Hugo Inzirillo et.al.|[2409.15161](http://arxiv.org/abs/2409.15161)|**[link](https://github.com/remigenet/kamoe)**|
|**2024-09-23**|**Multi-Modal Generative AI: Multi-modal LLM, Diffusion and Beyond**|Hong Chen et.al.|[2409.14993](http://arxiv.org/abs/2409.14993)|null|
|**2024-10-01**|**On-Device Collaborative Language Modeling via a Mixture of Generalists and Specialists**|Dongyang Fan et.al.|[2409.13931](http://arxiv.org/abs/2409.13931)|**[link](https://github.com/epfml/comigs)**|
|**2024-09-18**|**Mixture of Diverse Size Experts**|Manxi Sun et.al.|[2409.12210](http://arxiv.org/abs/2409.12210)|null|
|**2024-09-18**|**GRIN: GRadient-INformed MoE**|Liyuan Liu et.al.|[2409.12136](http://arxiv.org/abs/2409.12136)|null|
|**2024-09-17**|**LPT++: Efficient Training on Mixture of Long-tailed Experts**|Bowen Dong et.al.|[2409.11323](http://arxiv.org/abs/2409.11323)|null|
|**2024-09-10**|**DA-MoE: Towards Dynamic Expert Allocation for Mixture-of-Experts Models**|Maryam Akhavan Aghdam et.al.|[2409.06669](http://arxiv.org/abs/2409.06669)|null|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

## SSMs

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-24**|**Taipan: Efficient and Expressive State Space Language Models with Selective Attention**|Chien Van Nguyen et.al.|[2410.18572](http://arxiv.org/abs/2410.18572)|null|高效的长上下文语言建模仍然是自然语言处理（NLP）中的一个重要挑战。虽然Transformer在语言任务中占据主导地位，但它们在处理长序列时会遇到困难，因为训练时的计算复杂度为二次方，而在推理时内存成本线性增长。最近的状态空间模型（SSMs），如Mamba，提供了常数内存使用的替代方案，但在需要大量上下文检索的任务中表现不佳。我们引入了一种新的混合架构Taipan，它结合了Mamba-2和选择性注意力层（SALs）。这些SALs能够识别需要长距离交互的标记，去除不太重要的特征，并使用注意力模块增强其表示。这种方法平衡了Mamba的效率与Transformer在内存密集型任务中的性能。通过限制注意力预算，Taipan可以将准确预测扩展到多达100万个标记的上下文长度，同时保持计算效率。我们的实验表明，Taipan在各种规模和任务中表现出色，为高效的长上下文语言建模提供了一个有前景的解决方案。|
|**2024-10-21**|**START: A Generalized State Space Model with Saliency-Driven Token-Aware Transformation**|Jintao Guo et.al.|[2410.16020](http://arxiv.org/abs/2410.16020)|null|域泛化（DG）旨在通过从多个源域学习来使模型能够泛化到未见过的目标域。现有的DG方法主要依赖于卷积神经网络（CNNs），这些网络由于其有限的感受野而天生倾向于学习纹理偏差，导致容易过拟合源域。虽然一些工作引入了基于Transformer的方法（ViTs）以利用全局感受野，但这些方法由于自注意力机制的二次复杂度而带来了高昂的计算成本。最近，先进的状态空间模型（SSMs），如Mamba，在监督学习任务中表现出色，通过在训练过程中实现序列长度的线性复杂度以及在推理过程中快速的RNN式计算。受此启发，我们研究了Mamba模型在域迁移下的泛化能力，并发现SSMs中的输入依赖矩阵可能会累积并放大特定域的特征，从而阻碍模型的泛化。为了解决这个问题，我们提出了一种具有显著性感知标记变换（称为START）的新颖SSM架构，该架构达到了最先进的性能，并为CNNs和ViTs提供了一个有竞争力的替代方案。我们的START可以通过选择性地扰动和抑制SSMs输入依赖矩阵中显著标记内的特定域特征，有效减少不同域之间的差异。在五个基准数据集上的广泛实验表明，START以高效的线性复杂度超越了现有的SOTA DG方法。我们的代码可以在https://github.com/lingeringlight/START获取。|
|**2024-10-21**|**Revealing and Mitigating the Local Pattern Shortcuts of Mamba**|Wangjie You et.al.|[2410.15678](http://arxiv.org/abs/2410.15678)|**[link](https://github.com/zetangforward/global_mamba)**|**大型语言模型（LLMs）由于注意力机制的引入而取得了显著进步，但其二次复杂度和线性内存需求限制了它们在长上下文任务中的表现。最近，研究人员推出了基于状态空间模型（SSMs）的先进模型Mamba，该模型提供了线性复杂度和常数内存。尽管据报道Mamba的性能可以匹配甚至超过基于注意力的模型，但我们的分析显示存在一个性能差距：Mamba在涉及局部关键信息的任务中表现出色，但在需要处理分布广泛的关键信息的任务中面临挑战。我们控制实验表明，这种不一致性源于Mamba依赖于局部模式捷径，这使模型能够在有限的内存中记住局部关键信息，但阻碍了它保留更分散的信息。因此，我们在Mamba模型中引入了一个全局选择模块来解决这个问题。在现有和新提出的合成任务以及实际任务上的实验表明了我们方法的有效性。值得注意的是，仅通过增加400万个额外参数，我们的方法使Mamba模型（1.3亿参数）在处理分布式信息的任务上实现了显著改进，性能从0提高到了80.54分。**|
|**2024-10-20**|**Taming Mambas for Voxel Level 3D Medical Image Segmentation**|Luca Lumetti et.al.|[2410.15496](http://arxiv.org/abs/2410.15496)|null|最近，3D医学分割领域主要由使用卷积神经网络（CNN）和基于Transformer架构的深度学习模型主导，每种模型都有其独特的优势和局限性。CNN受到局部感受野的限制，而Transformer则因其巨大的内存需求和对数据的高度依赖，在处理3D医学体积时无法达到细粒度水平。因此，在对大型3D医学体积中的医学结构进行分割时，全卷积神经网络如nnUNet仍然占据主导地位。尽管在开发具有次二次时间和内存复杂度的Transformer变体方面取得了许多进展，但这些模型在基于内容的推理方面仍然不足。最近的一个突破是Mamba，这是一种基于状态空间模型（SSM）的递归神经网络（RNN），在著名的自然语言处理和基因组基准测试中，它在许多长上下文任务（百万长度序列）上优于Transformer，同时保持线性复杂度。|
|**2024-10-19**|**Spatial-Mamba: Effective Visual State Space Models via Structure-Aware State Fusion**|Chaodong Xiao et.al.|[2410.15091](http://arxiv.org/abs/2410.15091)|**[link](https://github.com/edwardchasel/spatial-mamba)**|**选择性状态空间模型（SSM），如Mamba，在捕捉一维序列数据中的长距离依赖方面表现出色，但在二维视觉任务的应用中仍面临挑战。目前的视觉SSM通常将图像转换为一维序列，并采用各种扫描模式来结合局部空间依赖性。然而，这些方法在有效捕捉复杂的图像空间结构以及由于加长的扫描路径导致的计算成本增加方面存在局限性。为了解决这些限制，我们提出了Spatial-Mamba，这是一种新方法，直接在状态空间中建立邻域连通性。除了依赖于顺序状态转换外，我们引入了一种结构感知的状态融合方程，利用空洞卷积来捕捉图像的空间结构依赖性，显著增强了视觉上下文信息的流动。Spatial-Mamba分为三个阶段：单向扫描中的初始状态计算、通过结构感知状态融合获取空间上下文，以及使用观测方程进行最终状态计算。我们的理论分析表明，Spatial-Mamba在同一矩阵乘法框架下统一了原始Mamba和线性注意力机制，为我们方法提供了更深层次的理解。实验结果表明，即使仅进行一次扫描，Spatial-Mamba也能在图像分类、检测和分割任务上达到或超越现有的基于SSM的最先进模型。源代码和训练好的模型可以在\href{https://github.com/EdwardChasel/Spatial-Mamba}{这个网址}找到。**|
|**2024-10-16**|**Rethinking Token Reduction for State Space Models**|Zheng Zhan et.al.|[2410.14725](http://arxiv.org/abs/2410.14725)|**[link](https://github.com/wuyushuwys/tor_ssm)**|**近期，状态空间模型（SSM）的最新进展引起了广泛关注，特别是在针对并行训练和处理长距离依赖性进行优化的模型方面。像Mamba这样的架构已经扩展到了数十亿参数，并采用了选择性SSM。为了促进Mamba在更广泛的应用中使用，探索其效率至关重要。虽然令牌减少技术提供了一种简单的后训练策略，但我们发现将现有方法直接应用于SSM会导致性能显著下降。通过深入分析，我们确定了这种失败的原因以及当前技术的局限性。为此，我们提出了一种针对SSM定制的统一后训练令牌减少方法。我们的方法结合了令牌的重要性和相似性，从而利用了剪枝和合并的优势，设计了一种细粒度的层内令牌减少策略。大量实验表明，与现有方法相比，我们的方法在六个基准测试中使用Mamba-2时平均提高了5.7%到13.1%的准确率，同时显著减少了计算需求和内存要求。**|
|**2024-10-17**|**Provable Benefits of Complex Parameterizations for Structured State Space Models**|Yuval Ran-Milo et.al.|[2410.14067](http://arxiv.org/abs/2410.14067)|null|结构化状态空间模型（SSM）是S4和Mamba等著名神经网络的核心引擎，它们是遵循特定结构（最显著的是对角线结构）的线性动态系统。与参数为实数的典型神经网络模块不同，SSM经常使用复数参数化。理论上解释复数参数化对SSM的好处仍然是一个未解决的问题。本文朝着解决这一问题迈出了一步，通过建立实数和复数对角线SSM之间的正式差距。首先，我们证明了虽然中等维度足以让复数SSM表达所有实数SSM的映射，但需要更高的维度才能让实数SSM表达复数SSM的映射。其次，我们证明了即使实数SSM的维度足够高以表达给定的映射，通常也需要实数SSM的参数持有指数级大的值，这在实践中无法学习。相比之下，复数SSM可以用适度的参数值表达任何给定的映射。实验验证了我们的理论，并暗示了一个可能扩展该理论的方向，即考虑选择性——一种新的架构特性，可以达到最先进的性能。|
|**2024-10-17**|**Quamba: A Post-Training Quantization Recipe for Selective State Space Models**|Hung-Yueh Chiang et.al.|[2410.13229](http://arxiv.org/abs/2410.13229)|null|状态空间模型（SSM）作为大型语言模型的一种有吸引力的替代方案，已经实现了与Transformer相当的精度，并且具有常数内存复杂度，这使得它们能够处理比基于注意力的网络更长的上下文长度。在长序列建模方面，SSM由于其卓越的计算效率而优于Transformer。然而，在请求密集型云服务和资源受限的边缘应用中提高SSM的效率仍然是一个艰巨的任务。SSM量化可能是解决这一问题的方法之一，它使SSM更适合广泛部署，同时保持其准确性。量化是一种常见的技术，用于减少模型大小并利用现代计算单元上的低比特宽度加速特性，但现有的量化技术对SSM并不适用。特别是，SSM在其选择性扫描机制（即线性递归）中的特征图非常敏感，并且输出激活中有大量异常值，这些情况在自注意力模块的令牌混合输出中是不存在的。为了解决这个问题，我们提出了一种静态8位每张量SSM量化方法，该方法通过抑制输入到选择性SSM的激活的最大值来实现更精细的量化精度，并使用Hadamard变换在无异常值的空间中量化输出激活。我们的8位权重-激活量化的Mamba 2.8B SSM受益于硬件加速，在Nvidia Orin Nano 8G上实现了1.72倍更低的生成延迟，而在零样本任务上的平均准确率仅下降了0.9%。实验表明了我们方法的有效性和实用性，适用于在云和边缘平台上部署各种规模的基于SSM的模型。|
|**2024-10-15**|**UmambaTSF: A U-shaped Multi-Scale Long-Term Time Series Forecasting Method Using Mamba**|Li Wu et.al.|[2410.11278](http://arxiv.org/abs/2410.11278)|null|多变量时间序列预测在交通、气象和金融等领域至关重要，尤其是在预测极端天气事件方面。目前最先进的方法主要依赖于Transformer架构，这些架构利用注意力机制来捕捉时间依赖性。然而，这些方法受到二次时间复杂度的限制，这限制了模型随着输入序列长度增加的可扩展性，从而大大限制了它们在实际应用中的实用性。基于状态空间模型（SSM）的Mamba提供了一种具有线性时间复杂度的解决方案，提高了对序列数据进行高效预测的可能性。在这项研究中，我们提出了UmambaTSF，这是一种新颖的长期时间序列预测框架，它将U型编码器-解码器多层感知机（MLP）的多尺度特征提取能力与Mamba的长序列表示相结合。为了提高性能和效率，该框架引入的Mamba模块采用了改进的残差结构和可适应设计，能够捕捉独特的时间信号并灵活处理通道。实验表明，UmambaTSF在广泛使用的基准数据集上实现了最先进的性能和优秀的通用性，同时保持了线性时间复杂度和低内存消耗。|
|**2024-10-14**|**Lambda-Skip Connections: the architectural component that prevents Rank Collapse**|Federico Arangath Joseph et.al.|[2410.10609](http://arxiv.org/abs/2410.10609)|null|最近，序列模型中的嵌入向量快速收敛到一个统一的标记或平衡状态的现象——即所谓的“秩崩溃”，在深度学习文献中引起了广泛关注。这种现象导致了表达能力的降低和由于梯度消失引起的潜在训练不稳定性。实证证据表明，像跳跃连接、LayerNorm和多层感知器（MLPs）这样的架构组件在缓解秩崩溃方面起着关键作用。虽然这个问题在变压器中已有详细记录，但近期受到关注的替代序列模型，如状态空间模型（SSMs），尚未被彻底检查是否存在类似脆弱性。本文通过一个涵盖这两种架构的统一框架，将秩崩溃理论从变压器扩展到了SSMs。我们研究了一种参数化的经典跳跃连接组件，称为lambda-跳跃连接，如何为防止秩崩溃提供保障。通过分析结果，我们提出了一个充分条件来保证防止上述所有架构中的秩崩溃。我们也通过消融研究和分析实例研究了该条件的必要性。据我们所知，这是首次提供一般性保证以防止秩崩溃的研究，并且是在SSMs背景下探讨秩崩溃问题的研究，为理论家和实践者提供了宝贵的理解。最后，我们通过实验验证了我们的发现，展示了像跳跃连接和门控机制这样的架构组件在防止秩崩溃中的关键作用。|
|**2024-10-24**|**The Implicit Bias of Structured State Space Models Can Be Poisoned With Clean Labels**|Yonatan Slutzky et.al.|[2410.10473](http://arxiv.org/abs/2410.10473)|**[link](https://github.com/yonislutzky98/imp-bias-ssm-poison)**|
|**2024-10-14**|**V2M: Visual 2-Dimensional Mamba for Image Representation Learning**|Chengkun Wang et.al.|[2410.10382](http://arxiv.org/abs/2410.10382)|**[link](https://github.com/wangck20/v2m)**|
|**2024-10-14**|**Hi-Mamba: Hierarchical Mamba for Efficient Image Super-Resolution**|Junbo Qiao et.al.|[2410.10140](http://arxiv.org/abs/2410.10140)|null|
|**2024-10-11**|**Parameter-Efficient Fine-Tuning of State Space Models**|Kevin Galim et.al.|[2410.09016](http://arxiv.org/abs/2410.09016)|**[link](https://github.com/furiosa-ai/ssm-peft)**|
|**2024-10-11**|**Drama: Mamba-Enabled Model-Based Reinforcement Learning Is Sample and Parameter Efficient**|Wenlong Wang et.al.|[2410.08893](http://arxiv.org/abs/2410.08893)|**[link](https://github.com/realwenlongwang/drama)**|
|**2024-10-10**|**CountMamba: Exploring Multi-directional Selective State-Space Models for Plant Counting**|Hulingxiao He et.al.|[2410.07528](http://arxiv.org/abs/2410.07528)|null|
|**2024-10-09**|**MatMamba: A Matryoshka State Space Model**|Abhinav Shukla et.al.|[2410.06718](http://arxiv.org/abs/2410.06718)|**[link](https://github.com/scaledfoundations/matmamba)**|
|**2024-10-08**|**TIMBA: Time series Imputation with Bi-directional Mamba Blocks and Diffusion models**|Javier Solís-García et.al.|[2410.05916](http://arxiv.org/abs/2410.05916)|null|
|**2024-10-08**|**Remote Sensing Image Segmentation Using Vision Mamba and Multi-Scale Multi-Frequency Feature Fusion**|Yice Cao et.al.|[2410.05624](http://arxiv.org/abs/2410.05624)|null|
|**2024-10-04**|**PRF: Parallel Resonate and Fire Neuron for Long Sequence Learning in Spiking Neural Networks**|Yulong Huang et.al.|[2410.03530](http://arxiv.org/abs/2410.03530)|null|
|**2024-10-04**|**S7: Selective and Simplified State Space Layers for Sequence Modeling**|Taylan Soydan et.al.|[2410.03464](http://arxiv.org/abs/2410.03464)|null|
|**2024-10-04**|**Demystifying the Token Dynamics of Deep Selective State Space Models**|Thieu N Vo et.al.|[2410.03292](http://arxiv.org/abs/2410.03292)|null|
|**2024-10-04**|**HRVMamba: High-Resolution Visual State Space Model for Dense Prediction**|Hao Zhang et.al.|[2410.03174](http://arxiv.org/abs/2410.03174)|null|

<p align=right>(<a href=#updated-on-20241025>back to top</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[contributors-url]: https://github.com/Vincentqyw/cv-arxiv-daily/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[forks-url]: https://github.com/Vincentqyw/cv-arxiv-daily/network/members
[stars-shield]: https://img.shields.io/github/stars/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[stars-url]: https://github.com/Vincentqyw/cv-arxiv-daily/stargazers
[issues-shield]: https://img.shields.io/github/issues/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[issues-url]: https://github.com/Vincentqyw/cv-arxiv-daily/issues

