[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## Updated on 2024.10.29
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
|**2024-10-25**|**Investigating the Role of Prompting and External Tools in Hallucination Rates of Large Language Models**|Liam Barkley et.al.|[2410.19385](http://arxiv.org/abs/2410.19385)|null|大型语言模型（LLMs）是强大的计算模型，训练于广泛的人类可读文本语料库上，使其能够执行通用的语言理解和生成任务。由于在各种自然语言处理（NLP）任务中的卓越表现，LLMs 在工业界和学术界都受到了极大的关注。尽管如此，LLMs 经常会产生不准确性，通常被称为幻觉。提示工程，即设计和制定指令以使 LLMs 执行特定任务的过程，已成为减少幻觉的关键方法之一。本文对不同的提示策略和框架进行了全面的经验评估，旨在降低 LLMs 的幻觉发生率。通过对一系列基准数据集应用各种提示技术来评估每种方法的准确性和幻觉率。此外，论文还探讨了工具调用代理（通过外部工具增强其能力超出语言生成范围的 LLMs）在同一基准测试中对幻觉率的影响。研究发现表明，最佳的提示技术取决于问题类型，并且较简单的技术往往比更复杂的方法更能有效减少幻觉。此外，结果显示，由于使用外部工具增加了复杂性，LLM 代理可能会表现出显著更高的幻觉率。|
|**2024-10-25**|**Designing LLM-Agents with Personalities: A Psychometric Approach**|Muhua Huang et.al.|[2410.19238](http://arxiv.org/abs/2410.19238)|null|这项研究介绍了一种新颖的方法，使用大五人格框架为基于大型语言模型的代理（Agents）分配可量化、可控且经过心理测量验证的人格特质。它旨在克服人类主体研究的限制，提出将Agents作为社会科学研究的一种便捷工具。通过四个系列的研究，本研究展示了向Agents分配心理测量有效的人格特质的可行性，使它们能够复制复杂的人类行为。第一个研究在大型语言模型的语义空间内建立了对人格结构和人格测试的理解。接下来的两个研究——分别使用实证数据和模拟数据——展示了创建Agents的过程，并通过展示人类与Agents在人格测试答案上的高度一致性来验证结果。最后一项研究进一步证实了这种一致性，即通过让Agents再现已知的人格特质与决策行为之间的关联，特别是在涉及风险承担和道德困境的情境中，从而验证了使用心理测量方法设计Agents的有效性及其在社会和行为研究中的应用性。|
|**2024-10-25**|**An LLM Agent for Automatic Geospatial Data Analysis**|Yuxing Chen et.al.|[2410.18792](http://arxiv.org/abs/2410.18792)|null|大型语言模型（LLM）在数据科学代码生成任务中得到应用，但在处理复杂的顺序任务时常常遇到逻辑错误。由于难以整合复杂的数据结构和空间约束、有效利用多样的函数调用以及倾向于使用较少使用的地理空间库，LLM在地理空间数据处理中的应用尤为具有挑战性。为了解决这些问题，我们引入了GeoAgent，这是一个新的交互式框架，旨在帮助LLM更有效地处理地理空间数据。GeoAgent首次将代码解释器、静态分析和检索增强生成（RAG）技术与蒙特卡洛树搜索（MCTS）算法相结合，为地理空间数据处理提供了一种新颖的方法。此外，我们还贡献了一个专门设计用于评估基于LLM方法在地理空间任务中的新基准。该基准利用了多种Python库，包括单轮和多轮任务，如数据获取、数据分析和可视化。通过在多样化的地理空间环境中进行全面评估，这一基准为开发基于LLM的地理空间数据分析方法设定了新的标准。我们的研究结果表明，仅依赖LLM的知识不足以准确完成地理空间任务编程，这需要连贯的多步骤过程和多次函数调用。与基线LLM相比，所提出的GeoAgent表现出色，在函数调用和任务完成方面取得了显著改进。此外，这些结果为未来基于LLM代理的自动地理空间数据分析任务编程的发展提供了宝贵见解。|
|**2024-10-24**|**PRACT: Optimizing Principled Reasoning and Acting of LLM Agent**|Zhiwei Liu et.al.|[2410.18528](http://arxiv.org/abs/2410.18528)|null|我们提出了一种新的从轨迹数据中学习和执行动作原则的方法——有原则的推理与行动（PRAct）框架。我们的方法核心是利用来自反思和优化引擎的文本梯度来推导这些动作原则。为了使动作原则适应特定任务需求，我们提出了一种新的优化框架——反思性原则优化（RPO）。在执行后，RPO使用一个反思器来批判当前的动作原则，并使用一个优化器相应地更新这些原则。我们在两种场景下开发了RPO框架：Reward-RPO，它使用环境奖励进行反思；Self-RPO，它在没有外部奖励的情况下进行自我反思。此外，还介绍了两种RPO方法，RPO-Traj 和 RPO-Batch，以适应不同的设置。在四个环境中的实验结果表明，利用RPO框架的PRAct代理能够有效地学习并应用动作原则来提高性能。|
|**2024-10-23**|**GraphTeam: Facilitating Large Language Model-based Graph Analysis via Multi-Agent Collaboration**|Xin Li et.al.|[2410.18032](http://arxiv.org/abs/2410.18032)|**[link](https://github.com/bupt-gamma/graphteam)**|**图在现实世界场景中被广泛用于建模关系数据，例如社交网络和城市计算。现有的基于大语言模型（LLM）的图分析方法要么将图神经网络（GNNs）集成到特定的机器学习任务中，限制了它们的可迁移性；要么仅仅依赖于LLM的内部推理能力，导致性能不佳。为了解决这些局限性，我们利用了最近在基于LLM的代理方面的进展，这些代理已经展示了利用外部知识或工具解决问题的能力。通过模拟人类的问题解决策略，如类比和协作，我们提出了一种基于LLM的多代理系统GraphTeam，用于图分析。GraphTeam由来自三个模块的五个基于LLM的代理组成，具有不同专长的代理可以相互协作以解决复杂问题。具体来说，(1) 输入-输出规范化模块：问题代理从原始问题中提取并精炼四个关键参数，促进问题理解，而答案代理则组织结果以满足输出要求；(2) 外部知识检索模块：我们首先构建了一个包含相关文档和经验信息的知识库，然后搜索代理为每个问题检索最相关的条目。(3) 问题解决模块：给定从搜索代理检索到的信息，编码代理使用既定算法通过编程生成解决方案；如果编码代理不起作用，则推理代理将直接计算结果而不进行编程。在六个图分析基准上的大量实验表明，GraphTeam实现了最先进的性能，在准确性方面平均提高了25.85%。代码和数据可在https://github.com/BUPT-GAMMA/GraphTeam获取。**|
|**2024-10-25**|**MiniFed : Integrating LLM-based Agentic-Workflow for Simulating FOMC Meeting**|Sungil Seok et.al.|[2410.18012](http://arxiv.org/abs/2410.18012)|null|在美国，联邦基金利率对国内外金融市场都起着重要作用。然而，研究主要集中在联邦基金利率调整的影响上，而不是决策过程本身。最近在大型语言模型（LLM）方面的进展为重建负责设定联邦基金利率的FOMC会议提供了一种潜在的方法。在本文中，我们提出了一个五阶段的FOMC会议模拟框架MiniFed，该框架利用LLM代理来模拟现实世界中的FOMC会议成员，并优化FOMC结构。这一框架有效地使FOMC会议过程焕发生机，并促进了联邦基金利率的预测。实验结果表明，我们提出的MiniFed框架不仅在联邦基金利率预测方面达到了高精度，而且其行为与现实世界中的对应者一致。鉴于很少有研究关注使用LLM代理来模拟大规模现实世界的会议，我们的工作可以作为未来发展的基准。|
|**2024-10-22**|**SELA: Tree-Search Enhanced LLM Agents for Automated Machine Learning**|Yizhou Chi et.al.|[2410.17238](http://arxiv.org/abs/2410.17238)|**[link](https://github.com/geekan/metagpt)**|**自动化机器学习（AutoML）方法包括优化固定模型选择和集成管道的传统方法，以及能够自主构建管道的新型基于大语言模型（LLM）的框架。虽然基于LLM的代理在自动化机器学习任务中显示出潜力，但它们通常生成的代码多样性低且次优，即使经过多次迭代也是如此。为克服这些限制，我们引入了一种树搜索增强的LLM代理（SELA），这是一种创新的基于代理的系统，利用蒙特卡洛树搜索（MCTS）来优化AutoML过程。通过将管道配置表示为树，我们的框架使代理能够智能地进行实验，并迭代改进其策略，从而更有效地探索机器学习解决方案空间。这种方法使得SELA能够根据实验反馈发现最优路径，提高解决方案的整体质量。通过对20个机器学习数据集的广泛评估，我们将传统和基于代理的AutoML方法进行了比较，结果表明SELA在所有数据集中对每个基线的胜率达到了65%到80%。这些结果突显了基于代理策略在AutoML中的巨大潜力，为解决复杂的机器学习挑战提供了新的视角。**|
|**2024-10-22**|**EnvBridge: Bridging Diverse Environments with Cross-Environment Knowledge Transfer for Embodied AI**|Tomoyuki Kagaya et.al.|[2410.16919](http://arxiv.org/abs/2410.16919)|null|近年来，大型语言模型（LLM）展示了高度的推理能力，因其在各种决策过程中的应用而备受关注。其中一个特别有前景的应用是机器人操作。最近的研究表明，LLM可以为机器人生成文本规划或控制代码，提供了极大的灵活性和交互能力。然而，这些方法在不同环境下的灵活性和适用性方面仍然面临挑战，限制了它们自主适应的能力。目前的方法通常分为两类：一类依赖于特定环境的策略训练，这限制了它们的可迁移性；另一类基于固定提示生成代码动作，当面对新环境时性能会下降。这些局限性显著限制了代理在机器人操作中的通用性。为了解决这些局限性，我们提出了一种名为EnvBridge的新方法。该方法涉及从源环境到目标环境的成功机器人控制代码的保留和转移。通过利用多个环境的见解，EnvBridge提高了代理在不同设置下的适应性和性能。值得注意的是，我们的方法缓解了环境约束，为机器人操作任务提供了一个更加灵活和通用的解决方案。我们使用机器人操作基准RLBench、MetaWorld和CALVIN验证了方法的有效性。实验表明，LLM代理可以成功地利用多样化的知识来源解决复杂任务。因此，我们的方法显著增强了机器人操作代理在跨不同环境规划中的适应性和鲁棒性。|
|**2024-10-22**|**CoPS: Empowering LLM Agents with Provable Cross-Task Experience Sharing**|Chen Yang et.al.|[2410.16670](http://arxiv.org/abs/2410.16670)|**[link](https://github.com/uclaml/cops)**|**在代理系统中，大型语言模型（LLMs）显著推进了序列推理的发展，但现有方法仍存在局限性。反思驱动的推理仅依赖于预训练模型中的知识，在新场景下的表现受限；而经验辅助的推理通常依赖外部经验，并且缺乏选择代表性经验的明确原则。为解决这些局限，我们提出了CoPS（跨任务经验共享），这是一种通用算法，通过跨任务的经验共享和选择来增强序列推理能力。具体来说，CoPS利用代理在先前任务上的经验，采用一种基于悲观策略的可证明方法选择分布匹配的经验，以最大化效用同时最小化由分布偏移带来的风险。在Alfworld、Webshop和HotPotQA等基准测试上进行的广泛实验表明，CoPS始终优于最先进的基线方法，具有更高的样本效率，适用于资源受限的情景。理论上，我们展示了该算法的性能取决于预训练LLM的质量以及代理的任务相关尝试分布与LLM生成的分布之间的匹配程度。我们的工作填补了现有序列推理范式之间的空白，验证了利用跨任务经验的有效性，揭示了提高代理在多样化任务中泛化能力和适应性的潜力。我们的代码可在\href{https://github.com/uclaml/COPS}{https://github.com/uclaml/COPS}获取。**|
|**2024-10-22**|**Adsorb-Agent: Autonomous Identification of Stable Adsorption Configurations via Large Language Model Agent**|Janghoon Ock et.al.|[2410.16658](http://arxiv.org/abs/2410.16658)|null|吸附能在催化中是一个关键的反应性描述符，能够有效地筛选潜在的催化剂。然而，确定吸附能需要比较多种吸附物-催化剂构型的能量，由于可能的构型数量庞大，因此计算上非常耗时。目前的算法方法通常通过枚举吸附位点和构型来实现，而没有充分利用理论见解来指导初始设置。在本工作中，我们提出了Adsorb-Agent，这是一种大型语言模型（LLM）代理，旨在以最少的人工干预高效地推导出特定系统的稳定吸附构型。Adsorb-Agent利用内置的知识和涌现的推理能力，显著减少了所需的初始构型数量，同时提高了预测最低吸附能的准确性。我们使用两个示例系统NNH-CuPd3 (111) 和 NNH-Mo3Pd (111) 来进行氮还原反应（NRR），这是哈柏-波施过程的一种可持续替代方案，展示了其性能。与传统的“启发式”和“随机”算法相比，Adsorb-Agent能够以更少的初始设置识别出更低能量的构型，从而降低了计算成本并提高了准确性。这突显了其在加速催化剂发现方面的潜力。|
|**2024-10-23**|**IBGP: Imperfect Byzantine Generals Problem for Zero-Shot Robustness in Communicative Multi-Agent Systems**|Yihuan Mao et.al.|[2410.16237](http://arxiv.org/abs/2410.16237)|null|
|**2024-10-21**|**NetSafe: Exploring the Topological Safety of Multi-agent Networks**|Miao Yu et.al.|[2410.15686](http://arxiv.org/abs/2410.15686)|null|
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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

## llm

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-25**|**Counting Ability of Large Language Models and Impact of Tokenization**|Xiang Zhang et.al.|[2410.19730](http://arxiv.org/abs/2410.19730)|null|Transformer作为现代大型语言模型（LLM）的基石，面临固有的架构限制，这些限制阻碍了它们的推理能力。与循环网络不同，Transformer缺乏循环连接，导致它们只能进行恒定深度的计算。这一限制使它们处于复杂性类TC $^0$ 中，理论上无法解决需要随着输入长度增加而不断增加推理深度的任务。计数是许多推理任务的基本组成部分，也需要推理深度线性增长才能进行归纳。尽管先前的研究已经确定了基于Transformer的专业模型（即专门训练用于计数任务的模型）的计数能力上限，但这些发现并不能直接扩展到通用LLM，因为两者的推理机制存在差异。最近的工作强调了Chain of Thought（CoT）推理如何帮助缓解Transformer在计数任务中的某些架构限制。然而，很少有研究关注分词在这些模型中的作用。与通常使用字符级分词的专业模型不同，LLM通常依赖于字节级（BPE）分词器，这从根本上改变了推理处理的方式。我们的工作研究了分词对LLM计数能力的影响，揭示了由于输入分词差异导致的显著性能变化。我们提供了理论和实验分析，为分词选择如何影响模型的理论可计算性提供了见解，从而启发设计新的分词方法以增强LLM的推理能力。|
|**2024-10-25**|**FISHNET: Financial Intelligence from Sub-querying, Harmonizing, Neural-Conditioning, Expert Swarms, and Task Planning**|Nicole Cho et.al.|[2410.19727](http://arxiv.org/abs/2410.19727)|null|从大量数据源生成金融情报通常依赖于传统的知识图谱构建或数据库工程技术。最近，出现了针对金融领域的微调大型语言模型（LLMs）。虽然这些进展很有前景，但仍然存在一些限制，比如高昂的推理成本、幻觉现象以及同时分析高维金融数据的复杂性。这促使我们发明了FISHNET（基于子查询、协调、神经条件、专家群集和任务规划的金融情报生成），这是一种代理架构，能够完成对超过98,000份监管文件的高度复杂的分析任务，这些文件在语义、数据层次结构或格式上差异极大。FISHNET在生成金融洞察方面表现出色（成功率为61.8%，路由为5.0%，RAG R-Precision为45.6%）。我们进行了严格的消融实验，以实证证明FISHNET的成功、每个代理的重要性以及所有代理组合后的优化性能。我们的模块化架构可以应用于多种用途，提供对于金融任务至关重要的可扩展性、灵活性和数据完整性。|
|**2024-10-25**|**2D-DPO: Scaling Direct Preference Optimization with 2-Dimensional Supervision**|Shilong Li et.al.|[2410.19720](http://arxiv.org/abs/2410.19720)|null|最近，直接偏好优化（DPO）的进展显著提高了大型语言模型（LLMs）与人类偏好的一致性，这得益于其简单性和有效性。然而，现有的方法通常只优化一个标量分数或排名奖励，从而忽略了人类偏好的多维性质。在这项工作中，我们提出将DPO的偏好扩展到两个维度：段落和方面。我们首先引入了一个名为HelpSteer-2D的二维监督数据集。对于段落维度，我们将回复分成句子，并为每个段落分配分数。对于方面维度，我们精心设计了几个标准，涵盖了回复质量的各个方面。利用二维信号作为反馈，我们开发了一个2D-DPO框架，将整体目标分解为多段落和多方面的目标。在流行基准上的大量实验表明，2D-DPO的表现优于那些仅优化标量或一维偏好的方法。|
|**2024-10-25**|**Less is More: Extreme Gradient Boost Rank-1 Adaption for Efficient Finetuning of LLMs**|Yifei Zhang et.al.|[2410.19694](http://arxiv.org/abs/2410.19694)|null|微调大型语言模型（LLMs）已成为将预训练模型适应下游任务的关键技术。然而，LLMs的巨大规模在计算复杂性和资源需求方面带来了重大挑战。低秩适应（LoRA）作为一种有前景的解决方案应运而生。但是，在低秩适应的实际性能与其理论最优值之间存在差距。在这项工作中，我们提出了极端梯度提升LoRA（XGBLoRA），这是一种新颖的框架，通过利用集成学习的力量来弥合这一差距。受到梯度提升的启发，XGBLoRA迭代地学习并合并一系列LoRA适应以优化模型预测。它比标准LoRA表现更好，同时享受了秩-1适应的计算效率。我们提供了理论分析以展示方法的收敛性和最优性，并在一系列自然语言处理任务上进行了广泛的实验。结果表明，XGBLoRA始终优于标准LoRA，并且在显著减少可训练参数数量的情况下达到了与完全微调相当的性能。这项工作推进了LLMs的参数高效微调，并为在优化性能和效率的同时将LLMs适应到下游任务提供了一个有前景的解决方案。|
|**2024-10-25**|**APRICOT: Active Preference Learning and Constraint-Aware Task Planning with LLMs**|Huaxiaoyue Wang et.al.|[2410.19656](http://arxiv.org/abs/2410.19656)|null|家庭机器人在执行个性化任务时必须巧妙地平衡用户偏好与环境条件。我们专注于在有限空间内进行组织任务，例如将物品放入冰箱中，在这种情况下，放置偏好可能会与物理限制产生冲突。机器人需要根据少量的演示来推断用户的偏好，这比让用户详尽地定义所有需求要容易得多。尽管最近的一些研究使用大型语言模型（LLM）从用户演示中学习偏好，但它们遇到了两个基本挑战。首先，在解释用户行为时存在固有的模糊性，因为多种偏好往往可以解释同一观察到的行为。其次，并非所有的用户偏好都能因环境中的几何限制而实际可行。为了解决这些挑战，我们提出了APRICOT，这是一种新颖的方法，它结合了基于LLM的贝叶斯主动偏好学习与约束感知的任务规划。APRICOT通过积极向用户查询来细化其生成的偏好，并动态调整计划以尊重环境约束。我们在一个多样化的组织任务数据集上对APRICOT进行了评估，并在真实场景中展示了其有效性，表明在偏好满足度和计划可行性方面都有显著提升。项目网站位于https://portal-cornell.github.io/apricot/|
|**2024-10-25**|**Take Caution in Using LLMs as Human Surrogates: Scylla Ex Machina**|Yuan Gao et.al.|[2410.19599](http://arxiv.org/abs/2410.19599)|null|最近的研究表明，大型语言模型（LLMs）可以表现出类似人类的推理能力，在经济实验、调查和政治讨论中与人类行为保持一致。这导致许多人提出可以将LLMs作为社会科学研究所用的人类替代品。然而，LLMs在本质上与人类不同，它们依赖于概率模式，缺乏塑造人类认知的身体体验或生存目标。我们通过11-20金钱请求游戏来评估LLMs的推理深度。除了在一个使用大量人类行为数据进行微调的情况下外，几乎所有高级方法都无法在许多模型中复制人类行为分布。失败的原因多种多样，涉及到输入语言、角色和保护机制等问题。这些结果告诫人们不要使用LLMs来研究人类行为或将它们作为人类的替代品。|
|**2024-10-25**|**Diverse Sign Language Translation**|Xin Shen et.al.|[2410.19586](http://arxiv.org/abs/2410.19586)|null|像口语一样，单一的手语表达可能对应多种有效的文本解释。因此，对于手语翻译（SLT）模型来说，学习一个严格的一对一映射可能是不够的，特别是在数据有限的情况下。在这项工作中，我们引入了一个多样化的手语翻译（DivSLT）任务，旨在为手语视频生成多样化且准确的翻译。首先，我们利用大型语言模型（LLM）为广泛使用的CSL-Daily和PHOENIX14T SLT数据集生成多个参考译文。这里，仅邀请母语使用者修正不准确的参考译文，从而显著提高了标注效率。其次，我们提供了一个基准模型以促进该领域的研究。具体而言，我们探讨了多参考训练策略，使我们的DivSLT模型能够实现多样化的翻译。然后，为了提高翻译准确性，我们采用了最大化奖励驱动的强化学习目标，以最大化翻译结果的奖励。此外，我们使用多种指标来评估DivSLT任务的准确性、多样性和语义精确度。在丰富后的数据集上的实验结果表明，我们的DivSLT方法不仅实现了更好的翻译性能，而且还产生了多样化的翻译结果。|
|**2024-10-25**|**ChunkRAG: Novel LLM-Chunk Filtering Method for RAG Systems**|Ritvik Aggarwal Ishneet Sukhvinder Singh Ibrahim Allahverdiyev et.al.|[2410.19572](http://arxiv.org/abs/2410.19572)|null|使用大型语言模型（LLM）的检索增强生成（RAG）系统由于检索到不相关或关联较弱的信息，常常生成不准确的回答。现有的方法在文档级别操作，无法有效过滤掉这些内容。我们提出了基于LLM的块过滤方法ChunkRAG，该框架通过在块级别评估和过滤检索到的信息来增强RAG系统。我们的方法采用语义分块技术将文档分割成连贯的部分，并利用基于LLM的相关性评分来评估每个块与用户查询的一致性。通过在生成阶段之前过滤掉不太相关的块，我们显著减少了幻觉并提高了事实准确性。实验表明，我们的方法在需要精确信息检索的任务上比现有RAG模型表现更好。这一进步提高了RAG系统的可靠性，特别适用于事实核查和多跳推理等应用。|
|**2024-10-25**|**Brain-like Functional Organization within Large Language Models**|H. Sun et.al.|[2410.19542](http://arxiv.org/abs/2410.19542)|null|人脑长期以来一直启发着对人工智能（AI）的追求。最近，神经影像学研究提供了有力证据，表明人工神经网络（ANNs）的计算表征与人类大脑对刺激的神经反应之间存在一致性，这表明ANNs可能采用了类似大脑的信息处理策略。虽然这种一致性在视觉、听觉和语言等感觉模式中都有观察到，但大部分关注点集中在人工神经元（ANs）群体层面的行为上，而个体ANs的功能组织如何促进这种类似大脑的过程则很大程度上未被探索。在这项研究中，我们通过直接将人工神经元子群与功能脑网络（FBNs）——即人脑的基础组织结构——相耦合，来填补这一空白。具体来说，我们从大型语言模型（LLMs）中的人工神经元的时间响应中提取代表性模式，并将其作为固定回归因子构建体素级别的编码模型，以预测功能性磁共振成像（fMRI）记录的大脑活动。该框架将人工神经元子群与FBNs联系起来，使得能够在LLMs中描绘出类似大脑的功能组织。我们的发现揭示了LLMs（BERT和Llama 1-3）展现出类似大脑的功能架构，其中人工神经元子群反映了已建立的功能脑网络的组织模式。值得注意的是，随着复杂性和能力的提高，LLMs的类脑功能组织不断发展，实现了计算行为多样性和功能特化一致性之间的更好平衡。这项研究代表了首次探索LLMs中的类脑功能组织，为基于人脑原理开发人工通用智能（AGI）提供了新的见解。|
|**2024-10-25**|**Detection of Human and Machine-Authored Fake News in Urdu**|Muhammad Zain Ali et.al.|[2410.19517](http://arxiv.org/abs/2410.19517)|null|社交媒体的兴起放大了假新闻的传播，现在由于像ChatGPT这样的大型语言模型（LLMs）能够生成高度可信且无错误的误导信息，使得公众越来越难以区分真假。传统的依赖语言线索的假新闻检测方法变得不那么有效。此外，目前的检测器主要集中在二元分类和英文文本上，往往忽略了机器生成的真实与虚假新闻之间的区别以及在资源较少的语言中的检测问题。为此，我们更新了检测方案，将重点放在机器生成的新闻上，并特别关注乌尔都语。我们进一步提出了一种层次化的检测策略，以提高准确性和鲁棒性。实验表明，该方法在四种不同设置下的四个数据集上均表现出有效性。|
|**2024-10-24**|**Unbounded: A Generative Infinite Game of Character Life Simulation**|Jialu Li et.al.|[2410.18975](http://arxiv.org/abs/2410.18975)|null|
|**2024-10-24**|**Does Data Contamination Detection Work (Well) for LLMs? A Survey and Evaluation on Detection Assumptions**|Yujuan Fu et.al.|[2410.18966](http://arxiv.org/abs/2410.18966)|null|
|**2024-10-24**|**OSCAR: Operating System Control via State-Aware Reasoning and Re-Planning**|Xiaoqiang Wang et.al.|[2410.18963](http://arxiv.org/abs/2410.18963)|null|
|**2024-10-24**|**Bridge-Coder: Unlocking LLMs' Potential to Overcome Language Gaps in Low-Resource Code**|Jipeng Zhang et.al.|[2410.18957](http://arxiv.org/abs/2410.18957)|null|
|**2024-10-24**|**BioMistral-NLU: Towards More Generalizable Medical Language Understanding through Instruction Tuning**|Yujuan Velvin Fu et.al.|[2410.18955](http://arxiv.org/abs/2410.18955)|null|
|**2024-10-24**|**Dynamic Vocabulary Pruning in Early-Exit LLMs**|Jort Vincenti et.al.|[2410.18952](http://arxiv.org/abs/2410.18952)|**[link](https://github.com/matteonulli/vocabulary_pruning)**|
|**2024-10-24**|**From Blind Solvers to Logical Thinkers: Benchmarking LLMs' Logical Integrity on Faulty Mathematical Problems**|A M Muntasir Rahman et.al.|[2410.18921](http://arxiv.org/abs/2410.18921)|null|
|**2024-10-25**|**A Survey on Speech Large Language Models**|Jing Peng et.al.|[2410.18908](http://arxiv.org/abs/2410.18908)|null|
|**2024-10-24**|**PRISM: A Methodology for Auditing Biases in Large Language Models**|Leif Azzopardi et.al.|[2410.18906](http://arxiv.org/abs/2410.18906)|**[link](https://github.com/cis-phawm/prism)**|
|**2024-10-24**|**LLMs for Extremely Low-Resource Finno-Ugric Languages**|Taido Purason et.al.|[2410.18902](http://arxiv.org/abs/2410.18902)|null|
|**2024-10-23**|**LongRAG: A Dual-Perspective Retrieval-Augmented Generation Paradigm for Long-Context Question Answering**|Qingfei Zhao et.al.|[2410.18050](http://arxiv.org/abs/2410.18050)|**[link](https://github.com/qingfei1/longrag)**|
|**2024-10-23**|**Key Algorithms for Keyphrase Generation: Instruction-Based LLMs for Russian Scientific Keyphrases**|Anna Glazkova et.al.|[2410.18040](http://arxiv.org/abs/2410.18040)|null|
|**2024-10-23**|**MiniFed : Integrating LLM-based Agentic-Workflow for Simulating FOMC Meeting**|Sungil Seok et.al.|[2410.18012](http://arxiv.org/abs/2410.18012)|null|
|**2024-10-23**|**ExpertFlow: Optimized Expert Activation and Token Allocation for Efficient Mixture-of-Experts Inference**|Xin He et.al.|[2410.17954](http://arxiv.org/abs/2410.17954)|null|
|**2024-10-23**|**SimRAG: Self-Improving Retrieval-Augmented Generation for Adapting Large Language Models to Specialized Domains**|Ran Xu et.al.|[2410.17952](http://arxiv.org/abs/2410.17952)|null|
|**2024-10-23**|**Benchmarking Floworks against OpenAI & Anthropic: A Novel Framework for Enhanced LLM Function Calling**|Nirav Bhan et.al.|[2410.17950](http://arxiv.org/abs/2410.17950)|null|
|**2024-10-23**|**Guide for Defense (G4D): Dynamic Guidance for Robust and Balanced Defense in Large Language Models**|He Cao et.al.|[2410.17922](http://arxiv.org/abs/2410.17922)|**[link](https://github.com/idea-xl/g4d)**|
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
|**2024-10-22**|**Towards Automated Penetration Testing: Introducing LLM Benchmark, Analysis, and Improvements**|Isamu Isozaki et.al.|[2410.17141](http://arxiv.org/abs/2410.17141)|**[link](https://github.com/isamu-isozaki/AI-Pentest-Benchmark)**|
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
|**2024-09-16**|**LLM as BT-Planner: Leveraging LLMs for Behavior Tree Generation in Robot Task Planning**|Jicong Ao et.al.|[2409.10444](http://arxiv.org/abs/2409.10444)|**[link](https://github.com/proneverfake/kios)**|
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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

## Communication Intelligence

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-09-21**|**LLM Agents as 6G Orchestrator: A Paradigm for Task-Oriented Physical-Layer Automation**|Zhuoran Xiao et.al.|[2410.03688](http://arxiv.org/abs/2410.03688)|null|生成式预训练模型的快速发展正在推动技术进步从基础应用如聊天机器人向更复杂的基于代理的系统转变。将6G系统与大型语言模型（LLM）代理和数字孪生（DT）相结合，具有巨大的潜力和必要性，以管理具备新兴特性（如原生AI服务和感知功能）的高度复杂通信系统。通过6G导向的代理，基站能够理解各种动态上层任务的传输需求，自动编排最优系统工作流程。通过对6G DT持续反馈进行强化学习，代理最终可以相应地提高实际系统的性能。不同于现有的为通用应用设计的LLM代理，6G导向的代理旨在利用大量的额外专业知识进行高度严谨和精确的规划，这不可避免地需要从模型训练到实现的特定系统设计。本文提出了一种构建面向任务的6G LLM代理的新综合方法。我们首先提出了一种两阶段连续预训练和微调方案，用于构建领域基础模型及满足各种应用场景需求的多种专业化专家模型。此外，还提出了一种基于语义检索的新推理框架，以利用现有的通信相关功能。实验结果，如物理层任务分解等示例任务，表明了所提范式的可行性和有效性。|
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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

## RAG

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-25**|**FISHNET: Financial Intelligence from Sub-querying, Harmonizing, Neural-Conditioning, Expert Swarms, and Task Planning**|Nicole Cho et.al.|[2410.19727](http://arxiv.org/abs/2410.19727)|null|从大量数据源生成金融情报通常依赖于传统的知识图谱构建或数据库工程方法。最近，出现了针对金融领域的微调大型语言模型（LLM）。虽然这些进展很有前景，但仍然存在一些限制，如高昂的推理成本、幻觉现象以及同时分析高维金融数据的复杂性。这促使我们发明了FISHNET（Financial Intelligence from Sub-querying, Harmonizing, Neural-Conditioning, Expert swarming, and Task planning），这是一种代理架构，能够完成对超过98,000份监管文件的高度复杂的分析任务，这些文件在语义、数据层次结构和格式方面差异极大。FISHNET在金融洞察生成方面表现出色（成功率为61.8%，路由为5.0%，RAG R-Precision为45.6%）。我们进行了严格的消融实验，以实证证明FISHNET的成功、每个代理的重要性以及组装所有代理后的优化性能。我们的模块化架构可以应用于多种用途，提供对于金融任务至关重要的可扩展性、灵活性和数据完整性。|
|**2024-10-25**|**ChunkRAG: Novel LLM-Chunk Filtering Method for RAG Systems**|Ritvik Aggarwal Ishneet Sukhvinder Singh Ibrahim Allahverdiyev et.al.|[2410.19572](http://arxiv.org/abs/2410.19572)|null|使用大型语言模型（LLMs）的检索增强生成（RAG）系统由于检索到不相关或关联松散的信息，常常会生成不准确的回答。现有的方法在文档级别操作，无法有效过滤这些内容。我们提出了一个基于LLM的块过滤框架ChunkRAG，通过在块级别评估和过滤检索到的信息来增强RAG系统。我们的方法采用语义分块将文档分割成连贯的部分，并利用基于LLM的相关性评分来评估每个块与用户查询的一致性。通过在生成阶段前过滤掉不太相关的块，我们显著减少了幻觉现象并提高了事实准确性。实验表明，我们的方法优于现有的RAG模型，在需要精确信息检索的任务中达到了更高的准确性。这一进步提高了RAG系统的可靠性，使其特别适用于诸如事实核查和多跳推理等应用。|
|**2024-10-24**|**PDL: A Declarative Prompt Programming Language**|Mandana Vaziri et.al.|[2410.19135](http://arxiv.org/abs/2410.19135)|null|大型语言模型（LLM）通过使许多以前难以实现的人工智能应用变得可行，已经在全球范围内引起了轰动。LLM 通过高度表达性的文本提示进行控制，并返回文本答案。不幸的是，这种非结构化的文本输入和输出使得基于 LLM 的应用程序变得脆弱。这促使了提示框架的兴起，这些框架在 LLM 和外部世界之间起到中介作用。然而，现有的提示框架要么学习曲线很高，要么从开发者手中夺走了对确切提示的控制权。为了解决这一困境，本文介绍了提示声明语言（PDL）。PDL 是一种简单的声明性数据导向语言，以 YAML 为基础，将提示放在首位。PDL 与许多 LLM 平台和 LLM 兼容。它支持编写调用 LLM 和工具的交互式应用程序，并且易于实现聊天机器人、RAG 或代理等常见用例。我们希望 PDL 能够使提示编程变得更简单、更稳定且更加愉快。|
|**2024-10-24**|**LoRANN: Low-Rank Matrix Factorization for Approximate Nearest Neighbor Search**|Elias Jääsaari et.al.|[2410.18926](http://arxiv.org/abs/2410.18926)|**[link](https://github.com/ejaasaari/lorann)**|**近似最近邻（ANN）搜索是许多现代机器学习流水线中的关键组件；最近的用例包括检索增强生成（RAG）和向量数据库。基于聚类的ANN算法，使用基于乘积量化（PQ）的评分计算方法，由于其可扩展性和适用于分布式及磁盘实现的特点，在工业规模应用中经常被使用。然而，它们的查询时间比领先的基于图的ANN算法更慢。在这项工作中，我们提出了一种新的监督评分计算方法，该方法基于内积近似是一个可以由降秩回归有效解决的多元（多输出）回归问题这一观察。我们的实验表明，在现代高维数据集上，所提出的降秩回归（RRR）方法在查询延迟和内存使用方面都优于PQ。我们还介绍了LoRANN，一个利用所提出的评分计算方法的基于聚类的ANN库。LoRANN与领先的基于图的算法具有竞争力，并且在高维数据集上超越了最先进的GPU ANN方法。**|
|**2024-10-25**|**An LLM Agent for Automatic Geospatial Data Analysis**|Yuxing Chen et.al.|[2410.18792](http://arxiv.org/abs/2410.18792)|null|大型语言模型（LLM）正在被用于数据科学代码生成任务中，但它们在处理复杂的顺序任务时常常遇到困难，导致逻辑错误。将这些模型应用于地理空间数据处理尤其具有挑战性，因为难以整合复杂的数据结构和空间约束、有效利用多种函数调用，并且倾向于幻想较少使用的地理空间库。为了解决这些问题，我们引入了GeoAgent，这是一个新的交互式框架，旨在帮助LLM更有效地处理地理空间数据处理。GeoAgent开创性地在一个蒙特卡洛树搜索（MCTS）算法中集成了代码解释器、静态分析和检索增强生成（RAG）技术，为地理空间数据处理提供了一种新方法。此外，我们还贡献了一个新的基准测试，专门设计用于评估基于LLM的方法在地理空间任务中的表现。该基准测试利用了多种Python库，包括单轮和多轮任务，如数据获取、数据分析和可视化。通过在多样化的地理空间环境中进行全面评估，这个基准测试为开发基于LLM的地理空间数据分析任务设定了新标准。我们的研究结果表明，仅依赖LLM的知识不足以准确完成地理空间任务编程，这需要连贯的多步骤过程和多次函数调用。与基线LLM相比，所提出的GeoAgent展示了优越的性能，在函数调用和任务完成方面取得了显著改进。此外，这些结果为未来开发自动地理空间数据分析任务编程的LLM代理提供了宝贵的见解。|
|**2024-10-24**|**Bielik 7B v0.1: A Polish Language Model -- Development, Insights, and Evaluation**|Krzysztof Ociepa et.al.|[2410.18565](http://arxiv.org/abs/2410.18565)|null|我们介绍了Bielik 7B v0.1，这是一个拥有70亿参数的生成式文本模型，专门用于波兰语语言处理。该模型在精选的波兰语语料库上进行训练，通过创新技术解决了语言模型开发中的关键挑战。这些技术包括加权指令交叉熵损失，它平衡了不同类型指令的学习，以及自适应学习率，它根据训练进度动态调整学习率。为了评估性能，我们创建了Open PL LLM排行榜和波兰MT-Bench，这两个新框架可以评估各种自然语言处理任务和对话能力。Bielik 7B v0.1展示了显著的改进，在RAG阅读任务中比Mistral-7B-v0.1平均得分提高了9个百分点。它还在波兰MT-Bench中表现出色，特别是在推理（6.15/10）和角色扮演（7.83/10）类别中。该模型代表了波兰语人工智能的重大进步，为多种语言应用提供了强大的工具，并在该领域设定了新的基准。|
|**2024-10-24**|**Aggregated Knowledge Model: Enhancing Domain-Specific QA with Fine-Tuned and Retrieval-Augmented Generation Models**|Fengchen Liu et.al.|[2410.18344](http://arxiv.org/abs/2410.18344)|null|本文介绍了一种增强封闭领域问答系统（QA）的新方法，重点关注劳伦斯伯克利国家实验室（LBL）科学信息技术（ScienceIT）领域的特定需求。利用从ScienceIT文档中提取的丰富数据集，我们的研究对两个微调的大规模语言模型和五个检索增强生成（RAG）模型进行了详细的比较。通过数据处理技术，我们将文档转换为结构化的上下文-问题-答案三元组，并利用最新的大规模语言模型（AWS Bedrock、GCP PaLM2、Meta LLaMA2、OpenAI GPT-4、Google Gemini-Pro）进行数据驱动的洞察。此外，我们引入了聚合知识模型（AKM），该模型通过K-means聚类选择最具代表性的答案来综合上述七个模型的响应。通过对这些模型在多个指标上的评估，全面展示了它们在LBL ScienceIT环境中的有效性和适用性。结果表明，整合微调和检索增强策略具有潜在优势，AKM实现了显著的性能提升。本研究获得的见解可以用于开发针对特定领域的专业QA系统。|
|**2024-10-23**|**LongRAG: A Dual-Perspective Retrieval-Augmented Generation Paradigm for Long-Context Question Answering**|Qingfei Zhao et.al.|[2410.18050](http://arxiv.org/abs/2410.18050)|**[link](https://github.com/qingfei1/longrag)**|**长上下文问答（LCQA）是一项具有挑战性的任务，旨在通过对长上下文文档进行推理来提供准确的答案。现有的用于LCQA的长上下文大型语言模型（LLMs）经常遇到“迷失在中间”的问题。检索增强生成（RAG）通过提供外部事实证据来缓解这一问题。然而，其分块策略破坏了全局长上下文信息，并且在长上下文中低质量的检索由于大量噪音而阻碍了LLMs识别有效的事实细节。为此，我们提出了LongRAG，这是一种通用的、双视角的、鲁棒的基于LLM的RAG系统范式，用于LCQA，以增强RAG对复杂长上下文知识（即全局信息和事实细节）的理解。我们将LongRAG设计为即插即用的范式，便于适应各种领域和LLMs。在三个多跳数据集上的广泛实验表明，LongRAG显著优于长上下文LLMs（提高6.94%）、先进的RAG（提高6.16%）以及原始RAG（提高17.25%）。此外，我们进行了定量消融研究和多维度分析，突出了系统组件和微调策略的有效性。数据和代码可从https://github.com/QingFei1/LongRAG获取。**|
|**2024-10-23**|**SimRAG: Self-Improving Retrieval-Augmented Generation for Adapting Large Language Models to Specialized Domains**|Ran Xu et.al.|[2410.17952](http://arxiv.org/abs/2410.17952)|null|检索增强生成（RAG）通过整合外部知识来提高大型语言模型（LLM）的问题回答（QA）能力。然而，将通用的RAG系统适应于科学和医学等专业领域时，由于分布偏移和领域特定数据有限而面临独特挑战。为了解决这一问题，我们提出了SimRAG，这是一种自训练方法，使LLM具备问题回答和问题生成的联合能力，以实现领域适应。我们的方法首先在指令跟随、问题回答和搜索相关数据上对LLM进行微调。然后，提示同一个LLM从未标记的语料库中生成多样化的领域相关问题，并采用额外的过滤策略保留高质量的合成示例。通过利用这些合成示例，LLM可以在领域特定的RAG任务上提高性能。在11个数据集上的实验，涵盖了两个骨干规模和三个领域，表明SimRAG比基线方法提高了1.2%到8.6%。|
|**2024-10-23**|**Leveraging the Domain Adaptation of Retrieval Augmented Generation Models for Question Answering and Reducing Hallucination**|Salman Rakin et.al.|[2410.17783](http://arxiv.org/abs/2410.17783)|null|尽管大型语言模型在各种自然语言处理任务中取得了显著的成功，但检索增强生成模型（RAG）在诸如问答等下游应用中表现出色。最近，RAG-end2end模型进一步优化了架构，在领域适应方面实现了显著的性能提升。然而，当这些基于RAG的架构针对如客户服务等特定领域的细调以构建可靠的对话AI系统时，其有效性仍然相对未被充分探索。此外，在保持高领域特定准确性的同时减少幻觉现象是一个持续存在的关键挑战。在本文中，我们通过领域适应研究了不同RAG和类似RAG架构的表现，并评估了它们根据上下文知识库生成准确且相关响应的能力。为了便于对模型进行评估，我们构建了一个名为HotelConvQA的新数据集，该数据集来源于广泛的酒店相关对话，并在此特定领域数据集上对所有模型进行了微调。我们还解决了确定领域适应对减少不同RAG架构中幻觉影响的关键研究空白，这是之前工作没有充分测量的一个方面。我们的评估显示，通过采用领域适应方法，在所有指标上都取得了积极的结果，表明在问答任务上的强大表现，并提供了关于减少幻觉效果的见解。我们的研究结果清楚地表明，领域适应不仅增强了模型在问答任务中的表现，而且显著减少了所有评估的RAG架构中的幻觉现象。|
|**2024-10-23**|**An Adaptive Framework for Generating Systematic Explanatory Answer in Online Q&A Platforms**|Ziyang Chen et.al.|[2410.17694](http://arxiv.org/abs/2410.17694)|**[link](https://github.com/czy1999/synthrag)**|
|**2024-10-23**|**Graphusion: A RAG Framework for Knowledge Graph Construction with a Global Perspective**|Rui Yang et.al.|[2410.17600](http://arxiv.org/abs/2410.17600)|null|
|**2024-10-22**|**IPL: Leveraging Multimodal Large Language Models for Intelligent Product Listing**|Kang Chen et.al.|[2410.16977](http://arxiv.org/abs/2410.16977)|null|
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
|**2024-10-11**|**StructRAG: Boosting Knowledge Intensive Reasoning of LLMs via Inference-time Hybrid Information Structurization**|Zhuoqun Li et.al.|[2410.08815](http://arxiv.org/abs/2410.08815)|**[link](https://github.com/li-z-q/structrag)**|
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
|**2024-10-10**|**LLM-based SPARQL Query Generation from Natural Language over Federated Knowledge Graphs**|Vincent Emonet et.al.|[2410.06062](http://arxiv.org/abs/2410.06062)|**[link](https://github.com/sib-swiss/sparql-llm)**|
|**2024-10-08**|**Long-Context LLMs Meet RAG: Overcoming Challenges for Long Inputs in RAG**|Bowen Jin et.al.|[2410.05983](http://arxiv.org/abs/2410.05983)|null|
|**2024-10-08**|**Fortify Your Foundations: Practical Privacy and Security for Foundation Model Deployments In The Cloud**|Marcin Chrapek et.al.|[2410.05930](http://arxiv.org/abs/2410.05930)|null|
|**2024-10-08**|**Retrieving, Rethinking and Revising: The Chain-of-Verification Can Improve Retrieval Augmented Generation**|Bolei He et.al.|[2410.05801](http://arxiv.org/abs/2410.05801)|null|
|**2024-10-08**|**LightRAG: Simple and Fast Retrieval-Augmented Generation**|Zirui Guo et.al.|[2410.05779](http://arxiv.org/abs/2410.05779)|**[link](https://github.com/hkuds/lightrag)**|
|**2024-10-07**|**Deciphering the Interplay of Parametric and Non-parametric Memory in Retrieval-augmented Language Models**|Mehrdad Farahani et.al.|[2410.05162](http://arxiv.org/abs/2410.05162)|**[link](https://github.com/m3hrdadfi/rag-memory-interplay)**|
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
|**2024-08-16**|**Extracting polygonal footprints in off-nadir images with Segment Anything Model**|Kai Li et.al.|[2408.08645](http://arxiv.org/abs/2408.08645)|**[link](https://github.com/likaiucas/obm)**|
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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

## text2sql

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-15**|**LR-SQL: A Supervised Fine-Tuning Method for Text2SQL Tasks under Low-Resource Scenarios**|Wen Wuzhenghong et.al.|[2410.11457](http://arxiv.org/abs/2410.11457)|**[link](https://github.com/hongwin/lr-sql)**|**大型语言模型通过监督微调在Text2SQL领域带来了革命性的变化，但一个关键的限制被忽视了：数据库的复杂性导致上下文长度增加，进而增加了模型微调时对GPU内存的需求。为了解决这个问题，我们提出了LR-SQL。LR-SQL包括两个监督微调模型：schema_link模型和SQL_generation模型，其中schema_link模型是整个过程中简化的核心。在schema_link模型的微调过程中，LR-SQL将完整的数据库分解成具有可调节数量的表格组合，使模型能够从这些分散的片段中学习整个数据库中的关系。此外，为了增强模型在推理过程中感知各种离散片段之间关系的能力，LR-SQL对该任务训练了模型的思维链能力。实验结果表明，与现有的微调方法相比，LR-SQL可以将总的GPU内存使用量减少40%，而仅在schema_link任务中损失2%的表预测准确性。对于整体的Text2SQL任务，执行准确率下降了0.6%。我们的项目现已在https://github.com/hongWin/LR-SQL上可用。**|
|**2024-08-27**|**Text2SQL is Not Enough: Unifying AI and Databases with TAG**|Asim Biswal et.al.|[2408.14717](http://arxiv.org/abs/2408.14717)|**[link](https://github.com/tag-research/tag-bench)**|**能够通过自然语言问题查询数据库的人工智能系统有望释放巨大的价值。这类系统允许用户利用语言模型的强大推理和知识能力，同时结合数据管理系统的大规模计算能力。这些综合能力将使用户能够对自定义数据源提出任意的自然语言问题。然而，现有的方法和基准测试在这一领域探索不足。Text2SQL方法仅关注可以通过关系代数表达的自然语言问题，这仅代表了实际用户希望提出的问题的一小部分。同样，检索增强生成（RAG）考虑的是可以通过对数据库中的一个或少数几个数据记录进行点查找来回答的有限子集查询。我们提出了表格增强生成（TAG），这是一种统一且通用的范式，用于回答数据库上的自然语言问题。TAG模型代表了语言模型与数据库之间广泛互动的可能性，这些可能性以前未曾被充分探索，并为利用语言模型的世界知识和推理能力处理数据创造了令人兴奋的研究机会。我们系统地开发了研究TAG问题的基准测试，并发现标准方法正确回答的问题不超过20%，这证实了该领域需要进一步研究。我们在https://github.com/TAG-Research/TAG-Bench上发布了基准测试代码。**|
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
|**2024-08-09**|**A Survey of NL2SQL with Large Language Models: Where are we, and where are we going?**|Xinyu Liu et.al.|[2408.05109](http://arxiv.org/abs/2408.05109)|**[link](https://github.com/hkustdial/nl2sql_handbook)**|**将用户的自然语言查询（NL）转换为SQL查询（即NL2SQL）可以显著降低访问关系数据库的障碍，并支持各种商业应用。随着大型语言模型（LLMs）的出现，NL2SQL的性能得到了极大提升。在这篇综述中，我们全面回顾了基于LLMs的NL2SQL技术，涵盖了其整个生命周期的以下四个方面：(1) 模型：处理不仅包括自然语言的模糊性和不明确性，还包括正确映射自然语言与数据库模式和实例的NL2SQL翻译技术；(2) 数据：从训练数据的收集、因训练数据稀缺而进行的数据合成，到NL2SQL基准测试；(3) 评估：使用不同的度量标准和粒度从多个角度评估NL2SQL方法；以及(4) 错误分析：分析NL2SQL错误以找到根本原因，并指导NL2SQL模型的发展。此外，我们提供了一套开发NL2SQL解决方案的经验法则。最后，我们讨论了在LLMs时代NL2SQL的研究挑战和开放问题。**|
|**2024-07-21**|**Towards Automated Data Sciences with Natural Language and SageCopilot: Practices and Lessons Learned**|Yuan Liao et.al.|[2407.21040](http://arxiv.org/abs/2407.21040)|null|尽管自然语言转SQL（NL2SQL）领域在将自然语言指令翻译成可执行的SQL脚本用于数据查询和处理方面取得了显著进展，但在更广泛的数据科学管道中实现全面自动化——包括数据查询、分析、可视化和报告——仍然是一个复杂的挑战。本研究介绍了SageCopilot，这是一个先进的工业级系统，通过整合大规模语言模型（LLMs）、自主代理（AutoAgents）和语言用户界面（LUIs），实现了数据科学管道的自动化。具体来说，SageCopilot采用了一个两阶段设计：在线组件通过上下文学习（ICL）精炼用户的输入为可执行脚本，并运行这些脚本来生成结果报告与可视化；离线准备在线阶段ICL请求所需的演示。一系列流行策略如思维链和提示调优被用来增强SageCopilot的性能。经过严格的测试和与基于提示解决方案的比较分析，SageCopilot已被实证验证，在使用真实世界数据集生成或执行脚本以及提供带有可视化的结果方面具有优越的端到端性能。我们的深入消融研究表明了SageCopilot所使用的各种组件和策略对数据科学端到端正确性的单独贡献。|
|**2024-06-12**|**DeTriever: Decoder-representation-based Retriever for Improving NL2SQL In-Context Learning**|Yuxi Feng et.al.|[2406.07913](http://arxiv.org/abs/2406.07913)|null|尽管在上下文学习（ICL）已被证明是一种有效的方法，能够提升大型语言模型（LLMs）在多种复杂任务中的表现，特别是在将自然语言问题转换为结构化查询语言（NL2SQL）方面，如何选择最有利的示例仍然是一个开放的研究问题。虽然先前的工作经常采用现成的编码器来动态检索示例，但外部检索器和LLMs之间在表示能力上存在固有的差异。此外，优化示例的选择是一个非平凡的任务，因为没有直接的方法可以在不进行两两推理的情况下评估示例的相对收益。为了解决这些问题，我们提出了DeTriever，这是一种新颖的示例检索框架，它学习了LLM隐藏状态的加权组合，在其中编码了丰富的语义信息。为了训练模型，我们提出了一种代理分数，该分数基于输出查询之间的相似性来估计示例的相对收益。在两个流行的NL2SQL基准测试上的实验表明，我们的方法在单次NL2SQL任务中显著优于最先进的基线方法。|
|**2024-07-27**|**The Dawn of Natural Language to SQL: Are We Fully Ready?**|Boyan Li et.al.|[2406.01265](http://arxiv.org/abs/2406.01265)|**[link](https://github.com/hkustdial/nl2sql360)**|**将用户的自然语言问题转换为SQL查询（即NL2SQL）显著降低了访问关系数据库的门槛。大型语言模型的出现为NL2SQL任务引入了新的范式，极大地增强了其能力。然而，这引发了一个关键问题：我们是否已经完全准备好在生产环境中部署NL2SQL模型？为了解答这个问题，我们提出了一个多角度的NL2SQL评估框架——NL2SQL360，以帮助研究人员设计和测试新的NL2SQL方法。通过NL2SQL360，我们在不同的应用场景下对领先的NL2SQL方法进行了详细比较，如不同的数据领域和SQL特征，为选择最适合特定需求的NL2SQL方法提供了宝贵的见解。此外，我们探索了NL2SQL的设计空间，利用NL2SQL360自动识别针对用户特定需求的最佳NL2SQL解决方案。具体来说，NL2SQL360在Spider数据集上使用执行准确率指标识别出一种有效的NL2SQL方法——SuperSQL。值得注意的是，SuperSQL在Spider和BIRD测试集上的执行准确率分别达到了87%和62.66%，表现出了很强的竞争力。**|
|**2024-05-01**|**ChatBI: Towards Natural Language to Complex Business Intelligence SQL**|Jinqing Lian et.al.|[2405.00527](http://arxiv.org/abs/2405.00527)|null|自然语言转SQL（NL2SQL）技术为不熟悉数据库的非专家用户提供了一个使用SQL进行数据分析的机会。将自然语言转换为商业智能（NL2BI）是实际生产系统中NL2SQL的一种流行应用场景。与NL2SQL相比，NL2BI带来了更多的挑战。在本文中，我们提出了一种全面且高效的技术ChatBI来解决NL2BI任务。首先，我们分析了交互模式，这是NL2SQL和NL2BI在使用上一个重要但不同的模块，并设计了一个更小、成本更低的模型来匹配这种交互模式。在BI场景中，表格包含大量的列，这使得依赖大型语言模型（LLMs）进行模式链接的现有NL2SQL方法由于令牌限制而无法继续。此外，BI场景中模糊列的比例较高也增加了模式链接的难度。ChatBI结合了数据库社区现有的视图技术，首先将模式链接问题分解为单一视图选择问题，然后使用一个更小、成本更低的机器学习模型从显著减少数量的列中选择单个视图。接着，该单个视图的列作为模式链接所需的列传递给大型语言模型。最后，ChatBI提出了与现有流程不同的分阶段处理流程，这使得ChatBI能够更准确地生成包含复杂语义和比较关系的SQL。我们已经在百度的数据平台上部署了ChatBI，并将其集成到多个产品线中进行了大规模生产任务评估。所获得的结果突显了其在实用性、通用性和效率方面的优越性。同时，在我们真实的BI场景数据表和查询下，与当前主流的NL2SQL技术相比，它也取得了最佳效果。|
|**2024-03-29**|**PURPLE: Making a Large Language Model a Better SQL Writer**|Tonghui Ren et.al.|[2403.20014](http://arxiv.org/abs/2403.20014)|null|大型语言模型（LLM）技术在自然语言到SQL（NL2SQL）的转换中发挥着越来越重要的作用。通过大量语料库训练的LLM具有强大的自然语言理解和基本的SQL生成能力，无需针对NL2SQL任务进行额外的微调。现有的基于LLM的NL2SQL方法试图通过增强用户意图理解来改进翻译。然而，由于缺乏组织复杂逻辑运算符组合的知识，LLM有时无法生成合适的SQL。一种有前景的方法是向LLM输入示例，这些示例包括来自各种数据库的已知NL2SQL翻译。LLM可以从输入的示例中学习如何为给定任务组织运算符组合。在本文中，我们提出了PURPLE（利用预训练模型检索提示以增强逻辑），它通过检索包含所需逻辑运算符组合的示例来提高准确性，从而指导LLM生成更好的SQL翻译。PURPLE在流行的NL2SQL基准测试Spider的验证集上达到了80.5%的确切集合匹配准确率和87.8%的执行匹配准确率的新高水平。PURPLE在多样化的基准、预算限制和不同LLM下保持了高准确性，显示出其鲁棒性和成本效益。|
|**2024-03-24**|**SQL-Encoder: Improving NL2SQL In-Context Learning Through a Context-Aware Encoder**|Mohammadreza Pourreza et.al.|[2403.16204](http://arxiv.org/abs/2403.16204)|null|检测查询之间的结构相似性对于在上下文学习模型中选择示例至关重要。然而，仅基于查询的自然语言表达来评估结构相似性而不考虑SQL查询，这构成了一个重大挑战。本文探讨了这种相似性度量的重要性，并提出了一种准确估计它的模型。为此，我们利用了一个包含17万个问题对的数据集，精心策划以训练相似性预测模型。全面的评估表明，所提出的模型能够很好地捕捉问题之间的结构相似性，这一点通过肯德尔-陶距离和精确率@k指标的改进得到了证实。值得注意的是，我们的模型超越了来自OpenAI和Cohere的强大竞争性嵌入模型。此外，与这些竞争模型相比，我们提出的编码器在单次上下文学习场景下提升了NL2SQL模型的下游性能：对于GPT-3.5-turbo提高了1-2%，对于CodeLlama-7B提高了4-8%，对于CodeLlama-13B提高了2-3%。|
|**2024-06-02**|**PET-SQL: A Prompt-Enhanced Two-Round Refinement of Text-to-SQL with Cross-consistency**|Zhishuai Li et.al.|[2403.09732](http://arxiv.org/abs/2403.09732)|**[link](https://github.com/zhshlii/petsql)**|**最近在文本到SQL（Text2SQL）领域的进展强调了通过上下文学习来刺激大型语言模型（LLM），取得了显著的成果。然而，当面对冗长的数据库信息和复杂的用户意图时，它们仍然面临挑战。本文提出了一种两阶段框架，以提高当前基于LLM的自然语言到SQL系统的表现。首先，我们引入了一种新的提示表示方法，称为参考增强表示，该方法包括模式信息和从表中随机抽取的单元格值，用以指导LLM生成SQL查询。然后，在第一阶段，检索问题-SQL对作为少量示例演示，促使LLM生成初步的SQL（PreSQL）。之后，解析PreSQL中提到的实体来进行模式链接，这可以显著压缩有用信息。在第二阶段，利用已链接的模式简化提示中的模式信息，并指示LLM产生最终的SQL。最后，作为后处理模块，我们建议使用不同LLM之间的交叉一致性而不是单个LLM内部的自一致性。我们的方法在Spider基准测试上达到了新的最先进结果，执行准确率为87.6%。**|
|**2024-09-05**|**Aligning Large Language Models to a Domain-specific Graph Database for NL2GQL**|Yuanyuan Liang et.al.|[2402.16567](http://arxiv.org/abs/2402.16567)|null|
|**2024-08-06**|**Intent-Based Access Control: Using LLMs to Intelligently Manage Access Control**|Pranav Subramaniam et.al.|[2402.07332](http://arxiv.org/abs/2402.07332)|null|

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

## PPC

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-25**|**MetaTrading: An Immersion-Aware Model Trading Framework for Vehicular Metaverse Services**|Hongjia Wu et.al.|[2410.19665](http://arxiv.org/abs/2410.19665)|null|更新大量物联网（IoT）数据对于车联元宇宙服务的沉浸感至关重要。然而，在不稳定且资源受限的车联网络中提供高质量和可持续的数据仍然是一个重大挑战。为了解决这个问题，我们提出了一种新的沉浸感知模型交易框架，该框架激励元宇宙用户（MUs）贡献由其最新本地数据训练的学习模型，以增强现实（AR）服务在车联元宇宙中的应用，同时通过联邦学习保护其隐私。为了全面评估MUs提供的本地训练学习模型对AR服务的贡献，我们设计了一个新的沉浸度量标准，该标准通过考虑学习模型的新鲜度和准确性以及用于训练的原始数据的数量和潜在价值来捕捉服务沉浸感。我们将元宇宙服务提供商（MSPs）与MUs之间的交易互动建模为一个带均衡约束的均衡问题（EPEC），以分析和平衡他们的成本和收益。此外，考虑到动态网络条件和隐私问题，我们将MSPs的奖励决策表述为一个多智能体马尔可夫决策过程。然后，提出了一种基于深度强化学习的完全分布式动态奖励方法，该方法无需任何关于MUs和其他MSPs的私人信息即可运行。实验结果表明，与基准方案相比，所提出的框架可以有效地为真实AR相关车辆数据集上的AR服务提供更高价值的对象检测和分类模型。|
|**2024-10-25**|**FLiP: Privacy-Preserving Federated Learning based on the Principle of Least Privileg**|ShiMao Xu et.al.|[2410.19548](http://arxiv.org/abs/2410.19548)|null|联邦学习（FL）允许用户共享知识而非原始数据来训练高精度模型。不幸的是，在训练过程中，用户会失去对所共享知识的控制，这导致了严重的数据隐私问题。我们认为用户只愿意并且只需要分享对训练任务至关重要的知识以获得高精度的FL模型。然而，现有的方法无法帮助用户在FL训练过程中根据其意图最小化共享的知识。本工作提出了FLiP，旨在将最小权限原则（PoLP）引入FL训练中。FLiP的关键设计是通过本地-全局数据集蒸馏设计对训练数据进行精细的信息缩减。我们通过属性推断和成员推断攻击来衡量隐私性能。广泛的实验表明，FLiP在模型准确性和隐私保护之间取得了良好的平衡。|
|**2024-10-28**|**Free-Rider and Conflict Aware Collaboration Formation for Cross-Silo Federated Learning**|Mengmeng Chen et.al.|[2410.19321](http://arxiv.org/abs/2410.19321)|null|联邦学习（FL）是一种机器学习范式，允许多个FL参与者（FL-PTs）在不共享私有数据的情况下协作训练模型。由于数据异质性，在FL训练过程中可能会发生负面迁移。这就需要根据数据互补性来选择FL-PTs。在跨机构FL中，从事商业活动的组织是FL-PTs的主要来源。由此形成的FL生态系统具有两个特点：(i) 自利性和(ii) FL-PTs之间的竞争。这要求理想的FL-PT选择策略能够同时缓解搭便车问题和竞争对手之间的利益冲突。为此，我们提出了一种最优的FL合作形成策略——FedEgoists——该策略确保：(1) 只有当一个FL-PT对FL生态系统有益时，它才能从FL中获益；(2) 一个FL-PT不会对其竞争对手或其支持者做出贡献。它提供了一种有效的聚类解决方案，将FL-PTs分组为联盟，确保每个联盟内的FL-PTs具有相同的利益。我们从理论上证明了所形成的FL-PT联盟是最优的，因为没有任何联盟可以通过合作来提高任何成员的效用。在广泛采用的基准数据集上进行的大量实验表明，与九种最先进的基线方法相比，FedEgoists的有效性及其在参与商业活动的跨机构FL中建立高效协作网络的能力。|
|**2024-10-24**|**Equitable Federated Learning with Activation Clustering**|Antesh Upadhyay et.al.|[2410.19207](http://arxiv.org/abs/2410.19207)|null|联邦学习是一种突出的分布式学习范式，它通过不同客户端之间的协作来促进数据本地化，从而确保隐私。这些客户端在数据生成过程中有着各自的技术、文化和其它偏见。然而，当前的标准往往忽略了这种偏见/异质性，反而加剧了对某些群体的偏见，而不是缓解它。为了解决这一问题，我们提出了一种基于公平聚类的框架，其中客户端根据彼此之间的相似性进行分类/聚类。我们提出了一种独特的方法来构建使用激活向量的相似性矩阵。此外，我们还提出了一种客户端加权机制，以确保每个聚类都获得同等的重要性，并建立了达到ε-平稳解的O(1/√K)收敛速率。我们将所提出的策略与常见的基线方法进行了评估，证明其在减少不同客户端聚类之间存在的偏见以及改善针对特定群体的算法偏见方面具有有效性。|
|**2024-10-24**|**LanFL: Differentially Private Federated Learning with Large Language Models using Synthetic Samples**|Huiyu Wu et.al.|[2410.19114](http://arxiv.org/abs/2410.19114)|null|联邦学习（FL）是一种协作式、保护隐私的机器学习框架，它使多个参与者能够共同训练一个全局模型。然而，由于最近出现的强大语言模型（LLM）具有数十亿到数百亿的参数，将传统的FL方法直接应用于LLM变得不切实际，因为这会导致极高的计算和通信成本。此外，LLM的最终用户往往无法访问模型的完整架构和权重，使得参与者无法直接微调这些模型。本文介绍了一种名为LanFL的新型FL方案，该方案完全基于提示，并将底层LLM视为黑盒。我们开发了一种差异私有的合成样本生成机制，以促进参与者之间的知识共享，并设计了一种提示优化方案，使其能够从合成样本中学习。大量实验表明，LanFL在各种任务中成功地促进了参与者之间的学习，同时保护了本地数据集的隐私。|
|**2024-10-24**|**FedSPD: A Soft-clustering Approach for Personalized Decentralized Federated Learning**|I-Cheng Lin et.al.|[2410.18862](http://arxiv.org/abs/2410.18862)|null|联邦学习作为一种框架，让分布式的客户端能够使用本地数据协同训练一个机器学习模型，近年来越来越受欢迎。虽然传统的联邦学习依赖于中央服务器进行模型聚合，但最近的进展采用了去中心化的框架，允许客户端之间直接交换模型，消除了单点故障。然而，现有的去中心化框架通常假设所有客户端都训练一个共享模型。对每个客户端的模型进行个性化可以提高性能，尤其是在客户端数据分布不均匀的情况下。我们提出了FedSPD，这是一种高效的针对去中心化环境设计的个性化联邦学习算法，并展示了它即使在网络连接性较低的情况下也能学习到准确的模型。为了提供关于收敛性的理论保证，我们引入了一个基于聚类的框架，该框架使得不同数据簇之间的模型达成共识，同时根据不同的客户端上独特的数据簇混合情况进行个性化处理。这种灵活性，即基于数据分布选择性地更新模型，相比之前的去中心化个性化联邦学习方法显著降低了通信成本。在真实世界数据集上的实验结果表明，特别是在网络连接性低的情况下，FedSPD的表现优于多种去中心化的个性化联邦学习算法变体。|
|**2024-10-24**|**Adapting MLOps for Diverse In-Network Intelligence in 6G Era: Challenges and Solutions**|Peizheng Li et.al.|[2410.18793](http://arxiv.org/abs/2410.18793)|null|无缝集成人工智能（AI）和机器学习（ML）技术与无线系统是6G AInization的关键步骤。然而，这种集成在模型功能和生命周期管理方面面临挑战。ML运维（MLOps）提供了一种系统化的方法来应对这些挑战。现有的针对集中式平台实施MLOps的方法往往忽略了不同学习范式和网络异构性带来的挑战。本文提出了一种新的MLOps方法，旨在解决未来无线网络的复杂性。考虑到未来无线接入网（RAN）的独特方面，我们制定了三种操作流程，即强化学习运维（RLOps）、联邦学习运维（FedOps）和生成式AI运维（GenOps）。这些流程为将各种学习/推理能力无缝集成到网络中奠定了基础。我们概述了每种操作的具体挑战和提出的解决方案，促进了大规模部署AI原生6G网络。|
|**2024-10-24**|**Classifier Clustering and Feature Alignment for Federated Learning under Distributed Concept Drift**|Junbao Chen et.al.|[2410.18478](http://arxiv.org/abs/2410.18478)|**[link](https://github.com/chen-junbao/fedccfa)**|**数据异质性是联邦学习中的一个关键挑战，已经有很多研究致力于解决这个问题。然而，带有数据异质性的分布式概念漂移，即客户端可能经历不同的概念漂移，仍然是一个未被充分探索的领域。在这项工作中，我们专注于真实漂移，其中条件分布P(Y,X)发生变化。我们首先研究了分布式概念漂移如何影响模型训练，并发现局部分类器在漂移适应中起着关键作用。此外，为了解决数据异质性问题，我们研究了在分布式概念漂移下的特征对齐，并发现对于特征对齐有两个重要因素：条件分布P(Y,X)和数据异质性的程度。受上述发现的启发，我们提出了FedCCFA，这是一种具有分类器聚类和特征对齐的联邦学习框架。为了在分布式概念漂移下增强协作，FedCCFA在类别级别上对局部分类器进行聚类，并根据聚类结果生成聚类特征锚点。借助这些锚点，FedCCFA基于标签分布P(Y)的熵自适应地对齐客户端的特征空间，从而缓解特征空间的一致性问题。我们的结果显示，在各种概念漂移设置下，FedCCFA显著优于现有方法。代码可在https://github.com/Chen-Junbao/FedCCFA获取。**|
|**2024-10-24**|**FedBaF: Federated Learning Aggregation Biased by a Foundation Model**|Jong-Ik Park et.al.|[2410.18352](http://arxiv.org/abs/2410.18352)|null|由于基础模型能够泛化到各种任务，它们现在成为了领先技术组织的主要关注点。现有将基础模型适应于新应用的方法通常依赖于联邦学习（FL），并在使用基础模型初始化全局模型时向客户端披露基础模型的权重。虽然这些方法确保了客户端数据的隐私，但它们损害了模型和信息的安全性。在本文中，我们提出了一种新的方法——由基础模型偏置的联邦学习聚合（FedBaF），该方法能够在联邦学习聚合阶段动态集成预训练的基础模型权重。与传统方法不同，FedBaF保持了基础模型的机密性，同时仍然利用其力量来训练更准确的模型，尤其是在非独立同分布和对抗性场景中。我们的全面实验使用了Pre-ResNet和诸如Vision Transformer这样的基础模型来证明，FedBaF不仅达到了，而且经常超过了传统权重初始化方法的测试准确性，在独立同分布设置下最高提高了11.4%，在非独立同分布设置下最高提高了15.8%。此外，当应用于基于Transformer的语言模型时，FedBaF显著降低了困惑度，最高减少了39.2%。|
|**2024-10-23**|**LEGO: Language Model Building Blocks**|Shrenik Bhansali et.al.|[2410.18287](http://arxiv.org/abs/2410.18287)|null|大型语言模型（LLMs）在自然语言处理（NLP）中至关重要，但在数据收集、预训练、微调和推理方面成本高昂。针对特定任务的小型语言模型（SLMs）虽然成本较低，但缺乏鲁棒性和泛化能力。本文提出了一种新颖的技术LEGO，可以从LLM中提取SLM并重新组合。利用最先进的LLM剪枝策略，我们可以创建针对任务和用户特定的SLM构建块，这些构建块在微调和推理时效率高，并且能够保护用户数据隐私。LEGO利用联邦学习和一种新的聚合方案来重建LLM，在不增加高成本的情况下保持鲁棒性，并保护用户数据隐私。我们通过实验展示了LEGO的多功能性，表明其能够实现模型异质性，缓解数据异质性的影响，同时保持LLM的鲁棒性。|
|**2024-10-23**|**ProFL: Performative Robust Optimal Federated Learning**|Xue Zheng et.al.|[2410.18075](http://arxiv.org/abs/2410.18075)|null|
|**2024-10-23**|**Federated Transformer: Multi-Party Vertical Federated Learning on Practical Fuzzily Linked Data**|Zhaomin Wu et.al.|[2410.17986](http://arxiv.org/abs/2410.17986)|**[link](https://github.com/xtra-computing/fet)**|
|**2024-10-23**|**Multi-Continental Healthcare Modelling Using Blockchain-Enabled Federated Learning**|Rui Sun et.al.|[2410.17933](http://arxiv.org/abs/2410.17933)|null|
|**2024-10-23**|**Enhancing Federated Learning Convergence with Dynamic Data Queue and Data Entropy-driven Participant Selection**|Charuka Herath et.al.|[2410.17792](http://arxiv.org/abs/2410.17792)|null|
|**2024-10-23**|**Towards Active Participant-Centric Vertical Federated Learning: Some Representations May Be All You Need**|Jon Irureta et.al.|[2410.17648](http://arxiv.org/abs/2410.17648)|null|
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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

## moe

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-25**|**DMT-HI: MOE-based Hyperbolic Interpretable Deep Manifold Transformation for Unspervised Dimensionality Reduction**|Zelin Zang et.al.|[2410.19504](http://arxiv.org/abs/2410.19504)|null|降维（DR）在数据工程和可视化等多个领域中发挥着关键作用，通过简化复杂数据集同时保留重要信息。然而，在处理高维数据时，平衡DR的准确性和可解释性仍然是一个关键挑战。传统DR方法通常面临精度与透明度之间的权衡，优化性能可能会导致可解释性降低，反之亦然。这种局限性在图像、表格和文本数据分析等实际应用中尤为突出，这些应用既需要准确性也需要可解释性。为了解决这些挑战，本文提出了基于MOE的双曲可解释深度流形变换（DMT-HI）。该方法结合了能够有效捕捉复杂层次结构的双曲嵌入和根据输入特征动态分配任务的混合专家（MOE）模型。DMT-HI通过利用双曲嵌入来表示数据的层次性质，从而提高DR的准确性，同时通过MOE结构明确地将输入数据、嵌入结果和关键特征联系起来，从而改善可解释性。大量实验表明，DMT-HI在DR准确性和模型可解释性方面均表现出色，是复杂数据分析的强大解决方案。代码可在https://github.com/zangzelin/code_dmthi获取。|
|**2024-10-25**|**Hierarchical Mixture of Experts: Generalizable Learning for High-Level Synthesis**|Weikai Li et.al.|[2410.19225](http://arxiv.org/abs/2410.19225)|null|高层次综合（HLS）是设计现场可编程门阵列（FPGA）中广泛使用的工具。HLS 通过将源代码编译成 FPGA 电路，使软件编程语言能够用于 FPGA 设计。源代码包括一个程序（称为“内核”）和若干指示硬件综合的 pragma，如并行化、流水线等。虽然软件开发者相对容易设计程序，但设计 pragma 需要大量的硬件知识，这对软件开发者来说是一个很大的挑战。最近，提出了不同的机器学习算法，如图神经网络（GNN），通过性能预测来自动设计 pragma。然而，在新内核上应用训练好的模型时，显著的领域迁移通常会导致不满意的性能。我们提出了一种更具领域泛化能力的模型结构：两级层次化的专家混合（MoE）模型，可以灵活地适应任何 GNN 模型。不同的专家网络可以学习处理表示空间中的不同区域，并利用旧内核和新内核之间的相似模式。在低级 MoE 中，我们在程序的三个自然粒度上应用 MoE：节点、基本块和图。高级 MoE 学习聚合这三个粒度以进行最终决策。为了稳定地训练层次化的 MoE，我们进一步提出了一种两阶段训练方法。广泛的实验验证了层次化 MoE 的有效性。|
|**2024-10-24**|**Read-ME: Refactorizing LLMs as Router-Decoupled Mixture of Experts with System Co-Design**|Ruisi Cai et.al.|[2410.19123](http://arxiv.org/abs/2410.19123)|null|大型语言模型（LLM）的激增促使了混合专家（MoE）架构的采用，这种架构通过动态利用专业子网络来提高效率和性能。尽管具有这些优点，MoE模型在推理过程中仍面临显著挑战，包括由于模型架构与系统策略设计选择不一致导致的内存管理低效和批处理不佳等问题。此外，从零开始训练MoE的传统方法成本越来越高。在这篇论文中，我们提出了一种新的框架Read-ME，该框架可以将预训练的密集型LLM转换为更小的MoE模型（与“升级”通用型MoE相对），从而避免了从头开始训练的高昂成本。我们的方法利用激活稀疏性来提取专家。为了组合专家，我们研究了广泛采用的层间路由器设计，并展示了其冗余性，因此引入了一个与MoE主干解耦的预门控路由器，它促进了系统友好的预计算和前瞻调度，增强了基于专家的批处理和缓存。因此，我们的协同设计在算法和系统两个方面解决了关键差距，为资源受限环境中的LLM推理提供了一种可扩展且高效的替代方案。Read-ME优于其他流行的类似规模开源密集模型，在MMLU上最高提升了10.1%，平均端到端延迟提高了6.1%。代码可以在以下网址获取：https://github.com/VITA-Group/READ-ME。|
|**2024-10-24**|**Mixture of Parrots: Experts improve memorization more than reasoning**|Samy Jelassi et.al.|[2410.19034](http://arxiv.org/abs/2410.19034)|null|混合专家（MoE）架构能够在总模型参数显著增加的情况下，保持最低的计算开销。然而，尚不清楚MoE与标准密集型变换器之间是否存在性能上的权衡。在本文中，我们展示了随着专家数量的增加（同时固定激活参数的数量），记忆性能持续提高，而推理能力趋于饱和。我们首先分析了MoE在推理方面的理论限制。我们证明了存在某些图问题，无论多少个特定宽度的专家都无法解决这些问题；然而，一个稍微宽一些的密集模型却可以轻松解决同样的任务。另一方面，我们发现，在依赖大量记忆的任务上，MoE可以通过使用少量激活参数和大量专家来有效记忆数据。我们在合成图问题和需要大量记忆的闭卷检索任务上对这些发现进行了实证验证。最后，我们预训练了一系列MoE和密集型变换器，并在常用的数学和自然语言基准上评估了它们。我们发现，增加专家数量有助于解决知识密集型任务，但对于推理任务却没有带来同样的好处。|
|**2024-10-23**|**Robust and Explainable Depression Identification from Speech Using Vowel-Based Ensemble Learning Approaches**|Kexin Feng et.al.|[2410.18298](http://arxiv.org/abs/2410.18298)|null|本研究探讨了用于从语音中识别抑郁症的可解释机器学习算法。基于抑郁症影响运动控制和元音产生的语音产生证据，使用预训练的基于元音的嵌入，整合了具有语义意义的语言单位。随后，一种集成学习方法将问题分解为由特定抑郁症状和严重程度水平表征的组成部分。研究探索了两种方法：一种是“自下而上”的方法，通过8个模型预测个体患者健康问卷-8（PHQ-8）项目得分；另一种是使用带有路由模块的专家混合（MoE）的“自上而下”方法来评估抑郁严重程度。两种方法的表现都与最先进的基线相当，表现出稳健性并降低了对数据集均值/中位数的敏感性。讨论了系统可解释性的优势，强调了其在辅助临床医生进行抑郁症诊断和筛查方面的潜力。|
|**2024-10-23**|**MiLoRA: Efficient Mixture of Low-Rank Adaptation for Large Language Models Fine-tuning**|Jingfan Zhang et.al.|[2410.18035](http://arxiv.org/abs/2410.18035)|null|低秩适应（LoRA）及其混合专家（MOE）变体是高效的参数高效微调（PEFT）方法。然而，由于在Transformer层中多个线性模块添加了LoRA模块和MOE路由器，这些方法在多租户环境中引入了显著的延迟。为了解决这个问题，我们提出了一种新颖且高效的LoRA变体——混合低秩适应（MiLoRA）。MiLoRA与之前的MOE风格的LoRA方法不同之处在于，它将每个LoRA模块视为一个专家，并采用一种提示感知的路由机制。该机制在生成第一个新标记之前计算一次专家路由结果，并在后续标记中重用这些结果，从而减少延迟。在常识推理任务、数学推理任务以及广泛使用的LLM评估基准上的大量实验和分析表明，MiLoRA在可调节参数预算相当的情况下，始终优于强大的PEFT基线。此外，与之前的基于LoRA的方法相比，MiLoRA在多租户环境中显著降低了延迟。|
|**2024-10-23**|**ExpertFlow: Optimized Expert Activation and Token Allocation for Efficient Mixture-of-Experts Inference**|Xin He et.al.|[2410.17954](http://arxiv.org/abs/2410.17954)|null|稀疏混合专家（MoE）模型虽然在性能上优于密集型大语言模型（LLM），但在推理过程中由于其高内存需求而面临显著的部署挑战。现有的卸载技术涉及将激活和空闲的专家在GPU和CPU之间交换，但这些技术通常受到僵化的专家缓存机制的限制。这些机制无法适应动态路由，导致缓存利用效率低下，或者预测训练成本过高。为了解决这些特定于推理的挑战，我们引入了ExpertFlow，这是一个专门设计用于通过适应灵活路由并实现CPU和GPU之间的高效专家调度来提高推理效率的综合系统。这减少了开销并提升了系统性能。我们的方法核心是一种基于预测路由路径的卸载机制，该机制使用轻量级预测器在计算开始前准确预测路由路径。这种主动策略允许实时纠正专家缓存中的错误，显著提高了缓存命中率，并减少了专家转移的频率，从而最小化了I/O开销。此外，我们还实施了一种动态令牌调度策略，通过对不同批次中的输入令牌进行重新排列来优化MoE推理。这种方法不仅减少了每批激活的专家数量，还提高了计算效率。大量实验表明，与基线方法相比，ExpertFlow实现了高达93.72%的GPU内存节省，并将推理速度提高了2到10倍，突显了其作为资源受限推理场景中强大解决方案的有效性和实用性。|
|**2024-10-22**|**Optimizing Mixture-of-Experts Inference Time Combining Model Deployment and Communication Scheduling**|Jialong Li et.al.|[2410.17043](http://arxiv.org/abs/2410.17043)|null|随着机器学习模型的规模和复杂性不断增加，其计算需求成为一个重要障碍。Mixture-of-Experts (MoE) 模型通过选择性激活相关专家来缓解这一问题。尽管如此，MoE 模型仍然受到全通信操作带来的高通信开销、由于同步通信约束导致的低 GPU 利用率以及异构 GPU 环境带来的复杂性的限制。本文介绍了 Aurora，它通过优化模型部署和全通信调度来解决 MoE 推理中的这些挑战。Aurora 通过战略性地安排全通信中的令牌传输顺序，实现了最小的通信时间。它通过将不同模型的专家共置于同一设备上，避免了同步全通信的限制，从而提高了 GPU 利用率。我们从理论角度分析了 Aurora 的优化策略在四种常见的 GPU 集群设置下的表现：独占与共置模型在 GPU 上，以及同构与异构 GPU。Aurora 为三种情况提供了最优解，对于剩下的 NP 难问题，它提供了一个多项式时间次优解，仅比最优解差 1.07 倍。Aurora 是首个通过最优模型部署和通信调度在各种场景下最小化 MoE 推理时间的方法。评估表明，Aurora 显著加速了推理过程，在同构集群中最高达到 2.38 倍的速度提升，在异构环境中最高达到 3.54 倍。此外，Aurora 相比现有方法最多可提高 1.5 倍的 GPU 利用率。|
|**2024-10-22**|**CartesianMoE: Boosting Knowledge Sharing among Experts via Cartesian Product Routing in Mixture-of-Experts**|Zhenpeng Su et.al.|[2410.16077](http://arxiv.org/abs/2410.16077)|null|最近，大型语言模型（LLM）因其在各种下游任务中的出色表现而受到了广泛关注。根据著名的缩放定律，扩大密集型LLM的规模可以增强其能力，但也会显著增加计算复杂度。混合专家（MoE）模型通过允许模型大小增长而不大幅提高训练或推理成本来解决这个问题。然而，MoE模型面临着专家之间知识共享的挑战，这使得它们的性能对路由准确性较为敏感。为了解决这一问题，之前的工作引入了共享专家，并以“加法”的方式将其输出与前K个路由专家的输出结合。在这篇论文中，受到集体矩阵分解学习数据间共享知识的启发，我们提出了CartesianMoE，它以更类似于“乘法”的方式实现了专家之间更有效的知识共享。广泛的实验结果表明，在困惑度和下游任务性能方面，CartesianMoE优于之前的MoE模型用于构建LLM。我们还发现CartesianMoE实现了更好的专家路由鲁棒性。|
|**2024-10-21**|**Generalizing Motion Planners with Mixture of Experts for Autonomous Driving**|Qiao Sun et.al.|[2410.15774](http://arxiv.org/abs/2410.15774)|**[link](https://github.com/tsinghua-mars-lab/statetransformer)**|**大型真实驾驶数据集激发了对自动驾驶数据驱动运动规划器多个方面的研究，包括数据增强、模型架构、奖励设计、训练策略和规划器流水线。这些规划器在复杂和少量样本情况下比以前的方法展现出更好的泛化能力。然而，实验结果显示，由于设计过于复杂或训练范式的原因，许多方法在规划性能上的泛化能力有限。本文回顾并基准测试了之前专注于泛化的各种方法。实验结果表明，随着模型适当扩展，许多设计元素变得多余。我们介绍了StateTransformer-2 (STR2)，这是一种可扩展的仅解码器运动规划器，它使用视觉变换器（ViT）编码器和混合专家（MoE）因果变换器架构。MoE骨干通过训练过程中的专家路由解决了模态崩溃和奖励平衡问题。在NuPlan数据集上进行的大量实验表明，我们的方法在不同测试集和闭环仿真中比之前的方法具有更好的泛化能力。此外，我们评估了其在数十亿个真实城市驾驶场景中的可扩展性，展示了随着数据量和模型规模的增长，准确性的持续提升。**|
|**2024-10-21**|**ViMoE: An Empirical Study of Designing Vision Mixture-of-Experts**|Xumeng Han et.al.|[2410.15732](http://arxiv.org/abs/2410.15732)|null|
|**2024-10-20**|**Unveiling and Consulting Core Experts in Retrieval-Augmented MoE-based LLMs**|Xin Zhou et.al.|[2410.15438](http://arxiv.org/abs/2410.15438)|null|
|**2024-10-20**|**LoRA-IR: Taming Low-Rank Experts for Efficient All-in-One Image Restoration**|Yuang Ai et.al.|[2410.15385](http://arxiv.org/abs/2410.15385)|**[link](https://github.com/shallowdream204/lora-ir)**|
|**2024-10-19**|**MENTOR: Mixture-of-Experts Network with Task-Oriented Perturbation for Visual Reinforcement Learning**|Suning Huang et.al.|[2410.14972](http://arxiv.org/abs/2410.14972)|null|
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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

## SSMs

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-25**|**Multi-Agent Reinforcement Learning with Selective State-Space Models**|Jemma Daniel et.al.|[2410.19382](http://arxiv.org/abs/2410.19382)|null|Transformer模型在多个领域中展示了其成功，包括在多智能体强化学习（MARL）中，其中多智能体Transformer（MAT）已成为该领域的领先算法。然而，Transformer模型的一个显著缺点是其计算复杂度相对于输入大小呈二次增长，这使得在扩展到更大输入时计算成本非常高。这一限制影响了MAT在包含大量智能体环境中的可扩展性。最近，状态空间模型（SSMs）因其计算效率而受到关注，但它们在MARL中的应用尚未得到探索。在这项工作中，我们研究了近期提出的SSM——Mamba，在MARL中的使用，并评估它是否能在提供显著效率提升的同时匹配MAT的性能。我们引入了一个改进版的MAT，集成了标准和双向Mamba块，以及一种新颖的“交叉注意力”Mamba块。广泛的测试表明，我们的多智能体Mamba（MAM）在多个标准多智能体环境中与MAT表现相当，同时在扩展到更多智能体场景时提供了更优的可扩展性。这对MARL社区来说意义重大，因为它表明SSMs可以在不牺牲性能的情况下取代Transformers，同时也支持更有效地扩展至更高数量的智能体。我们的项目页面位于https://sites.google.com/view/multi-agent-mamba。|
|**2024-10-24**|**Taipan: Efficient and Expressive State Space Language Models with Selective Attention**|Chien Van Nguyen et.al.|[2410.18572](http://arxiv.org/abs/2410.18572)|null|高效的长上下文语言建模仍然是自然语言处理（NLP）中的一个重要挑战。尽管Transformer在语言任务中占据主导地位，但它们在处理长序列时会遇到训练计算复杂度为二次方以及推理过程中内存成本线性增长的问题。最近的状态空间模型（SSM），如Mamba，提供了常数内存使用量的替代方案，但在需要大量上下文检索的任务中表现不佳。我们提出了一种新的混合架构Taipan，它结合了Mamba-2和选择性注意力层（SAL）。这些SAL能够识别需要长距离交互的标记，去除不重要的特征，并通过注意力模块增强其表示。这种方法平衡了Mamba的效率与类似Transformer在内存密集型任务中的性能。通过限制注意力预算，Taipan能够将准确预测扩展到长达100万个标记的上下文长度，同时保持计算效率。我们的实验表明，Taipan在各种规模和任务上表现出色，为高效长上下文语言建模提供了一个有前景的解决方案。|
|**2024-10-21**|**START: A Generalized State Space Model with Saliency-Driven Token-Aware Transformation**|Jintao Guo et.al.|[2410.16020](http://arxiv.org/abs/2410.16020)|null|域泛化（DG）旨在通过从多个源域学习，使模型能够泛化到未见过的目标域。现有的DG方法主要依赖于卷积神经网络（CNNs），这些网络由于其有限的感受野而固有地学习了纹理偏差，容易对源域过拟合。虽然一些工作引入了基于变换器的方法（ViTs）以利用全局感受野来解决DG问题，但这些方法由于自注意力机制的二次复杂度而导致较高的计算成本。最近，先进的状态空间模型（SSMs），如Mamba，在监督学习任务中展示了有希望的结果，它在训练过程中实现了序列长度的线性复杂度，并且在推理过程中具有快速的RNN样式的计算。受此启发，我们研究了Mamba模型在域偏移下的泛化能力，发现SSMs中的输入依赖矩阵可能会累积和放大域特定特征，从而阻碍模型泛化。为了解决这个问题，我们提出了一种新颖的基于SSM的架构，具有显著性感知的令牌意识转换（称为START），该架构达到了最先进的性能，并为CNNs和ViTs提供了一个有竞争力的替代方案。我们的START可以有选择地扰动并抑制SSMs输入依赖矩阵中显著令牌内的域特定特征，从而有效减少不同域之间的差异。在五个基准测试上的广泛实验表明，START以高效的线性复杂度超越了现有的SOTA DG方法。我们的代码可在https://github.com/lingeringlight/START获取。|
|**2024-10-21**|**Revealing and Mitigating the Local Pattern Shortcuts of Mamba**|Wangjie You et.al.|[2410.15678](http://arxiv.org/abs/2410.15678)|**[link](https://github.com/zetangforward/global_mamba)**|**大型语言模型（LLMs）由于注意力机制而取得了显著进展，但其二次复杂度和线性内存需求限制了它们在长上下文任务中的性能。最近，研究人员引入了Mamba，这是一种基于状态空间模型（SSMs）的先进模型，它提供了线性复杂度和常数内存。尽管据报道Mamba的表现与基于注意力的模型相当甚至超越，但我们的分析显示了一个性能差距：Mamba在涉及局部关键信息的任务中表现出色，但在需要处理分布式关键信息的任务中面临挑战。我们控制实验表明，这种不一致性源于Mamba依赖于局部模式捷径，这使得模型能够在有限的内存中记住局部关键信息，但却阻碍了它保留更分散的信息。因此，我们在Mamba模型中引入了一个全局选择模块来解决这个问题。在现有和提议的合成任务以及实际任务上的实验表明，我们的方法是有效的。值得注意的是，通过仅增加400万个额外参数，我们的方法使Mamba模型（1.3亿参数）在处理分布式信息的任务上实现了显著提升，其性能从0提高到了80.54分。**|
|**2024-10-20**|**Taming Mambas for Voxel Level 3D Medical Image Segmentation**|Luca Lumetti et.al.|[2410.15496](http://arxiv.org/abs/2410.15496)|null|最近，3D医学分割领域主要由采用卷积神经网络（CNN）和基于Transformer架构的深度学习模型主导，每种模型都有其独特的优势和局限性。CNN受到局部感受野的限制，而Transformer则因其巨大的内存需求和数据饥饿性，在处理3D医学体积的细粒度级别时并不理想。因此，在对3D大医学体积中的医学结构进行分割时，全卷积神经网络如nnUNet仍然占据主导地位。尽管在开发具有次二次时间和内存复杂度的Transformer变体方面取得了许多进展，但这些模型在基于内容的推理方面仍显不足。最近的一项突破是Mamba，这是一种基于状态空间模型（SSM）的循环神经网络（RNN），在著名的自然语言处理和基因组基准测试中，它在许多长上下文任务（百万长度序列）上超越了Transformer，并保持线性复杂度。|
|**2024-10-19**|**Spatial-Mamba: Effective Visual State Space Models via Structure-Aware State Fusion**|Chaodong Xiao et.al.|[2410.15091](http://arxiv.org/abs/2410.15091)|**[link](https://github.com/edwardchasel/spatial-mamba)**|**选择性状态空间模型（SSMs），如Mamba，在捕捉一维序列数据中的长距离依赖关系方面表现出色，但在二维视觉任务的应用中仍面临挑战。当前的视觉SSMs通常将图像转换为一维序列，并采用各种扫描模式来结合局部空间依赖关系。然而，这些方法在有效捕捉复杂的图像空间结构以及由于加长的扫描路径导致的计算成本增加方面存在局限性。为了解决这些限制，我们提出了Spatial-Mamba，这是一种新的方法，它直接在状态空间中建立邻域连接。除了依赖顺序状态转移外，我们引入了一个结构感知的状态融合方程，该方程利用空洞卷积来捕捉图像的空间结构依赖关系，显著增强了视觉上下文信息的流动。Spatial-Mamba分为三个阶段：单向扫描中的初始状态计算、通过结构感知状态融合获取空间上下文以及使用观测方程进行最终状态计算。我们的理论分析表明，Spatial-Mamba在同一矩阵乘法框架下统一了原始的Mamba和线性注意力机制，提供了对我们方法更深入的理解。实验结果表明，即使只进行一次扫描，Spatial-Mamba也能在图像分类、检测和分割等任务上达到或超越现有的基于SSM模型的表现。源代码和训练好的模型可以在\href{https://github.com/EdwardChasel/Spatial-Mamba}{这里}找到。**|
|**2024-10-16**|**Rethinking Token Reduction for State Space Models**|Zheng Zhan et.al.|[2410.14725](http://arxiv.org/abs/2410.14725)|**[link](https://github.com/wuyushuwys/tor_ssm)**|**近期，状态空间模型（SSM）的最新进展引起了广泛关注，特别是在那些为并行训练和处理长距离依赖而优化的模型上。像Mamba这样的架构已经通过选择性SSM扩展到了数十亿参数。为了促进Mamba更广泛的应用，探索其效率至关重要。虽然令牌减少技术提供了一种直接的后训练策略，但我们发现将现有方法直接应用于SSM会导致性能显著下降。通过深入分析，我们确定了这种失败的原因以及当前技术的局限性。作为回应，我们提出了一种针对SSM量身定制的统一后训练令牌减少方法。我们的方法结合了令牌的重要性和相似性，从而利用了剪枝和合并的优势，设计出一种细粒度的层内令牌减少策略。广泛的实验表明，与现有方法相比，我们的方法在六个基准测试中使用Mamba-2时平均准确率提高了5.7%到13.1%，同时大幅减少了计算需求和内存要求。**|
|**2024-10-17**|**Provable Benefits of Complex Parameterizations for Structured State Space Models**|Yuval Ran-Milo et.al.|[2410.14067](http://arxiv.org/abs/2410.14067)|null|结构化状态空间模型（SSM）是诸如S4和Mamba等著名神经网络的核心引擎，它们是遵循特定结构（最显著的是对角线结构）的线性动态系统。与参数化为实数的典型神经网络模块不同，SSM经常使用复数参数化。理论上解释复数参数化对于SSM的好处仍然是一个开放的问题。本文通过建立实数和复数对角线SSM之间的正式差异，向解决这一问题迈出了第一步。首先，我们证明了虽然中等维度足以让复数SSM表达所有实数SSM的映射，但要让实数SSM表达复数SSM的映射则需要高得多的维度。其次，我们证明了即使实数SSM的维度足够高以表达给定映射，通常也需要其实数SSM的参数具有指数级大的值，这在实践中无法学习。相比之下，复数SSM可以用适中的参数值表达任何给定映射。实验结果支持了我们的理论，并提示该理论可能扩展到考虑选择性——一种新的架构特征，能够达到最先进的性能。|
|**2024-10-17**|**Quamba: A Post-Training Quantization Recipe for Selective State Space Models**|Hung-Yueh Chiang et.al.|[2410.13229](http://arxiv.org/abs/2410.13229)|null|状态空间模型（SSM）作为大型语言模型的替代方案，已经展现出其吸引力，与基于注意力机制的网络相比，它们以常数内存复杂度实现了最先进的准确率，并能够处理更长的上下文长度。在长序列建模方面，SSM的优越计算效率使其在许多场景中比Transformer更具优势。然而，在请求密集型云服务和资源受限的边缘应用中提高SSM的效率仍然是一个艰巨的任务。SSM量化是一种可能的解决方案，它使得SSM更适合广泛部署，同时保持其准确性。量化是一种常见的技术，用于减小模型大小并利用现代计算单元上的低比特宽度加速特性，但现有的量化技术对于SSM来说并不适用。特别是，SSM在线性递归的选择性扫描机制内具有高度敏感的特征图以及输出激活中的大量异常值，这些是在自注意力模块中的token混合过程中不存在的问题。为了解决这个问题，我们提出了一种静态每张量8位SSM量化方法，该方法通过抑制输入到选择性SSM的激活的最大值来实现更精细的量化精度，并使用Hadamard变换在无异常值的空间中对输出激活进行量化。我们的8位权重-激活量化的Mamba 2.8B SSM得益于硬件加速，在Nvidia Orin Nano 8G上实现了1.72倍更低的生成延迟，而在零样本任务上的平均准确率仅下降了0.9%。实验表明了我们方法的有效性和实际应用性，适用于所有规模的基于SSM的模型在云端和边缘平台上的部署。|
|**2024-10-15**|**UmambaTSF: A U-shaped Multi-Scale Long-Term Time Series Forecasting Method Using Mamba**|Li Wu et.al.|[2410.11278](http://arxiv.org/abs/2410.11278)|null|多变量时间序列预测在交通、气象和金融等领域尤为重要，特别是在极端天气事件的预测中。目前最先进的方法主要依赖于Transformer架构，该架构利用注意力机制来捕捉时间依赖性。然而，这些方法受到二次时间复杂度的限制，随着输入序列长度的增加，模型的可扩展性受到极大限制，这极大地影响了它们在实际应用中的实用性。基于状态空间模型（SSM）的Mamba提供了一种线性时间复杂度的解决方案，增加了对序列数据进行高效预测的可能性。在这项研究中，我们提出了UmambaTSF，这是一种新颖的长期时间序列预测框架，它结合了U形编码器-解码器多层感知机（MLP）的多尺度特征提取能力和Mamba的长序列表示能力。为了提高性能和效率，框架中引入的Mamba块采用了改进的残差结构和适应性设计，能够捕捉独特的时间信号并灵活处理通道。实验表明，UmambaTSF在广泛使用的基准数据集上达到了最先进水平的表现，并具有出色的通用性，同时保持了线性时间复杂度和低内存消耗。|
|**2024-10-14**|**Lambda-Skip Connections: the architectural component that prevents Rank Collapse**|Federico Arangath Joseph et.al.|[2410.10609](http://arxiv.org/abs/2410.10609)|null|
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

<p align=right>(<a href=#updated-on-20241029>back to top</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[contributors-url]: https://github.com/Vincentqyw/cv-arxiv-daily/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[forks-url]: https://github.com/Vincentqyw/cv-arxiv-daily/network/members
[stars-shield]: https://img.shields.io/github/stars/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[stars-url]: https://github.com/Vincentqyw/cv-arxiv-daily/stargazers
[issues-shield]: https://img.shields.io/github/issues/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[issues-url]: https://github.com/Vincentqyw/cv-arxiv-daily/issues

