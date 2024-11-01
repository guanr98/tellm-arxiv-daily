[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## Updated on 2024.11.01
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
|**2024-10-30**|**Evaluating Cultural and Social Awareness of LLM Web Agents**|Haoyi Qiu et.al.|[2410.23252](http://arxiv.org/abs/2410.23252)|null|随着大型语言模型（LLM）扩展到执行现实世界的应用程序，而不仅仅是传统的自然语言处理任务，评估其鲁棒性变得越来越重要。然而，现有的基准测试往往忽略了文化和社会意识等关键维度。为了解决这些问题，我们引入了CASA基准测试，旨在评估LLM代理在两个基于网络的任务中对文化和社交规范的敏感度：在线购物和社交讨论论坛。我们的方法评估了LLM代理检测并适当响应违反规范的用户查询和观察的能力。此外，我们提出了一种全面的评估框架，该框架衡量意识覆盖率、处理用户查询的帮助程度以及面对误导性网络内容时的违规率。实验表明，当前的LLM在非代理环境中的表现显著优于基于网络的代理环境，代理的意识覆盖率不到10%，违规率超过40%。为了提高性能，我们探索了两种方法：提示和微调，并发现结合这两种方法可以提供互补的优势——在特定文化数据集上进行微调大大增强了代理跨不同地区的一般化能力，而提示则提高了代理处理复杂任务的能力。这些发现强调了在开发周期中不断基准测试LLM代理的文化和社会意识的重要性。|
|**2024-10-30**|**Explainable Behavior Cloning: Teaching Large Language Model Agents through Learning by Demonstration**|Yanchu Guan et.al.|[2410.22916](http://arxiv.org/abs/2410.22916)|null|随着移动应用程序复杂性的增加，自主移动应用交互变得越来越重要。开发能够有效导航和与移动应用交互的智能代理仍然是一个重大挑战。在本文中，我们提出了一种可解释的行为克隆大语言模型代理（EBC-LLMAgent），这是一种新颖的方法，它结合了大语言模型（LLMs）和通过学习演示的行为克隆技术，以创建用于自主移动应用交互的智能且可解释的代理。EBC-LLMAgent由三个核心模块组成：演示编码、代码生成和用户界面映射，这些模块协同工作，以捕获用户演示、生成可执行代码，并建立代码与用户界面元素之间的准确对应关系。我们引入了行为克隆链融合技术来增强代理的泛化能力。在五个来自不同领域的流行移动应用程序上的广泛实验表明，EBC-LLMAgent在任务完成方面具有较高的成功率，能够有效地泛化到未见过的场景，并生成有意义的解释。|
|**2024-10-30**|**$\textbf{EMOS}$: $\textbf{E}$mbodiment-aware Heterogeneous $\textbf{M}$ulti-robot $\textbf{O}$perating $\textbf{S}$ ystem with LLM Agents**|Junting Chen et.al.|[2410.22662](http://arxiv.org/abs/2410.22662)|null|异构多机器人系统（HMRS）已成为解决单一机器人无法独立完成的复杂任务的强大方法。当前基于大语言模型的多智能体系统（LLM-based MAS）在软件开发和操作系统等领域已经取得成功，但在机器人控制方面的应用面临着独特的挑战。特别是，在一个多机器人系统中，每个智能体的能力与其物理组成紧密相关，而不是预定义的角色。为了解决这个问题，我们提出了一种新的多智能体框架，旨在促进具有不同实体和能力的异构机器人之间的有效协作，并引入了一个名为Habitat-MAS的新基准。我们的一个关键设计是“机器人简历”：我们不采用人类设计的角色扮演，而是提出一种自我提示的方法，让智能体理解机器人的URDF文件并调用机器人运动学工具来生成描述其物理能力的信息，以指导它们在任务规划和动作执行中的行为。Habitat-MAS基准旨在评估多智能体框架如何处理需要实体感知推理的任务，这些任务包括1) 操纵、2) 感知、3) 导航以及4) 综合性的多楼层物体重排。实验结果表明，机器人的简历以及我们多智能体系统的分层设计对于在这种复杂问题情境下有效运作异构多机器人系统至关重要。|
|**2024-10-29**|**BENCHAGENTS: Automated Benchmark Creation with Agent Interaction**|Natasha Butt et.al.|[2410.22584](http://arxiv.org/abs/2410.22584)|null|评估受到基准可用性的限制。随着模型的发展，需要创建能够衡量新生成能力进展的基准。然而，通过人工标注创建新基准既缓慢又昂贵，这限制了对任何能力进行全面评估的可能性。我们引入了BENCHAGENTS框架，该框架系统地利用大型语言模型（LLMs）来自动化为复杂能力创建基准的过程，同时固有地确保数据和度量的质量。BENCHAGENTS将基准创建过程分解为规划、生成、数据验证和评估四个步骤，每个步骤都由一个LLM代理执行。这些代理相互交互，并利用来自基准开发人员的人机循环反馈，以明确改进并灵活控制数据多样性和质量。我们使用BENCHAGENTS创建了用于评估与文本生成过程中规划和约束满足相关的能力的基准。然后，我们使用这些基准研究了七个最先进模型，并从中提取出关于常见故障模式和模型差异的新见解。|
|**2024-10-29**|**Auto-Intent: Automated Intent Discovery and Self-Exploration for Large Language Model Web Agents**|Jaekyeom Kim et.al.|[2410.22552](http://arxiv.org/abs/2410.22552)|null|在本文中，我们介绍了Auto-Intent方法，该方法可以在不直接微调的情况下将预训练的大规模语言模型（LLM）适应为目标领域的代理，我们在实验中特别关注网页导航任务。我们的方法首先从目标领域的演示中无监督地发现潜在意图，并将其压缩为高度紧凑的形式（最多三个词）。利用提取出的意图，我们训练意图预测器根据代理过去的观察和行动来预测下一个意图。特别是，我们提出了一种自我探索方法，其中将最有可能的前k个意图预测作为提示提供给预训练的LLM代理，从而增强了其决策能力。Auto-Intent显著提高了GPT-3.5、GPT-4和Llama-3.1-70B、Llama-3.1-405B代理在Mind2Web的大规模真实网站导航基准测试以及来自WebArena的在线导航任务中的表现，并展示了从Mind2Web到其他基准测试的跨基准泛化能力。|
|**2024-10-29**|**SceneGenAgent: Precise Industrial Scene Generation with Coding Agent**|Xiao Xia et.al.|[2410.21909](http://arxiv.org/abs/2410.21909)|**[link](https://github.com/thudm/scenegenagent)**|**工业场景的建模对于工业制造中的仿真至关重要。虽然大型语言模型（LLMs）在从文本描述生成通用3D场景方面取得了显著进展，但由于工业场景对精确测量和定位的需求以及复杂的空间布局规划要求，使用LLMs生成工业场景面临着独特的挑战。为了解决这一挑战，我们引入了SceneGenAgent，这是一种基于LLM的代理，通过C#代码生成工业场景。SceneGenAgent通过结构化且可计算的格式、布局验证和迭代优化来确保精确的布局规划，以满足工业场景的定量需求。实验结果表明，由SceneGenAgent支持的LLMs超越了其原始性能，在实际工业场景生成任务中达到了高达81.0%的成功率，并有效满足了大多数场景生成需求。为了进一步提高可访问性，我们构建了SceneInstruct数据集，旨在微调开源LLMs以便集成到SceneGenAgent中。实验显示，在SceneInstruct上微调开源LLMs带来了显著的性能提升，其中Llama3.1-70B接近GPT-4o的能力。我们的代码和数据可在https://github.com/THUDM/SceneGenAgent 获取。**|
|**2024-10-28**|**Can Machines Think Like Humans? A Behavioral Evaluation of LLM-Agents in Dictator Games**|Ji Ma et.al.|[2410.21359](http://arxiv.org/abs/2410.21359)|null|随着基于大型语言模型（LLM）的代理越来越多地承担现实世界的任务并与人类社会互动，我们对其行为的理解程度如何？本研究（1）探讨了不同人格如何诱导LLM代理的亲社会行为——这是一种基本的社会规范，并将其与人类行为进行基准比较；（2）引入了一种行为方法来评估LLM代理在复杂决策场景中的表现。我们探索了不同人格和实验框架如何影响这些AI代理在独裁者游戏中的利他行为，并在同一LLM家族内、不同家族之间以及与人类行为进行了比较。我们的发现揭示了LLM之间存在显著的变化和不一致性，以及与人类行为相比的明显差异。仅仅赋予LLM类人身份并不能产生类人行为。尽管这些AI代理接受了大量人类生成数据的训练，但它们无法准确预测人类的决策。LLM代理无法捕捉到人类决策过程中的内在机制，其与人类行为的一致性高度可变且依赖于特定的模型架构和提示公式；更糟糕的是，这种依赖性并不遵循一个明确的模式。|
|**2024-10-28**|**Automatic Generation of Benchmarks and Reliable LLM Judgment for Code Tasks**|Eitan Farchi et.al.|[2410.21071](http://arxiv.org/abs/2410.21071)|null|大型语言模型（LLMs）可以用于多种与代码相关的任务，如将一种编程语言翻译成另一种编程语言、实现自然语言需求和代码摘要。最先进的LLM技术生成的工件预期是有用的，用户只需进行少量简单的修改即可使用。量化这一模糊概念是具有挑战性的，因此很难确定与代码相关的LLM解决方案的质量。我们将使用LLM判断来评估LLM解决方案的方法称为“LLM作为法官”，或简称LaaJ。在这项工作中，我们介绍了一种生成和评估LaaJ实现的方法论，并利用自动生成的基准来进行。该基准有两个目的：一方面用于开发和验证LaaJs，另一方面用于通过LaaJs验证和测试与代码相关的LLM解决方案。为此，我们开发了一个自动基准生成引擎，该引擎能够为多个代码相关任务生成多种编程语言的代码，作为LaaJ评估的输入。我们采用一个表示潜在代码生成物的图G。图中的顶点是生成的工件，边则表示可能的生成过程，例如从其自然语言需求生成Java程序。通过一系列LLM代理和图G，我们生成了与代码相关的工件。利用图G中的循环，我们对生成的工件制定了期望。利用这些制定的期望，使我们能够开发和测试可靠的LLM判断，以评估解决方案生成的工件的有用性。我们的方法能够创建高质量的代码任务解决方案。|
|**2024-10-28**|**Guide-LLM: An Embodied LLM Agent and Text-Based Topological Map for Robotic Guidance of People with Visual Impairments**|Sangmim Song et.al.|[2410.20666](http://arxiv.org/abs/2410.20666)|null|导航对于视障人士（PVI）来说是一个重大挑战。虽然传统的辅助工具如白手杖和导盲犬非常宝贵，但它们在提供详细的环境信息和精确的路线引导方面存在不足。最近，在大型语言模型（LLMs）和视觉-语言模型（VLMs）方面的进展为增强辅助导航提供了新的途径。在这篇论文中，我们介绍了Guide-LLM，这是一种基于实体化LLM的代理，旨在帮助PVI在大型室内环境中导航。我们的方法包括一种新颖的文字拓扑地图，使LLM能够使用简化的环境表示来规划全局路径，重点放在直线路径和直角转弯上，以促进导航。此外，我们利用LLM的常识推理来进行危险检测，并根据用户偏好进行个性化路径规划。模拟实验表明了该系统在指导PVI方面的有效性，突显了它作为辅助技术领域的重要进步的潜力。结果强调了Guide-LLM提供高效、适应性强且个性化的导航辅助的能力，指出了该领域的有希望的发展方向。|
|**2024-10-27**|**TrajAgent: An Agent Framework for Unified Trajectory Modelling**|Yuwei Du et.al.|[2410.20445](http://arxiv.org/abs/2410.20445)|**[link](https://github.com/tsinghua-fib-lab/trajagent)**|**轨迹建模，包括轨迹数据模式挖掘和未来预测的研究，在生活服务、城市交通和公共管理等领域有着广泛的应用。为了解决轨迹建模中的特定问题，已经提出了许多方法。然而，由于数据的异质性和轨迹任务的多样性，实现统一的轨迹建模仍然是一个重要而具有挑战性的任务。在本文中，我们提出了TrajAgent，一个基于大型语言模型的代理框架，以统一各种轨迹建模任务。在TrajAgent中，我们首先开发了UniEnv，一个具有统一数据和模型接口的执行环境，以支持各种模型的执行和训练。在此基础上，我们引入了TAgent，一种针对不同轨迹任务自动轨迹建模的代理工作流程。具体来说，我们在TAgent中设计了AutOpt，一个系统优化模块，以进一步提高集成模型的性能。通过输入自然语言描述的各种轨迹任务，TrajAgent能够通过训练和执行适当的模型自动生成有竞争力的结果。在四个真实世界数据集上的四个任务的广泛实验表明，TrajAgent在统一轨迹建模方面是有效的，平均性能比基线方法提高了15.43%。**|
|**2024-10-25**|**Cooperative Strategic Planning Enhances Reasoning Capabilities in Large Language Models**|Danqing Wang et.al.|[2410.20007](http://arxiv.org/abs/2410.20007)|null|
|**2024-10-29**|**Reinforcement Learning for Aligning Large Language Models Agents with Interactive Environments: Quantifying and Mitigating Prompt Overfitting**|Mohamed Salim Aissi et.al.|[2410.19920](http://arxiv.org/abs/2410.19920)|null|
|**2024-10-25**|**Investigating the Role of Prompting and External Tools in Hallucination Rates of Large Language Models**|Liam Barkley et.al.|[2410.19385](http://arxiv.org/abs/2410.19385)|null|
|**2024-10-25**|**Designing LLM-Agents with Personalities: A Psychometric Approach**|Muhua Huang et.al.|[2410.19238](http://arxiv.org/abs/2410.19238)|null|
|**2024-10-25**|**An LLM Agent for Automatic Geospatial Data Analysis**|Yuxing Chen et.al.|[2410.18792](http://arxiv.org/abs/2410.18792)|null|
|**2024-10-24**|**PRACT: Optimizing Principled Reasoning and Acting of LLM Agent**|Zhiwei Liu et.al.|[2410.18528](http://arxiv.org/abs/2410.18528)|null|
|**2024-10-23**|**GraphTeam: Facilitating Large Language Model-based Graph Analysis via Multi-Agent Collaboration**|Xin Li et.al.|[2410.18032](http://arxiv.org/abs/2410.18032)|**[link](https://github.com/bupt-gamma/graphteam)**|
|**2024-10-25**|**MiniFed : Integrating LLM-based Agentic-Workflow for Simulating FOMC Meeting**|Sungil Seok et.al.|[2410.18012](http://arxiv.org/abs/2410.18012)|null|
|**2024-10-22**|**SELA: Tree-Search Enhanced LLM Agents for Automated Machine Learning**|Yizhou Chi et.al.|[2410.17238](http://arxiv.org/abs/2410.17238)|**[link](https://github.com/geekan/metagpt)**|
|**2024-10-22**|**EnvBridge: Bridging Diverse Environments with Cross-Environment Knowledge Transfer for Embodied AI**|Tomoyuki Kagaya et.al.|[2410.16919](http://arxiv.org/abs/2410.16919)|null|
|**2024-10-22**|**CoPS: Empowering LLM Agents with Provable Cross-Task Experience Sharing**|Chen Yang et.al.|[2410.16670](http://arxiv.org/abs/2410.16670)|**[link](https://github.com/uclaml/cops)**|
|**2024-10-22**|**Adsorb-Agent: Autonomous Identification of Stable Adsorption Configurations via Large Language Model Agent**|Janghoon Ock et.al.|[2410.16658](http://arxiv.org/abs/2410.16658)|null|
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
|**2024-10-18**|**SRAP-Agent: Simulating and Optimizing Scarce Resource Allocation Policy with LLM-based Agent**|Jiarui Ji et.al.|[2410.14152](http://arxiv.org/abs/2410.14152)|**[link](https://github.com/jijiarui-cather/srapagent_framework)**|
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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

## llm

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-30**|**Evaluating Cultural and Social Awareness of LLM Web Agents**|Haoyi Qiu et.al.|[2410.23252](http://arxiv.org/abs/2410.23252)|null|随着大型语言模型（LLMs）扩展到执行现实世界的应用任务，而不仅仅是传统的自然语言处理任务，评估其鲁棒性变得越来越重要。然而，现有的基准测试往往忽略了文化和社会意识等关键维度。为了解决这些问题，我们引入了CASA基准测试，旨在评估LLM代理在在线购物和社交讨论论坛两个网络任务中对文化和社交规范的敏感度。我们的方法评估了LLM代理检测并适当响应违规用户查询和观察的能力。此外，我们提出了一种全面的评估框架，该框架衡量了意识覆盖率、管理用户查询的帮助性以及面对误导性网络内容时的违规率。实验表明，当前的LLM在非代理环境中的表现显著优于在网络代理环境中，代理的意识覆盖率低于10%，违规率超过40%。为了提高性能，我们探索了两种方法：提示和微调，并发现结合这两种方法可以提供互补的优势——在特定文化数据集上进行微调显著增强了代理跨不同地区的一般化能力，而提示则提升了代理处理复杂任务的能力。这些发现强调了在开发周期中持续基准测试LLM代理的文化和社会意识的重要性。|
|**2024-10-30**|**A little less conversation, a little more action, please: Investigating the physical common-sense of LLMs in a 3D embodied environment**|Matteo G. Mecattaf et.al.|[2410.23242](http://arxiv.org/abs/2410.23242)|null|作为通用工具，大型语言模型（LLM）经常需要对日常物理环境进行推理。在问答能力方面，理解物理对象之间的相互作用可能是提供适当响应的必要条件。此外，LLM越来越多地被用作代理系统的推理引擎，设计和控制其动作序列。绝大多数研究使用静态基准来解决这个问题，这些基准由关于物理世界的文本或基于图像的问题组成。然而，这些基准并不能捕捉现实生活中的物理过程的复杂性和细微差别。在这里，我们提倡第二种相对未探索的方法：通过让LLM在一个3D环境中控制一个代理来“赋予”它们身体。我们提出了第一个具有身体感知和认知意义的LLM物理常识推理评估框架。我们的框架允许直接比较LLM与其他具身代理，如基于深度强化学习的代理，以及人类和非人类动物。我们使用Animal-AI（AAI）环境，一个模拟的3D虚拟实验室，来研究LLM中的物理常识推理。为此，我们利用了AAI测试平台，这是一套复制了非人类动物实验的实验，用于研究包括距离估计、跟踪视线之外的对象以及工具使用在内的物理推理能力。我们证明了无需微调的最先进的多模态模型可以完成这种类型的任务，从而能够与2019年Animal-AI奥运会竞赛的参赛者及人类儿童进行有意义的比较。我们的结果显示，在这些任务上，LLM目前的表现不如人类儿童。我们认为，这种方法允许使用直接来自认知科学的生态有效的实验来研究物理推理，提高了LLM的可预测性和可靠性。|
|**2024-10-30**|**EMOTION: Expressive Motion Sequence Generation for Humanoid Robots with In-Context Learning**|Peide Huang et.al.|[2410.23234](http://arxiv.org/abs/2410.23234)|null|本文介绍了一个名为EMOTION的框架，用于生成类人机器人中的富有表现力的动作序列，以增强它们进行类似人类的非言语交流的能力。非言语线索如面部表情、手势和身体动作在有效的人际互动中起着关键作用。尽管机器人行为方面已有进步，但现有方法往往难以模仿人类非言语交流的多样性和微妙之处。为了解决这一问题，我们的方法利用大型语言模型（LLM）的上下文学习能力，动态生成适用于人机交互的社会性适当的手势动作序列。我们使用该框架生成了10种不同的富有表现力的手势，并进行了在线用户研究，比较了EMOTION及其结合人类反馈版本EMOTION++所生成动作与人类操作员所生成动作在自然度和可理解性方面的表现。结果显示，在某些场景下，我们的方法在生成可理解和自然的机器人动作方面能够达到或超越人类的表现。我们还提供了未来研究在生成富有表现力的机器人手势时应考虑的一系列变量的设计启示。|
|**2024-10-31**|**Grounding by Trying: LLMs with Reinforcement Learning-Enhanced Retrieval**|Sheryl Hsu et.al.|[2410.23214](http://arxiv.org/abs/2410.23214)|null|大型语言模型（LLMs）的幻觉问题正通过允许这些模型搜索信息并将答案基于真实来源来逐渐得到缓解。不幸的是，当处理复杂或间接主题时，LLMs往往难以提出正确的搜索查询。观察到LLMs可以通过尝试不同的查询并学习提升那些能够成功产生相关结果的查询权重来学会搜索相关信息，我们引入了一种名为LeReT（Learning to Retrieve by Trying）的强化学习框架，该框架探索搜索查询，并使用基于偏好的优化方法来提高查询质量。LeReT可以将绝对检索准确率提高至多29%，并将下游生成器评估提高17%。LeReT的简单性和灵活性使其能够应用于任意现成的检索器，这使其成为一种有前景的技术，用于改进通用LLM流程。项目网站：http://sherylhsu.com/LeReT/|
|**2024-10-30**|**ProTransformer: Robustify Transformers via Plug-and-Play Paradigm**|Zhichao Hou et.al.|[2410.23182](http://arxiv.org/abs/2410.23182)|null|基于Transformer的架构近年来在机器学习的各个领域占据了主导地位。在这篇论文中，我们介绍了一种新颖的鲁棒注意力机制，旨在增强Transformer架构的韧性。重要的是，这种技术可以作为即插即用层集成到现有的Transformer中，无需额外的训练或微调就能提高其鲁棒性。通过全面的实验和消融研究，我们展示了ProTransformer显著提高了Transformer模型在各种预测任务、攻击机制、骨干架构和数据域中的鲁棒性。值得注意的是，在没有进一步微调的情况下，ProTransformer在经典TextFooler攻击下分别将BERT、ALBERT、DistilBERT和RoBERTa的性能提高了19.5%、28.3%、16.1%和11.4%。此外，ProTransformer在大型语言模型（LLMs）中也表现出对基于提示攻击的良好抵抗力，将T5和LLaMA的性能分别提高了24.8%和17.8%，并将Vicuna针对Jailbreaking攻击的性能平均提高了10.4%。除了语言领域外，ProTransformer还在视觉和图领域展示了出色的鲁棒性。|
|**2024-10-30**|**ReasoningRec: Bridging Personalized Recommendations and Human-Interpretable Explanations through LLM Reasoning**|Millennium Bismay et.al.|[2410.23180](http://arxiv.org/abs/2410.23180)|**[link](https://github.com/millenniumbismay/reasoningrec)**|**本文介绍了ReasoningRec，这是一种基于推理的推荐框架，利用大型语言模型（LLM）来弥合推荐与人类可解释性解释之间的差距。与依赖隐式用户-项目交互的传统推荐系统不同，ReasoningRec使用LLM来建模用户和项目，重点关注偏好、厌恶和解释性推理。该框架利用一个较大的LLM为用户偏好生成合成解释，随后用于微调较小的LLM，以提高推荐准确性和人类可解释性解释。我们的实验研究探讨了推理和上下文信息对个性化推荐的影响，揭示了上下文和个人数据的质量显著影响LLM生成合理解释的能力。实证评估表明，ReasoningRec在推荐预测方面比最先进方法高出12.5%，同时提供人类可理解的解释。代码可在以下网址获取：https://github.com/millenniumbismay/reasoningrec。**|
|**2024-10-30**|**SciPIP: An LLM-based Scientific Paper Idea Proposer**|Wenxiao Wang et.al.|[2410.23166](http://arxiv.org/abs/2410.23166)|null|知识的指数增长和跨学科研究的日益复杂给研究人员带来了重大挑战，包括信息过载和探索新想法的困难。大型语言模型（LLMs）如GPT-4的进步在增强想法提案方面显示出了巨大潜力，但如何有效利用大型模型进行合理的想法提案尚未被充分探索。本文提出了一种科学论文想法提案者（SciPIP）。基于用户提供的研究背景，SciPIP从文献数据库中检索有用的论文，同时利用LLMs的能力生成更具新颖性和可行性的想法。为此，1) 我们构建了一个文献检索数据库，提取了大量论文的多维度信息以便快速访问。然后，我们提出了一种基于语义、实体和引用共现的文献检索方法，根据用户提供的背景从多个角度搜索相关文献。2) 在文献检索之后，我们引入了双路径想法提案策略，一条路径从检索到的文献中推断解决方案，另一条路径通过模型头脑风暴生成原创想法。我们将两者结合以实现可行性与原创性之间的良好平衡。通过对自然语言处理（NLP）领域的广泛实验，我们证明了SciPIP能够检索出与现有顶级会议论文相似的引用，并生成许多与此一致的想法。此外，我们使用大型语言模型评估了SciPIP生成的其他想法的原创性，进一步验证了我们所提方法的有效性。代码和数据库发布于https://github.com/cheerss/SciPIP。|
|**2024-10-30**|**Real-Time Personalization for LLM-based Recommendation with Customized In-Context Learning**|Keqin Bao et.al.|[2410.23136](http://arxiv.org/abs/2410.23136)|**[link](https://github.com/ym689/rec_icl)**|**频繁更新基于大型语言模型（LLM）的推荐系统以适应新的用户兴趣——就像对传统推荐系统所做的那样——由于高昂的训练成本而不切实际，即使使用加速方法也是如此。本研究探索了在不进行任何模型更新的情况下通过利用上下文学习（ICL）来适应动态用户兴趣的方法。ICL允许LLM从输入中提供的少量示例中学习新任务。通过将新的兴趣示例作为ICL中的少量示例，LLM可以直接学习实时兴趣，从而避免了模型更新的需求。然而，现有的基于LLM的推荐系统在推荐调优过程中往往失去了上下文学习能力，而原始LLM的上下文学习缺乏针对推荐的具体焦点。为了解决这个问题，我们提出了RecICL，它定制了特定于推荐的上下文学习，用于实时推荐。RecICL以一种上下文学习格式组织训练示例，确保在调优过程中保留并调整上下文学习能力以符合推荐任务。广泛的实验表明，RecICL能够在不需要模型更新的情况下有效提供实时推荐。我们的代码可以在https://github.com/ym689/rec_icl获得。**|
|**2024-10-30**|**On Memorization of Large Language Models in Logical Reasoning**|Chulin Xie et.al.|[2410.23123](http://arxiv.org/abs/2410.23123)|null|大型语言模型（LLM）在具有挑战性的推理基准测试中表现出良好的性能，但同时也可能犯一些基本的推理错误。这种对比行为在理解LLM推理能力背后的机制时显得非常令人困惑。一种假设是，这些模型在常见推理基准测试中的高且接近饱和的性能可能是由于记忆了类似的问题。在这篇论文中，我们使用基于骑士与无赖（K&K）谜题动态生成的逻辑推理基准，系统地研究了这一假设，并定量测量了推理任务中的记忆效应。我们发现，经过微调后，LLM能够很好地插值训练谜题（达到近乎完美的准确率），但在这些谜题稍微被扰动时却失败了，这表明模型在解决训练谜题时严重依赖于记忆。另一方面，尽管微调导致了大量的记忆效应，但它也始终提高了泛化性能。通过扰动测试、跨难度级别的可迁移性、探测模型内部以及用错误答案进行微调的深入分析表明，尽管存在训练数据的记忆效应，LLM仍学会了如何解答K&K谜题。这一现象表明，LLM在记忆和真正的推理能力之间展现出了复杂的相互作用。最后，我们的单样本记忆分数分析揭示了LLM在解决逻辑谜题时是如何在推理和记忆之间切换的。我们的代码和数据可以在https://memkklogic.github.io获取。|
|**2024-10-31**|**Why Gradient Subspace? Identifying and Mitigating LoRA's Bottlenecks in Federated Fine-Tuning of Large Language Models**|Navyansh Mahla et.al.|[2410.23111](http://arxiv.org/abs/2410.23111)|null|大型语言模型（LLMs）在文本和视觉数据的任务泛化方面展示了显著的能力。虽然微调这些模型可以显著提高其在特定下游任务上的性能，但这通常需要高质量的数据，而这些数据由于隐私问题无法共享。联邦学习（FL）为无需直接数据共享的协作训练提供了一个有前景的解决方案。然而，许多基于低秩适应（LoRA）的LLM参数高效微调策略在FL中面临局限性。在这篇论文中，我们批判性地分析了使用LoRA的流行FL框架的收敛性和性能保证，指出了由于低秩矩阵的受限子空间学习而导致的次优性质。这一限制阻碍了LLM在联邦设置中的有效微调。通过严格的分析和实证评估，我们证明了直接权重平均优于基于LoRA的策略，从而为微调模型带来更优越的性能。我们的全面比较揭示了LoRA方法的效率低下，并强调了直接权重聚合的优势。我们将分析扩展到局部训练步骤中使用的低秩梯度优化器，如GaLore。研究结果表明，GaLore是一种更有效的替代方案，在文本和图像模态上均优于联邦LoRA方法，如FlexLoRA和FFA-LoRA。尽管隐私在FL讨论中仍然是最重要的，但我们的重点是评估联邦微调模型的性能结果，并从理论和实证角度评估各种FL框架。我们的发现建议重新评估FL上下文中对LoRA的依赖，为更高效的训练方法铺平道路。|
|**2024-10-29**|**Online Detecting LLM-Generated Texts via Sequential Hypothesis Testing by Betting**|Can Chen et.al.|[2410.22318](http://arxiv.org/abs/2410.22318)|**[link](https://github.com/canchen-cc/online-llm-detection)**|
|**2024-10-29**|**Natural Language Inference Improves Compositionality in Vision-Language Models**|Paola Cascante-Bonilla et.al.|[2410.22315](http://arxiv.org/abs/2410.22315)|null|
|**2024-10-29**|**GPT-4o reads the mind in the eyes**|James W. A. Strachan et.al.|[2410.22309](http://arxiv.org/abs/2410.22309)|null|
|**2024-10-29**|**SVIP: Towards Verifiable Inference of Open-source Large Language Models**|Yifan Sun et.al.|[2410.22307](http://arxiv.org/abs/2410.22307)|null|
|**2024-10-29**|**Flow-DPO: Improving LLM Mathematical Reasoning through Online Multi-Agent Learning**|Yihe Deng et.al.|[2410.22304](http://arxiv.org/abs/2410.22304)|null|
|**2024-10-29**|**LLMs are Highly-Constrained Biophysical Sequence Optimizers**|Angelica Chen et.al.|[2410.22296](http://arxiv.org/abs/2410.22296)|null|
|**2024-10-29**|**Fine-Tuning LLMs for Code Mutation: A New Era of Cyber Threats**|Mohammad Setak et.al.|[2410.22293](http://arxiv.org/abs/2410.22293)|null|
|**2024-10-29**|**Embedding-based classifiers can detect prompt injection attacks**|Md. Ahsan Ayub et.al.|[2410.22284](http://arxiv.org/abs/2410.22284)|**[link](https://github.com/AhsanAyub/malicious-prompt-detection)**|
|**2024-10-29**|**Whose ChatGPT? Unveiling Real-World Educational Inequalities Introduced by Large Language Models**|Renzhe Yu et.al.|[2410.22282](http://arxiv.org/abs/2410.22282)|null|
|**2024-10-29**|**Are Decoder-Only Large Language Models the Silver Bullet for Code Search?**|Yuxuan Chen et.al.|[2410.22240](http://arxiv.org/abs/2410.22240)|null|
|**2024-10-28**|**Arithmetic Without Algorithms: Language Models Solve Math With a Bag of Heuristics**|Yaniv Nikankin et.al.|[2410.21272](http://arxiv.org/abs/2410.21272)|**[link](https://github.com/technion-cs-nlp/llm-arithmetic-heuristics)**|
|**2024-10-28**|**LongReward: Improving Long-context Large Language Models with AI Feedback**|Jiajie Zhang et.al.|[2410.21252](http://arxiv.org/abs/2410.21252)|**[link](https://github.com/THUDM/LongReward)**|
|**2024-10-28**|**Zero-Shot Dense Retrieval with Embeddings from Relevance Feedback**|Nour Jedidi et.al.|[2410.21242](http://arxiv.org/abs/2410.21242)|null|
|**2024-10-28**|**Hierarchical Knowledge Graph Construction from Images for Scalable E-Commerce**|Zhantao Yang et.al.|[2410.21237](http://arxiv.org/abs/2410.21237)|null|
|**2024-10-28**|**Flaming-hot Initiation with Regular Execution Sampling for Large Language Models**|Weizhe Chen et.al.|[2410.21236](http://arxiv.org/abs/2410.21236)|null|
|**2024-10-28**|**Lifting the Veil on the Large Language Model Supply Chain: Composition, Risks, and Mitigations**|Kaifeng Huang et.al.|[2410.21218](http://arxiv.org/abs/2410.21218)|null|
|**2024-10-28**|**M2rc-Eval: Massively Multilingual Repository-level Code Completion Evaluation**|Jiaheng Liu et.al.|[2410.21157](http://arxiv.org/abs/2410.21157)|null|
|**2024-10-28**|**Palisade -- Prompt Injection Detection Framework**|Sahasra Kokkula et.al.|[2410.21146](http://arxiv.org/abs/2410.21146)|null|
|**2024-10-28**|**LLM-initialized Differentiable Causal Discovery**|Shiv Kampani et.al.|[2410.21141](http://arxiv.org/abs/2410.21141)|null|
|**2024-10-28**|**Do LLMs generate test oracles that capture the actual or the expected program behaviour?**|Michael Konstantinou et.al.|[2410.21136](http://arxiv.org/abs/2410.21136)|null|
|**2024-10-25**|**Counting Ability of Large Language Models and Impact of Tokenization**|Xiang Zhang et.al.|[2410.19730](http://arxiv.org/abs/2410.19730)|**[link](https://github.com/juntaic7/impact-of-tokenization-in-the-counting-ability-of-language-models)**|
|**2024-10-25**|**FISHNET: Financial Intelligence from Sub-querying, Harmonizing, Neural-Conditioning, Expert Swarms, and Task Planning**|Nicole Cho et.al.|[2410.19727](http://arxiv.org/abs/2410.19727)|null|
|**2024-10-25**|**2D-DPO: Scaling Direct Preference Optimization with 2-Dimensional Supervision**|Shilong Li et.al.|[2410.19720](http://arxiv.org/abs/2410.19720)|null|
|**2024-10-25**|**Less is More: Extreme Gradient Boost Rank-1 Adaption for Efficient Finetuning of LLMs**|Yifei Zhang et.al.|[2410.19694](http://arxiv.org/abs/2410.19694)|null|
|**2024-10-25**|**APRICOT: Active Preference Learning and Constraint-Aware Task Planning with LLMs**|Huaxiaoyue Wang et.al.|[2410.19656](http://arxiv.org/abs/2410.19656)|null|
|**2024-10-25**|**Take Caution in Using LLMs as Human Surrogates: Scylla Ex Machina**|Yuan Gao et.al.|[2410.19599](http://arxiv.org/abs/2410.19599)|null|
|**2024-10-25**|**Diverse Sign Language Translation**|Xin Shen et.al.|[2410.19586](http://arxiv.org/abs/2410.19586)|null|
|**2024-10-25**|**ChunkRAG: Novel LLM-Chunk Filtering Method for RAG Systems**|Ritvik Aggarwal Ishneet Sukhvinder Singh Ibrahim Allahverdiyev et.al.|[2410.19572](http://arxiv.org/abs/2410.19572)|null|
|**2024-10-25**|**Brain-like Functional Organization within Large Language Models**|H. Sun et.al.|[2410.19542](http://arxiv.org/abs/2410.19542)|null|
|**2024-10-25**|**Detection of Human and Machine-Authored Fake News in Urdu**|Muhammad Zain Ali et.al.|[2410.19517](http://arxiv.org/abs/2410.19517)|**[link](https://github.com/zainali93/UrduHMFND2024)**|
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
|**2024-09-30**|**VideoINSTA: Zero-shot Long Video Understanding via Informative Spatial-Temporal Reasoning with LLMs**|Ruotong Liao et.al.|[2409.20365](http://arxiv.org/abs/2409.20365)|**[link](https://github.com/mayhugotong/videoinsta)**|
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
|**2024-09-18**|**To CoT or not to CoT? Chain-of-thought helps mainly on math and symbolic reasoning**|Zayne Sprague et.al.|[2409.12183](http://arxiv.org/abs/2409.12183)|**[link](https://github.com/zayne-sprague/to-cot-or-not-to-cot)**|
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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

## Communication Intelligence

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-09-21**|**LLM Agents as 6G Orchestrator: A Paradigm for Task-Oriented Physical-Layer Automation**|Zhuoran Xiao et.al.|[2410.03688](http://arxiv.org/abs/2410.03688)|null|生成式预训练模型的快速发展正在推动技术进步从基本应用如聊天机器人向更复杂的基于代理的系统转变。将6G系统与大型语言模型（LLM）代理和数字孪生（DT）结合具有巨大的潜力和必要性，以管理具有新出现功能（如原生AI服务和感知）的高度复杂通信系统。借助面向6G的代理，基站可以理解各种动态上层任务的传输需求，自动编排最优系统工作流程。通过不断从6G DT获取反馈进行强化，代理最终能够相应地提高实际系统的性能。不同于为通用应用设计的现有LLM代理，面向6G的代理旨在利用大量额外的专业知识做出高度严谨和精确的规划，这不可避免地需要从模型训练到实施的特定系统设计。本文提出了一种构建面向任务的6G LLM代理的新综合方法。我们首先提出了一种两阶段持续预训练和微调方案，用于构建领域基础模型和满足各种应用场景需求的各种专业化专家模型。此外，还提出了一种基于语义检索的新推理框架，以利用现有的通信相关功能。物理层任务分解等示例任务的实验结果表明了所提范式的可行性和有效性。|
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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

## RAG

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-30**|**CORAL: Benchmarking Multi-turn Conversational Retrieval-Augmentation Generation**|Yiruo Cheng et.al.|[2410.23090](http://arxiv.org/abs/2410.23090)|null|检索增强生成（RAG）已成为通过外部知识检索来增强大型语言模型（LLMs）的强大范式。尽管它受到了广泛关注，但现有的学术研究主要集中在单轮RAG上，未能解决现实应用中多轮对话的复杂性问题。为了解决这一问题，我们引入了CORAL，这是一个大规模基准测试，旨在评估在现实多轮对话场景中的RAG系统。CORAL包含了从维基百科自动衍生出的多样化信息寻求对话，并解决了诸如开放领域覆盖、知识密集度、自由形式响应和话题转换等关键挑战。它支持会话RAG的三个核心任务：段落检索、响应生成和引用标注。我们提出了一种统一框架来标准化各种会话RAG方法，并对这些方法在CORAL上的表现进行了全面评估，展示了改进现有方法的巨大潜力。|
|**2024-10-30**|**Emotional RAG: Enhancing Role-Playing Agents through Emotional Retrieval**|Le Huang et.al.|[2410.23041](http://arxiv.org/abs/2410.23041)|null|随着大型语言模型（LLMs）展现出高度的人类能力，越来越多的关注被放在了角色扮演研究领域，在这些领域中，由LLMs生成的回复被期望能够模仿人类的回答。这促进了角色扮演代理在各种应用中的探索，例如可以与用户进行自然对话的聊天机器人以及可以提供个性化支持和指导的虚拟助手。角色扮演任务中的关键因素是有效利用角色记忆，这种记忆存储了角色的档案、经历和历史对话。检索增强生成（RAG）技术被用来访问相关记忆以增强角色扮演代理的响应生成。大多数现有的研究基于记忆的语义相似性来检索相关信息，以保持角色的个性化特征，而在检索增强生成（RAG）过程中很少尝试整合情绪因素。受到情绪依赖记忆理论的启发——该理论指出，如果人们能够在回忆时重新体验到学习时的情绪状态，则能更好地回忆起某一事件——我们提出了一种新的情感感知记忆检索框架，称为情感RAG，它在角色扮演代理中考虑情绪状态来召回相关记忆。具体来说，我们设计了两种检索策略，即组合策略和顺序策略，在检索过程中同时结合记忆语义和情绪状态。在三个代表性角色扮演数据集上的广泛实验表明，我们的情感RAG框架在维持角色扮演代理个性方面优于不考虑情绪因素的方法。这为进一步强化心理学中的情绪依赖记忆理论提供了证据。|
|**2024-10-31**|**Long $^2$ RAG: Evaluating Long-Context & Long-Form Retrieval-Augmented Generation with Key Point Recall**|Zehan Qi et.al.|[2410.23000](http://arxiv.org/abs/2410.23000)|null|检索增强生成（RAG）是一种有前景的方法，用于解决大型语言模型（LLMs）中固定知识的局限性。然而，当前用于评估RAG系统的基准存在两个主要不足：(1) 由于缺乏反映检索文档特征的数据集，它们未能充分衡量LLMs处理长上下文检索的能力；(2) 缺乏全面评估LLMs利用检索信息生成长篇响应能力的方法。为了解决这些不足，我们引入了Long²RAG基准和关键点召回率（KPR）指标。Long²RAG包含跨越10个领域的280个问题，涵盖8个问题类别，每个问题都关联着5篇检索文档，平均长度为2,444词。KPR评估LLMs在生成的回答中纳入从检索文档提取的关键点的程度，从而更细致地评估其利用检索信息的能力。|
|**2024-10-30**|**Semantic Enrichment of the Quantum Cascade Laser Properties in Text- A Knowledge Graph Generation Approach**|Deperias Kerre et.al.|[2410.22996](http://arxiv.org/abs/2410.22996)|null|一种结构良好的量子级联激光器（QCL）设计和工作特性数据集合为分析和理解这些特性之间的关系提供了平台。通过分析这些关系，我们可以深入了解不同设计特征如何影响激光性能特性，如工作温度。大多数QCL特性都记录在科学文本中。因此，需要有效的方法来从文本中提取QCL特性，并生成一个语义丰富且互相关联的平台，在这个平台上可以分析这些特性以揭示隐藏的关系。同时还需要保持基于这些特性的来源和参考信息。诸如本体论和知识图谱等语义网技术已经在各种领域展示了提供互相关联的数据平台进行知识表示的能力。在本文中，我们提出了一种方法，用于从文本生成QCL特性知识图谱，以实现特性的语义丰富化。该方法基于QCL本体论和由GPT 4-Turbo语言模型支持的信息提取管道。感兴趣的特性包括：工作温度、激光设计类型、激光频率、激光光功率以及异质结构。实验结果表明了这种方法的有效性和可行性，可以从非结构化文本中高效地提取QCL特性并生成QCL特性知识图谱，这在QCL数据的语义丰富化和分析方面具有潜在应用价值。|
|**2024-10-30**|**Retrieval-Augmented Generation with Estimation of Source Reliability**|Jeongyeon Hwang et.al.|[2410.22954](http://arxiv.org/abs/2410.22954)|null|检索增强生成（RAG）通过结合外部数据库解决了大型语言模型（LLM）的关键局限性，如幻觉和知识过时问题。这些数据库通常会咨询多个来源以涵盖最新和多样的信息。然而，标准的RAG方法往往忽略了多源数据库中不同来源的可靠性，在仅基于相关性检索文档时容易传播错误信息。为了解决这一问题，我们提出了可靠性感知的RAG（RA-RAG），该方法估计多个来源的可靠性并将这些信息纳入检索和聚合过程中。具体来说，它迭代地估计一组查询的来源可靠性和真实答案，而无需标注。然后，它从少数可靠的来源中选择性地检索相关文档，并使用加权多数投票进行聚合，这种选择性检索确保了可扩展性而不影响性能。我们还引入了一个旨在反映具有异构来源可靠性的现实世界场景的基准，并展示了与一系列基线相比RA-RAG的有效性。|
|**2024-10-30**|**Eliciting Critical Reasoning in Retrieval-Augmented Language Models via Contrastive Explanations**|Leonardo Ranaldi et.al.|[2410.22874](http://arxiv.org/abs/2410.22874)|null|检索增强生成（RAG）已成为当代自然语言处理中支持大型语言模型（LLM）系统地访问更丰富事实背景的关键机制。然而，RAG机制的集成带来了其固有的挑战，因为LLM需要处理潜在的嘈杂上下文。最近的研究表明，LLM在批判性分析基于RAG的上下文信息方面仍然存在困难，这种局限性可能导致错误推断和幻觉。在本文中，我们研究了如何通过对比解释来激发RAG中的批判性推理。特别地，我们提出了对比RAG（C-RAG），这是一个框架，它（i）根据查询检索相关文档，（ii）选择并示例相关段落，并（iii）生成明确对比段落相关性的解释以（iv）支持最终答案。我们展示了C-RAG通过从LLM构建对比推理演示来指导较小模型进行检索增强任务的影响。大量实验表明，C-RAG改进了最先进的RAG模型，同时（a）显著减少了提示和演示的数量，并且（b）对检索文档中的扰动具有鲁棒性。|
|**2024-10-30**|**HijackRAG: Hijacking Attacks against Retrieval-Augmented Large Language Models**|Yucheng Zhang et.al.|[2410.22832](http://arxiv.org/abs/2410.22832)|null|检索增强生成（RAG）系统通过整合外部知识来增强大型语言模型（LLM），使其能够适应各种应用并具有成本效益。然而，对这些系统的日益依赖也引入了潜在的安全风险。在这项工作中，我们揭示了一种新的漏洞——检索提示劫持攻击（HijackRAG），攻击者可以通过将恶意文本注入知识数据库来操纵RAG系统的检索机制。当RAG系统遇到目标问题时，它会生成攻击者预先设定的答案，而不是正确答案，从而破坏系统的完整性和可信度。我们将HijackRAG形式化为一个优化问题，并提出了针对不同攻击者知识水平的黑盒和白盒攻击策略。在多个基准数据集上的广泛实验表明，HijackRAG始终能实现高攻击成功率，超越现有的基线攻击方法。此外，我们还展示了该攻击在不同检索器模型之间的可迁移性，突显了其对RAG系统的广泛威胁。最后，我们对各种防御机制的探索表明，它们不足以对抗HijackRAG，强调了在实际部署中迫切需要更强大的安全措施来保护RAG系统。|
|**2024-10-29**|**Understanding Synthetic Context Extension via Retrieval Heads**|Xinyu Zhao et.al.|[2410.22316](http://arxiv.org/abs/2410.22316)|null|长上下文的大型语言模型（LLM）在诸如检索增强生成等应用中越来越受到需求。为了降低在长上下文上预训练LLM的成本，最近的研究采取了一种合成上下文扩展的方法：在后训练阶段使用合成生成的长上下文数据进行微调。然而，这种合成上下文扩展如何以及为何赋予模型在下游长上下文任务中的能力仍不清楚。在本文中，我们研究了三种需要检索和推理的长上下文任务上的合成数据微调。我们改变了需要检索的“针”概念的真实性和周围“干草堆”上下文的多样性，从使用LLM构建合成文档到使用模板关系并创建符号数据集。我们发现，在合成数据上训练的模型表现不如真实数据上的模型，但令人惊讶的是，这种不匹配可以通过一组特殊的注意力头来解释甚至预测，这些注意力头负责在长上下文中进行检索：检索头（Wu等人，2024）。在合成数据上学到的检索头主要是在真实数据上学到的检索头的子集，并且头部学习的召回率与模型在下游任务上的性能之间存在很强的相关性。此外，通过注意力敲除和激活修补，我们从机制上展示了检索头对于模型性能是必要的，并能解释模型性能，尽管它们并不是完全充分的。我们的结果为理解合成数据微调性能提供了启示，并指出了如何创建更好的数据以学习实际世界中的长上下文能力。|
|**2024-10-29**|**Not All Languages are Equal: Insights into Multilingual Retrieval-Augmented Generation**|Suhang Wu et.al.|[2410.21970](http://arxiv.org/abs/2410.21970)|**[link](https://github.com/H-shw/futurepedia)**|**检索增强语言模型（RALMs）通过整合外部文本资源来扩展其知识范围。然而，全球知识的多语言特性要求RALMs能够处理多种语言，这一话题在研究中受到的关注有限。在这项工作中，我们提出了一个精心设计的基准测试集Futurepedia，其中包含八种代表性语言的平行文本。我们使用该基准测试集评估了六个多语言RALMs，以探讨多语言RALMs面临的挑战。实验结果揭示了语言间的不平等现象：1）高资源语言在单语知识提取方面表现突出；2）印欧语系语言使RALMs能够直接从文档中提供答案，从而减轻了跨语言表达答案的挑战；3）英语受益于RALMs的选择偏差，在多语言知识选择中更为突出。基于这些发现，我们为改进多语言检索增强生成提供了建议。对于单语知识提取，需要特别注意将低资源语言翻译成高资源语言时可能出现的级联错误。在跨语言知识迁移中，鼓励RALMs在不同语言的文档中提供答案可以提高迁移性能。对于多语言知识选择，纳入更多非英语文档并重新定位英语文档可以帮助缓解RALMs的选择偏差。通过全面的实验，我们强调了多语言RALMs固有的复杂性，并为未来的研究提供了宝贵的见解。**|
|**2024-10-29**|**Beyond Text: Optimizing RAG with Multimodal Inputs for Industrial Applications**|Monica Riedler et.al.|[2410.21943](http://arxiv.org/abs/2410.21943)|**[link](https://github.com/riedlerm/multimodal_rag_for_industry)**|**大型语言模型（LLM）在回答问题方面展示了令人印象深刻的能力，但它们缺乏特定领域的知识，并且容易产生幻觉。检索增强生成（RAG）是一种解决这些挑战的方法，而多模态模型作为能够处理文本和图像的有前景的人工智能助手正在兴起。在本文中，我们描述了一系列实验，旨在确定如何最好地将多模态模型集成到工业领域的RAG系统中。实验的目的是确定在工业领域文档中加入图像是否能提高RAG性能，并找到这种多模态RAG系统的最佳配置。我们的实验包括两种图像处理和检索方法，以及两种用于答案合成的语言模型（GPT4-Vision和LLaVA）。这些图像处理策略涉及使用多模态嵌入和从图像生成文本摘要。我们采用“LLM作为裁判”的方法来评估实验结果。结果显示，多模态RAG可以超越单一模态RAG设置的表现，尽管图像检索比文本检索更具挑战性。此外，利用图像的文本摘要相比使用多模态嵌入来说是一个更有前途的方法，为未来的进步提供了更多机会。**|
|**2024-10-29**|**Improving In-Context Learning with Small Language Model Ensembles**|M. Mehdi Mojarradi et.al.|[2410.21868](http://arxiv.org/abs/2410.21868)|**[link](https://github.com/mehdimojarradi/Ensemble-SuperICL)**|
|**2024-10-28**|**AiSciVision: A Framework for Specializing Large Multimodal Models in Scientific Image Classification**|Brendan Hogan et.al.|[2410.21480](http://arxiv.org/abs/2410.21480)|**[link](https://github.com/gomes-lab/AiSciVision)**|
|**2024-10-28**|**Vision Search Assistant: Empower Vision-Language Models as Multimodal Search Engines**|Zhixin Zhang et.al.|[2410.21220](http://arxiv.org/abs/2410.21220)|**[link](https://github.com/cnzzx/vsa)**|
|**2024-10-28**|**CRAT: A Multi-Agent Framework for Causality-Enhanced Reflective and Retrieval-Augmented Translation with Large Language Models**|Meiqi Chen et.al.|[2410.21067](http://arxiv.org/abs/2410.21067)|null|
|**2024-10-28**|**Geo-FuB: A Method for Constructing an Operator-Function Knowledge Base for Geospatial Code Generation Tasks Using Large Language Models**|Shuyang Hou et.al.|[2410.20975](http://arxiv.org/abs/2410.20975)|**[link](https://github.com/whuhsy/geo-fub)**|
|**2024-10-28**|**AutoRAG: Automated Framework for optimization of Retrieval Augmented Generation Pipeline**|Dongkyu Kim et.al.|[2410.20878](http://arxiv.org/abs/2410.20878)|**[link](https://github.com/marker-inc-korea/autorag_aragog_paper)**|
|**2024-10-28**|**LLMs are Biased Evaluators But Not Biased for Retrieval Augmented Generation**|Yen-Shan Chen et.al.|[2410.20833](http://arxiv.org/abs/2410.20833)|null|
|**2024-10-28**|**Plan $\times$ RAG: Planning-guided Retrieval Augmented Generation**|Prakhar Verma et.al.|[2410.20753](http://arxiv.org/abs/2410.20753)|null|
|**2024-10-28**|**Simple is Effective: The Roles of Graphs and Large Language Models in Knowledge-Graph-Based Retrieval-Augmented Generation**|Mufei Li et.al.|[2410.20724](http://arxiv.org/abs/2410.20724)|null|
|**2024-10-28**|**Combining Domain-Specific Models and LLMs for Automated Disease Phenotyping from Survey Data**|Gal Beeri et.al.|[2410.20695](http://arxiv.org/abs/2410.20695)|null|
|**2024-10-27**|**R^3AG: First Workshop on Refined and Reliable Retrieval Augmented Generation**|Zihan Wang et.al.|[2410.20598](http://arxiv.org/abs/2410.20598)|null|
|**2024-10-27**|**WindTunnel -- A Framework for Community Aware Sampling of Large Corpora**|Michael Iannelli et.al.|[2410.20301](http://arxiv.org/abs/2410.20301)|null|
|**2024-10-25**|**FISHNET: Financial Intelligence from Sub-querying, Harmonizing, Neural-Conditioning, Expert Swarms, and Task Planning**|Nicole Cho et.al.|[2410.19727](http://arxiv.org/abs/2410.19727)|null|
|**2024-10-25**|**ChunkRAG: Novel LLM-Chunk Filtering Method for RAG Systems**|Ritvik Aggarwal Ishneet Sukhvinder Singh Ibrahim Allahverdiyev et.al.|[2410.19572](http://arxiv.org/abs/2410.19572)|null|
|**2024-10-24**|**PDL: A Declarative Prompt Programming Language**|Mandana Vaziri et.al.|[2410.19135](http://arxiv.org/abs/2410.19135)|**[link](https://github.com/IBM/prompt-declaration-language)**|
|**2024-10-24**|**LoRANN: Low-Rank Matrix Factorization for Approximate Nearest Neighbor Search**|Elias Jääsaari et.al.|[2410.18926](http://arxiv.org/abs/2410.18926)|**[link](https://github.com/ejaasaari/lorann)**|
|**2024-10-25**|**An LLM Agent for Automatic Geospatial Data Analysis**|Yuxing Chen et.al.|[2410.18792](http://arxiv.org/abs/2410.18792)|null|
|**2024-10-24**|**Bielik 7B v0.1: A Polish Language Model -- Development, Insights, and Evaluation**|Krzysztof Ociepa et.al.|[2410.18565](http://arxiv.org/abs/2410.18565)|null|
|**2024-10-24**|**Aggregated Knowledge Model: Enhancing Domain-Specific QA with Fine-Tuned and Retrieval-Augmented Generation Models**|Fengchen Liu et.al.|[2410.18344](http://arxiv.org/abs/2410.18344)|null|
|**2024-10-23**|**LongRAG: A Dual-Perspective Retrieval-Augmented Generation Paradigm for Long-Context Question Answering**|Qingfei Zhao et.al.|[2410.18050](http://arxiv.org/abs/2410.18050)|**[link](https://github.com/qingfei1/longrag)**|
|**2024-10-23**|**SimRAG: Self-Improving Retrieval-Augmented Generation for Adapting Large Language Models to Specialized Domains**|Ran Xu et.al.|[2410.17952](http://arxiv.org/abs/2410.17952)|null|
|**2024-10-23**|**Leveraging the Domain Adaptation of Retrieval Augmented Generation Models for Question Answering and Reducing Hallucination**|Salman Rakin et.al.|[2410.17783](http://arxiv.org/abs/2410.17783)|null|
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
|**2024-10-15**|**DynamicER: Resolving Emerging Mentions to Dynamic Entities for RAG**|Jinyoung Kim et.al.|[2410.11494](http://arxiv.org/abs/2410.11494)|**[link](https://github.com/jiny1623/dynamicer)**|
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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

## text2sql

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-30**|**BIS: NL2SQL Service Evaluation Benchmark for Business Intelligence Scenarios**|Bora Caglayan et.al.|[2410.22925](http://arxiv.org/abs/2410.22925)|**[link](https://github.com/boracaglayan/bis-nl2sql)**|**近年来，自然语言到结构化查询语言（NL2SQL）的转换在商业智能（BI）应用程序中得到了广泛应用。然而，现有的NL2SQL基准并不适合生产环境中的BI场景，因为它们不是为常见的商业智能问题设计的。为了解决这一问题，我们开发了一个新的基准，专注于工业BI场景中典型的自然语言问题。我们讨论了构建BI导向基准所面临的挑战以及现有基准的不足之处。此外，我们介绍了反映常见BI询问的问题类别。最后，我们提出了两种新颖的语义相似性评估指标，用于评估BI应用和服务中的NL2SQL能力。**|
|**2024-10-15**|**LR-SQL: A Supervised Fine-Tuning Method for Text2SQL Tasks under Low-Resource Scenarios**|Wen Wuzhenghong et.al.|[2410.11457](http://arxiv.org/abs/2410.11457)|**[link](https://github.com/hongwin/lr-sql)**|**大型语言模型通过有监督微调在Text2SQL方面取得了革命性进展，但一个关键的限制被忽视了：数据库的复杂性导致上下文长度增加，从而增加了模型微调时对GPU内存的需求。为了解决这个问题，我们提出了LR-SQL。LR-SQL包括两个有监督微调模型：schema_link模型和SQL_generation模型，其中schema_link模型是简化整个过程的核心。在对schema_link模型进行微调时，LR-SQL将完整的数据库分解成可调整数量的表的灵活组合，使模型能够从这些分散的片段中学习整个数据库中的关系。此外，为了增强模型在推理过程中感知不同离散片段之间关系的能力，LR-SQL训练了模型的Chain-of-Thought能力来完成这一任务。实验结果表明，与现有的微调方法相比，LR-SQL可以减少40%的总GPU内存使用量，而在schema_link任务中的表预测准确率仅下降2%。对于整体的Text2SQL任务，执行准确率仅下降了0.6%。我们的项目现已在https://github.com/hongWin/LR-SQL上开放。**|
|**2024-08-27**|**Text2SQL is Not Enough: Unifying AI and Databases with TAG**|Asim Biswal et.al.|[2408.14717](http://arxiv.org/abs/2408.14717)|**[link](https://github.com/tag-research/tag-bench)**|**能够通过自然语言问题访问数据库的人工智能系统有望释放巨大的价值。这样的系统允许用户利用语言模型（LMs）强大的推理和知识能力，以及数据管理系统可扩展的计算能力。这些综合能力将使用户能够对自定义数据源提出任意的自然语言问题。然而，现有的方法和基准测试未能充分探索这一领域。Text2SQL方法仅关注可以通过关系代数表达的自然语言问题，这仅代表了真实用户想要询问的问题的一小部分。同样，检索增强生成（RAG）考虑的是可以通过数据库中一个或少数几个数据记录的点查询来回答的有限子集查询。我们提出了表增强生成（TAG），这是一种统一且通用的方法，用于回答基于数据库的自然语言问题。TAG模型代表了之前未被充分探索的LM与数据库之间广泛交互的可能性，并为利用LM在数据上的世界知识和推理能力创造了令人兴奋的研究机会。我们系统地开发了研究TAG问题的基准，并发现标准方法正确回答的问题不超过20%，证实了该领域需要进一步研究。我们在https://github.com/TAG-Research/TAG-Bench上发布了基准代码。**|
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
|**2024-08-09**|**A Survey of NL2SQL with Large Language Models: Where are we, and where are we going?**|Xinyu Liu et.al.|[2408.05109](http://arxiv.org/abs/2408.05109)|**[link](https://github.com/hkustdial/nl2sql_handbook)**|**将用户的自然语言查询（NL）转换为SQL查询（即NL2SQL）可以显著降低访问关系数据库的障碍，并支持各种商业应用。随着大型语言模型（LLMs）的出现，NL2SQL的性能得到了极大的提升。在这篇综述中，我们全面回顾了由LLMs驱动的NL2SQL技术，涵盖了从以下四个方面看其整个生命周期：(1) 模型：处理不仅NL的歧义和表述不足问题，还能够正确地将NL与数据库模式和实例映射起来的NL2SQL翻译技术；(2) 数据：从训练数据收集、因训练数据稀缺而进行的数据合成到NL2SQL基准测试；(3) 评估：使用不同的指标和粒度从多个角度评估NL2SQL方法；(4) 错误分析：分析NL2SQL错误以找到根本原因，并指导NL2SQL模型进化。此外，我们为开发NL2SQL解决方案提供了经验法则。最后，我们讨论了在LLM时代NL2SQL的研究挑战和开放问题。**|
|**2024-07-21**|**Towards Automated Data Sciences with Natural Language and SageCopilot: Practices and Lessons Learned**|Yuan Liao et.al.|[2407.21040](http://arxiv.org/abs/2407.21040)|null|尽管自然语言转SQL（NL2SQL）领域在将自然语言指令转化为可执行的SQL脚本用于数据查询和处理方面取得了显著进展，但在更广泛的数据科学流程中实现全面自动化——包括数据查询、分析、可视化和报告——仍然是一个复杂的挑战。本研究介绍了一种先进的工业级系统SageCopilot，该系统通过集成大型语言模型（LLMs）、自主代理（AutoAgents）和语言用户界面（LUIs）来自动化数据科学流程。特别地，SageCopilot采用了两阶段设计：在线组件通过上下文学习（ICL）细化用户的输入为可执行脚本，并运行这些脚本来进行结果报告与可视化；离线准备演示则是根据在线阶段ICL请求而完成的。一系列流行策略如思维链和提示调优被用来增强SageCopilot的性能。通过严格的测试和与基于提示解决方案的对比分析，SageCopilot已在生成或执行脚本以及提供带有可视化的结果方面经实证验证其卓越的端到端表现，这得到了真实世界数据集的支持。我们深入的消融研究表明了SageCopilot所使用的各种组件和策略对数据科学端到端正确性的单独贡献。|
|**2024-06-12**|**DeTriever: Decoder-representation-based Retriever for Improving NL2SQL In-Context Learning**|Yuxi Feng et.al.|[2406.07913](http://arxiv.org/abs/2406.07913)|null|尽管上下文学习（ICL）已被证明是提高大型语言模型（LLMs）在多种复杂任务中表现的有效技术，尤其是在将自然语言问题转换为结构化查询语言（NL2SQL）方面，如何选择最有益的示例仍然是一个开放的研究问题。虽然之前的工作通常采用现成的编码器来动态检索示例，但外部检索器和LLM之间存在固有的表示能力差异。此外，优化示例选择是一项非平凡的任务，因为没有直接的方法可以在不进行成对推理的情况下评估示例的相对收益。为了解决这些问题，我们提出了DeTriever，这是一种新颖的演示检索框架，它学习了LLM隐藏状态的加权组合，其中编码了丰富的语义信息。为了训练模型，我们提出了一种代理分数，该分数基于输出查询之间的相似性来估计示例的相对收益。在两个流行的NL2SQL基准上的实验表明，我们的方法在一次性NL2SQL任务上显著优于最先进的基线。|
|**2024-07-27**|**The Dawn of Natural Language to SQL: Are We Fully Ready?**|Boyan Li et.al.|[2406.01265](http://arxiv.org/abs/2406.01265)|**[link](https://github.com/hkustdial/nl2sql360)**|**将用户的自然语言问题转换为SQL查询（即NL2SQL）显著降低了访问关系数据库的门槛。大型语言模型的出现为NL2SQL任务引入了新的范式，极大地增强了其能力。然而，这引发了一个关键问题：我们是否已经完全准备好将NL2SQL模型投入生产？为了解决这个问题，我们提出了一种多角度的NL2SQL评估框架NL2SQL360，以帮助研究人员设计和测试新的NL2SQL方法。通过NL2SQL360，我们对领先的NL2SQL方法在不同应用场景下进行了详细的比较，如不同的数据领域和SQL特性，提供了宝贵的信息来选择最适合特定需求的NL2SQL方法。此外，我们探索了NL2SQL设计空间，利用NL2SQL360自动化地识别出针对用户特定需求的最佳NL2SQL解决方案。特别地，NL2SQL360在Spdier数据集上使用执行准确度指标识别出一种有效的NL2SQL方法SuperSQL。值得注意的是，SuperSQL在Spider和BIRD测试集上分别达到了87%和62.66%的竞争性执行准确度。**|
|**2024-05-01**|**ChatBI: Towards Natural Language to Complex Business Intelligence SQL**|Jinqing Lian et.al.|[2405.00527](http://arxiv.org/abs/2405.00527)|null|自然语言转SQL（NL2SQL）技术为不熟悉数据库的非专家用户提供了一个使用SQL进行数据分析的机会。将自然语言转换为商业智能（NL2BI）是实际生产系统中NL2SQL的一个流行应用场景。与NL2SQL相比，NL2BI引入了更多挑战。在本文中，我们提出了ChatBI，这是一种全面而高效的技术，用于解决NL2BI任务。首先，我们分析了交互模式，这是NL2SQL和NL2BI在使用上一个重要的不同模块，并设计了一个更小且成本更低的模型来匹配这种交互模式。在BI场景中，表包含大量的列，这使得依赖大型语言模型（LLMs）进行模式链接的现有NL2SQL方法由于令牌限制而无法继续。此外，BI场景中模糊列的比例更高也使模式链接变得困难。ChatBI结合了数据库社区中的现有视图技术，首先将模式链接问题分解为单个视图选择问题，然后使用一个更小且成本更低的机器学习模型来选择具有显著减少列数的单一视图。接着，这个单一视图的列被作为模式链接所需的列传递给LLM。最后，ChatBI提出了一种不同于现有流程的分阶段过程流，这使得ChatBI能够更准确地生成包含复杂语义和比较关系的SQL。我们已经在百度的数据平台上部署了ChatBI，并将其集成到多条产品线中进行了大规模的生产任务评估。所获得的结果突显了其在实用性、通用性和效率方面的优越性。同时，在我们的真实BI场景数据表和查询下，与当前主流的NL2SQL技术相比，它也取得了最佳结果。|
|**2024-03-29**|**PURPLE: Making a Large Language Model a Better SQL Writer**|Tonghui Ren et.al.|[2403.20014](http://arxiv.org/abs/2403.20014)|null|大型语言模型（LLM）技术在自然语言到SQL（NL2SQL）翻译中发挥着越来越重要的作用。通过广泛语料库训练的LLM具有强大的自然语言理解和基本的SQL生成能力，无需针对NL2SQL任务进行额外调整。现有的基于LLM的NL2SQL方法试图通过增强用户意图理解来改进翻译效果。然而，由于缺乏组织复杂逻辑运算符组合的知识，LLM有时无法生成适当的SQL。一种有前景的方法是向LLM输入示例，这些示例包括来自各种数据库的已知NL2SQL翻译。LLM可以从给定任务的输入示例中学习如何组织运算符组合。在这篇论文中，我们提出了PURPLE（利用预训练模型检索用于逻辑增强的提示），它通过检索包含当前NL2SQL任务所需逻辑运算符组合的示例来提高准确性，从而引导LLM产生更好的SQL翻译。PURPLE在流行的NL2SQL基准测试Spider的验证集上达到了80.5%的确切集合匹配准确率和87.8%的执行匹配准确率的新高水平。PURPLE在不同基准、预算限制和各种LLM下保持高准确性，显示出鲁棒性和成本效益。|
|**2024-03-24**|**SQL-Encoder: Improving NL2SQL In-Context Learning Through a Context-Aware Encoder**|Mohammadreza Pourreza et.al.|[2403.16204](http://arxiv.org/abs/2403.16204)|null|检测查询之间的结构相似性对于在上下文学习模型中选择示例至关重要。然而，仅基于查询的自然语言表达而不考虑SQL查询来评估结构相似性是一个重大挑战。本文探讨了这一相似性度量的重要性，并提出了一种能够准确估计它的模型。为此，我们利用了一个包含17万对问题的数据集，精心策划以训练一个相似性预测模型。全面的评估表明，所提出的模型能够很好地捕捉问题之间的结构相似性，这一点通过肯德尔-陶距离和精确度@k指标的改进得到了证明。值得注意的是，我们的模型超越了来自OpenAI和Cohere的强大竞争性嵌入模型。此外，与这些竞争性模型相比，我们提出的编码器在1-shot上下文学习场景中提升了NL2SQL模型的下游性能，其中GPT-3.5-turbo提高了1-2%，CodeLlama-7B提高了4-8%，CodeLlama-13B提高了2-3%。|
|**2024-06-02**|**PET-SQL: A Prompt-Enhanced Two-Round Refinement of Text-to-SQL with Cross-consistency**|Zhishuai Li et.al.|[2403.09732](http://arxiv.org/abs/2403.09732)|**[link](https://github.com/zhshlii/petsql)**|
|**2024-09-05**|**Aligning Large Language Models to a Domain-specific Graph Database for NL2GQL**|Yuanyuan Liang et.al.|[2402.16567](http://arxiv.org/abs/2402.16567)|null|
|**2024-08-06**|**Intent-Based Access Control: Using LLMs to Intelligently Manage Access Control**|Pranav Subramaniam et.al.|[2402.07332](http://arxiv.org/abs/2402.07332)|null|

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

## PPC

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-31**|**(FL) $^2$: Overcoming Few Labels in Federated Semi-Supervised Learning**|Seungjoo Lee et.al.|[2410.23227](http://arxiv.org/abs/2410.23227)|**[link](https://github.com/seungjoo-ai/FLFL-NeurIPS24)**|**联邦学习（FL）是一种分布式机器学习框架，能够在保护客户隐私敏感数据的同时训练出准确的全局模型。然而，大多数FL方法假设客户端拥有带标签的数据，这在实际中往往不是这样。联邦半监督学习（FSSL）解决了标签不足的问题，针对的是只有服务器拥有少量带标签数据而客户端没有的情况。但是，集中式半监督学习（SSL）和FSSL之间存在显著的性能差距。这种差距是由于确认偏差造成的，在FSSL中更为明显，因为多轮本地训练周期以及有标签和无标签数据的分离加剧了这一问题。我们提出了$(FL)^2$ ，这是一种使用尖锐度感知一致性正则化的无标签客户端鲁棒训练方法。我们表明，对原始伪标签损失进行正则化是次优的，因此我们精心选择了用于正则化的无标签样本。我们进一步引入了客户端特定的自适应阈值和学习状态感知聚合来根据每个客户端的学习进度调整训练过程。我们在三个基准数据集上的实验表明，我们的方法显著提高了性能，并缩小了与SSL之间的差距，特别是在标签数据稀缺的情况下。**|
|**2024-10-30**|**Federated Learning under Periodic Client Participation and Heterogeneous Data: A New Communication-Efficient Algorithm and Analysis**|Michael Crawshaw et.al.|[2410.23131](http://arxiv.org/abs/2410.23131)|null|在联邦学习中，通常假设客户端总是可以参与训练，这在实际的用户设备中可能并不现实。最近的一些工作分析了在更现实的参与模式下的联邦学习，例如循环客户端可用性或任意参与。然而，所有这些工作要么需要强假设（例如，所有客户端几乎肯定在有限窗口内参与），要么不能实现线性加速和减少通信轮次，或者不适用于一般的非凸设置。在这项工作中，我们专注于非凸优化，并考虑一种参与模式，在这种模式下，所有客户端在一个固定轮次窗口内的参与机会是相等的，这包括循环客户端可用性作为特殊情况。在这种设定下，我们提出了一种新算法，名为Amplified SCAFFOLD，并证明它能够同时实现线性加速、减少通信和对数据异质性的鲁棒性。特别地，对于循环参与情况，我们的算法被证明能够在非凸随机设置中找到 $\epsilon$-平稳点所需通信轮次为$\mathcal{O}(\epsilon^{-2})$。相比之下，相同设定下的先前工作需要$\mathcal{O}(\kappa^2 \epsilon^{-4})$通信轮次，其中$\kappa$表示数据异质性。因此，由于在$\epsilon$和$\kappa$方面有更好的依赖关系，我们的算法显著减少了通信轮次。我们的分析依赖于对客户端参与与控制变量误差之间嵌套依赖关系的细致处理，从而比之前的工作提供了更紧的保证。我们还通过(1)合成数据和(2)大量客户端($N = 250$ )的真实世界数据提供了实验结果，展示了我们的算法在周期性客户端参与下的有效性。|
|**2024-10-31**|**Why Gradient Subspace? Identifying and Mitigating LoRA's Bottlenecks in Federated Fine-Tuning of Large Language Models**|Navyansh Mahla et.al.|[2410.23111](http://arxiv.org/abs/2410.23111)|null|大型语言模型（LLM）在文本和视觉数据的任务泛化方面展示了卓越的能力。虽然微调这些模型可以显著提高其在特定下游任务上的性能，但这通常需要高质量的数据，而这些数据由于隐私问题无法共享。联邦学习（FL）为无需直接数据共享的协作训练提供了一个有前景的解决方案。然而，在FL中用于LLM的许多基于低秩适应（LoRA）的参数高效微调策略存在局限性。在这篇论文中，我们批判性地分析了使用LoRA的流行FL框架的收敛性和性能保证，指出了由于低秩矩阵的受限子空间学习而导致的次优性质。这种限制阻碍了LLM在联邦设置中的有效微调。通过严格的分析和实证评估，我们证明了直接权重平均优于基于LoRA的策略，从而为微调模型带来更优越的性能。我们的全面比较揭示了LoRA方法的低效，并强调了直接权重聚合的优势。我们将分析扩展到局部训练步骤中使用的低秩梯度优化器，如GaLore。我们的研究结果表明，GaLore是一种更有效的替代方案，在文本和图像模态上都优于联邦LoRA方法，如FlexLoRA和FFA-LoRA。尽管隐私在FL讨论中仍然至关重要，但我们的重点是评估联邦微调模型的性能结果，并从理论和实证角度评价各种FL框架。我们的发现主张重新评估FL环境中对LoRA的依赖，为更高效的训练方法铺平道路。|
|**2024-10-30**|**A Study of Secure Algorithms for Vertical Federated Learning: Take Secure Logistic Regression as an Example**|Huan-Chih Wang et.al.|[2410.22960](http://arxiv.org/abs/2410.22960)|null|进入大数据时代后，越来越多的公司利用机器学习技术来构建服务。然而，对于公司来说，收集数据并自行提取有用的手工特征成本很高。虽然与其他公司的数据结合可以提升模型性能，但这种做法可能受到法律限制。换句话说，在与他人共享数据和防止隐私泄露之间找到平衡是一个值得关注的重要话题。本文聚焦于分布式数据，并在垂直联邦学习框架下执行安全的模型训练任务。这里，“安全”意味着整个过程是在加密域中执行的，因此隐私问题得到了解决。|
|**2024-10-30**|**CopRA: A Progressive LoRA Training Strategy**|Zhan Zhuang et.al.|[2410.22911](http://arxiv.org/abs/2410.22911)|null|低秩适应（LoRA）是一种参数高效的快速微调基础模型的技术。在标准的LoRA训练过程中，模型往往会迅速收敛到接近初始化的一个局部最优解。然而，这个局部最优解可能不适用于分布外数据或任务，如模型合并和剪枝。在这项工作中，我们提出了一种新的渐进式训练策略，该策略结合了随机层丢弃。此策略还优化了每层LoRA参数的Shapley值，将每一层视为合作博弈中的一个参与者。我们将这种方法称为合作LoRA（CopRA）。我们的实验结果表明，使用CopRA训练的参数表现出线性模式连接性，这使得模型合并更加高效。这也为通过LoRA合并实现联邦学习和多任务学习铺平了道路。此外，通过优化Shapley值，CopRA在剪枝任务中表现出色。|
|**2024-10-30**|**Federated UCBVI: Communication-Efficient Federated Regret Minimization with Heterogeneous Agents**|Safwan Labbi et.al.|[2410.22908](http://arxiv.org/abs/2410.22908)|null|在本文中，我们提出了联邦上置信界值迭代算法（Fed-UCBVI），这是对UCBVI算法（Azar等人，2017）的一种新颖扩展，专门针对联邦学习框架进行了调整。我们证明了Fed-UCBVI的遗憾界为约O(√(H^3 S A T / M))，其中S是状态数量，A是动作数量，H是情节长度，M是智能体数量，T是情节数量。此外，还有一个由于异质性导致的小额外项。值得注意的是，在单智能体设置下，此上界与最小极大下界匹配至多对数因子，而在多智能体场景中，Fed-UCBVI具有线性加速效果。为了进行我们的分析，我们引入了一种新的异质性度量方法，该方法可能具有独立的理论价值。此外，我们还展示了与现有的联邦强化学习方法不同，Fed-UCBVI的通信复杂度仅随智能体数量略有增加。|
|**2024-10-30**|**Towards Robust and Efficient Federated Low-Rank Adaptation with Heterogeneous Clients**|Jabin Koo et.al.|[2410.22815](http://arxiv.org/abs/2410.22815)|null|联邦微调在大型语言模型（LLMs）中由于传输大型模型更新的通信开销巨大而受到关注。低秩适应（LoRA）被提出作为一种解决方案，但在联邦学习中的应用因聚合不一致而变得复杂。现有的解决这种不一致的方法在低秩和数据异构性高的情况下往往会出现性能下降。为此，我们提出了LoRA-A2（交替冻结与自适应秩选择的低秩适应），该方法在低秩和高数据异构性的挑战性设置下表现出鲁棒性。实验结果表明，即使在极端异构性和低秩条件下，LoRA-A2仍能保持性能，并且与全微调相比，上传参数减少了高达99.8%，同时不牺牲性能。这种自适应机制提高了联邦微调的鲁棒性和通信效率，使得LLMs能够在资源受限的环境中实际部署。|
|**2024-10-30**|**Byzantine-Robust Federated Learning: An Overview With Focus on Developing Sybil-based Attacks to Backdoor Augmented Secure Aggregation Protocols**|Atharv Deshmukh et.al.|[2410.22680](http://arxiv.org/abs/2410.22680)|null|联邦学习（FL）范式使大量客户端能够在其私有数据上协作训练机器学习模型。然而，由于其多方性质，传统的FL方案容易受到试图通过注入恶意后门来损害模型性能的拜占庭攻击。已经提出了各种各样的预防方法来保护框架免受此类攻击。本文提供了一个详尽且最新的现有方法和框架的分类，然后深入分析了联邦学习鲁棒性（RoFL）协议的优点和缺点。在此基础上，我们提出了两种新的基于Sybil的攻击，这些攻击利用了RoFL中的漏洞。最后，我们以全面的未来测试建议结束，描述并详细说明了所提出的攻击的实现，并为RoFL协议以及整个拜占庭鲁棒框架提供了改进方向。|
|**2024-10-30**|**FISC: Federated Domain Generalization via Interpolative Style Transfer and Contrastive Learning**|Dung Thuy Nguyen et.al.|[2410.22622](http://arxiv.org/abs/2410.22622)|null|联邦学习（FL）在保护隐私和实现协作学习方面显示出潜力。然而，大多数当前的解决方案主要关注从单一领域收集的私有数据。当客户端数据来自不同领域（即领域迁移）时，会导致在未见领域上的性能较差，这构成了一个重大挑战。现有的联邦领域泛化方法解决了这个问题，但它们假设每个客户端持有整个领域的数据，这限制了其在具有领域异质性和客户端采样现实场景中的实用性。为了解决这一问题，我们引入了FISC，这是一种新的FL领域泛化范式，能够处理客户端之间更复杂的领域分布。FISC通过从局部风格中提取插值风格并采用对比学习来实现跨领域的学习。这种策略使客户端获得多领域表示和无偏收敛目标。在多个数据集上的实证结果，包括PACS、Office-Home和IWildCam，表明FISC优于最先进的方法。我们的方法在未见领域上实现了3.64%到57.22%的准确率提升。我们的代码可以在https://anonymous.4open.science/r/FISC-AAAI-16107获取。|
|**2024-10-29**|**Vertical Federated Learning with Missing Features During Training and Inference**|Pedro Valdeira et.al.|[2410.22564](http://arxiv.org/abs/2410.22564)|null|垂直联邦学习从跨多个客户端的特征分割数据集中训练模型，这些客户端在不共享本地数据的情况下进行协作。标准方法假设在训练和推理过程中所有特征分区都可用。然而，在实践中，这一假设很少成立，因为对于许多样本来说，只有一部分客户端观察到它们的分区。然而，不在训练中利用不完整的样本会损害泛化能力，而在推理中不支持这些样本则限制了模型的实用性。此外，如果任何客户端在训练后离开联邦，其分区将变得不可用，导致所学模型无法使用。因此，缺失特征块是限制垂直联邦学习在实际场景中应用的关键挑战。为了解决这个问题，我们提出了LASER-VFL，这是一种基于拆分神经网络模型的垂直联邦学习方法，能够处理任意集合的分区。我们的方法简单而有效，依赖于策略性地共享模型参数以及任务采样来训练一系列预测器。我们表明，对于非凸目标，LASER-VFL可以达到 $\mathcal{O}({1}/{\sqrt{T}})$的收敛率；对于足够大的批量大小，可以达到$\mathcal{O}({1}/{T})$ 的收敛率；并且在Polyak-{\L}ojasiewicz不等式下具有线性收敛速度。数值实验显示，即使在没有缺失特征的情况下，LASER-VFL的表现也优于基线。例如，在CIFAR-100上，当四个特征块中的每一个以0.5的概率被观察时，准确率提高了21.4%；当所有特征都被观察时，准确率提高了12.2%。|
|**2024-10-29**|**$\mathsf{OPA}$ : One-shot Private Aggregation with Single Client Interaction and its Applications to Federated Learning**|Harish Karthikeyan et.al.|[2410.22303](http://arxiv.org/abs/2410.22303)|null|
|**2024-10-29**|**$r$Age-$k$ : Communication-Efficient Federated Learning Using Age Factor**|Matin Mortaheb et.al.|[2410.22192](http://arxiv.org/abs/2410.22192)|null|
|**2024-10-29**|**Cognitive Semantic Augmentation LEO Satellite Networks for Earth Observation**|Hong-fu Chou et.al.|[2410.21916](http://arxiv.org/abs/2410.21916)|null|
|**2024-10-29**|**Online Mirror Descent for Tchebycheff Scalarization in Multi-Objective Optimization**|Meitong Liu et.al.|[2410.21764](http://arxiv.org/abs/2410.21764)|null|
|**2024-10-29**|**BF-Meta: Secure Blockchain-enhanced Privacy-preserving Federated Learning for Metaverse**|Wenbo Liu et.al.|[2410.21675](http://arxiv.org/abs/2410.21675)|null|
|**2024-10-28**|**Personalized Federated Learning with Mixture of Models for Adaptive Prediction and Model Fine-Tuning**|Pouya M. Ghari et.al.|[2410.21547](http://arxiv.org/abs/2410.21547)|**[link](https://github.com/pouyamghari/Fed-POE)**|
|**2024-10-28**|**On Homomorphic Encryption Based Strategies for Class Imbalance in Federated Learning**|Arpit Guleria et.al.|[2410.21192](http://arxiv.org/abs/2410.21192)|null|
|**2024-10-28**|**Unharmful Backdoor-based Client-side Watermarking in Federated Learning**|Kaijing Luo et.al.|[2410.21179](http://arxiv.org/abs/2410.21179)|null|
|**2024-10-28**|**A Unified Solution to Diverse Heterogeneities in One-shot Federated Learning**|Jun Bai et.al.|[2410.21119](http://arxiv.org/abs/2410.21119)|null|
|**2024-10-28**|**Federated Time Series Generation on Feature and Temporally Misaligned Data**|Chenrui Fan et.al.|[2410.21072](http://arxiv.org/abs/2410.21072)|null|
|**2024-10-28**|**Enhanced channel estimation for near-field IRS-aided multi-user MIMO system via deep residual network**|Yan Wang et.al.|[2410.20992](http://arxiv.org/abs/2410.20992)|null|
|**2024-10-28**|**A Statistical Analysis of Deep Federated Learning for Intrinsically Low-dimensional Data**|Saptarshi Chakraborty et.al.|[2410.20659](http://arxiv.org/abs/2410.20659)|**[link](https://github.com/saptarshic27/fl)**|
|**2024-10-27**|**FuseFL: One-Shot Federated Learning through the Lens of Causality with Progressive Model Fusion**|Zhenheng Tang et.al.|[2410.20380](http://arxiv.org/abs/2410.20380)|**[link](https://github.com/wizard1203/fusefl)**|
|**2024-10-26**|**FL-DABE-BC: A Privacy-Enhanced, Decentralized Authentication, and Secure Communication for Federated Learning Framework with Decentralized Attribute-Based Encryption and Blockchain for IoT Scenarios**|Sathwik Narkedimilli et.al.|[2410.20259](http://arxiv.org/abs/2410.20259)|null|
|**2024-10-26**|**FedMABA: Towards Fair Federated Learning through Multi-Armed Bandits Allocation**|Zhichao Wang et.al.|[2410.20141](http://arxiv.org/abs/2410.20141)|null|
|**2024-10-26**|**Anatomical 3D Style Transfer Enabling Efficient Federated Learning with Extremely Low Communication Costs**|Yuto Shibata et.al.|[2410.20102](http://arxiv.org/abs/2410.20102)|null|
|**2024-10-25**|**MetaTrading: An Immersion-Aware Model Trading Framework for Vehicular Metaverse Services**|Hongjia Wu et.al.|[2410.19665](http://arxiv.org/abs/2410.19665)|null|
|**2024-10-25**|**FLiP: Privacy-Preserving Federated Learning based on the Principle of Least Privileg**|ShiMao Xu et.al.|[2410.19548](http://arxiv.org/abs/2410.19548)|null|
|**2024-10-28**|**Free-Rider and Conflict Aware Collaboration Formation for Cross-Silo Federated Learning**|Mengmeng Chen et.al.|[2410.19321](http://arxiv.org/abs/2410.19321)|null|
|**2024-10-24**|**Equitable Federated Learning with Activation Clustering**|Antesh Upadhyay et.al.|[2410.19207](http://arxiv.org/abs/2410.19207)|null|
|**2024-10-24**|**LanFL: Differentially Private Federated Learning with Large Language Models using Synthetic Samples**|Huiyu Wu et.al.|[2410.19114](http://arxiv.org/abs/2410.19114)|null|
|**2024-10-24**|**FedSPD: A Soft-clustering Approach for Personalized Decentralized Federated Learning**|I-Cheng Lin et.al.|[2410.18862](http://arxiv.org/abs/2410.18862)|null|
|**2024-10-24**|**Adapting MLOps for Diverse In-Network Intelligence in 6G Era: Challenges and Solutions**|Peizheng Li et.al.|[2410.18793](http://arxiv.org/abs/2410.18793)|null|
|**2024-10-24**|**Classifier Clustering and Feature Alignment for Federated Learning under Distributed Concept Drift**|Junbao Chen et.al.|[2410.18478](http://arxiv.org/abs/2410.18478)|**[link](https://github.com/chen-junbao/fedccfa)**|
|**2024-10-24**|**FedBaF: Federated Learning Aggregation Biased by a Foundation Model**|Jong-Ik Park et.al.|[2410.18352](http://arxiv.org/abs/2410.18352)|null|
|**2024-10-23**|**LEGO: Language Model Building Blocks**|Shrenik Bhansali et.al.|[2410.18287](http://arxiv.org/abs/2410.18287)|null|
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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

## moe

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-30**|**Stealing User Prompts from Mixture of Experts**|Itay Yona et.al.|[2410.22884](http://arxiv.org/abs/2410.22884)|null|混合专家（MoE）模型通过将每个令牌路由到每一层中的少数专家来提高密集语言模型的效率和可扩展性。在本文中，我们展示了攻击者如何能够安排他们的查询与受害者的查询出现在同一个样本批次中，从而利用专家选择路由完全披露受害者的提示。我们成功地在一个两层Mixtral模型上展示了这种攻击的有效性，利用了torch.topk CUDA实现中的平手处理行为。我们的结果显示，我们可以使用 $O({VM}^2)$次查询（词汇量为$V$，提示长度为$M$ ）或平均每次令牌100次查询来提取整个提示。这是首次利用架构缺陷来提取用户提示的攻击，引入了一类新的大语言模型漏洞。|
|**2024-10-29**|**ProMoE: Fast MoE-based LLM Serving using Proactive Caching**|Xiaoniu Song et.al.|[2410.22134](http://arxiv.org/abs/2410.22134)|null|大型语言模型的有前景应用往往受到边缘设备上有限GPU内存容量的限制。混合专家（MoE）模型通过仅激活计算过程中的一部分模型参数来缓解这个问题，允许未使用的参数被卸载到主机内存中，从而减少整体GPU内存需求。然而，现有的基于缓存的卸载解决方案在处理缓存未命中时是被动的，并且显著影响系统性能。在本文中，我们提出了ProMoE，这是一种新颖的主动缓存系统，它利用中间模型结果来预测后续参数使用情况。通过提前主动获取专家参数，ProMoE将加载时间从关键路径中移除，并减少了卸载的性能开销。我们的评估表明，与现有卸载解决方案相比，ProMoE在预填充和解码阶段分别实现了平均2.13倍和2.84倍的速度提升。|
|**2024-10-29**|**Efficient and Effective Weight-Ensembling Mixture of Experts for Multi-Task Model Merging**|Li Shen et.al.|[2410.21804](http://arxiv.org/abs/2410.21804)|null|多任务学习（MTL）利用共享模型完成多个任务并促进知识迁移。最近关于基于任务算术的多任务学习研究显示，合并独立微调模型的参数可以有效地实现多任务学习。然而，现有的合并方法主要在原始模型参数空间内寻求静态最优解，这往往由于任务间的内在多样性和潜在干扰导致性能下降。为了解决这一挑战，本文提出了一种权重集成专家混合（WEMoE）方法用于多任务模型合并。具体来说，我们首先通过分析Transformer模型核心模块在微调前后的参数变化来识别关键（或敏感）模块。然后，我们的WEMoE方法静态地合并非关键模块，同时将关键模块转换为专家混合（MoE）结构。在推理过程中，根据输入样本动态合并MoE中的专家模块，从而实现更灵活和自适应的合并方法。基于WEMoE，我们进一步引入了一种高效且有效的WEMoE（E-WEMoE）方法，其核心机制是消除WEMoE中关键模块的非必要元素，并在多个MoE模块间实现共享路由，从而显著减少可训练参数、总体参数数量和计算开销。实验结果表明，在不同架构和任务上，WEMoE和E-WEMoE在多任务学习性能、泛化能力和鲁棒性方面均优于现有最先进的模型合并方法。|
|**2024-10-29**|**Neural Experts: Mixture of Experts for Implicit Neural Representations**|Yizhak Ben-Shabat et.al.|[2410.21643](http://arxiv.org/abs/2410.21643)|null|隐式神经表示（INRs）在图像、形状、音频和视频重建等多种任务中表现出色。这些INRs通常从采样的输入点学习隐式场。这通常是通过使用单一网络覆盖整个域来实现的，对单个函数施加了许多全局约束。在本文中，我们提出了一种基于专家混合（MoE）的隐式神经表示方法，该方法能够学习局部分段连续函数，并同时学习如何细分域并进行局部拟合。我们展示了将专家混合架构引入现有的INR公式中，可以提高速度、准确性和内存需求。此外，我们还为门控网络引入了新的条件设置和预训练方法，以改进收敛到期望解的过程。我们在多个重建任务上评估了我们方法的有效性，包括表面重建、图像重建和音频信号重建，并展示了相比非MoE方法的性能提升。|
|**2024-10-28**|**FinTeamExperts: Role Specialized MOEs For Financial Analysis**|Yue Yu et.al.|[2410.21338](http://arxiv.org/abs/2410.21338)|null|大型语言模型（LLM），如ChatGPT、Phi3和Llama-3，正在引领人工智能的重大飞跃，因为它们可以在不进行微调的情况下将训练中的知识泛化到新任务上。然而，这些模型在金融领域的应用仍然相对有限。金融领域本质上是复杂的，需要从宏观经济趋势到微观经济分析再到定量分析等多方面的深刻理解。鉴于这种复杂性，为特定金融领域定制的专家混合型LLM可以为复杂的金融任务提供更全面的理解。在这篇论文中，我们提出了FinTeamExperts，这是一个面向角色的专业化LLM框架，结构上采用专家混合（MOEs）模式来进行金融分析。该框架通过训练每个模型专注于不同的角色：宏观分析师、微观分析师和定量分析师，模拟了一个协作团队的设置。这种基于角色的专业化增强了模型整合其领域特定专长的能力。我们通过训练三个80亿参数的模型来实现这一点，每个模型都在不同的语料库上训练，以擅长特定的金融相关角色。然后我们在下游任务上对FinTeamExperts进行指令调优，使其与实际金融任务保持一致。实验结果显示，在四个数据集中的三个上，FinTeamExperts的表现优于所有同规模甚至更大规模的模型。在第四个更为复杂任务的数据集上，FinTeamExperts依然超越了所有同规模的模型。这突显了我们基于角色专业化方法以及FinTeamExperts持续训练方法的成功。|
|**2024-10-28**|**Efficient Mixture-of-Expert for Video-based Driver State and Physiological Multi-task Estimation in Conditional Autonomous Driving**|Jiyao Wang et.al.|[2410.21086](http://arxiv.org/abs/2410.21086)|null|道路安全仍然是全球面临的一个关键挑战，每年约有135万人因交通事故死亡，这些事故通常是由人为错误引起的。随着车辆自动化水平的提高，在进行非驾驶相关任务（NDRTs）时，自动化驾驶可能会对驾驶员造成认知过载，或者如果驾驶是唯一任务，则可能导致驾驶员困倦。这迫切需要一个有效的驾驶员监控系统（DMS），能够在SAE 2/3级自动驾驶环境中评估认知负荷和困倦状态。在这项研究中，我们提出了一种新的多任务DMS，称为VDMoE，它利用RGB视频输入来非侵入性地监控驾驶员状态。通过使用关键面部特征以减少计算负载，并集成远程光电容积描记法（rPPG）以获取生理信息，我们的方法在保持效率的同时提高了检测准确性。此外，我们优化了混合专家（MoE）框架，以适应多模态输入并提高不同任务的性能。引入了一种新颖的包含先验知识的正则化方法，使模型输出与统计先验对齐，从而加速收敛并降低过拟合风险。我们通过创建一个新的数据集（MCDD）来验证我们的方法，该数据集包括来自42名参与者的RGB视频和生理指标，以及两个公共数据集。研究结果表明，VDMoE在监控驾驶员状态方面非常有效，有助于构建更安全的自动驾驶系统。代码和数据将被公开发布。|
|**2024-10-27**|**GUMBEL-NERF: Representing Unseen Objects as Part-Compositional Neural Radiance Fields**|Yusuke Sekikawa et.al.|[2410.20306](http://arxiv.org/abs/2410.20306)|null|我们提出了Gumbel-NeRF，这是一种具有后见专家选择机制的混合专家（MoE）神经辐射场（NeRF）模型，用于合成未见过物体的新视角。先前的研究表明，MoE结构能够为由许多物体组成的大规模场景提供高质量的表示。然而，我们观察到当将这种MoE NeRF模型应用于从单个或少量输入中生成未见过物体的新视角时，往往在专家边界附近产生低质量的表示。我们发现这种退化主要由前瞻性的专家选择机制引起，该机制可能导致物体形状在专家边界附近出现不自然的不连续性。Gumbel-NeRF采用了一种后见的专家选择机制，保证了即使在专家边界附近密度场也能保持连续性。使用SRN汽车数据集进行的实验表明，在各种图像质量指标上，Gumbel-NeRF优于基线方法。|
|**2024-10-25**|**DMT-HI: MOE-based Hyperbolic Interpretable Deep Manifold Transformation for Unspervised Dimensionality Reduction**|Zelin Zang et.al.|[2410.19504](http://arxiv.org/abs/2410.19504)|null|降维（DR）在数据工程和可视化等多个领域中发挥着关键作用，通过简化复杂数据集同时保留重要信息。然而，在处理高维数据时，用户面临的一个重要挑战是如何平衡DR的准确性和可解释性。传统DR方法通常需要在精度和透明度之间进行权衡，优化性能可能会导致可解释性降低，反之亦然。这种局限性在图像、表格和文本数据分析等实际应用中尤为突出，这些场景下准确性和可解释性都至关重要。为了解决这些挑战，本工作提出了基于MOE的双曲可解释深度流形变换（DMT-HI）。该方法结合了能够有效捕捉复杂层次结构的双曲嵌入与根据输入特征动态分配任务的混合专家（MOE）模型。DMT-HI通过利用双曲嵌入来表示数据的层次特性，从而提高DR准确性，并通过MOE结构明确链接输入数据、嵌入结果和关键特征，进而提升可解释性。大量实验表明，DMT-HI在DR准确性和模型可解释性方面均持续表现出色，是复杂数据分析的强大解决方案。代码可在https://github.com/zangzelin/code_dmthi获取。|
|**2024-10-25**|**Hierarchical Mixture of Experts: Generalizable Learning for High-Level Synthesis**|Weikai Li et.al.|[2410.19225](http://arxiv.org/abs/2410.19225)|null|高层次综合（HLS）是设计现场可编程门阵列（FPGA）时广泛使用的工具。HLS 通过将源代码编译成 FPGA 电路，使得使用软件编程语言进行 FPGA 设计成为可能。源代码包括一个程序（称为“内核”）和多个指导硬件合成的 pragma，如并行化、流水线等。虽然软件开发者相对容易设计程序，但设计这些 pragma 需要深厚的硬件知识，这对软件开发者来说是一个很大的挑战。最近，提出了不同的机器学习算法，例如图神经网络（GNN），通过性能预测来自动化 pragma 设计。然而，在新内核上应用训练好的模型时，显著的领域迁移往往导致性能不佳。我们提出了一种更具领域泛化能力的模型结构：两级层次化的专家混合模型（MoE），它可以灵活地适应任何 GNN 模型。不同的专家网络可以学习处理表示空间中的不同区域，并利用旧内核和新内核之间的相似模式。在低级 MoE 中，我们在程序的三个自然粒度上应用 MoE：节点、基本块和图。高级 MoE 学习聚合这三个粒度以做出最终决策。为了稳定训练层次化的 MoE，我们进一步提出了一种两阶段训练方法。广泛的实验验证了层次化 MoE 的有效性。|
|**2024-10-24**|**Read-ME: Refactorizing LLMs as Router-Decoupled Mixture of Experts with System Co-Design**|Ruisi Cai et.al.|[2410.19123](http://arxiv.org/abs/2410.19123)|null|大型语言模型（LLM）的普及促使了混合专家（MoE）架构的应用，这种架构通过动态利用专门的子网络来提高效率和性能。尽管具有诸多优势，但MoE模型在推理过程中面临着显著挑战，包括内存管理不高效以及由于模型架构与系统策略之间的设计选择不一致导致的次优批处理问题。此外，从零开始训练MoE的传统方法在成本上越来越难以承受。在本文中，我们提出了一种名为Read-ME的新框架，该框架可以将预训练的密集型LLM转换为更小的MoE模型（与“升级”通用型MoE相反），从而避免了从头开始训练带来的高昂成本。我们的方法利用激活稀疏性来提取专家。为了组合专家，我们检查了广泛采用的逐层路由器设计，并展示了其冗余性，因此引入了与MoE骨干分离的前置门控路由器，这促进了系统友好的预计算和前瞻调度，增强了基于专家的批处理和缓存。因此，我们的协同设计解决了算法和系统两个方面的重要差距，为资源受限环境中的LLM推理提供了一个可扩展且高效的替代方案。Read-ME在MMLU上比其他流行的开源密集型模型提高了多达10.1%，并将平均端到端延迟改善了高达6.1%。代码可在以下网址获取：https://github.com/VITA-Group/READ-ME。|
|**2024-10-24**|**Mixture of Parrots: Experts improve memorization more than reasoning**|Samy Jelassi et.al.|[2410.19034](http://arxiv.org/abs/2410.19034)|null|
|**2024-10-23**|**Robust and Explainable Depression Identification from Speech Using Vowel-Based Ensemble Learning Approaches**|Kexin Feng et.al.|[2410.18298](http://arxiv.org/abs/2410.18298)|null|
|**2024-10-23**|**MiLoRA: Efficient Mixture of Low-Rank Adaptation for Large Language Models Fine-tuning**|Jingfan Zhang et.al.|[2410.18035](http://arxiv.org/abs/2410.18035)|null|
|**2024-10-23**|**ExpertFlow: Optimized Expert Activation and Token Allocation for Efficient Mixture-of-Experts Inference**|Xin He et.al.|[2410.17954](http://arxiv.org/abs/2410.17954)|null|
|**2024-10-22**|**Optimizing Mixture-of-Experts Inference Time Combining Model Deployment and Communication Scheduling**|Jialong Li et.al.|[2410.17043](http://arxiv.org/abs/2410.17043)|null|
|**2024-10-22**|**CartesianMoE: Boosting Knowledge Sharing among Experts via Cartesian Product Routing in Mixture-of-Experts**|Zhenpeng Su et.al.|[2410.16077](http://arxiv.org/abs/2410.16077)|null|
|**2024-10-21**|**Generalizing Motion Planners with Mixture of Experts for Autonomous Driving**|Qiao Sun et.al.|[2410.15774](http://arxiv.org/abs/2410.15774)|**[link](https://github.com/tsinghua-mars-lab/statetransformer)**|
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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

## SSMs

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-10-28**|**Multi-Agent Reinforcement Learning with Selective State-Space Models**|Jemma Daniel et.al.|[2410.19382](http://arxiv.org/abs/2410.19382)|null|Transformer模型在包括多智能体强化学习（MARL）在内的多个领域中取得了显著成功，其中多智能体Transformer（MAT）已成为该领域的领先算法。然而，Transformer模型的一个主要缺点是其计算复杂度与输入规模呈二次关系，这使得当输入规模增大时计算成本非常高昂。这一限制阻碍了MAT在大量智能体环境中的扩展性。最近，状态空间模型（SSM）因其计算效率而受到关注，但其在MARL中的应用尚未得到探索。在这项工作中，我们研究了近期提出的SSM——Mamba在MARL中的使用，并评估它是否能在保持与MAT相当性能的同时提供显著的效率提升。我们引入了一种改进版的MAT，集成了标准和双向Mamba模块，以及一种新颖的“交叉注意力”Mamba模块。广泛的测试表明，我们的多智能体Mamba（MAM）在多个标准多智能体环境中表现与MAT相当，同时在更大数量智能体场景下展现出更优的可扩展性。这对MARL社区来说意义重大，因为它表明SSM可能取代Transformer而不牺牲性能，同时也支持更有效地扩展到更高数量的智能体。我们的项目页面可在https://sites.google.com/view/multi-agent-mamba 查看。|
|**2024-10-24**|**Taipan: Efficient and Expressive State Space Language Models with Selective Attention**|Chien Van Nguyen et.al.|[2410.18572](http://arxiv.org/abs/2410.18572)|null|高效的长上下文语言建模仍然是自然语言处理（NLP）中的一个重要挑战。尽管Transformer在语言任务中占据主导地位，但它们在处理长序列时会遇到困难，因为训练过程中的计算复杂度为二次方，并且在推理过程中内存成本线性增加。最近的状态空间模型（SSMs），如Mamba，提供了常数内存使用率的替代方案，但在需要广泛上下文检索的任务中表现不佳。我们提出了Taipan，这是一种新颖的混合架构，结合了Mamba-2和选择性注意力层（SALs）。这些SALs能够识别需要长距离交互的标记，移除不重要的特征，然后通过注意力模块增强其表示。这种方法平衡了Mamba的效率与类似Transformer在内存密集型任务中的性能。通过限制注意力预算，Taipan可以将准确预测扩展到长达100万个标记的上下文长度，同时保持计算效率。我们的实验表明，Taipan在各种规模和任务中表现出色，为高效长上下文语言建模提供了一个有前景的解决方案。|
|**2024-10-21**|**START: A Generalized State Space Model with Saliency-Driven Token-Aware Transformation**|Jintao Guo et.al.|[2410.16020](http://arxiv.org/abs/2410.16020)|null|领域泛化（DG）旨在通过从多个源域学习，使模型能够泛化到未见过的目标域。现有的DG方法主要依赖于卷积神经网络（CNNs），这些网络由于其有限的感受野而固有地学习纹理偏差，导致容易过拟合源域。虽然一些工作引入了基于变换器的方法（ViTs）用于DG，以利用全局感受野，但这些方法由于自注意力机制的二次复杂度而导致高计算成本。最近，先进的状态空间模型（SSMs），如Mamba，在监督学习任务中表现出色，通过在训练过程中实现序列长度的线性复杂度和在推理过程中快速的RNN式计算。受此启发，我们研究了Mamba模型在领域偏移下的泛化能力，并发现SSMs中的输入依赖矩阵可能会累积并放大特定领域的特征，从而阻碍模型泛化。为了解决这个问题，我们提出了一种新颖的基于SSM的架构，称为START，它通过显著性感知的令牌转换实现了最先进的性能，并为CNNs和ViTs提供了一个有竞争力的替代方案。我们的START可以有选择地扰动并抑制SSMs输入依赖矩阵中显著令牌内的特定领域特征，从而有效地减少不同领域间的差异。在五个基准测试上的广泛实验表明，START以高效的线性复杂度超越了现有的SOTA DG方法。我们的代码可以在https://github.com/lingeringlight/START获取。|
|**2024-10-21**|**Revealing and Mitigating the Local Pattern Shortcuts of Mamba**|Wangjie You et.al.|[2410.15678](http://arxiv.org/abs/2410.15678)|**[link](https://github.com/zetangforward/global_mamba)**|**大型语言模型（LLMs）由于注意力机制而取得了显著进展，但其二次复杂度和线性内存需求限制了它们在长上下文任务中的表现。最近，研究人员引入了Mamba，这是一种基于状态空间模型（SSMs）的先进模型，它提供了线性复杂度和常数内存。尽管据报道Mamba的性能可以匹配甚至超过基于注意力的模型，但我们的分析显示了一个性能差距：Mamba在涉及局部关键信息的任务中表现出色，但在需要处理分布广泛的关键信息的任务中面临挑战。我们的控制实验表明，这种不一致性源于Mamba依赖于局部模式捷径，这使得模型能够在有限的内存中记住局部关键信息，但却阻碍了它保留更分散的信息的能力。因此，我们在Mamba模型中引入了一个全局选择模块来解决这个问题。在现有和提出的合成任务以及真实世界任务上的实验表明了我们方法的有效性。值得注意的是，仅通过增加400万额外参数，我们的方法使Mamba模型（1.3亿参数）在处理分布广泛信息的任务上实现了显著提升，性能从0提高到了80.54分。**|
|**2024-10-20**|**Taming Mambas for Voxel Level 3D Medical Image Segmentation**|Luca Lumetti et.al.|[2410.15496](http://arxiv.org/abs/2410.15496)|null|最近，3D医学分割领域主要由使用卷积神经网络（CNNs）和基于Transformer架构的深度学习模型主导，每种模型都有其独特的优势和局限性。CNNs受到局部感受野的限制，而Transformers则因其巨大的内存需求和数据饥饿性，在处理3D医学体积时难以达到细粒度水平。因此，在对大尺寸3D医学体积进行结构分割时，全卷积神经网络如nnUNet仍然占据主导地位。尽管在开发具有次二次时间和内存复杂性的Transformer变体方面取得了许多进展，但这些模型在基于内容的推理方面仍显不足。最近的一个突破是Mamba，这是一种基于状态空间模型（SSMs）的循环神经网络（RNN），在许多长上下文任务（百万长度序列）中超越了Transformers的表现，包括著名的自然语言处理和基因组基准测试，并且保持了线性复杂度。|
|**2024-10-19**|**Spatial-Mamba: Effective Visual State Space Models via Structure-Aware State Fusion**|Chaodong Xiao et.al.|[2410.15091](http://arxiv.org/abs/2410.15091)|**[link](https://github.com/edwardchasel/spatial-mamba)**|**选择性状态空间模型（SSM），如Mamba，在捕捉一维序列数据中的长距离依赖关系方面表现出色，但在二维视觉任务上的应用仍面临挑战。当前的视觉SSM通常将图像转换为一维序列，并采用各种扫描模式来引入局部空间依赖性。然而，这些方法在有效捕捉复杂的图像空间结构以及由于延长的扫描路径导致的计算成本增加方面存在局限性。为了解决这些问题，我们提出了Spatial-Mamba，这是一种新颖的方法，它直接在状态空间中建立邻域连通性。除了依赖于顺序的状态转移外，我们还引入了一个结构感知状态融合方程，该方程利用空洞卷积来捕捉图像的空间结构依赖性，显著增强了视觉上下文信息的流动。Spatial-Mamba分三个阶段进行：单向扫描中的初始状态计算、通过结构感知状态融合获取空间上下文，以及使用观测方程进行最终状态计算。我们的理论分析表明，Spatial-Mamba在相同的矩阵乘法框架下统一了原始Mamba和线性注意力机制，为我们方法提供了更深层次的理解。实验结果表明，即使只进行一次扫描，Spatial-Mamba在图像分类、检测和分割任务上也能达到或超越基于SSM的最先进模型。源代码和训练好的模型可以在https://github.com/EdwardChasel/Spatial-Mamba找到。**|
|**2024-10-16**|**Rethinking Token Reduction for State Space Models**|Zheng Zhan et.al.|[2410.14725](http://arxiv.org/abs/2410.14725)|**[link](https://github.com/wuyushuwys/tor_ssm)**|**最近，状态空间模型（SSM）的最新进展引起了广泛关注，特别是在优化并行训练和处理长距离依赖关系的模型方面。像Mamba这样的架构已经通过选择性SSM扩展到了数十亿参数。为了促进Mamba在更广泛应用中的使用，探索其效率至关重要。虽然令牌减少技术提供了一种直接的后训练策略，但我们发现将现有方法直接应用于SSM会导致性能显著下降。通过深入分析，我们找出了这种失败的原因以及当前技术的局限性。作为回应，我们提出了一种针对SSM量身定制的统一后训练令牌减少方法。我们的方法结合了令牌重要性和相似性，利用了剪枝和合并的优势，设计了一种细粒度的层内令牌减少策略。大量实验表明，与现有方法相比，我们的方法在六个基准测试中使用Mamba-2时平均准确率提高了5.7%到13.1%，同时大幅降低了计算需求和内存要求。**|
|**2024-10-31**|**Provable Benefits of Complex Parameterizations for Structured State Space Models**|Yuval Ran-Milo et.al.|[2410.14067](http://arxiv.org/abs/2410.14067)|null|结构化状态空间模型（SSM）是诸如S4和Mamba等著名神经网络的核心引擎，它们是遵循特定结构的线性动力系统，最显著的是对角结构。与参数化为实数的典型神经网络模块不同，SSM通常使用复数参数化。理论上解释复数参数化对SSM的好处仍然是一个开放问题。本文朝着解决这个问题迈出了一步，通过建立实数和复数对角SSM之间的正式差异。首先，我们证明了虽然适度的维度足以使复数SSM表达所有实数SSM的映射，但要让实数SSM表达复数SSM的映射则需要高得多的维度。其次，我们证明即使实数SSM的维度足够高以表达给定映射，通常也需要其实数SSM的参数具有指数级大的值，这在实践中是无法学习到的。相比之下，复数SSM可以用适中的参数值表达任何给定映射。实验验证了我们的理论，并提示了一个潜在的理论扩展，该扩展考虑了选择性这一新的架构特性，从而达到最先进的性能。|
|**2024-10-17**|**Quamba: A Post-Training Quantization Recipe for Selective State Space Models**|Hung-Yueh Chiang et.al.|[2410.13229](http://arxiv.org/abs/2410.13229)|null|状态空间模型（SSM）已成为大型语言模型中吸引人的替代方案，它们在保持常数内存复杂度的同时达到了最先进的准确率，允许比基于注意力的网络持有更长的上下文长度。SSM在长序列建模中的卓越计算效率使其在许多场景中优于Transformer。然而，在请求密集型云服务和资源受限的边缘应用中提高SSM的效率仍然是一个艰巨的任务。SSM量化是解决这一问题的一种可能方法，使SSM更适合广泛部署，同时仍能保持其准确性。量化是一种常见的技术，用于减少模型大小并利用现代计算单元上的低比特宽度加速特性，但现有的量化技术对SSM来说并不适用。最值得注意的是，SSM在其选择性扫描机制（即线性递归）内具有高度敏感的特征图，并且在输出激活中有大量的异常值，这些在自注意力模块的令牌混合输出中是不存在的。为了解决这个问题，我们提出了一种静态8位每张量SSM量化方法，该方法通过抑制输入到选择性SSM的激活的最大值来实现更精细的量化精度，并使用Hadamard变换在无异常值的空间中量化输出激活。我们的8位权重-激活量化的Mamba 2.8B SSM受益于硬件加速，在Nvidia Orin Nano 8G上实现了1.72倍更低的生成延迟，而在零样本任务上的平均准确率仅下降了0.9%。实验表明了我们的方法在部署各种规模的基于SSM的模型于云端和边缘平台上的有效性和实际应用性。|
|**2024-10-15**|**UmambaTSF: A U-shaped Multi-Scale Long-Term Time Series Forecasting Method Using Mamba**|Li Wu et.al.|[2410.11278](http://arxiv.org/abs/2410.11278)|null|多变量时间序列预测在交通、气象和金融等领域尤为重要，特别是在预测极端天气事件方面。目前最先进的方法主要依赖于Transformer架构，该架构利用注意力机制来捕捉时间依赖性。然而，这些方法受到二次时间复杂度的限制，这使得模型的可扩展性受限于输入序列长度，极大地限制了它们在实际中的应用。基于状态空间模型（SSM）的Mamba提供了一种具有线性时间复杂度的解决方案，提高了对序列数据进行高效预测的可能性。在这项研究中，我们提出了UmambaTSF，这是一种新颖的长期时间序列预测框架，它将U形编码器-解码器多层感知机（MLP）的多尺度特征提取能力与Mamba的长序列表示相结合。为了提高性能和效率，框架中引入的Mamba模块采用了改进的残差结构和自适应设计，能够捕捉独特的时间信号并灵活处理通道。实验表明，UmambaTSF在广泛使用的基准数据集上达到了最先进的性能，并且具有出色的通用性，同时保持了线性时间复杂度和低内存消耗。|
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

<p align=right>(<a href=#updated-on-20241101>back to top</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[contributors-url]: https://github.com/Vincentqyw/cv-arxiv-daily/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[forks-url]: https://github.com/Vincentqyw/cv-arxiv-daily/network/members
[stars-shield]: https://img.shields.io/github/stars/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[stars-url]: https://github.com/Vincentqyw/cv-arxiv-daily/stargazers
[issues-shield]: https://img.shields.io/github/issues/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[issues-url]: https://github.com/Vincentqyw/cv-arxiv-daily/issues

