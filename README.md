[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## Updated on 2025.05.25
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
|**2025-05-22**|**Beyond Correlation: Towards Causal Large Language Model Agents in Biomedicine**|Adib Bazgir et.al.|[2505.16982](http://arxiv.org/abs/2505.16982)|null|大型语言模型（LLM）在生物医学领域显示出潜力，但缺乏真正的因果理解，而是依赖于相关性。本文设想了能够整合多模态数据（文本、图像、基因组等）并通过干预推理来推断因果关系的因果LLM代理。解决这一问题需要克服几个关键挑战：设计安全可控的代理框架；开发严格的因果评估基准；整合异构数据源；以及协同结合LLM与结构化知识（KG）和正式因果推理工具。这样的代理可以解锁变革性的机会，包括通过自动化假设生成和模拟加速药物发现，通过患者特定的因果模型实现个性化医疗。这一研究议程旨在促进跨学科努力，将因果概念与基础模型结合起来，以开发可靠的AI伙伴，推动生物医学的进步。|
|**2025-05-22**|**A Comprehensive Evaluation of Contemporary ML-Based Solvers for Combinatorial Optimization**|Shengyu Feng et.al.|[2505.16952](http://arxiv.org/abs/2505.16952)|null|机器学习（ML）在支持组合优化（CO）问题的模型设计和优化方面展示了巨大的潜力。然而，迄今为止的许多进展都是在小规模、合成数据集上评估的，这引发了关于基于ML的求解器在现实世界大规模CO场景中实际效果的担忧。此外，许多现有的CO基准缺乏足够的训练数据，限制了它们对数据驱动方法评估的实用性。为了解决这些局限性，我们引入了FrontierCO，这是一个全面的基准，涵盖了八种典型的CO问题类型，并评估了16种代表性的基于ML的求解器——包括图神经网络和大型语言模型（LLM）代理。FrontierCO包含从工业应用和前沿CO研究中抽取的具有挑战性的实例，提供了现实的问题难度和丰富的训练数据。我们的实证结果提供了关于当前ML方法优势和局限性的关键见解，有助于指导在机器学习和组合优化交叉领域更稳健且实际相关的进步。我们的数据可在https://huggingface.co/datasets/CO-Bench/FrontierCO获取。|
|**2025-05-22**|**AGENTIF: Benchmarking Instruction Following of Large Language Models in Agentic Scenarios**|Yunjia Qi et.al.|[2505.16944](http://arxiv.org/abs/2505.16944)|null|大型语言模型（LLM）在现实世界的代理应用中展示了先进的能力。越来越多的研究致力于开发基于LLM的代理以应对实际需求，这引入了一个新的挑战：代理场景通常涉及包含复杂约束的冗长指令，例如扩展的系统提示和详细的工具规范。虽然遵循这些指令对于代理应用至关重要，但LLM是否能够可靠地遵循这些指令仍待深入研究。在这篇论文中，我们介绍了AgentIF，这是第一个系统评估LLM在代理场景下指令跟随能力的基准。AgentIF具有三个关键特征：(1) 现实性，由50个真实世界的代理应用构建而成；(2) 长度大，平均每条指令1,723词，最长达到15,630词；(3) 复杂性，平均每条指令包含11.9个约束条件，涵盖多样化的约束类型，如工具规范和条件约束。为了构建AgentIF，我们从工业应用代理和开源代理系统中收集了跨越50个代理任务的707个人工标注的指令。对于每条指令，我们都标注了相关的约束及其对应的评估指标，包括基于代码的评估、基于LLM的评估以及混合代码-LLM评估。我们使用AgentIF系统地评估现有的先进LLM。观察发现，当前模型总体表现不佳，尤其是在处理复杂的约束结构和工具规范方面。我们进一步进行了错误分析及关于指令长度和元约束的分析实验，揭示了一些现有LLM失败模式的发现。我们已发布了代码和数据以促进未来的研究。|
|**2025-05-22**|**Beyond Needle(s) in the Embodied Haystack: Environment, Architecture, and Training Considerations for Long Context Reasoning**|Bosung Kim et.al.|[2505.16928](http://arxiv.org/abs/2505.16928)|null|我们介绍了 $\infty$-THOR，这是一个针对长时域具身任务的新框架，旨在推进具身人工智能中的长上下文理解。$\infty$ -THOR提供了：(1) 一个生成框架，用于合成可扩展、可重复且无限的长时域轨迹；(2) 一种新颖的具身问答任务“具身干草堆中的针”，通过在扩展轨迹中散布多个线索来测试代理的长上下文推理能力；以及(3) 一个长时域数据集和基准套件，其中包含跨越数百个环境步骤的复杂任务，每个任务都配有真实动作序列。为了实现这一能力，我们探索了架构适应性，包括交错的目标-状态-行动建模、上下文扩展技术和上下文并行化，以使基于大语言模型的代理能够进行极端长上下文的推理和交互。实验结果和分析突出了我们的基准所提出的挑战，并提供了关于训练策略和模型在长时域条件下的行为的见解。我们的工作为下一代能够进行稳健长期推理和规划的具身人工智能系统奠定了基础。|
|**2025-05-22**|**Code Graph Model (CGM): A Graph-Integrated Large Language Model for Repository-Level Software Engineering Tasks**|Hongyuan Tao et.al.|[2505.16901](http://arxiv.org/abs/2505.16901)|null|最近在大型语言模型（LLM）方面的进展显示出在函数级代码生成方面的潜力，但仓库级软件工程任务仍然具有挑战性。当前的解决方案主要依赖于专有LLM代理，这引入了不可预测性并限制了可访问性，引发了关于数据隐私和模型定制的担忧。本文研究了开源LLM是否能够在不使用基于代理的方法的情况下有效解决仓库级任务。我们通过使LLM能够理解代码库中的函数和文件的语义信息和结构依赖关系来证明这是可能的。为此，我们引入了代码图模型（CGMs），将仓库代码图结构集成到LLM的注意力机制中，并使用专门的适配器将节点属性映射到LLM的输入空间。当与无代理的图RAG框架结合时，我们的方法在SWE-bench Lite基准测试中使用开源Qwen2.5-72B模型达到了43.00%的解决率。这一表现在开源权重模型中排名第一，在具有开源系统的方法中排名第二，总体上排名第八，超过了之前最佳的基于开源模型的方法12.33%。|
|**2025-05-22**|**MCP-RADAR: A Multi-Dimensional Benchmark for Evaluating Tool Use Capabilities in Large Language Models**|Xuanqi Gao et.al.|[2505.16700](http://arxiv.org/abs/2505.16700)|null|随着大型语言模型（LLMs）从被动的文本生成器演变为能够进行工具交互的主动推理代理，模型上下文协议（MCP）作为一种标准化框架出现，用于动态工具发现和编排。尽管在业界得到了广泛采用，现有的评估方法未能充分评估这种新范式下的工具利用能力。本文介绍了MCP-RADAR，这是第一个专门为评估MCP框架下LLM性能而设计的全面基准测试，通过一种新颖的五维方法来衡量：答案准确性、工具选择效率、计算资源效率、参数构建准确性和执行速度。与依赖主观人类评价或二元成功指标的传统基准不同，MCP-RADAR采用了跨多个任务领域的客观、可量化的测量方法，包括软件工程、数学推理和一般问题解决。我们对领先的商业和开源LLM的评估揭示了具有显著权衡的独特能力特征，在准确性、效率和速度之间存在明显差异，挑战了传统的单一指标性能排名。此外，我们为开发者提供了宝贵的指导，以优化其工具的最大模型兼容性和有效性。虽然由于其标准化的方法而专注于MCP，但我们的方法论适用于所有LLM代理工具集成框架，为LLM开发人员和工具创建者优化整个LLM-工具交互生态系统提供了有价值的见解。我们在评估中使用的实现、配置和数据集可在https://anonymous.4open.science/r/MCPRadar-B143公开获取。|
|**2025-05-22**|**O $^2$-Searcher: A Searching-based Agent Model for Open-Domain Open-Ended Question Answering**|Jianbiao Mei et.al.|[2505.16582](http://arxiv.org/abs/2505.16582)|null|尽管大型语言模型（LLMs）取得了进步，但它们本质上受限于静态参数化知识，这阻碍了它们在需要开放领域最新信息的任务中的表现。虽然使LLMs能够与外部知识环境交互是一个有前景的解决方案，但目前的努力主要集中在封闭式问题上。开放式问题，其特点是缺乏标准答案或提供非唯一且多样的答案，仍然未被充分探索。为了解决这一差距，我们提出了O$^2$-Searcher，这是一种利用强化学习有效处理开放领域中开放式和封闭式问题的新搜索代理。O$^2$-Searcher利用一个高效的本地模拟搜索环境进行动态知识获取，有效地将外部世界知识与模型的复杂推理过程解耦。它采用了一种统一的训练机制，并精心设计了奖励函数，使代理能够识别问题类型并适应不同的答案生成策略。此外，为了评估在复杂的开放式任务上的性能，我们构建了O$^2$-QA，这是一个高质量基准，包含300个手动策划的、跨领域的开放式问题及其相关的网页缓存。广泛的实验表明，仅使用3B模型的O$^2$-Searcher在O$^2$ -QA上显著超越了领先的LLM代理。它还在各种封闭式问答基准测试中达到了同类规模模型的最佳结果，同时表现与更大规模的模型相当。|
|**2025-05-22**|**Psychology-driven LLM Agents for Explainable Panic Prediction on Social Media during Sudden Disaster Events**|Mengzhu Liu et.al.|[2505.16455](http://arxiv.org/abs/2505.16455)|null|在突发灾难事件中，准确预测社交媒体上的公众恐慌情绪对于主动治理和危机管理至关重要。当前针对这一问题的研究面临三个主要挑战：缺乏精细标注的数据阻碍了情绪预测研究，未建模的风险感知导致预测不准确，以及恐慌形成机制的解释性不足。我们通过提出一个基于情绪唤醒理论的心理学驱动生成代理框架（PsychoAgent）来解决这些问题。具体来说，我们首先通过人与大型语言模型（LLMs）的合作构建了一个细粒度的开放恐慌情绪数据集（即COPE），以减轻语义偏差。然后，我们开发了一个整合跨域异构数据并基于心理机制的框架，以建模风险感知和情绪生成中的认知差异。为了提高解释性，我们设计了一个基于LLM的角色扮演代理，通过专门设计的提示模拟个体心理链。在我们标注的数据集上进行的实验结果表明，与基线模型相比，PsychoAgent将恐慌情绪预测性能提高了12.6%到21.7%。此外，我们的方法的解释性和泛化能力得到了验证。重要的是，这代表了从不透明的“数据驱动拟合”向透明的“基于角色模拟与机制解释”的范式转变，用于紧急情况下的恐慌情绪预测。我们的实现公开发布于：https://anonymous.4open.science/r/PsychoAgent-19DD。|
|**2025-05-22**|**CT-Agent: A Multimodal-LLM Agent for 3D CT Radiology Question Answering**|Yuren Mao et.al.|[2505.16229](http://arxiv.org/abs/2505.16229)|null|计算机断层扫描（CT）生成的三维体积医学数据可以被视为数百个横截面图像（即切片），为诊断提供了详细的解剖信息。对于放射科医生来说，创建CT放射学报告既耗时又容易出错。迫切需要一种视觉问答（VQA）系统，该系统能够回答放射科医生关于CT扫描中某些解剖区域的问题，甚至自动生成放射学报告。然而，现有的VQA系统无法充分处理CT放射学问答（CTQA）任务，原因在于：(1) 解剖复杂性使得CT图像难以理解；(2) 跨数百个切片的空间关系难以捕捉。为了解决这些问题，本文提出了CT-Agent，这是一种用于CTQA的多模态代理框架。CT-Agent采用解剖独立工具来分解解剖复杂性；此外，它通过全局-局部令牌压缩策略有效地捕捉跨切片的空间关系。在两个3D胸部CT数据集CT-RATE和RadGenome-ChestCT上的实验结果验证了CT-Agent的优越性能。|
|**2025-05-21**|**How Memory Management Impacts LLM Agents: An Empirical Study of Experience-Following Behavior**|Zidi Xiong et.al.|[2505.16067](http://arxiv.org/abs/2505.16067)|null|记忆是基于大型语言模型（LLM）的代理的关键组成部分，使它们能够存储和检索过去的执行以随着时间的推移提高任务性能。在这篇论文中，我们对记忆管理选择如何影响LLM代理的行为，特别是其长期性能进行了实证研究。具体来说，我们关注了两个被许多代理框架广泛使用的基本记忆操作——添加，将新经验纳入记忆库；以及删除，有选择地移除过去的经验——系统地研究它们对代理行为的影响。通过我们的定量分析，我们发现LLM代理显示出一种经验跟随属性：任务输入与检索到的记忆记录中的输入之间高度相似时，通常会导致非常相似的代理输出。进一步的分析揭示了与此属性相关的两个重要挑战：错误传播，即过去经验中的不准确之处会累积并降低未来性能；以及经验回放错位，即过时或无关的经验会对当前任务产生负面影响。通过控制实验，我们展示了结合选择性添加和删除策略可以帮助减轻这些负面影响，与简单的记忆增长相比，平均绝对性能提高了10%。此外，我们还强调了在任务分布变化和内存资源受限等具有挑战性的条件下，记忆管理选择如何影响代理的行为。我们的发现为理解LLM代理记忆系统的动态行为提供了见解，并为设计支持稳健、长期代理性能的记忆组件提供了实用指导。我们也发布了我们的代码以促进进一步的研究。|
|**2025-05-21**|**ReflAct: World-Grounded Decision Making in LLM Agents via Goal-State Reflection**|Jeonghye Kim et.al.|[2505.15182](http://arxiv.org/abs/2505.15182)|null|
|**2025-05-21**|**lmgame-Bench: How Good are LLMs at Playing Games?**|Lanxiang Hu et.al.|[2505.15146](http://arxiv.org/abs/2505.15146)|**[link](https://github.com/lmgame-org/gamingagent)**|
|**2025-05-21**|**Multicrossmodal Automated Agent for Integrating Diverse Materials Science Data**|Adib Bazgir et.al.|[2505.15132](http://arxiv.org/abs/2505.15132)|null|
|**2025-05-21**|**An Empirical Study on Reinforcement Learning for Reasoning-Search Interleaved LLM Agents**|Bowen Jin et.al.|[2505.15117](http://arxiv.org/abs/2505.15117)|**[link](https://github.com/petergriffinjin/search-r1)**|
|**2025-05-21**|**StepSearch: Igniting LLMs Search Ability via Step-Wise Proximal Policy Optimization**|Ziliang Wang et.al.|[2505.15107](http://arxiv.org/abs/2505.15107)|null|
|**2025-05-20**|**ContextAgent: Context-Aware Proactive LLM Agents with Open-World Sensory Perceptions**|Bufang Yang et.al.|[2505.14668](http://arxiv.org/abs/2505.14668)|null|
|**2025-05-20**|**DSMentor: Enhancing Data Science Agents with Curriculum Learning and Online Knowledge Accumulation**|He Wang et.al.|[2505.14163](http://arxiv.org/abs/2505.14163)|null|
|**2025-05-20**|**MAS-KCL: Knowledge component graph structure learning with large language model-based agentic workflow**|Yuan-Hao Jiang et.al.|[2505.14126](http://arxiv.org/abs/2505.14126)|null|
|**2025-05-20**|**BAR: A Backward Reasoning based Agent for Complex Minecraft Tasks**|Weihong Du et.al.|[2505.14079](http://arxiv.org/abs/2505.14079)|**[link](https://github.com/scunlp/bar)**|
|**2025-05-20**|**Divide by Question, Conquer by Agent: SPLIT-RAG with Question-Driven Graph Partitioning**|Ruiyi Yang et.al.|[2505.13994](http://arxiv.org/abs/2505.13994)|null|
|**2025-05-20**|**DrugPilot: LLM-based Parameterized Reasoning Agent for Drug Discovery**|Kun Li et.al.|[2505.13940](http://arxiv.org/abs/2505.13940)|null|
|**2025-05-20**|**Structured Agent Distillation for Large Language Model**|Jun Liu et.al.|[2505.13820](http://arxiv.org/abs/2505.13820)|null|
|**2025-05-19**|**Adversarial Testing in LLMs: Insights into Decision-Making Vulnerabilities**|Lili Zhang et.al.|[2505.13195](http://arxiv.org/abs/2505.13195)|null|
|**2025-05-20**|**From Assistants to Adversaries: Exploring the Security Risks of Mobile LLM Agents**|Liangxuan Wu et.al.|[2505.12981](http://arxiv.org/abs/2505.12981)|null|
|**2025-05-19**|**The Traitors: Deception and Trust in Multi-Agent Language Model Simulations**|Pedro M. P. Curvo et.al.|[2505.12923](http://arxiv.org/abs/2505.12923)|**[link](https://github.com/pedrocurvo/thetraitors)**|
|**2025-05-19**|**Forewarned is Forearmed: A Survey on Large Language Model-based Agents in Autonomous Cyberattacks**|Minrui Xu et.al.|[2505.12786](http://arxiv.org/abs/2505.12786)|null|
|**2025-05-18**|**A Survey of Attacks on Large Language Models**|Wenrui Xu et.al.|[2505.12567](http://arxiv.org/abs/2505.12567)|null|
|**2025-05-18**|**ALAS: A Stateful Multi-LLM Agent Framework for Disruption-Aware Planning**|Edward Y. Chang et.al.|[2505.12501](http://arxiv.org/abs/2505.12501)|null|
|**2025-05-18**|**Learning to Play Like Humans: A Framework for LLM Adaptation in Interactive Fiction Games**|Jinming Zhang et.al.|[2505.12439](http://arxiv.org/abs/2505.12439)|null|
|**2025-05-18**|**Automated Profile Inference with Language Model Agents**|Yuntao Du et.al.|[2505.12402](http://arxiv.org/abs/2505.12402)|null|
|**2025-05-20**|**LLM-DSE: Searching Accelerator Parameters with LLM Agents**|Hanyu Wang et.al.|[2505.12188](http://arxiv.org/abs/2505.12188)|**[link](https://github.com/nozidoali/llm-dse)**|
|**2025-05-17**|**LifelongAgentBench: Evaluating LLM Agents as Lifelong Learners**|Junhao Zheng et.al.|[2505.11942](http://arxiv.org/abs/2505.11942)|**[link](https://github.com/caixd-220529/LifelongAgentBench)**|
|**2025-05-16**|**Can AI automatically analyze public opinion? A LLM agents-based agentic pipeline for timely public opinion analysis**|Jing Liu et.al.|[2505.11401](http://arxiv.org/abs/2505.11401)|null|
|**2025-05-16**|**GuideBench: Benchmarking Domain-Oriented Guideline Following for LLM Agents**|Lingxiao Diao et.al.|[2505.11368](http://arxiv.org/abs/2505.11368)|null|
|**2025-05-16**|**From Intent Discovery to Recognition with Topic Modeling and Synthetic Data**|Aaron Rodrigues et.al.|[2505.11176](http://arxiv.org/abs/2505.11176)|null|
|**2025-05-16**|**MPMA: Preference Manipulation Attack Against Model Context Protocol**|Zihan Wang et.al.|[2505.11154](http://arxiv.org/abs/2505.11154)|null|
|**2025-05-16**|**Think Twice Before You Act: Enhancing Agent Behavioral Safety with Thought Correction**|Changyue Jiang et.al.|[2505.11063](http://arxiv.org/abs/2505.11063)|**[link](https://github.com/thu-coai/agent-safetybench)**|
|**2025-05-16**|**Group-in-Group Policy Optimization for LLM Agent Training**|Lang Feng et.al.|[2505.10978](http://arxiv.org/abs/2505.10978)|**[link](https://github.com/langfengq/verl-agent)**|
|**2025-05-16**|**Let the Trial Begin: A Mock-Court Approach to Vulnerability Detection using LLM-Based Agents**|Ratnadira Widyasari et.al.|[2505.10961](http://arxiv.org/abs/2505.10961)|null|
|**2025-05-16**|**Connecting the Dots: A Chain-of-Collaboration Prompting Framework for LLM Agents**|Jiaxing Zhao et.al.|[2505.10936](http://arxiv.org/abs/2505.10936)|null|
|**2025-05-15**|**Automating Security Audit Using Large Language Model based Agent: An Exploration Experiment**|Jia Hui Chin et.al.|[2505.10732](http://arxiv.org/abs/2505.10732)|null|
|**2025-05-15**|**Interpretable Risk Mitigation in LLM Agent Systems**|Jan Chojnacki et.al.|[2505.10670](http://arxiv.org/abs/2505.10670)|**[link](https://github.com/samsung/llm-agent-sae)**|
|**2025-05-15**|**AutoPentest: Enhancing Vulnerability Management With Autonomous LLM Agents**|Julius Henke et.al.|[2505.10321](http://arxiv.org/abs/2505.10321)|**[link](https://github.com/juliushenke/autopentest)**|
|**2025-05-15**|**Pre-Act: Multi-Step Planning and Reasoning Improves Acting in LLM Agents**|Mrinal Rawat et.al.|[2505.09970](http://arxiv.org/abs/2505.09970)|null|
|**2025-05-14**|**WorldView-Bench: A Benchmark for Evaluating Global Cultural Perspectives in Large Language Models**|Abdullah Mushtaq et.al.|[2505.09595](http://arxiv.org/abs/2505.09595)|null|
|**2025-05-14**|**The Influence of Human-inspired Agentic Sophistication in LLM-driven Strategic Reasoners**|Vince Trencsenyi et.al.|[2505.09396](http://arxiv.org/abs/2505.09396)|null|
|**2025-05-14**|**Reproducibility Study of "Cooperate or Collapse: Emergence of Sustainable Cooperation in a Society of LLM Agents"**|Pedro M. P. Curvo et.al.|[2505.09289](http://arxiv.org/abs/2505.09289)|**[link](https://github.com/giorgiopiatti/govsim)**|
|**2025-05-13**|**Strategy-Augmented Planning for Large Language Models via Opponent Exploitation**|Shuai Xu et.al.|[2505.08459](http://arxiv.org/abs/2505.08459)|null|
|**2025-05-13**|**Scalable UAV Multi-Hop Networking via Multi-Agent Reinforcement Learning with Large Language Models**|Yanggang Xu et.al.|[2505.08448](http://arxiv.org/abs/2505.08448)|null|
|**2025-05-13**|**Benchmarking AI scientists in omics data-driven biological research**|Erpai Luo et.al.|[2505.08341](http://arxiv.org/abs/2505.08341)|**[link](https://github.com/eperluo/baisbench)**|
|**2025-05-12**|**Are LLMs complicated ethical dilemma analyzers?**|Jiashen et.al.|[2505.08106](http://arxiv.org/abs/2505.08106)|**[link](https://github.com/alt-js/ethicallm)**|
|**2025-05-12**|**MLE-Dojo: Interactive Environments for Empowering LLM Agents in Machine Learning Engineering**|Rushi Qiang et.al.|[2505.07782](http://arxiv.org/abs/2505.07782)|**[link](https://github.com/MLE-Dojo/MLE-Dojo)**|
|**2025-05-12**|**YuLan-OneSim: Towards the Next Generation of Social Simulator with Large Language Models**|Lei Wang et.al.|[2505.07581](http://arxiv.org/abs/2505.07581)|**[link](https://github.com/RUC-GSAI/YuLan-OneSim)**|
|**2025-05-12**|**Can Generative AI agents behave like humans? Evidence from laboratory market experiments**|R. Maria del Rio-Chanona et.al.|[2505.07457](http://arxiv.org/abs/2505.07457)|null|
|**2025-05-09**|**ScaleMCP: Dynamic and Auto-Synchronizing Model Context Protocol Tools for LLM Agents**|Elias Lumer et.al.|[2505.06416](http://arxiv.org/abs/2505.06416)|null|
|**2025-05-09**|**AgentXploit: End-to-End Redteaming of Black-Box AI Agents**|Zhun Wang et.al.|[2505.05849](http://arxiv.org/abs/2505.05849)|null|
|**2025-05-08**|**Not Like Us, Hunty: Measuring Perceptions and Behavioral Effects of Minoritized Anthropomorphic Cues in LLMs**|Jeffrey Basoah et.al.|[2505.05660](http://arxiv.org/abs/2505.05660)|null|
|**2025-05-07**|**Large Language Models are Autonomous Cyber Defenders**|Sebastián R. Castro et.al.|[2505.04843](http://arxiv.org/abs/2505.04843)|**[link](https://github.com/r4wd3r/llms-are-acd)**|
|**2025-05-07**|**CompileAgent: Automated Real-World Repo-Level Compilation with Tool-Integrated LLM-based Agent System**|Li Hu et.al.|[2505.04254](http://arxiv.org/abs/2505.04254)|null|
|**2025-05-07**|**Identification and Optimization of Redundant Code Using Large Language Models**|Shamse Tasnim Cynthia et.al.|[2505.04040](http://arxiv.org/abs/2505.04040)|null|
|**2025-05-06**|**Divide, Optimize, Merge: Fine-Grained LLM Agent Optimization at Scale**|Jiale Liu et.al.|[2505.03973](http://arxiv.org/abs/2505.03973)|null|
|**2025-05-08**|**The Power of Stories: Narrative Priming Shapes How LLM Agents Collaborate and Compete**|Gerrit Großmann et.al.|[2505.03961](http://arxiv.org/abs/2505.03961)|**[link](https://github.com/storyagents25/story-agents)**|
|**2025-05-06**|**WebGen-Bench: Evaluating LLMs on Generating Interactive and Functional Websites from Scratch**|Zimu Lu et.al.|[2505.03733](http://arxiv.org/abs/2505.03733)|**[link](https://github.com/mnluzimu/webgen-bench)**|
|**2025-05-06**|**Procedural Memory Is Not All You Need: Bridging Cognitive Gaps in LLM-Based Agents**|Schaun Wheeler et.al.|[2505.03434](http://arxiv.org/abs/2505.03434)|null|
|**2025-05-05**|**The Art of Repair: Optimizing Iterative Program Repair with Instruction-Tuned Models**|Fernando Vallecillos Ruiz et.al.|[2505.02931](http://arxiv.org/abs/2505.02931)|null|
|**2025-05-04**|**MemEngine: A Unified and Modular Library for Developing Advanced Memory of LLM-based Agents**|Zeyu Zhang et.al.|[2505.02099](http://arxiv.org/abs/2505.02099)|**[link](https://github.com/nuster1128/memengine)**|
|**2025-05-04**|**Leveraging LLM Agents and Digital Twins for Fault Handling in Process Plants**|Milapji Singh Gill et.al.|[2505.02076](http://arxiv.org/abs/2505.02076)|**[link](https://github.com/aisl-at-imperial-college-london/fault-handling-agentic-llms-for-controlled-operations)**|
|**2025-05-03**|**Model Context Protocol-based Internet of Experts For Wireless Environment-aware LLM Agents**|Zongxi Liu et.al.|[2505.01834](http://arxiv.org/abs/2505.01834)|null|
|**2025-05-02**|**VTS-LLM: Domain-Adaptive LLM Agent for Enhancing Awareness in Vessel Traffic Services through Natural Language**|Sijin Sun et.al.|[2505.00989](http://arxiv.org/abs/2505.00989)|null|
|**2025-05-02**|**Seeking to Collide: Online Safety-Critical Scenario Generation for Autonomous Driving with Retrieval Augmented Large Language Models**|Yuewen Mei et.al.|[2505.00972](http://arxiv.org/abs/2505.00972)|null|
|**2025-05-02**|**SSRLBot: Designing and Developing an LLM-based Agent using Socially Shared Regulated Learning**|Xiaoshan Huang et.al.|[2505.00945](http://arxiv.org/abs/2505.00945)|null|
|**2025-05-01**|**HMCF: A Human-in-the-loop Multi-Robot Collaboration Framework Based on Large Language Models**|Zhaoxing Li et.al.|[2505.00820](http://arxiv.org/abs/2505.00820)|null|
|**2025-05-01**|**A Survey on Large Language Model based Human-Agent Systems**|Henry Peng Zou et.al.|[2505.00753](http://arxiv.org/abs/2505.00753)|**[link](https://github.com/HenryPengZou/Awesome-LLM-Based-Human-Agent-System-Papers)**|
|**2025-05-01**|**Rethinking Memory in AI: Taxonomy, Operations, Topics, and Future Directions**|Yiming Du et.al.|[2505.00675](http://arxiv.org/abs/2505.00675)|**[link](https://github.com/elvin-yiming-du/survey_memory_in_ai)**|
|**2025-05-01**|**UserCentrix: An Agentic Memory-augmented AI Framework for Smart Spaces**|Alaa Saleh et.al.|[2505.00472](http://arxiv.org/abs/2505.00472)|null|
|**2025-05-02**|**Self-Generated In-Context Examples Improve LLM Agents for Sequential Decision-Making Tasks**|Vishnu Sarukkai et.al.|[2505.00234](http://arxiv.org/abs/2505.00234)|null|
|**2025-04-30**|**Unsupervised Feature Transformation via In-context Generation, Generator-critic LLM Agents, and Duet-play Teaming**|Nanxu Gong et.al.|[2504.21304](http://arxiv.org/abs/2504.21304)|null|
|**2025-04-29**|**Toward Efficient Exploration by Large Language Model Agents**|Dilip Arumugam et.al.|[2504.20997](http://arxiv.org/abs/2504.20997)|null|
|**2025-04-29**|**Using LLMs in Generating Design Rationale for Software Architecture Decisions**|Xiyu Zhou et.al.|[2504.20781](http://arxiv.org/abs/2504.20781)|**[link](https://github.com/eric0052/llm4dr)**|
|**2025-04-30**|**TAMO:Fine-Grained Root Cause Analysis via Tool-Assisted LLM Agent with Multi-Modality Observation Data**|Qi Wang et.al.|[2504.20462](http://arxiv.org/abs/2504.20462)|null|
|**2025-04-29**|**CrashFixer: A crash resolution agent for the Linux kernel**|Alex Mathai et.al.|[2504.20412](http://arxiv.org/abs/2504.20412)|null|
|**2025-04-28**|**ResearchCodeAgent: An LLM Multi-Agent System for Automated Codification of Research Methodologies**|Shubham Gandhi et.al.|[2504.20117](http://arxiv.org/abs/2504.20117)|null|
|**2025-04-28**|**AutoP2C: An LLM-Based Agent Framework for Code Repository Generation from Multimodal Content in Academic Papers**|Zijie Lin et.al.|[2504.20115](http://arxiv.org/abs/2504.20115)|**[link](https://github.com/shoushouyu/automated-paper-to-code)**|
|**2025-04-28**|**Prompt Injection Attack to Tool Selection in LLM Agents**|Jiawen Shi et.al.|[2504.19793](http://arxiv.org/abs/2504.19793)|null|
|**2025-04-28**|**Evolution of Cooperation in LLM-Agent Societies: A Preliminary Study Using Different Punishment Strategies**|Kavindu Warnakulasuriya et.al.|[2504.19487](http://arxiv.org/abs/2504.19487)|null|
|**2025-05-01**|**BrowseComp-ZH: Benchmarking Web Browsing Ability of Large Language Models in Chinese**|Peilin Zhou et.al.|[2504.19314](http://arxiv.org/abs/2504.19314)|**[link](https://github.com/palin2018/browsecomp-zh)**|
|**2025-04-27**|**AndroidGen: Building an Android Language Agent under Data Scarcity**|Hanyu Lai et.al.|[2504.19298](http://arxiv.org/abs/2504.19298)|null|
|**2025-04-26**|**Stealing Creator's Workflow: A Creator-Inspired Agentic Framework with Iterative Feedback Loop for Improved Scientific Short-form Generation**|Jong Inn Park et.al.|[2504.18805](http://arxiv.org/abs/2504.18805)|null|
|**2025-04-26**|**A Vision for Auto Research with LLM Agents**|Chengwei Liu et.al.|[2504.18765](http://arxiv.org/abs/2504.18765)|null|
|**2025-04-25**|**Proof-of-TBI -- Fine-Tuned Vision Language Model Consortium and OpenAI-o3 Reasoning LLM-Based Medical Diagnosis Support System for Mild Traumatic Brain Injury (TBI) Prediction**|Ross Gore et.al.|[2504.18671](http://arxiv.org/abs/2504.18671)|null|
|**2025-04-25**|**Towards Adaptive Software Agents for Debugging**|Yacine Majdoub et.al.|[2504.18316](http://arxiv.org/abs/2504.18316)|null|
|**2025-04-25**|**MultiMind: Enhancing Werewolf Agents with Multimodal Reasoning and Theory of Mind**|Zheng Zhang et.al.|[2504.18039](http://arxiv.org/abs/2504.18039)|null|
|**2025-04-24**|**LLM Agent Swarm for Hypothesis-Driven Drug Discovery**|Kevin Song et.al.|[2504.17967](http://arxiv.org/abs/2504.17967)|null|
|**2025-04-24**|**Collaborating Action by Action: A Multi-agent LLM Framework for Embodied Reasoning**|Isadora White et.al.|[2504.17950](http://arxiv.org/abs/2504.17950)|null|
|**2025-04-24**|**Toward a Human-Centered Evaluation Framework for Trustworthy LLM-Powered GUI Agents**|Chaoran Chen et.al.|[2504.17934](http://arxiv.org/abs/2504.17934)|null|
|**2025-04-24**|**DataScout: Automatic Data Fact Retrieval for Statement Augmentation with an LLM-Based Agent**|Chuer Chen et.al.|[2504.17334](http://arxiv.org/abs/2504.17334)|null|
|**2025-04-23**|**Leveraging LLMs as Meta-Judges: A Multi-Agent Framework for Evaluating LLM Judgments**|Yuran Li et.al.|[2504.17087](http://arxiv.org/abs/2504.17087)|null|
|**2025-04-26**|**A Survey of AI Agent Protocols**|Yingxuan Yang et.al.|[2504.16736](http://arxiv.org/abs/2504.16736)|null|
|**2025-04-26**|**Enhancing LLM-Based Agents via Global Planning and Hierarchical Execution**|Junjie Chen et.al.|[2504.16563](http://arxiv.org/abs/2504.16563)|**[link](https://github.com/cjj826/goalact)**|
|**2025-04-23**|**ClarifyCoder: Clarification-Aware Fine-Tuning for Programmatic Problem Solving**|Jie JW Wu et.al.|[2504.16331](http://arxiv.org/abs/2504.16331)|null|
|**2025-04-22**|**MR. Video: "MapReduce" is the Principle for Long Video Understanding**|Ziqi Pang et.al.|[2504.16082](http://arxiv.org/abs/2504.16082)|null|
|**2025-04-22**|**LLMs are Greedy Agents: Effects of RL Fine-tuning on Decision-Making Abilities**|Thomas Schmied et.al.|[2504.16078](http://arxiv.org/abs/2504.16078)|null|
|**2025-04-22**|**A closer look at how large language models trust humans: patterns and biases**|Valeria Lerman et.al.|[2504.15801](http://arxiv.org/abs/2504.15801)|null|
|**2025-04-22**|**WALL-E 2.0: World Alignment by NeuroSymbolic Learning improves World Model-based LLM Agents**|Siyu Zhou et.al.|[2504.15785](http://arxiv.org/abs/2504.15785)|**[link](https://github.com/elated-sawyer/WALL-E)**|
|**2025-04-22**|**A Comprehensive Survey in LLM(-Agent) Full Stack Safety: Data, Training and Deployment**|Kun Wang et.al.|[2504.15585](http://arxiv.org/abs/2504.15585)|null|
|**2025-04-22**|**A Framework for Testing and Adapting REST APIs as LLM Tools**|Jayachandu Bandlamudi et.al.|[2504.15546](http://arxiv.org/abs/2504.15546)|null|
|**2025-04-21**|**Agent for User: Testing Multi-User Interactive Features in TikTok**|Sidong Feng et.al.|[2504.15474](http://arxiv.org/abs/2504.15474)|null|
|**2025-04-21**|**Interpretable Locomotion Prediction in Construction Using a Memory-Driven LLM Agent With Chain-of-Thought Reasoning**|Ehsan Ahmadi et.al.|[2504.15263](http://arxiv.org/abs/2504.15263)|null|
|**2025-04-20**|**SWE-Synth: Synthesizing Verifiable Bug-Fix Data to Enable Large Language Models in Resolving Real-World Bugs**|Minh V. T. Pham et.al.|[2504.14757](http://arxiv.org/abs/2504.14757)|null|
|**2025-04-20**|**A Framework for Benchmarking and Aligning Task-Planning Safety in LLM-Based Embodied Agents**|Yuting Huang et.al.|[2504.14650](http://arxiv.org/abs/2504.14650)|null|
|**2025-04-22**|**FAIRGAME: a Framework for AI Agents Bias Recognition using Game Theory**|Alessio Buscemi et.al.|[2504.14325](http://arxiv.org/abs/2504.14325)|null|
|**2025-04-18**|**Science Hierarchography: Hierarchical Organization of Science Literature**|Muhan Gao et.al.|[2504.13834](http://arxiv.org/abs/2504.13834)|**[link](https://github.com/jhu-clsp/science-hierarchography)**|
|**2025-04-18**|**OpenDeception: Benchmarking and Investigating AI Deceptive Behaviors via Open-ended Interaction Simulation**|Yichen Wu et.al.|[2504.13707](http://arxiv.org/abs/2504.13707)|null|
|**2025-04-18**|**CodeVisionary: An Agent-based Framework for Evaluating Large Language Models in Code Generation**|Xinchen Wang et.al.|[2504.13472](http://arxiv.org/abs/2504.13472)|null|
|**2025-04-18**|**Exploring Expert Failures Improves LLM Agent Tuning**|Li-Cheng Lan et.al.|[2504.13145](http://arxiv.org/abs/2504.13145)|null|
|**2025-04-17**|**Retrieval-Augmented Generation with Conflicting Evidence**|Han Wang et.al.|[2504.13079](http://arxiv.org/abs/2504.13079)|**[link](https://github.com/hannight/ramdocs)**|
|**2025-04-17**|**WebLists: Extracting Structured Information From Complex Interactive Websites Using Executable LLM Agents**|Arth Bohra et.al.|[2504.12682](http://arxiv.org/abs/2504.12682)|null|
|**2025-04-17**|**MetaSynth: Meta-Prompting-Driven Agentic Scaffolds for Diverse Synthetic Data Generation**|Haris Riaz et.al.|[2504.12563](http://arxiv.org/abs/2504.12563)|null|
|**2025-04-16**|**Towards LLM Agents for Earth Observation**|Chia Hsiang Kao et.al.|[2504.12110](http://arxiv.org/abs/2504.12110)|null|
|**2025-04-16**|**Progent: Programmable Privilege Control for LLM Agents**|Tianneng Shi et.al.|[2504.11703](http://arxiv.org/abs/2504.11703)|**[link](https://github.com/sunblaze-ucb/progent)**|
|**2025-04-16**|**Steering Prosocial AI Agents: Computational Basis of LLM's Decision Making in Social Simulation**|Ji Ma et.al.|[2504.11671](http://arxiv.org/abs/2504.11671)|null|
|**2025-04-15**|**GraphicBench: A Planning Benchmark for Graphic Design with Language Agents**|Dayeon Ki et.al.|[2504.11571](http://arxiv.org/abs/2504.11571)|null|
|**2025-04-15**|**Can Large Language Models Trade? Testing Financial Theories with LLM Agents in Market Simulations**|Alejandro Lopez-Lira et.al.|[2504.10789](http://arxiv.org/abs/2504.10789)|null|
|**2025-04-14**|**Characterizing LLM-driven Social Network: The Chirper.ai Case**|Yiming Zhu et.al.|[2504.10286](http://arxiv.org/abs/2504.10286)|null|
|**2025-04-14**|**SocioVerse: A World Model for Social Simulation Powered by LLM Agents and A Pool of 10 Million Real-World Users**|Xinnong Zhang et.al.|[2504.10157](http://arxiv.org/abs/2504.10157)|**[link](https://github.com/fudandisc/socioverse)**|
|**2025-04-14**|**A Survey of Personalization: From RAG to Agent**|Xiaopeng Li et.al.|[2504.10147](http://arxiv.org/abs/2504.10147)|**[link](https://github.com/Applied-Machine-Learning-Lab/Awesome-Personalized-RAG-Agent)**|
|**2025-04-14**|**StruPhantom: Evolutionary Injection Attacks on Black-Box Tabular Agents Powered by Large Language Models**|Yang Feng et.al.|[2504.09841](http://arxiv.org/abs/2504.09841)|null|
|**2025-04-14**|**Training Small Reasoning LLMs with Cognitive Preference Alignment**|Wenrui Cai et.al.|[2504.09802](http://arxiv.org/abs/2504.09802)|null|
|**2025-04-14**|**Reasoning Court: Combining Reasoning, Action, and Judgment for Multi-Hop Reasoning**|Jingtian Wu et.al.|[2504.09781](http://arxiv.org/abs/2504.09781)|null|
|**2025-04-13**|**AgentA/B: Automated and Scalable Web A/BTesting with Interactive LLM Agents**|Dakuo Wang et.al.|[2504.09723](http://arxiv.org/abs/2504.09723)|null|
|**2025-04-13**|**MLRC-Bench: Can Language Agents Solve Machine Learning Research Challenges?**|Yunxiang Zhang et.al.|[2504.09702](http://arxiv.org/abs/2504.09702)|null|
|**2025-04-13**|**UXAgent: A System for Simulating Usability Testing of Web Design with LLM Agents**|Yuxuan Lu et.al.|[2504.09407](http://arxiv.org/abs/2504.09407)|null|
|**2025-04-11**|**Do LLMs trust AI regulation? Emerging behaviour of game-theoretic LLM agents**|Alessio Buscemi et.al.|[2504.08640](http://arxiv.org/abs/2504.08640)|null|
|**2025-04-11**|**Task Memory Engine (TME): Enhancing State Awareness for Multi-Step LLM Agent Tasks**|Ye Ye et.al.|[2504.08525](http://arxiv.org/abs/2504.08525)|**[link](https://github.com/biubiutomato/tme-agent)**|
|**2025-04-11**|**Adopting Large Language Models to Automated System Integration**|Robin D. Pesl et.al.|[2504.08490](http://arxiv.org/abs/2504.08490)|null|
|**2025-04-10**|**Deceptive Automated Interpretability: Language Models Coordinating to Fool Oversight Systems**|Simon Lermen et.al.|[2504.07831](http://arxiv.org/abs/2504.07831)|null|
|**2025-04-10**|**MOSAIC: Modeling Social AI for Content Dissemination and Regulation in Multi-Agent Simulations**|Genglin Liu et.al.|[2504.07830](http://arxiv.org/abs/2504.07830)|**[link](https://github.com/genglinliu/MOSAIC)**|
|**2025-04-10**|**Enhancing Player Enjoyment with a Two-Tier DRL and LLM-Based Agent System for Fighting Games**|Shouren Wang et.al.|[2504.07425](http://arxiv.org/abs/2504.07425)|null|
|**2025-04-11**|**Review of Case-Based Reasoning for LLM Agents: Theoretical Foundations, Architectural Components, and Cognitive Integration**|Kostas Hatalis et.al.|[2504.06943](http://arxiv.org/abs/2504.06943)|null|
|**2025-04-09**|**FamilyTool: A Multi-hop Personalized Tool Use Benchmark**|Yuxin Wang et.al.|[2504.06766](http://arxiv.org/abs/2504.06766)|**[link](https://github.com/yxzwang/FamilyTool)**|
|**2025-04-09**|**Right Prediction, Wrong Reasoning: Uncovering LLM Misalignment in RA Disease Diagnosis**|Umakanta Maharana et.al.|[2504.06581](http://arxiv.org/abs/2504.06581)|**[link](https://github.com/Umakantamaharana/right-prediction-wrong-reasoning)**|
|**2025-04-08**|**FEABench: Evaluating Language Models on Multiphysics Reasoning Ability**|Nayantara Mudur et.al.|[2504.06260](http://arxiv.org/abs/2504.06260)|**[link](https://github.com/google/feabench)**|
|**2025-04-08**|**Are Generative AI Agents Effective Personalized Financial Advisors?**|Takehiro Takayanagi et.al.|[2504.05862](http://arxiv.org/abs/2504.05862)|**[link](https://github.com/TTsamurai/LLMAdvisor_supplementary)**|
|**2025-04-07**|**SciSciGPT: Advancing Human-AI Collaboration in the Science of Science**|Erzhuo Shao et.al.|[2504.05559](http://arxiv.org/abs/2504.05559)|null|
|**2025-04-07**|**How to evaluate control measures for LLM agents? A trajectory from today to superintelligence**|Tomek Korbak et.al.|[2504.05259](http://arxiv.org/abs/2504.05259)|null|
|**2025-04-07**|**AI for Climate Finance: Agentic Retrieval and Multi-Step Reasoning for Early Warning System Investments**|Saeid Ario Vaghefi et.al.|[2504.05104](http://arxiv.org/abs/2504.05104)|null|
|**2025-04-07**|**BIASINSPECTOR: Detecting Bias in Structured Data through LLM Agents**|Haoxuan Li et.al.|[2504.04855](http://arxiv.org/abs/2504.04855)|null|
|**2025-04-07**|**scAgent: Universal Single-Cell Annotation via a LLM Agent**|Yuren Mao et.al.|[2504.04698](http://arxiv.org/abs/2504.04698)|null|
|**2025-04-06**|**Building LLM Agents by Incorporating Insights from Computer Systems**|Yapeng Mi et.al.|[2504.04485](http://arxiv.org/abs/2504.04485)|null|
|**2025-04-06**|**VideoAgent2: Enhancing the LLM-Based Agent System for Long-Form Video Understanding by Uncertainty-Aware CoT**|Zhuo Zhi et.al.|[2504.04471](http://arxiv.org/abs/2504.04471)|null|
|**2025-04-06**|**Human-Level Competitive Pokémon via Scalable Offline Reinforcement Learning with Transformers**|Jake Grigsby et.al.|[2504.04395](http://arxiv.org/abs/2504.04395)|null|
|**2025-04-06**|**AutoPDL: Automatic Prompt Optimization for LLM Agents**|Claudio Spiess et.al.|[2504.04365](http://arxiv.org/abs/2504.04365)|null|
|**2025-04-06**|**OmniDrive: A Holistic Vision-Language Dataset for Autonomous Driving with Counterfactual Reasoning**|Shihao Wang et.al.|[2504.04348](http://arxiv.org/abs/2504.04348)|null|
|**2025-04-06**|**CO-Bench: Benchmarking Language Model Agents in Algorithm Search for Combinatorial Optimization**|Weiwei Sun et.al.|[2504.04310](http://arxiv.org/abs/2504.04310)|**[link](https://github.com/sunnweiwei/co-bench)**|
|**2025-04-04**|**SynWorld: Virtual Scenario Synthesis for Agentic Action Knowledge Refinement**|Runnan Fang et.al.|[2504.03561](http://arxiv.org/abs/2504.03561)|**[link](https://github.com/zjunlp/synworld)**|
|**2025-04-04**|**Agentic Knowledgeable Self-awareness**|Shuofei Qiao et.al.|[2504.03553](http://arxiv.org/abs/2504.03553)|**[link](https://github.com/zjunlp/knowself)**|
|**2025-04-04**|**Inherent and emergent liability issues in LLM-based agentic systems: a principal-agent perspective**|Garry A. Gabison et.al.|[2504.03255](http://arxiv.org/abs/2504.03255)|null|
|**2025-04-04**|**Les Dissonances: Cross-Tool Harvesting and Polluting in Multi-Tool Empowered LLM Agents**|Zichuan Li et.al.|[2504.03111](http://arxiv.org/abs/2504.03111)|null|
|**2025-04-03**|**Ontologies in Design: How Imagining a Tree Reveals Possibilites and Assumptions in Large Language Models**|Nava Haghighi et.al.|[2504.03029](http://arxiv.org/abs/2504.03029)|null|
|**2025-04-02**|**Automated Survey Collection with LLM-based Conversational Agents**|Kurmanbek Kaiyrbekov et.al.|[2504.02891](http://arxiv.org/abs/2504.02891)|null|
|**2025-04-03**|**Multi-Mission Tool Bench: Assessing the Robustness of LLM based Agents through Related and Dynamic Missions**|PeiJie Yu et.al.|[2504.02623](http://arxiv.org/abs/2504.02623)|**[link](https://github.com/yupeijei1997/MMTB)**|
|**2025-04-02**|**On Simulation-Guided LLM-based Code Generation for Safe Autonomous Driving Software**|Ali Nouri et.al.|[2504.02141](http://arxiv.org/abs/2504.02141)|null|
|**2025-04-02**|**Building Knowledge from Interactions: An LLM-Based Architecture for Adaptive Tutoring and Social Reasoning**|Luca Garello et.al.|[2504.01588](http://arxiv.org/abs/2504.01588)|null|
|**2025-04-01**|**Catastrophic Forgetting in LLMs: A Comparative Analysis Across Language Tasks**|Naimul Haque et.al.|[2504.01241](http://arxiv.org/abs/2504.01241)|null|
|**2025-04-01**|**Personality-Driven Decision-Making in LLM-Based Autonomous Agents**|Lewis Newsham et.al.|[2504.00727](http://arxiv.org/abs/2504.00727)|null|
|**2025-04-01**|**GraphMaster: Automated Graph Synthesis via LLM Agents in Data-Limited Environments**|Enjun Du et.al.|[2504.00711](http://arxiv.org/abs/2504.00711)|null|
|**2025-04-01**|**AgentNet: Decentralized Evolutionary Coordination for LLM-based Multi-Agent Systems**|Yingxuan Yang et.al.|[2504.00587](http://arxiv.org/abs/2504.00587)|null|
|**2025-04-01**|**Automated detection of atomicity violations in large-scale systems**|Hang He et.al.|[2504.00521](http://arxiv.org/abs/2504.00521)|null|
|**2025-04-01**|**When Persuasion Overrides Truth in Multi-Agent LLM Debates: Introducing a Confidence-Weighted Persuasion Override Rate (CW-POR)**|Mahak Agarwal et.al.|[2504.00374](http://arxiv.org/abs/2504.00374)|null|
|**2025-03-31**|**Large Language Models in Numberland: A Quick Test of Their Numerical Reasoning Abilities**|Roussel Rahman et.al.|[2504.00226](http://arxiv.org/abs/2504.00226)|null|
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
|**2025-03-16**|**A Survey on the Optimization of Large Language Model-based Agents**|Shangheng Du et.al.|[2503.12434](http://arxiv.org/abs/2503.12434)|**[link](https://github.com/youngdubbydu/llm-agent-optimization)**|
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
|**2025-03-03**|**Can (A)I Change Your Mind?**|Miriam Havin et.al.|[2503.01844](http://arxiv.org/abs/2503.01844)|**[link](https://github.com/Ariel-Goldstein-Lab/Can-AI-Change-Your-Mind)**|
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
|**2025-02-18**|**Demonstrating specification gaming in reasoning models**|Alexander Bondarenko et.al.|[2502.13295](http://arxiv.org/abs/2502.13295)|**[link](https://github.com/palisaderesearch/ctfish)**|
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
|**2025-02-09**|**MetaChain: A Fully-Automated and Zero-Code Framework for LLM Agents**|Jiabin Tang et.al.|[2502.05957](http://arxiv.org/abs/2502.05957)|**[link](https://github.com/hkuds/autoagent)**|
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
|**2025-01-14**|**Addressing the sustainable AI trilemma: a case study on LLM agents and RAG**|Hui Wu et.al.|[2501.08262](http://arxiv.org/abs/2501.08262)|**[link](https://github.com/huiwxing/llmagent_trilemma)**|
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
|**2024-12-13**|**You Name It, I Run It: An LLM Agent to Execute Tests of Arbitrary Projects**|Islem Bouzenia et.al.|[2412.10133](http://arxiv.org/abs/2412.10133)|**[link](https://github.com/sola-st/executionagent)**|
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

<p align=right>(<a href=#updated-on-20250525>back to top</a>)</p>

## llm

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-05-22**|**CrossLMM: Decoupling Long Video Sequences from LMMs via Dual Cross-Attention Mechanisms**|Shilin Yan et.al.|[2505.17020](http://arxiv.org/abs/2505.17020)|null|大型多模态模型（LMMs）的出现显著增强了大型语言模型（LLMs）处理和解释多种数据模态（如图像和视频）的能力。然而，随着输入复杂性的增加，特别是长视频序列，所需的标记数量显著增长，导致计算成本呈二次方增长。这使得在LMMs中高效压缩视频标记同时保持性能完整性成为了一个紧迫的研究挑战。在本文中，我们提出了CrossLMM，通过双交叉注意力机制将长视频序列从LMMs中解耦，从而大幅减少了视觉标记的数量且性能损失极小。具体来说，我们首先通过池化方法从预训练的视觉编码器实现显著的标记减少。然后，在LLM层中，我们采用了一种视觉到视觉的交叉注意力机制，其中池化的视觉标记作为查询与原始视觉标记集进行交互。该模块使标记利用更加高效，同时保留了细粒度的信息保真度。此外，我们还引入了一种文本到视觉的交叉注意力机制，通过与原始视觉标记的交互来增强文本标记，丰富了文本标记的视觉理解能力。全面的实证评估表明，尽管使用了更少的计算资源，我们的方法在多样化的基于视频的LMM基准测试中实现了可比或更优的性能。|
|**2025-05-22**|**Delving into RL for Image Generation with CoT: A Study on DPO vs. GRPO**|Chengzhuo Tong et.al.|[2505.17017](http://arxiv.org/abs/2505.17017)|null|最近的进展强调了强化学习（RL）在增强大型语言模型（LLMs）的链式思维（CoT）推理能力方面的显著作用。两种突出的RL算法，直接偏好优化（DPO）和群体相对策略优化（GRPO），在这些发展中占据核心地位，展示了各自不同的优缺点。自回归图像生成也可以解释为一种顺序的CoT推理过程，它带来了与基于LLM的CoT推理不同的独特挑战。这些挑战包括确保文本-图像一致性、提高图像美学质量以及设计复杂的奖励模型，而不仅仅是依赖简单的基于规则的奖励。尽管近期的努力已经将RL扩展到了这一领域，但这些探索通常缺乏对领域特定挑战和不同RL策略特性的深入分析。为了填补这一空白，我们首次全面调查了GRPO和DPO算法在自回归图像生成中的应用，评估了它们在域内性能和跨域泛化能力，同时仔细审查了不同奖励模型对其各自能力的影响。我们的研究发现，GRPO和DPO表现出独特的优点，并且关键的是，具有更强内在泛化能力的奖励模型可能增强所应用的RL算法的泛化潜力。此外，我们系统地探讨了三种普遍的扩展策略，以增强它们在域内和跨域的专业性，从而为每个范式的性能提升提供了独特的见解。我们希望这项研究能够为未来开发更有效的RL算法以实现自回归图像生成中稳健的CoT推理开辟新的道路。代码发布于https://github.com/ZiyuGuo99/Image-Generation-CoT|
|**2025-05-22**|**R1-Searcher++: Incentivizing the Dynamic Knowledge Acquisition of LLMs via Reinforcement Learning**|Huatong Song et.al.|[2505.17005](http://arxiv.org/abs/2505.17005)|null|大型语言模型（LLMs）虽然强大，但由于静态知识的限制容易产生幻觉。检索增强生成（RAG）通过注入外部信息来帮助解决这一问题，但当前的方法往往成本高昂、泛化能力差或忽视了模型的内部知识。在本文中，我们介绍了一种名为R1-Searcher++的新框架，旨在训练LLMs自适应地利用内部和外部知识源。R1-Searcher++采用两阶段训练策略：首先是SFT冷启动阶段，用于初步格式学习；随后是动态知识获取的强化学习（RL）阶段。RL阶段使用结果监督来鼓励探索，结合奖励机制以促进内部知识的利用，并整合记忆机制以持续吸收检索到的信息，从而丰富模型的内部知识。通过利用内部知识和外部搜索引擎，该模型不断改进其能力，实现高效的检索增强推理。我们的实验表明，R1-Searcher++优于之前的RAG和推理方法，实现了高效的检索。代码可在https://github.com/RUCAIBox/R1-Searcher-plus获取。|
|**2025-05-22**|**Do Large Language Models Excel in Complex Logical Reasoning with Formal Language?**|Jin Jiang et.al.|[2505.16998](http://arxiv.org/abs/2505.16998)|null|大型语言模型（LLM）在复杂的逻辑推理任务上已经展示了突破性的性能。然而，大多数现有的研究都集中在使用形式语言来指导LLM推导出可靠的推理路径，而对这些能力的系统性评估仍然有限。在本文中，我们旨在利用形式语言对各种逻辑推理问题进行全面评估。从三个维度来看，即LLM的谱系、任务分类和轨迹格式，我们的主要发现是：1）思维模型显著优于指令模型，尤其是在使用形式语言时；2）所有LLM在归纳推理能力方面都表现出局限性，无论它们是否使用形式语言；3）采用PoT格式的数据在其他语言中实现了最佳的泛化性能。此外，我们还整理了与形式相关的训练数据，以进一步增强小型语言模型，实验结果表明，一种简单的拒绝微调方法可以更好地使LLM在形式语言之间泛化，并实现最佳的整体性能。我们的代码和报告可在https://github.com/jiangjin1999/FormalEval获取。|
|**2025-05-22**|**DecoupledESC: Enhancing Emotional Support Generation via Strategy-Response Decoupled Preference Optimization**|Chao Zhang et.al.|[2505.16995](http://arxiv.org/abs/2505.16995)|null|近期在情感支持对话（ESC）方面的进展通过监督微调（SFT）改进了大型语言模型（LLMs）的情感支持生成。然而，常见的心理错误仍然存在。虽然直接偏好优化（DPO）通过成对偏好学习显示出减少这类错误的潜力，但其在ESC任务中的有效性受到两个关键挑战的限制：（1）纠缠的数据结构：现有的ESC数据固有地将心理策略和响应内容纠缠在一起，使得构建高质量的偏好对变得困难；（2）优化模糊性：将纯DPO应用于这种纠缠的成对数据会导致模糊的训练目标。为了解决这些问题，我们引入了推断偏好挖掘（IPM）来构建高质量的偏好数据，形成了IPM-PrefDial数据集。基于这些数据，我们提出了一种解耦的ESC框架，该框架受Gross的情绪调节扩展过程模型启发，将ESC任务分解为两个顺序子任务：策略规划和共情响应生成。每个子任务都通过SFT进行训练，并随后通过DPO增强以符合心理偏好。广泛的实验表明，我们的解耦ESC框架优于联合优化基线，减少了偏好偏差并提高了响应质量。|
|**2025-05-22**|**T1: A Tool-Oriented Conversational Dataset for Multi-Turn Agentic Planning**|Amartya Chakraborty et.al.|[2505.16986](http://arxiv.org/abs/2505.16986)|null|大型语言模型（LLMs）已经展示了作为能够解决复杂问题的智能代理的强大能力。然而，在涉及API或工具调用之间依赖关系的情景中，特别是在多轮对话中，有效的规划仍然是一个重大挑战。为了解决这个问题，我们引入了T1，这是一个工具增强的、多领域、多轮对话数据集，专门设计用于捕捉和管理跨不同领域的工具间依赖关系。T1通过集成缓存机制支持短期和长期记忆，并支持动态重新规划，如决定是否重新计算或重用缓存结果，从而在九个不同的领域（4个单一领域和5个多领域）中严格评估代理协调工具使用的能力。除了促进关于工具使用和规划的研究外，T1还作为评估开源语言模型性能的基准。我们展示了由T1-Agent驱动的结果，突出了其在复杂的工具依赖情景中进行规划和推理的能力。|
|**2025-05-22**|**UFT: Unifying Supervised and Reinforcement Fine-Tuning**|Mingyang Liu et.al.|[2505.16984](http://arxiv.org/abs/2505.16984)|null|后训练在增强大型语言模型（LLMs）的推理能力方面展示了其重要性。主要的后训练方法可以分为监督微调（SFT）和强化微调（RFT）。SFT高效且适用于小型语言模型，但可能导致过拟合并限制较大模型的推理能力。相比之下，RFT通常提供更好的泛化能力，但严重依赖于基础模型的强度。为了解决SFT和RFT的局限性，我们提出了一种新的后训练范式——统一微调（UFT），它将SFT和RFT统一为一个集成过程。UFT使模型能够有效探索解决方案，同时结合信息丰富的监督信号，弥合了现有方法中记忆与思考之间的差距。值得注意的是，无论模型大小如何，UFT在总体上都优于SFT和RFT。此外，我们从理论上证明了UFT打破了RFT固有的指数级样本复杂度瓶颈，首次表明统一训练可以在长时推理任务上实现指数级加速收敛。|
|**2025-05-22**|**LLM as Effective Streaming Processor: Bridging Streaming-Batch Mismatches with Group Position Encoding**|Junlong Tong et.al.|[2505.16983](http://arxiv.org/abs/2505.16983)|null|大型语言模型（LLMs）主要设计用于批处理。现有的将LLMs适应于流式处理的方法要么依赖昂贵的重新编码，要么使用具有有限可扩展性的专门架构。本研究识别了在将面向批处理的LLMs适应于流式处理时存在的三个关键不匹配：(1) 输入注意力、(2) 输出注意力和 (3) 位置ID不匹配。虽然通常认为后两个不匹配需要频繁的重新编码，但我们的分析表明，只有输入注意力不匹配显著影响性能，这意味着重新编码输出在很大程度上是不必要的。为了更好地理解这一与普遍假设的差异，我们首次全面分析了位置编码对流式处理中LLMs的影响，表明保持源和目标上下文中的相对位置比维持绝对顺序更为关键。受上述分析启发，我们提出了一种基于批处理架构的组位置编码范式，以增强流式模式和批处理模式之间的一致性。广泛的跨语言和跨模态任务实验表明，我们的方法优于现有方法。该方法无需任何架构修改，并在流式和批处理模式下均表现出强大的泛化能力。代码可在https://github.com/EIT-NLP/StreamingLLM获取。|
|**2025-05-22**|**Beyond Correlation: Towards Causal Large Language Model Agents in Biomedicine**|Adib Bazgir et.al.|[2505.16982](http://arxiv.org/abs/2505.16982)|null|大型语言模型（LLM）在生物医学领域显示出潜力，但缺乏真正的因果理解能力，而是依赖于相关性。本文设想了能够整合多模态数据（文本、图像、基因组等）并进行基于干预的推理以推断因果关系的因果LLM代理。解决这一问题需要克服几个关键挑战：设计安全可控的代理框架；开发严格的因果评估基准；整合异构数据源；以及将LLM与结构化知识图谱（KGs）和形式化的因果推理工具协同结合。这样的代理可以解锁变革性的机会，包括通过自动假设生成和模拟加速药物发现，以及通过患者特定的因果模型实现个性化医疗。这一研究议程旨在促进跨学科努力，将因果概念与基础模型相结合，以开发可靠的AI伙伴来推动生物医学的进步。|
|**2025-05-22**|**HyGenar: An LLM-Driven Hybrid Genetic Algorithm for Few-Shot Grammar Generation**|Weizhi Tang et.al.|[2505.16978](http://arxiv.org/abs/2505.16978)|null|语法在自然语言处理和文本/代码生成中起着关键作用，它能够定义句法、创建解析器并指导结构化输出。尽管大型语言模型（LLMs）在各个领域展示了令人印象深刻的能力，但它们推断和生成语法的能力尚未得到充分探索。在这篇论文中，我们旨在研究和改进LLMs在少量样本下的语法生成能力，即从少量正例和反例中推断语法，并以Backus-Naur形式生成。为此，我们引入了一个包含540个结构化语法生成挑战的新数据集，设计了6种度量标准，并对8种不同的LLMs进行了评估。我们的发现表明，现有的LLMs在语法生成方面表现不佳。为了解决这个问题，我们提出了一种由LLM驱动的混合遗传算法，名为HyGenar，以优化语法生成。HyGenar在生成语法的句法和语义正确性方面实现了显著提升。|
|**2025-05-21**|**Keep Security! Benchmarking Security Policy Preservation in Large Language Model Contexts Against Indirect Attacks in Question Answering**|Hwan Chang et.al.|[2505.15805](http://arxiv.org/abs/2505.15805)|**[link](https://github.com/hwanchang00/CoPriva)**|
|**2025-05-21**|**Reverse Engineering Human Preferences with Reinforcement Learning**|Lisa Alazraki et.al.|[2505.15795](http://arxiv.org/abs/2505.15795)|null|
|**2025-05-21**|**HCRMP: A LLM-Hinted Contextual Reinforcement Learning Framework for Autonomous Driving**|Zhiwen Chen et.al.|[2505.15793](http://arxiv.org/abs/2505.15793)|null|
|**2025-05-21**|**Large Language Models as Computable Approximations to Solomonoff Induction**|Jun Wan et.al.|[2505.15784](http://arxiv.org/abs/2505.15784)|null|
|**2025-05-21**|**Beyond Hard and Soft: Hybrid Context Compression for Balancing Local and Global Information Retention**|Huanxuan Liao et.al.|[2505.15774](http://arxiv.org/abs/2505.15774)|null|
|**2025-05-21**|**Scalable Defense against In-the-wild Jailbreaking Attacks with Safety Context Retrieval**|Taiye Chen et.al.|[2505.15753](http://arxiv.org/abs/2505.15753)|null|
|**2025-05-21**|**Multi-modal Integration Analysis of Alzheimer's Disease Using Large Language Models and Knowledge Graphs**|Kanan Kiguchi et.al.|[2505.15747](http://arxiv.org/abs/2505.15747)|null|
|**2025-05-21**|**Evolutionary Computation and Large Language Models: A Survey of Methods, Synergies, and Applications**|Dikshit Chauhan et.al.|[2505.15741](http://arxiv.org/abs/2505.15741)|null|
|**2025-05-21**|**HybridProver: Augmenting Theorem Proving with LLM-Driven Proof Synthesis and Refinement**|Jilin Hu et.al.|[2505.15740](http://arxiv.org/abs/2505.15740)|null|
|**2025-05-21**|**Alignment Under Pressure: The Case for Informed Adversaries When Evaluating LLM Defenses**|Xiaoxue Yang et.al.|[2505.15738](http://arxiv.org/abs/2505.15738)|**[link](https://github.com/computationalprivacy/checkpoint-gcg)**|
|**2025-05-20**|**Mind the Gap: Bridging Thought Leap for Improved Chain-of-Thought Tuning**|Haolei Xu et.al.|[2505.14684](http://arxiv.org/abs/2505.14684)|null|
|**2025-05-20**|**UltraEdit: Training-, Subject-, and Memory-Free Lifelong Editing in Large Language Models**|Xiaojie Gu et.al.|[2505.14679](http://arxiv.org/abs/2505.14679)|**[link](https://github.com/xiaojiegu/ultraedit)**|
|**2025-05-20**|**Visionary-R1: Mitigating Shortcuts in Visual Reasoning with Reinforcement Learning**|Jiaer Xia et.al.|[2505.14677](http://arxiv.org/abs/2505.14677)|null|
|**2025-05-20**|**Quartet: Native FP4 Training Can Be Optimal for Large Language Models**|Roberto L. Castro et.al.|[2505.14669](http://arxiv.org/abs/2505.14669)|**[link](https://github.com/ist-daslab/quartet)**|
|**2025-05-20**|**ContextAgent: Context-Aware Proactive LLM Agents with Open-World Sensory Perceptions**|Bufang Yang et.al.|[2505.14668](http://arxiv.org/abs/2505.14668)|null|
|**2025-05-20**|**Beyond Words: Multimodal LLM Knows When to Speak**|Zikai Liao et.al.|[2505.14654](http://arxiv.org/abs/2505.14654)|null|
|**2025-05-20**|**General-Reasoner: Advancing LLM Reasoning Across All Domains**|Xueguang Ma et.al.|[2505.14652](http://arxiv.org/abs/2505.14652)|null|
|**2025-05-20**|**Think Only When You Need with Large Hybrid-Reasoning Models**|Lingjie Jiang et.al.|[2505.14631](http://arxiv.org/abs/2505.14631)|null|
|**2025-05-20**|**KERL: Knowledge-Enhanced Personalized Recipe Recommendation using Large Language Models**|Fnu Mohbat et.al.|[2505.14629](http://arxiv.org/abs/2505.14629)|**[link](https://github.com/mohbattharani/kerl)**|
|**2025-05-20**|**Debating for Better Reasoning: An Unsupervised Multimodal Approach**|Ashutosh Adhikari et.al.|[2505.14627](http://arxiv.org/abs/2505.14627)|null|
|**2025-05-19**|**Trust, But Verify: A Self-Verification Approach to Reinforcement Learning with Verifiable Rewards**|Xiaoyuan Liu et.al.|[2505.13445](http://arxiv.org/abs/2505.13445)|**[link](https://github.com/xyliu-cs/rise)**|
|**2025-05-19**|**Optimizing Anytime Reasoning via Budget Relative Policy Optimization**|Penghui Qi et.al.|[2505.13438](http://arxiv.org/abs/2505.13438)|**[link](https://github.com/sail-sg/anytimereasoner)**|
|**2025-05-19**|**Learnware of Language Models: Specialized Small Language Models Can Do Big**|Zhi-Hao Tan et.al.|[2505.13425](http://arxiv.org/abs/2505.13425)|**[link](https://github.com/learnware-lamda/learnware)**|
|**2025-05-19**|**Make Still Further Progress: Chain of Thoughts for Tabular Data Leaderboard**|Si-Yang Liu et.al.|[2505.13421](http://arxiv.org/abs/2505.13421)|null|
|**2025-05-19**|**AutoMathKG: The automated mathematical knowledge graph based on LLM and vector database**|Rong Bian et.al.|[2505.13406](http://arxiv.org/abs/2505.13406)|null|
|**2025-05-19**|**MR. Judge: Multimodal Reasoner as a Judge**|Renjie Pi et.al.|[2505.13403](http://arxiv.org/abs/2505.13403)|null|
|**2025-05-19**|**Seeing, Saying, Solving: An LLM-to-TL Framework for Cooperative Robots**|Dan BW Choe et.al.|[2505.13376](http://arxiv.org/abs/2505.13376)|null|
|**2025-05-19**|**Multi-Armed Bandits Meet Large Language Models**|Djallel Bouneffouf et.al.|[2505.13355](http://arxiv.org/abs/2505.13355)|null|
|**2025-05-20**|**Sense and Sensitivity: Examining the Influence of Semantic Recall on Long Context Code Reasoning**|Adam Štorek et.al.|[2505.13353](http://arxiv.org/abs/2505.13353)|null|
|**2025-05-19**|**Investigating the Vulnerability of LLM-as-a-Judge Architectures to Prompt-Injection Attacks**|Narek Maloyan et.al.|[2505.13348](http://arxiv.org/abs/2505.13348)|null|
|**2025-05-16**|**Improving Assembly Code Performance with Large Language Models via Reinforcement Learning**|Anjiang Wei et.al.|[2505.11480](http://arxiv.org/abs/2505.11480)|null|
|**2025-05-16**|**HelpSteer3-Preference: Open Human-Annotated Preference Data across Diverse Tasks and Languages**|Zhilin Wang et.al.|[2505.11475](http://arxiv.org/abs/2505.11475)|null|
|**2025-05-16**|**Disentangling Reasoning and Knowledge in Medical Large Language Models**|Rahul Thapa et.al.|[2505.11462](http://arxiv.org/abs/2505.11462)|null|
|**2025-05-16**|**ProxyPrompt: Securing System Prompts against Prompt Extraction Attacks**|Zhixiong Zhuang et.al.|[2505.11459](http://arxiv.org/abs/2505.11459)|null|
|**2025-05-16**|**LLMs unlock new paths to monetizing exploits**|Nicholas Carlini et.al.|[2505.11449](http://arxiv.org/abs/2505.11449)|null|
|**2025-05-16**|**Is Compression Really Linear with Code Intelligence?**|Xianzhen Luo et.al.|[2505.11441](http://arxiv.org/abs/2505.11441)|null|
|**2025-05-16**|**MegaScale-MoE: Large-Scale Communication-Efficient Training of Mixture-of-Experts Models in Production**|Chao Jin et.al.|[2505.11432](http://arxiv.org/abs/2505.11432)|null|
|**2025-05-16**|**EdgeWisePersona: A Dataset for On-Device User Profiling from Natural Language Interactions**|Patryk Bartkowiak et.al.|[2505.11417](http://arxiv.org/abs/2505.11417)|**[link](https://github.com/tclresearcheurope/edgewisepersona)**|
|**2025-05-16**|**MoE-CAP: Benchmarking Cost, Accuracy and Performance of Sparse Mixture-of-Experts Systems**|Yinsicheng Jiang et.al.|[2505.11415](http://arxiv.org/abs/2505.11415)|null|
|**2025-05-16**|**CARES: Comprehensive Evaluation of Safety and Adversarial Robustness in Medical LLMs**|Sijia Chen et.al.|[2505.11413](http://arxiv.org/abs/2505.11413)|null|
|**2025-05-15**|**Neural Thermodynamic Laws for Large Language Model Training**|Ziming Liu et.al.|[2505.10559](http://arxiv.org/abs/2505.10559)|null|
|**2025-05-15**|**RouteNator: A Router-Based Multi-Modal Architecture for Generating Synthetic Training Data for Function Calling LLMs**|Vibha Belavadi et.al.|[2505.10495](http://arxiv.org/abs/2505.10495)|null|
|**2025-05-15**|**Can You Really Trust Code Copilots? Evaluating Large Language Models from a Code Security Perspective**|Yutao Mou et.al.|[2505.10494](http://arxiv.org/abs/2505.10494)|**[link](https://github.com/murraytom/cov-eval)**|
|**2025-05-15**|**CL-RAG: Bridging the Gap in Retrieval-Augmented Generation with Curriculum Learning**|Shaohan Wang et.al.|[2505.10493](http://arxiv.org/abs/2505.10493)|null|
|**2025-05-15**|**Campus AI vs Commercial AI: A Late-Breaking Study on How LLM As-A-Service Customizations Shape Trust and Usage Patterns**|Leon Hannig et.al.|[2505.10490](http://arxiv.org/abs/2505.10490)|null|
|**2025-05-15**|**Large Language Models for Cancer Communication: Evaluating Linguistic Quality, Safety, and Accessibility in Generative AI**|Agnik Saha et.al.|[2505.10472](http://arxiv.org/abs/2505.10472)|null|
|**2025-05-15**|**AI Agents vs. Agentic AI: A Conceptual Taxonomy, Applications and Challenge**|Ranjan Sapkota et.al.|[2505.10468](http://arxiv.org/abs/2505.10468)|null|
|**2025-05-15**|**Superposition Yields Robust Neural Scaling**|Yizhou liu et.al.|[2505.10465](http://arxiv.org/abs/2505.10465)|**[link](https://github.com/liuyz0/superpositionscaling)**|
|**2025-05-15**|**Are Large Language Models Robust in Understanding Code Against Semantics-Preserving Mutations?**|Pedro Orvalho et.al.|[2505.10443](http://arxiv.org/abs/2505.10443)|null|
|**2025-05-15**|**Learning to Think: Information-Theoretic Reinforcement Fine-Tuning for LLMs**|Jingyao Wang et.al.|[2505.10425](http://arxiv.org/abs/2505.10425)|null|
|**2025-05-14**|**Customizing a Large Language Model for VHDL Design of High-Performance Microprocessors**|Nicolas Dupuis et.al.|[2505.09610](http://arxiv.org/abs/2505.09610)|null|
|**2025-05-14**|**Adversarial Suffix Filtering: a Defense Pipeline for LLMs**|David Khachaturov et.al.|[2505.09602](http://arxiv.org/abs/2505.09602)|null|
|**2025-05-14**|**How Hungry is AI? Benchmarking Energy, Water, and Carbon Footprint of LLM Inference**|Nidhal Jegham et.al.|[2505.09598](http://arxiv.org/abs/2505.09598)|null|
|**2025-05-14**|**WorldView-Bench: A Benchmark for Evaluating Global Cultural Perspectives in Large Language Models**|Abdullah Mushtaq et.al.|[2505.09595](http://arxiv.org/abs/2505.09595)|null|
|**2025-05-15**|**Beyond Likes: How Normative Feedback Complements Engagement Signals on Social Media**|Yuchen Wu et.al.|[2505.09583](http://arxiv.org/abs/2505.09583)|null|
|**2025-05-14**|**Ethics and Persuasion in Reinforcement Learning from Human Feedback: A Procedural Rhetorical Approach**|Shannon Lodoen et.al.|[2505.09576](http://arxiv.org/abs/2505.09576)|null|
|**2025-05-14**|**MIGRATION-BENCH: Repository-Level Code Migration Benchmark from Java 8**|Linbo Liu et.al.|[2505.09569](http://arxiv.org/abs/2505.09569)|**[link](https://github.com/amazon-science/self_debug)**|
|**2025-05-14**|**Layered Unlearning for Adversarial Relearning**|Timothy Qian et.al.|[2505.09500](http://arxiv.org/abs/2505.09500)|**[link](https://github.com/12tqian/layered-unlearning)**|
|**2025-05-14**|**Card Sorting Simulator: Augmenting Design of Logical Information Architectures with Large Language Models**|Eduard Kuric et.al.|[2505.09478](http://arxiv.org/abs/2505.09478)|null|
|**2025-05-14**|**Evaluating GPT- and Reasoning-based Large Language Models on Physics Olympiad Problems: Surpassing Human Performance and Implications for Educational Assessment**|Paul Tschisgale et.al.|[2505.09438](http://arxiv.org/abs/2505.09438)|null|
|**2025-05-13**|**CodePDE: An Inference Framework for LLM-driven PDE Solver Generation**|Shanda Li et.al.|[2505.08783](http://arxiv.org/abs/2505.08783)|**[link](https://github.com/lithiumda/codepde)**|
|**2025-05-13**|**DeepMath-Creative: A Benchmark for Evaluating Mathematical Creativity of Large Language Models**|Xiaoyang Chen et.al.|[2505.08744](http://arxiv.org/abs/2505.08744)|**[link](https://github.com/deepmathllm/deepmath)**|
|**2025-05-13**|**Probability Consistency in Large Language Models: Theoretical Foundations Meet Empirical Discrepancies**|Xiaoliang Luo et.al.|[2505.08739](http://arxiv.org/abs/2505.08739)|**[link](https://github.com/braingpt-lovelab/backwards)**|
|**2025-05-13**|**Securing RAG: A Risk Assessment and Mitigation Framework**|Lukas Ammann et.al.|[2505.08728](http://arxiv.org/abs/2505.08728)|null|
|**2025-05-13**|**PWC-MoE: Privacy-Aware Wireless Collaborative Mixture of Experts**|Yang Su et.al.|[2505.08719](http://arxiv.org/abs/2505.08719)|null|
|**2025-05-13**|**LLM-based Prompt Ensemble for Reliable Medical Entity Recognition from EHRs**|K M Sajjadul Islam et.al.|[2505.08704](http://arxiv.org/abs/2505.08704)|null|
|**2025-05-13**|**Adaptive Schema-aware Event Extraction with Retrieval-Augmented Generation**|Sheng Liang et.al.|[2505.08690](http://arxiv.org/abs/2505.08690)|null|
|**2025-05-13**|**Revealing economic facts: LLMs know more than they say**|Marcus Buckmann et.al.|[2505.08662](http://arxiv.org/abs/2505.08662)|null|
|**2025-05-13**|**Enhancing Software Development with Context-Aware Conversational Agents: A User Study on Developer Interactions with Chatbots**|Glaucia Melo et.al.|[2505.08648](http://arxiv.org/abs/2505.08648)|null|
|**2025-05-13**|**Visually Guided Decoding: Gradient-Free Hard Prompt Inversion with Language Models**|Donghoon Kim et.al.|[2505.08622](http://arxiv.org/abs/2505.08622)|null|
|**2025-05-12**|**Relative Overfitting and Accept-Reject Framework**|Yanxin Liu et.al.|[2505.07783](http://arxiv.org/abs/2505.07783)|null|
|**2025-05-12**|**MLE-Dojo: Interactive Environments for Empowering LLM Agents in Machine Learning Engineering**|Rushi Qiang et.al.|[2505.07782](http://arxiv.org/abs/2505.07782)|**[link](https://github.com/MLE-Dojo/MLE-Dojo)**|
|**2025-05-12**|**Agent RL Scaling Law: Agent RL with Spontaneous Code Execution for Mathematical Problem Solving**|Xinji Mai et.al.|[2505.07773](http://arxiv.org/abs/2505.07773)|**[link](https://github.com/anonymize-author/agentrl)**|
|**2025-05-12**|**Enhancing Code Generation via Bidirectional Comment-Level Mutual Grounding**|Yifeng Di et.al.|[2505.07768](http://arxiv.org/abs/2505.07768)|**[link](https://github.com/NecoraNyaru/PInG)**|
|**2025-05-12**|**Spoken Language Understanding on Unseen Tasks With In-Context Learning**|Neeraj Agrawal et.al.|[2505.07731](http://arxiv.org/abs/2505.07731)|null|
|**2025-05-12**|**Circuit Partitioning Using Large Language Models for Quantum Compilation and Simulations**|Pranav Sinha et.al.|[2505.07711](http://arxiv.org/abs/2505.07711)|null|
|**2025-05-12**|**PatchTrack: A Comprehensive Analysis of ChatGPT's Influence on Pull Request Outcomes**|Daniel Ogenrwot et.al.|[2505.07700](http://arxiv.org/abs/2505.07700)|null|
|**2025-05-12**|**SpecRouter: Adaptive Routing for Multi-Level Speculative Decoding in Large Language Models**|Hang Wu et.al.|[2505.07680](http://arxiv.org/abs/2505.07680)|null|
|**2025-05-13**|**OnPrem.LLM: A Privacy-Conscious Document Intelligence Toolkit**|Arun S. Maiya et.al.|[2505.07672](http://arxiv.org/abs/2505.07672)|**[link](https://github.com/amaiya/onprem)**|
|**2025-05-12**|**Benchmarking Retrieval-Augmented Generation for Chemistry**|Xianrui Zhong et.al.|[2505.07671](http://arxiv.org/abs/2505.07671)|null|
|**2025-05-09**|**From Millions of Tweets to Actionable Insights: Leveraging LLMs for User Profiling**|Vahid Rahimzadeh et.al.|[2505.06184](http://arxiv.org/abs/2505.06184)|null|
|**2025-05-09**|**A Large Language Model-Enhanced Q-learning for Capacitated Vehicle Routing Problem with Time Windows**|Linjiang Cao et.al.|[2505.06178](http://arxiv.org/abs/2505.06178)|null|
|**2025-05-09**|**Turbo-ICL: In-Context Learning-Based Turbo Equalization**|Zihang Song et.al.|[2505.06175](http://arxiv.org/abs/2505.06175)|null|
|**2025-05-09**|**A Scaling Law for Token Efficiency in LLM Fine-Tuning Under Fixed Compute Budgets**|Ryan Lagasse et.al.|[2505.06150](http://arxiv.org/abs/2505.06150)|null|
|**2025-05-09**|**LLMs Get Lost In Multi-Turn Conversation**|Philippe Laban et.al.|[2505.06120](http://arxiv.org/abs/2505.06120)|**[link](https://github.com/microsoft/lost_in_conversation)**|
|**2025-05-09**|**Free and Fair Hardware: A Pathway to Copyright Infringement-Free Verilog Generation using LLMs**|Sam Bush et.al.|[2505.06096](http://arxiv.org/abs/2505.06096)|null|
|**2025-05-09**|**Assessing Tenstorrent's RISC-V MatMul Acceleration Capabilities**|Hiari Pizzini Cavagna et.al.|[2505.06085](http://arxiv.org/abs/2505.06085)|null|
|**2025-05-09**|**Healthy LLMs? Benchmarking LLM Knowledge of UK Government Public Health Information**|Joshua Harris et.al.|[2505.06046](http://arxiv.org/abs/2505.06046)|null|
|**2025-05-09**|**Task-Adapter++: Task-specific Adaptation with Order-aware Alignment for Few-shot Action Recognition**|Congqi Cao et.al.|[2505.06002](http://arxiv.org/abs/2505.06002)|**[link](https://github.com/jaulin-bage/task-adapter-pp)**|
|**2025-05-09**|**NeoQA: Evidence-based Question Answering with Generated News Events**|Max Glockner et.al.|[2505.05949](http://arxiv.org/abs/2505.05949)|**[link](https://github.com/amazon-science/neoqa)**|
|**2025-05-08**|**ComPO: Preference Alignment via Comparison Oracles**|Peter Chen et.al.|[2505.05465](http://arxiv.org/abs/2505.05465)|null|
|**2025-05-08**|**Bring Reason to Vision: Understanding Perception and Reasoning through Model Merging**|Shiqi Chen et.al.|[2505.05464](http://arxiv.org/abs/2505.05464)|**[link](https://github.com/shiqichen17/vlm_merging)**|
|**2025-05-08**|**Conversational Process Model Redesign**|Nataliia Klievtsova et.al.|[2505.05453](http://arxiv.org/abs/2505.05453)|null|
|**2025-05-08**|**clem:todd: A Framework for the Systematic Benchmarking of LLM-Based Task-Oriented Dialogue System Realisations**|Chalamalasetti Kranti et.al.|[2505.05445](http://arxiv.org/abs/2505.05445)|null|
|**2025-05-08**|**GesPrompt: Leveraging Co-Speech Gestures to Augment LLM-Based Interaction in Virtual Reality**|Xiyun Hu et.al.|[2505.05441](http://arxiv.org/abs/2505.05441)|null|
|**2025-05-08**|**Ultra-FineWeb: Efficient Data Filtering and Verification for High-Quality LLM Training Data**|Yudong Wang et.al.|[2505.05427](http://arxiv.org/abs/2505.05427)|null|
|**2025-05-09**|**LiTransProQA: an LLM-based Literary Translation evaluation metric with Professional Question Answering**|Ran Zhang et.al.|[2505.05423](http://arxiv.org/abs/2505.05423)|**[link](https://github.com/zhangr2021/TransProQA)**|
|**2025-05-08**|**ICon: In-Context Contribution for Automatic Data Selection**|Yixin Yang et.al.|[2505.05327](http://arxiv.org/abs/2505.05327)|null|
|**2025-05-08**|**Toward Reasonable Parrots: Why Large Language Models Should Argue with Us by Design**|Elena Musi et.al.|[2505.05298](http://arxiv.org/abs/2505.05298)|null|
|**2025-05-08**|**HEXGEN-TEXT2SQL: Optimizing LLM Inference Request Scheduling for Agentic Text-to-SQL Workflow**|You Peng et.al.|[2505.05286](http://arxiv.org/abs/2505.05286)|**[link](https://github.com/relaxed-system-lab/hexgen-flow)**|
|**2025-05-07**|**OmniGIRL: A Multilingual and Multimodal Benchmark for GitHub Issue Resolution**|Lianghong Guo et.al.|[2505.04606](http://arxiv.org/abs/2505.04606)|**[link](https://github.com/deepsoftwareanalytics/omnigirl)**|
|**2025-05-08**|**MonoCoP: Chain-of-Prediction for Monocular 3D Object Detection**|Zhihao Zhang et.al.|[2505.04594](http://arxiv.org/abs/2505.04594)|null|
|**2025-05-07**|**ZeroSearch: Incentivize the Search Capability of LLMs without Searching**|Hao Sun et.al.|[2505.04588](http://arxiv.org/abs/2505.04588)|**[link](https://github.com/alibaba-nlp/zerosearch)**|
|**2025-05-07**|**SlideItRight: Using AI to Find Relevant Slides and Provide Feedback for Open-Ended Questions**|Chloe Qianhui Zhao et.al.|[2505.04584](http://arxiv.org/abs/2505.04584)|**[link](https://github.com/zqh0421/slideitright)**|
|**2025-05-07**|**Comparative Analysis of Carbon Footprint in Manual vs. LLM-Assisted Code Development**|Kuen Sum Cheung et.al.|[2505.04521](http://arxiv.org/abs/2505.04521)|null|
|**2025-05-07**|**Pangu Ultra MoE: How to Train Your Big MoE on Ascend NPUs**|Yehui Tang et.al.|[2505.04519](http://arxiv.org/abs/2505.04519)|null|
|**2025-05-07**|**CAD-Llama: Leveraging Large Language Models for Computer-Aided Design Parametric 3D Model Generation**|Jiahao Li et.al.|[2505.04481](http://arxiv.org/abs/2505.04481)|null|
|**2025-05-07**|**TrajEvo: Designing Trajectory Prediction Heuristics via LLM-driven Evolution**|Zhikai Zhao et.al.|[2505.04480](http://arxiv.org/abs/2505.04480)|**[link](https://github.com/ai4co/trajevo)**|
|**2025-05-07**|**M2Rec: Multi-scale Mamba for Efficient Sequential Recommendation**|Qianru Zhang et.al.|[2505.04445](http://arxiv.org/abs/2505.04445)|null|
|**2025-05-07**|**Towards Effectively Leveraging Execution Traces for Program Repair with Code LLMs**|Mirazul Haque et.al.|[2505.04441](http://arxiv.org/abs/2505.04441)|null|
|**2025-05-06**|**Graph Drawing for LLMs: An Empirical Evaluation**|Walter Didimo et.al.|[2505.03678](http://arxiv.org/abs/2505.03678)|null|
|**2025-05-06**|**PhysLLM: Harnessing Large Language Models for Cross-Modal Remote Physiological Sensing**|Yiping Xie et.al.|[2505.03621](http://arxiv.org/abs/2505.03621)|null|
|**2025-05-06**|**LlamaFirewall: An open source guardrail system for building secure AI agents**|Sahana Chennabasappa et.al.|[2505.03574](http://arxiv.org/abs/2505.03574)|null|
|**2025-05-06**|**Say It Another Way: A Framework for User-Grounded Paraphrasing**|Cléa Chataigner et.al.|[2505.03563](http://arxiv.org/abs/2505.03563)|null|
|**2025-05-06**|**A Comprehensive Survey of Large AI Models for Future Communications: Foundations, Applications and Challenges**|Feibo Jiang et.al.|[2505.03556](http://arxiv.org/abs/2505.03556)|**[link](https://github.com/jiangfeibo/comlam)**|
|**2025-05-06**|**A Hashgraph-Inspired Consensus Mechanism for Reliable Multi-Model Reasoning**|Kolawole E. Ogunsina et.al.|[2505.03553](http://arxiv.org/abs/2505.03553)|null|
|**2025-05-06**|**Faster MoE LLM Inference for Extremely Large Models**|Haoqi Yang et.al.|[2505.03531](http://arxiv.org/abs/2505.03531)|null|
|**2025-05-06**|**Ruled by the Representation Space: On the University's Embrace of Large Language Models**|Katia Schwerzmann et.al.|[2505.03513](http://arxiv.org/abs/2505.03513)|null|
|**2025-05-06**|**BadLingual: A Novel Lingual-Backdoor Attack against Large Language Models**|Zihan Wang et.al.|[2505.03501](http://arxiv.org/abs/2505.03501)|null|
|**2025-05-06**|**am-ELO: A Stable Framework for Arena-based LLM Evaluation**|Zirui Liu et.al.|[2505.03475](http://arxiv.org/abs/2505.03475)|null|
|**2025-05-05**|**Scenethesis: A Language and Vision Agentic Framework for 3D Scene Generation**|Lu Ling et.al.|[2505.02836](http://arxiv.org/abs/2505.02836)|null|
|**2025-05-05**|**ReplaceMe: Network Simplification via Layer Pruning and Linear Transformations**|Dmitriy Shopkhoev et.al.|[2505.02819](http://arxiv.org/abs/2505.02819)|**[link](https://github.com/mts-ai/replaceme)**|
|**2025-05-05**|**Towards Quantifying the Hessian Structure of Neural Networks**|Zhaorui Dong et.al.|[2505.02809](http://arxiv.org/abs/2505.02809)|**[link](https://github.com/zyushun/hessian-structure)**|
|**2025-05-05**|**Generating HomeAssistant Automations Using an LLM-based Chatbot**|Mathyas Giudici et.al.|[2505.02802](http://arxiv.org/abs/2505.02802)|null|
|**2025-05-05**|**HSplitLoRA: A Heterogeneous Split Parameter-Efficient Fine-Tuning Framework for Large Language Models**|Zheng Lin et.al.|[2505.02795](http://arxiv.org/abs/2505.02795)|null|
|**2025-05-05**|**Giving Simulated Cells a Voice: Evolving Prompt-to-Intervention Models for Cellular Control**|Nam H. Le et.al.|[2505.02766](http://arxiv.org/abs/2505.02766)|null|
|**2025-05-05**|**Bye-bye, Bluebook? Automating Legal Procedure with Large Language Models**|Matthew Dahl et.al.|[2505.02763](http://arxiv.org/abs/2505.02763)|null|
|**2025-05-06**|**Knowledge Graphs for Enhancing Large Language Models in Entity Disambiguation**|Gerard Pons et.al.|[2505.02737](http://arxiv.org/abs/2505.02737)|null|
|**2025-05-05**|**FormalMATH: Benchmarking Formal Mathematical Reasoning of Large Language Models**|Zhouliang Yu et.al.|[2505.02735](http://arxiv.org/abs/2505.02735)|**[link](https://github.com/sphere-ai-lab/formalmath-bench)**|
|**2025-05-05**|**Enhancing LLMs' Clinical Reasoning with Real-World Data from a Nationwide Sepsis Registry**|Junu Kim et.al.|[2505.02722](http://arxiv.org/abs/2505.02722)|**[link](https://github.com/starmpcc/c-reason)**|
|**2025-05-02**|**Document Retrieval Augmented Fine-Tuning (DRAFT) for safety-critical software assessments**|Regan Bolton et.al.|[2505.01307](http://arxiv.org/abs/2505.01307)|null|
|**2025-05-02**|**FlowDubber: Movie Dubbing with LLM-based Semantic-aware Learning and Flow Matching based Voice Enhancing**|Gaoxiang Cong et.al.|[2505.01263](http://arxiv.org/abs/2505.01263)|null|
|**2025-05-02**|**Digital Pathway Curation (DPC): a comparative pipeline to assess the reproducibility, consensus and accuracy across Gemini, PubMed, and scientific reviewers in biomedical research**|Flavio Lichtenstein et.al.|[2505.01259](http://arxiv.org/abs/2505.01259)|null|
|**2025-05-02**|**LLM Security: Vulnerabilities, Attacks, Defenses, and Countermeasures**|Francisco Aguilera-Martínez et.al.|[2505.01177](http://arxiv.org/abs/2505.01177)|null|
|**2025-05-02**|**Methodological Foundations for AI-Driven Survey Question Generation**|Ted K. Mburu et.al.|[2505.01150](http://arxiv.org/abs/2505.01150)|null|
|**2025-05-02**|**Retrieval-Augmented Generation in Biomedicine: A Survey of Technologies, Datasets, and Clinical Applications**|Jiawei He et.al.|[2505.01146](http://arxiv.org/abs/2505.01146)|null|
|**2025-05-02**|**MateICL: Mitigating Attention Dispersion in Large-Scale In-Context Learning**|Murtadha Ahmed et.al.|[2505.01110](http://arxiv.org/abs/2505.01110)|null|
|**2025-05-02**|**MADIL: An MDL-based Framework for Efficient Program Synthesis in the ARC Benchmark**|Sébastien Ferré et.al.|[2505.01081](http://arxiv.org/abs/2505.01081)|null|
|**2025-05-02**|**Zero-Shot Document-Level Biomedical Relation Extraction via Scenario-based Prompt Design in Two-Stage with LLM**|Lei Zhao et.al.|[2505.01077](http://arxiv.org/abs/2505.01077)|null|
|**2025-05-02**|**WirelessAgent: Large Language Model Agents for Intelligent Wireless Networks**|Jingwen Tong et.al.|[2505.01074](http://arxiv.org/abs/2505.01074)|**[link](https://github.com/jwentong/wirelessagent_r1)**|
|**2025-05-01**|**Steering Large Language Models with Register Analysis for Arbitrary Style Transfer**|Xinchen Yang et.al.|[2505.00679](http://arxiv.org/abs/2505.00679)|null|
|**2025-05-01**|**Rethinking Memory in AI: Taxonomy, Operations, Topics, and Future Directions**|Yiming Du et.al.|[2505.00675](http://arxiv.org/abs/2505.00675)|**[link](https://github.com/elvin-yiming-du/survey_memory_in_ai)**|
|**2025-05-01**|**DeepCritic: Deliberate Critique with Large Language Models**|Wenkai Yang et.al.|[2505.00662](http://arxiv.org/abs/2505.00662)|**[link](https://github.com/rucbm/deepcritic)**|
|**2025-05-01**|**Large Language Models Understanding: an Inherent Ambiguity Barrier**|Daniel N. Nissani et.al.|[2505.00654](http://arxiv.org/abs/2505.00654)|null|
|**2025-05-01**|**Open-Source LLM-Driven Federated Transformer for Predictive IoV Management**|Yazan Otoum et.al.|[2505.00651](http://arxiv.org/abs/2505.00651)|null|
|**2025-05-01**|**Investigating Task Arithmetic for Zero-Shot Information Retrieval**|Marco Braga et.al.|[2505.00649](http://arxiv.org/abs/2505.00649)|**[link](https://github.com/detectivemb/task-arithmetic-for-zs-ir)**|
|**2025-05-01**|**The Illusion of Role Separation: Hidden Shortcuts in LLM Role Learning (and How to Fix Them)**|Zihao Wang et.al.|[2505.00626](http://arxiv.org/abs/2505.00626)|null|
|**2025-05-01**|**FineScope : Precision Pruning for Domain-Specialized Large Language Models Using SAE-Guided Self-Data Cultivation**|Chaitali Bhattacharyya et.al.|[2505.00624](http://arxiv.org/abs/2505.00624)|null|
|**2025-05-01**|**Combining LLMs with Logic-Based Framework to Explain MCTS**|Ziyan An et.al.|[2505.00610](http://arxiv.org/abs/2505.00610)|null|
|**2025-05-01**|**Block Circulant Adapter for Large Language Models**|Xinyu Ding et.al.|[2505.00582](http://arxiv.org/abs/2505.00582)|null|
|**2025-04-30**|**TRUST: An LLM-Based Dialogue System for Trauma Understanding and Structured Assessments**|Sichang Tu et.al.|[2504.21851](http://arxiv.org/abs/2504.21851)|null|
|**2025-04-30**|**An Empirical Study on the Effectiveness of Large Language Models for Binary Code Understanding**|Xiuwei Shang et.al.|[2504.21803](http://arxiv.org/abs/2504.21803)|null|
|**2025-04-30**|**MAC-Tuning: LLM Multi-Compositional Problem Reasoning with Enhanced Knowledge Boundary Awareness**|Junsheng Huang et.al.|[2504.21773](http://arxiv.org/abs/2504.21773)|null|
|**2025-04-30**|**LLM-based Interactive Imitation Learning for Robotic Manipulation**|Jonas Werner et.al.|[2504.21769](http://arxiv.org/abs/2504.21769)|**[link](https://github.com/tubicor/llm-iteach)**|
|**2025-04-30**|**TheraQuest: A Gamified, LLM-Powered Simulation for Massage Therapy Training**|Shengqian Wang et.al.|[2504.21735](http://arxiv.org/abs/2504.21735)|null|
|**2025-04-30**|**Hoist with His Own Petard: Inducing Guardrails to Facilitate Denial-of-Service Attacks on Retrieval-Augmented Generation of LLMs**|Pan Suo et.al.|[2504.21680](http://arxiv.org/abs/2504.21680)|null|
|**2025-04-30**|**Traceback of Poisoning Attacks to Retrieval-Augmented Generation**|Baolei Zhang et.al.|[2504.21668](http://arxiv.org/abs/2504.21668)|null|
|**2025-04-30**|**Meeseeks: An Iterative Benchmark Evaluating LLMs Multi-Turn Instruction-Following Ability**|Jiaming Wang et.al.|[2504.21625](http://arxiv.org/abs/2504.21625)|null|
|**2025-04-30**|**RDF-Based Structured Quality Assessment Representation of Multilingual LLM Evaluations**|Jonas Gwozdz et.al.|[2504.21605](http://arxiv.org/abs/2504.21605)|null|
|**2025-04-30**|**Leveraging Pre-trained Large Language Models with Refined Prompting for Online Task and Motion Planning**|Huihui Guo et.al.|[2504.21596](http://arxiv.org/abs/2504.21596)|null|
|**2025-04-29**|**Toward Efficient Exploration by Large Language Model Agents**|Dilip Arumugam et.al.|[2504.20997](http://arxiv.org/abs/2504.20997)|null|
|**2025-04-29**|**X-Fusion: Introducing New Modality to Frozen Large Language Models**|Sicheng Mo et.al.|[2504.20996](http://arxiv.org/abs/2504.20996)|null|
|**2025-04-29**|**ACE: A Security Architecture for LLM-Integrated App Systems**|Evan Li et.al.|[2504.20984](http://arxiv.org/abs/2504.20984)|null|
|**2025-04-29**|**Real-Time Wayfinding Assistant for Blind and Low-Vision Users**|Dabbrata Das et.al.|[2504.20976](http://arxiv.org/abs/2504.20976)|null|
|**2025-04-29**|**SetKE: Knowledge Editing for Knowledge Elements Overlap**|Yifan Wei et.al.|[2504.20972](http://arxiv.org/abs/2504.20972)|null|
|**2025-04-29**|**OSVBench: Benchmarking LLMs on Specification Generation Tasks for Operating System Verification**|Shangyu Li et.al.|[2504.20964](http://arxiv.org/abs/2504.20964)|**[link](https://github.com/lishangyu-hkust/osvbench)**|
|**2025-04-29**|**Information Gravity: A Field-Theoretic Model for Token Selection in Large Language Models**|Maryna Vyshnyvetska et.al.|[2504.20951](http://arxiv.org/abs/2504.20951)|null|
|**2025-04-29**|**Trace-of-Thought: Enhanced Arithmetic Problem Solving via Reasoning Distillation From Large to Small Language Models**|Tyler McDonald et.al.|[2504.20946](http://arxiv.org/abs/2504.20946)|null|
|**2025-04-29**|**ChestX-Reasoner: Advancing Radiology Foundation Models with Reasoning through Step-by-Step Verification**|Ziqing Fan et.al.|[2504.20930](http://arxiv.org/abs/2504.20930)|**[link](https://github.com/MAGIC-AI4Med/ChestX-Reasoner)**|
|**2025-04-29**|**An Empirical Study on the Capability of LLMs in Decomposing Bug Reports**|Zhiyuan Chen et.al.|[2504.20911](http://arxiv.org/abs/2504.20911)|null|
|**2025-04-28**|**AutoJudge: Judge Decoding Without Manual Annotation**|Roman Garipov et.al.|[2504.20039](http://arxiv.org/abs/2504.20039)|null|
|**2025-04-28**|**Better To Ask in English? Evaluating Factual Accuracy of Multilingual LLMs in English and Low-Resource Languages**|Pritika Rohera et.al.|[2504.20022](http://arxiv.org/abs/2504.20022)|null|
|**2025-04-28**|**Modular Machine Learning: An Indispensable Path towards New-Generation Large Language Models**|Xin Wang et.al.|[2504.20020](http://arxiv.org/abs/2504.20020)|null|
|**2025-04-29**|**LLM-Generated Fake News Induces Truth Decay in News Ecosystem: A Case Study on Neural News Recommendation**|Beizhe Hu et.al.|[2504.20013](http://arxiv.org/abs/2504.20013)|null|
|**2025-04-28**|**Towards Automated Scoping of AI for Social Good Projects**|Jacob Emmerson et.al.|[2504.20010](http://arxiv.org/abs/2504.20010)|null|
|**2025-04-28**|**Knowledge Distillation of Domain-adapted LLMs for Question-Answering in Telecom**|Rishika Sen et.al.|[2504.20000](http://arxiv.org/abs/2504.20000)|null|
|**2025-04-28**|**TD-EVAL: Revisiting Task-Oriented Dialogue Evaluation by Combining Turn-Level Precision with Dialogue-Level Comparisons**|Emre Can Acikgoz et.al.|[2504.19982](http://arxiv.org/abs/2504.19982)|null|
|**2025-04-28**|**Accurate and Diverse LLM Mathematical Reasoning via Automated PRM-Guided GFlowNets**|Adam Younsi et.al.|[2504.19981](http://arxiv.org/abs/2504.19981)|null|
|**2025-04-29**|**From Concept to Practice: an Automated LLM-aided UVM Machine for RTL Verification**|Junhao Ye et.al.|[2504.19959](http://arxiv.org/abs/2504.19959)|null|
|**2025-04-28**|**Can AI Agents Design and Implement Drug Discovery Pipelines?**|Khachik Smbatyan et.al.|[2504.19912](http://arxiv.org/abs/2504.19912)|null|
|**2025-04-25**|**Investigating Co-Constructive Behavior of Large Language Models in Explanation Dialogues**|Leandra Fichtel et.al.|[2504.18483](http://arxiv.org/abs/2504.18483)|null|
|**2025-04-25**|**LLMpatronous: Harnessing the Power of LLMs For Vulnerability Detection**|Rajesh Yarra et.al.|[2504.18423](http://arxiv.org/abs/2504.18423)|null|
|**2025-04-25**|**BitNet v2: Native 4-bit Activations with Hadamard Transformation for 1-bit LLMs**|Hongyu Wang et.al.|[2504.18415](http://arxiv.org/abs/2504.18415)|null|
|**2025-04-25**|**Expressing stigma and inappropriate responses prevents LLMs from safely replacing mental health providers**|Jared Moore et.al.|[2504.18412](http://arxiv.org/abs/2504.18412)|**[link](https://github.com/jlcmoore/llms-as-therapists)**|
|**2025-04-25**|**Bridge the Domains: Large Language Models Enhanced Cross-domain Sequential Recommendation**|Qidong Liu et.al.|[2504.18383](http://arxiv.org/abs/2504.18383)|null|
|**2025-04-25**|**Auto-SLURP: A Benchmark Dataset for Evaluating Multi-Agent Frameworks in Smart Personal Assistant**|Lei Shen et.al.|[2504.18373](http://arxiv.org/abs/2504.18373)|null|
|**2025-04-25**|**ThreMoLIA: Threat Modeling of Large Language Model-Integrated Applications**|Felix Viktor Jedrzejewski et.al.|[2504.18369](http://arxiv.org/abs/2504.18369)|null|
|**2025-04-25**|**Revisiting Data Auditing in Large Vision-Language Models**|Hongyu Zhu et.al.|[2504.18349](http://arxiv.org/abs/2504.18349)|null|
|**2025-04-25**|**Comparing Uncertainty Measurement and Mitigation Methods for Large Language Models: A Systematic Review**|Toghrul Abbasli et.al.|[2504.18346](http://arxiv.org/abs/2504.18346)|null|
|**2025-04-25**|**Large Language Models to Accelerate Organic Chemistry Synthesis**|Yu Zhang et.al.|[2504.18340](http://arxiv.org/abs/2504.18340)|null|
|**2025-04-24**|**Replay to Remember: Retaining Domain Knowledge in Streaming Language Models**|Sneh Pillai et.al.|[2504.17780](http://arxiv.org/abs/2504.17780)|null|
|**2025-04-24**|**Towards Robust LLMs: an Adversarial Robustness Measurement Framework**|Natan Levy et.al.|[2504.17723](http://arxiv.org/abs/2504.17723)|null|
|**2025-04-24**|**Multilingual Performance Biases of Large Language Models in Education**|Vansh Gupta et.al.|[2504.17720](http://arxiv.org/abs/2504.17720)|null|
|**2025-04-24**|**Ensemble Bayesian Inference: Leveraging Small Language Models to Achieve LLM-level Accuracy in Profile Matching Tasks**|Haru-Tada Sato et.al.|[2504.17685](http://arxiv.org/abs/2504.17685)|null|
|**2025-04-24**|**Energy Considerations of Large Language Model Inference and Efficiency Optimizations**|Jared Fernandez et.al.|[2504.17674](http://arxiv.org/abs/2504.17674)|null|
|**2025-04-24**|**Cross-region Model Training with Communication-Computation Overlapping and Delay Compensation**|Ying Zhu et.al.|[2504.17672](http://arxiv.org/abs/2504.17672)|null|
|**2025-04-24**|**Towards a HIPAA Compliant Agentic AI System in Healthcare**|Subash Neupane et.al.|[2504.17669](http://arxiv.org/abs/2504.17669)|null|
|**2025-04-24**|**L3: DIMM-PIM Integrated Architecture and Coordination for Scalable Long-Context LLM Inference**|Qingyuan Liu et.al.|[2504.17584](http://arxiv.org/abs/2504.17584)|null|
|**2025-04-25**|**DeepDistill: Enhancing LLM Reasoning Capabilities via Large-Scale Difficulty-Graded Data Training**|Xiaoyu Tian et.al.|[2504.17565](http://arxiv.org/abs/2504.17565)|null|
|**2025-04-24**|**HalluLens: LLM Hallucination Benchmark**|Yejin Bang et.al.|[2504.17550](http://arxiv.org/abs/2504.17550)|null|
|**2025-04-23**|**IberBench: LLM Evaluation on Iberian Languages**|José Ángel González et.al.|[2504.16921](http://arxiv.org/abs/2504.16921)|null|
|**2025-04-23**|**Do Large Language Models know who did what to whom?**|Joseph M. Denning et.al.|[2504.16884](http://arxiv.org/abs/2504.16884)|null|
|**2025-04-23**|**Enhancing Critical Thinking with AI: A Tailored Warning System for RAG Models**|Xuyang Zhu et.al.|[2504.16883](http://arxiv.org/abs/2504.16883)|null|
|**2025-04-23**|**Context-Enhanced Vulnerability Detection Based on Large Language Model**|Yixin Yang et.al.|[2504.16877](http://arxiv.org/abs/2504.16877)|null|
|**2025-04-24**|**Exploring How LLMs Capture and Represent Domain-Specific Knowledge**|Mirian Hipolito Garcia et.al.|[2504.16871](http://arxiv.org/abs/2504.16871)|null|
|**2025-04-23**|**Emo Pillars: Knowledge Distillation to Support Fine-Grained Context-Aware and Context-Less Emotion Classification**|Alexander Shvets et.al.|[2504.16856](http://arxiv.org/abs/2504.16856)|null|
|**2025-04-23**|**Monte Carlo Planning with Large Language Model for Text-Based Game Agents**|Zijing Shi et.al.|[2504.16855](http://arxiv.org/abs/2504.16855)|null|
|**2025-04-23**|**Improving Significant Wave Height Prediction Using Chronos Models**|Yilin Zhai et.al.|[2504.16834](http://arxiv.org/abs/2504.16834)|null|
|**2025-04-23**|**LRASGen: LLM-based RESTful API Specification Generation**|Sida Deng et.al.|[2504.16833](http://arxiv.org/abs/2504.16833)|null|
|**2025-04-23**|**Decoupled Global-Local Alignment for Improving Compositional Understanding**|Xiaoxing Hu et.al.|[2504.16801](http://arxiv.org/abs/2504.16801)|null|
|**2025-04-22**|**TTRL: Test-Time Reinforcement Learning**|Yuxin Zuo et.al.|[2504.16084](http://arxiv.org/abs/2504.16084)|**[link](https://github.com/prime-rl/ttrl)**|
|**2025-04-22**|**LLMs are Greedy Agents: Effects of RL Fine-tuning on Decision-Making Abilities**|Thomas Schmied et.al.|[2504.16078](http://arxiv.org/abs/2504.16078)|null|
|**2025-04-22**|**PHYBench: Holistic Evaluation of Physical Perception and Reasoning in Large Language Models**|Shi Qiu et.al.|[2504.16074](http://arxiv.org/abs/2504.16074)|null|
|**2025-04-22**|**Automated Static Vulnerability Detection via a Holistic Neuro-symbolic Approach**|Penghui Li et.al.|[2504.16057](http://arxiv.org/abs/2504.16057)|null|
|**2025-04-22**|**Honey, I Shrunk the Language Model: Impact of Knowledge Distillation Methods on Performance and Explainability**|Daniel Hendriks et.al.|[2504.16056](http://arxiv.org/abs/2504.16056)|null|
|**2025-04-23**|**Certified Mitigation of Worst-Case LLM Copyright Infringement**|Jingyu Zhang et.al.|[2504.16046](http://arxiv.org/abs/2504.16046)|null|
|**2025-04-23**|**CAPO: Cost-Aware Prompt Optimization**|Tom Zehle et.al.|[2504.16005](http://arxiv.org/abs/2504.16005)|**[link](https://github.com/finitearth/capo)**|
|**2025-04-23**|**From Human Memory to AI Memory: A Survey on Memory Mechanisms in the Era of LLMs**|Yaxiong Wu et.al.|[2504.15965](http://arxiv.org/abs/2504.15965)|null|
|**2025-04-22**|**FairTranslate: An English-French Dataset for Gender Bias Evaluation in Machine Translation by Overcoming Gender Binarity**|Fanny Jourdan et.al.|[2504.15941](http://arxiv.org/abs/2504.15941)|**[link](https://github.com/fanny-jourdan/FairTranslate)**|
|**2025-04-22**|**StreamRL: Scalable, Heterogeneous, and Elastic RL for LLMs with Disaggregated Stream Generation**|Yinmin Zhong et.al.|[2504.15930](http://arxiv.org/abs/2504.15930)|null|
|**2025-04-21**|**Stop Summation: Min-Form Credit Assignment Is All Process Reward Model Needs for Reasoning**|Jie Cheng et.al.|[2504.15275](http://arxiv.org/abs/2504.15275)|**[link](https://github.com/cjreinforce/pure)**|
|**2025-04-21**|**Interpretable Locomotion Prediction in Construction Using a Memory-Driven LLM Agent With Chain-of-Thought Reasoning**|Ehsan Ahmadi et.al.|[2504.15263](http://arxiv.org/abs/2504.15263)|null|
|**2025-04-21**|**CRUST-Bench: A Comprehensive Benchmark for C-to-safe-Rust Transpilation**|Anirudh Khatry et.al.|[2504.15254](http://arxiv.org/abs/2504.15254)|**[link](https://github.com/anirudhkhatry/crust-bench)**|
|**2025-04-21**|**Evaluating Judges as Evaluators: The JETTS Benchmark of LLM-as-Judges as Test-Time Scaling Evaluators**|Yilun Zhou et.al.|[2504.15253](http://arxiv.org/abs/2504.15253)|**[link](https://github.com/salesforceairesearch/jetts-benchmark)**|
|**2025-04-21**|**MR. Guard: Multilingual Reasoning Guardrail using Curriculum Learning**|Yahan Yang et.al.|[2504.15241](http://arxiv.org/abs/2504.15241)|null|
|**2025-04-21**|**EvalAgent: Discovering Implicit Evaluation Criteria from the Web**|Manya Wadhwa et.al.|[2504.15219](http://arxiv.org/abs/2504.15219)|null|
|**2025-04-21**|**Integrating Symbolic Execution into the Fine-Tuning of Code-Generating LLMs**|Marina Sakharova et.al.|[2504.15210](http://arxiv.org/abs/2504.15210)|null|
|**2025-04-21**|**Compute-Optimal LLMs Provably Generalize Better With Scale**|Marc Finzi et.al.|[2504.15208](http://arxiv.org/abs/2504.15208)|null|
|**2025-04-21**|**Support Evaluation for the TREC 2024 RAG Track: Comparing Human versus LLM Judges**|Nandan Thakur et.al.|[2504.15205](http://arxiv.org/abs/2504.15205)|null|
|**2025-04-22**|**Synergistic Weak-Strong Collaboration by Aligning Preferences**|Yizhu Jiao et.al.|[2504.15188](http://arxiv.org/abs/2504.15188)|null|
|**2025-04-18**|**DP2Unlearning: An Efficient and Guaranteed Unlearning Framework for LLMs**|Tamim Al Mahmud et.al.|[2504.13774](http://arxiv.org/abs/2504.13774)|**[link](https://github.com/tamimalmahmud/DP2Unlearning)**|
|**2025-04-18**|**Detecting Malicious Source Code in PyPI Packages with LLMs: Does RAG Come in Handy?**|Motunrayo Ibiyo et.al.|[2504.13769](http://arxiv.org/abs/2504.13769)|null|
|**2025-04-18**|**Controlled Territory and Conflict Tracking (CONTACT): (Geo-)Mapping Occupied Territory from Open Source Intelligence**|Paul K. Mandal et.al.|[2504.13730](http://arxiv.org/abs/2504.13730)|**[link](https://github.com/paulkmandal/contact)**|
|**2025-04-18**|**OpenDeception: Benchmarking and Investigating AI Deceptive Behaviors via Open-ended Interaction Simulation**|Yichen Wu et.al.|[2504.13707](http://arxiv.org/abs/2504.13707)|null|
|**2025-04-18**|**Exploring Multimodal Prompt for Visualization Authoring with Large Language Models**|Zhen Wen et.al.|[2504.13700](http://arxiv.org/abs/2504.13700)|null|
|**2025-04-18**|**Intelligent Interaction Strategies for Context-Aware Cognitive Augmentation**|Xiangrong et.al.|[2504.13684](http://arxiv.org/abs/2504.13684)|null|
|**2025-04-18**|**Do Prompt Patterns Affect Code Quality? A First Empirical Assessment of ChatGPT-Generated Code**|Antonio Della Porta et.al.|[2504.13656](http://arxiv.org/abs/2504.13656)|null|
|**2025-04-18**|**Exploring the Potential for Large Language Models to Demonstrate Rational Probabilistic Beliefs**|Gabriel Freedman et.al.|[2504.13644](http://arxiv.org/abs/2504.13644)|**[link](https://github.com/GIFRN/Rational-Probabilistic-Beliefs)**|
|**2025-04-18**|**Divergent LLM Adoption and Heterogeneous Convergence Paths in Research Writing**|Cong William Lin et.al.|[2504.13629](http://arxiv.org/abs/2504.13629)|null|
|**2025-04-18**|**Compile Scene Graphs with Reinforcement Learning**|Zuyao Chen et.al.|[2504.13617](http://arxiv.org/abs/2504.13617)|**[link](https://github.com/gpt4vision/r1-sgg)**|
|**2025-04-17**|**Sleep-time Compute: Beyond Inference Scaling at Test-time**|Kevin Lin et.al.|[2504.13171](http://arxiv.org/abs/2504.13171)|**[link](https://github.com/letta-ai/sleep-time-compute)**|
|**2025-04-17**|**Exploring Expert Failures Improves LLM Agent Tuning**|Li-Cheng Lan et.al.|[2504.13145](http://arxiv.org/abs/2504.13145)|null|
|**2025-04-17**|**Energy-Based Reward Models for Robust Language Model Alignment**|Anamika Lochab et.al.|[2504.13134](http://arxiv.org/abs/2504.13134)|**[link](https://github.com/AnamikaLochab/EBRM)**|
|**2025-04-17**|**LLMs Meet Finance: Fine-Tuning Foundation Models for the Open FinLLM Leaderboard**|Varun Rao et.al.|[2504.13125](http://arxiv.org/abs/2504.13125)|null|
|**2025-04-17**|**VistaDPO: Video Hierarchical Spatial-Temporal Direct Preference Optimization for Large Video Models**|Haojian Huang et.al.|[2504.13122](http://arxiv.org/abs/2504.13122)|**[link](https://github.com/haroldchen19/vistadpo)**|
|**2025-04-17**|**EventVAD: Training-Free Event-Aware Video Anomaly Detection**|Yihua Shao et.al.|[2504.13092](http://arxiv.org/abs/2504.13092)|null|
|**2025-04-17**|**Retrieval-Augmented Generation with Conflicting Evidence**|Han Wang et.al.|[2504.13079](http://arxiv.org/abs/2504.13079)|**[link](https://github.com/hannight/ramdocs)**|
|**2025-04-17**|**Accuracy is Not Agreement: Expert-Aligned Evaluation of Crash Narrative Classification Models**|Sudesh Ramesh Bhagat et.al.|[2504.13068](http://arxiv.org/abs/2504.13068)|null|
|**2025-04-17**|**GraphAttack: Exploiting Representational Blindspots in LLM Safety Mechanisms**|Sinan He et.al.|[2504.13052](http://arxiv.org/abs/2504.13052)|null|
|**2025-04-17**|**How Large Language Models Are Changing MOOC Essay Answers: A Comparison of Pre- and Post-LLM Responses**|Leo Leppänen et.al.|[2504.13038](http://arxiv.org/abs/2504.13038)|null|
|**2025-04-16**|**BitNet b1.58 2B4T Technical Report**|Shuming Ma et.al.|[2504.12285](http://arxiv.org/abs/2504.12285)|null|
|**2025-04-16**|**HLS-Eval: A Benchmark and Framework for Evaluating LLMs on High-Level Synthesis Design Tasks**|Stefan Abi-Karam et.al.|[2504.12268](http://arxiv.org/abs/2504.12268)|**[link](https://github.com/stefanpie/hls-eval)**|
|**2025-04-16**|**FLIP Reasoning Challenge**|Andreas Plesner et.al.|[2504.12256](http://arxiv.org/abs/2504.12256)|**[link](https://github.com/aplesner/flip-reasoning-challenge)**|
|**2025-04-16**|**AnomalyGen: An Automated Semantic Log Sequence Generation Framework with LLM for Anomaly Detection**|Xinyu Li et.al.|[2504.12250](http://arxiv.org/abs/2504.12250)|null|
|**2025-04-16**|**Watermarking Needs Input Repetition Masking**|David Khachaturov et.al.|[2504.12229](http://arxiv.org/abs/2504.12229)|null|
|**2025-04-16**|**d1: Scaling Reasoning in Diffusion Large Language Models via Reinforcement Learning**|Siyan Zhao et.al.|[2504.12216](http://arxiv.org/abs/2504.12216)|null|
|**2025-04-16**|**What Do Large Language Models Know? Tacit Knowledge as a Potential Causal-Explanatory Structure**|Céline Budding et.al.|[2504.12187](http://arxiv.org/abs/2504.12187)|null|
|**2025-04-16**|**SALAD: Improving Robustness and Generalization through Contrastive Learning with Structure-Aware and LLM-Driven Augmented Data**|Suyoung Bae et.al.|[2504.12185](http://arxiv.org/abs/2504.12185)|null|
|**2025-04-16**|**Multilingual Contextualization of Large Language Models for Document-Level Machine Translation**|Miguel Moura Ramos et.al.|[2504.12140](http://arxiv.org/abs/2504.12140)|null|
|**2025-04-16**|**Clarifying Ambiguities: on the Role of Ambiguity Types in Prompting Methods for Clarification Generation**|Anfu Tang et.al.|[2504.12113](http://arxiv.org/abs/2504.12113)|null|
|**2025-04-15**|**TextArena**|Leon Guertler et.al.|[2504.11442](http://arxiv.org/abs/2504.11442)|**[link](https://github.com/leonguertler/textarena)**|
|**2025-04-15**|**A Dual-Space Framework for General Knowledge Distillation of Large Language Models**|Xue Zhang et.al.|[2504.11426](http://arxiv.org/abs/2504.11426)|null|
|**2025-04-15**|**Reinforcing Compositional Retrieval: Retrieving Step-by-Step for Composing Informative Contexts**|Quanyu Long et.al.|[2504.11420](http://arxiv.org/abs/2504.11420)|null|
|**2025-04-15**|**RankAlign: A Ranking View of the Generator-Validator Gap in Large Language Models**|Juan Diego Rodriguez et.al.|[2504.11381](http://arxiv.org/abs/2504.11381)|**[link](https://github.com/juand-r/rankalign)**|
|**2025-04-15**|**Cancer-Myth: Evaluating AI Chatbot on Patient Questions with False Presuppositions**|Wang Bill Zhu et.al.|[2504.11373](http://arxiv.org/abs/2504.11373)|**[link](https://github.com/bill1235813/cancer-myth)**|
|**2025-04-15**|**A Minimalist Approach to LLM Reasoning: from Rejection Sampling to Reinforce**|Wei Xiong et.al.|[2504.11343](http://arxiv.org/abs/2504.11343)|**[link](https://github.com/rlhflow/minimal-rl)**|
|**2025-04-15**|**Optimizing LLM Inference: Fluid-Guided Online Scheduling with Memory Constraints**|Ruicheng Ao et.al.|[2504.11320](http://arxiv.org/abs/2504.11320)|**[link](https://github.com/microsoft/vidur)**|
|**2025-04-15**|**Learning to Be A Doctor: Searching for Effective Medical Agent Architectures**|Yangyang Zhuang et.al.|[2504.11301](http://arxiv.org/abs/2504.11301)|null|
|**2025-04-15**|**The Obvious Invisible Threat: LLM-Powered GUI Agents' Vulnerability to Fine-Print Injections**|Chaoran Chen et.al.|[2504.11281](http://arxiv.org/abs/2504.11281)|null|
|**2025-04-15**|**From Misleading Queries to Accurate Answers: A Three-Stage Fine-Tuning Method for LLMs**|Guocong Li et.al.|[2504.11277](http://arxiv.org/abs/2504.11277)|null|
|**2025-04-14**|**InternVL3: Exploring Advanced Training and Test-Time Recipes for Open-Source Multimodal Models**|Jinguo Zhu et.al.|[2504.10479](http://arxiv.org/abs/2504.10479)|**[link](https://github.com/opengvlab/internvl)**|
|**2025-04-14**|**M1: Towards Scalable Test-Time Compute with Mamba Reasoning Models**|Junxiong Wang et.al.|[2504.10449](http://arxiv.org/abs/2504.10449)|**[link](https://github.com/jxiw/m1)**|
|**2025-04-14**|**Multimodal Long Video Modeling Based on Temporal Dynamic Context**|Haoran Hao et.al.|[2504.10443](http://arxiv.org/abs/2504.10443)|**[link](https://github.com/hoar012/tdc-video)**|
|**2025-04-14**|**LLM Can be a Dangerous Persuader: Empirical Study of Persuasion Safety in Large Language Models**|Minqian Liu et.al.|[2504.10430](http://arxiv.org/abs/2504.10430)|null|
|**2025-04-14**|**Can We Edit LLMs for Long-Tail Biomedical Knowledge?**|Xinhao Yi et.al.|[2504.10421](http://arxiv.org/abs/2504.10421)|**[link](https://github.com/xinhaoyi/edit_bio_long_tail)**|
|**2025-04-14**|**CliniChat: A Multi-Source Knowledge-Driven Framework for Clinical Interview Dialogue Reconstruction and Evaluation**|Jing Chen et.al.|[2504.10418](http://arxiv.org/abs/2504.10418)|null|
|**2025-04-14**|**LLM-SRBench: A New Benchmark for Scientific Equation Discovery with Large Language Models**|Parshin Shojaee et.al.|[2504.10415](http://arxiv.org/abs/2504.10415)|**[link](https://github.com/deep-symbolic-mathematics/llm-srbench)**|
|**2025-04-14**|**Performance of Large Language Models in Supporting Medical Diagnosis and Treatment**|Diogo Sousa et.al.|[2504.10405](http://arxiv.org/abs/2504.10405)|null|
|**2025-04-14**|**Can LLMs Assist Expert Elicitation for Probabilistic Causal Modeling?**|Olha Shaposhnyk et.al.|[2504.10397](http://arxiv.org/abs/2504.10397)|null|
|**2025-04-14**|**SymRTLO: Enhancing RTL Code Optimization with LLMs and Neuron-Inspired Symbolic Reasoning**|Yiting Wang et.al.|[2504.10369](http://arxiv.org/abs/2504.10369)|null|
|**2025-04-11**|**DocAgent: A Multi-Agent System for Automated Code Documentation Generation**|Dayu Yang et.al.|[2504.08725](http://arxiv.org/abs/2504.08725)|**[link](https://github.com/facebookresearch/docagent)**|
|**2025-04-11**|**Large Language Models as Span Annotators**|Zdeněk Kasner et.al.|[2504.08697](http://arxiv.org/abs/2504.08697)|null|
|**2025-04-11**|**TP-RAG: Benchmarking Retrieval-Augmented Large Language Model Agents for Spatiotemporal-Aware Travel Planning**|Hang Ni et.al.|[2504.08694](http://arxiv.org/abs/2504.08694)|null|
|**2025-04-11**|**Fast-Slow-Thinking: Complex Task Solving with Large Language Models**|Yiliu Sun et.al.|[2504.08690](http://arxiv.org/abs/2504.08690)|null|
|**2025-04-11**|**Voice Interaction With Conversational AI Could Facilitate Thoughtful Reflection and Substantive Revision in Writing**|Jiho Kim et.al.|[2504.08687](http://arxiv.org/abs/2504.08687)|null|
|**2025-04-11**|**Variability-Driven User-Story Generation using LLM and Triadic Concept Analysis**|Alexandre Bazin et.al.|[2504.08666](http://arxiv.org/abs/2504.08666)|null|
|**2025-04-11**|**Do LLMs trust AI regulation? Emerging behaviour of game-theoretic LLM agents**|Alessio Buscemi et.al.|[2504.08640](http://arxiv.org/abs/2504.08640)|null|
|**2025-04-11**|**Analyzing 16,193 LLM Papers for Fun and Profits**|Zhiqiu Xia et.al.|[2504.08619](http://arxiv.org/abs/2504.08619)|null|
|**2025-04-11**|**Task Memory Engine (TME): Enhancing State Awareness for Multi-Step LLM Agent Tasks**|Ye Ye et.al.|[2504.08525](http://arxiv.org/abs/2504.08525)|**[link](https://github.com/biubiutomato/tme-agent)**|
|**2025-04-11**|**Adopting Large Language Models to Automated System Integration**|Robin D. Pesl et.al.|[2504.08490](http://arxiv.org/abs/2504.08490)|null|
|**2025-04-10**|**C3PO: Critical-Layer, Core-Expert, Collaborative Pathway Optimization for Test-Time Expert Re-Mixing**|Zhongyang Li et.al.|[2504.07964](http://arxiv.org/abs/2504.07964)|**[link](https://github.com/tianyi-lab/c3po)**|
|**2025-04-10**|**VCR-Bench: A Comprehensive Evaluation Framework for Video Chain-of-Thought Reasoning**|Yukun Qi et.al.|[2504.07956](http://arxiv.org/abs/2504.07956)|null|
|**2025-04-10**|**Porting an LLM based Application from ChatGPT to an On-Premise Environment**|Teemu Paloniemi et.al.|[2504.07907](http://arxiv.org/abs/2504.07907)|null|
|**2025-04-10**|**Redefining Machine Translation on Social Network Services with Large Language Models**|Hongcheng Guo et.al.|[2504.07901](http://arxiv.org/abs/2504.07901)|**[link](https://github.com/HC-Guo/RedTrans)**|
|**2025-04-10**|**How do Large Language Models Understand Relevance? A Mechanistic Interpretability Perspective**|Qi Liu et.al.|[2504.07898](http://arxiv.org/abs/2504.07898)|**[link](https://github.com/liuqi6777/llm-relevance)**|
|**2025-04-10**|**Benchmarking Adversarial Robustness to Bias Elicitation in Large Language Models: Scalable Automated Assessment with LLM-as-a-Judge**|Riccardo Cantini et.al.|[2504.07887](http://arxiv.org/abs/2504.07887)|**[link](https://github.com/SCAlabUnical/CLEAR-Bias_LLM_benchmark)**|
|**2025-04-10**|**Token Level Routing Inference System for Edge Devices**|Jianshu She et.al.|[2504.07878](http://arxiv.org/abs/2504.07878)|null|
|**2025-04-11**|**Pangu Ultra: Pushing the Limits of Dense Large Language Models on Ascend NPUs**|Yichun Yin et.al.|[2504.07866](http://arxiv.org/abs/2504.07866)|null|
|**2025-04-10**|**Robust Hallucination Detection in LLMs via Adaptive Token Selection**|Mengjia Niu et.al.|[2504.07863](http://arxiv.org/abs/2504.07863)|null|
|**2025-04-10**|**Understanding Learner-LLM Chatbot Interactions and the Impact of Prompting Guidelines**|Cansu Koyuturk et.al.|[2504.07840](http://arxiv.org/abs/2504.07840)|null|
|**2025-04-09**|**Sculpting Subspaces: Constrained Full Fine-Tuning in LLMs for Continual Learning**|Nikhil Shivakumar Nayak et.al.|[2504.07097](http://arxiv.org/abs/2504.07097)|**[link](https://github.com/Red-Hat-AI-Innovation-Team/orthogonal-subspace-learning)**|
|**2025-04-09**|**KG-LLM-Bench: A Scalable Benchmark for Evaluating LLM Reasoning on Textualized Knowledge Graphs**|Elan Markowitz et.al.|[2504.07087](http://arxiv.org/abs/2504.07087)|null|
|**2025-04-09**|**A Survey on Personalized and Pluralistic Preference Alignment in Large Language Models**|Zhouhang Xie et.al.|[2504.07070](http://arxiv.org/abs/2504.07070)|null|
|**2025-04-09**|**HalluciNot: Hallucination Detection Through Context and Common Knowledge Verification**|Bibek Paudel et.al.|[2504.07069](http://arxiv.org/abs/2504.07069)|null|
|**2025-04-09**|**TASTE: Text-Aligned Speech Tokenization and Embedding for Spoken Language Modeling**|Liang-Hsuan Tseng et.al.|[2504.07053](http://arxiv.org/abs/2504.07053)|**[link](https://github.com/mtkresearch/taste-spokenlm)**|
|**2025-04-09**|**Evaluating Retrieval Augmented Generative Models for Document Queries in Transportation Safety**|Chad Melton et.al.|[2504.07022](http://arxiv.org/abs/2504.07022)|null|
|**2025-04-09**|**LLM-IFT: LLM-Powered Information Flow Tracking for Secure Hardware**|Nowfel Mashnoor et.al.|[2504.07015](http://arxiv.org/abs/2504.07015)|null|
|**2025-04-09**|**Towards LLMs Robustness to Changes in Prompt Format Styles**|Lilian Ngweta et.al.|[2504.06969](http://arxiv.org/abs/2504.06969)|null|
|**2025-04-09**|**Review of Case-Based Reasoning for LLM Agents: Theoretical Foundations, Architectural Components, and Cognitive Integration**|Kostas Hatalis et.al.|[2504.06943](http://arxiv.org/abs/2504.06943)|null|
|**2025-04-09**|**FeedbackEval: A Benchmark for Evaluating Large Language Models in Feedback-Driven Code Repair Tasks**|Dekun Dai et.al.|[2504.06939](http://arxiv.org/abs/2504.06939)|**[link](https://github.com/sysuselab/feedbackeval)**|
|**2025-04-08**|**GOLLuM: Gaussian Process Optimized LLMs -- Reframing LLM Finetuning through Bayesian Optimization**|Bojana Ranković et.al.|[2504.06265](http://arxiv.org/abs/2504.06265)|**[link](https://github.com/schwallergroup/gollum)**|
|**2025-04-08**|**Hogwild! Inference: Parallel LLM Generation via Concurrent Attention**|Gleb Rodionov et.al.|[2504.06261](http://arxiv.org/abs/2504.06261)|null|
|**2025-04-08**|**FEABench: Evaluating Language Models on Multiphysics Reasoning Ability**|Nayantara Mudur et.al.|[2504.06260](http://arxiv.org/abs/2504.06260)|**[link](https://github.com/google/feabench)**|
|**2025-04-08**|**LExT: Towards Evaluating Trustworthiness of Natural Language Explanations**|Krithi Shailya et.al.|[2504.06227](http://arxiv.org/abs/2504.06227)|null|
|**2025-04-08**|**Encoder-Decoder Gemma: Improving the Quality-Efficiency Trade-Off via Adaptation**|Biao Zhang et.al.|[2504.06225](http://arxiv.org/abs/2504.06225)|null|
|**2025-04-08**|**Can Performant LLMs Be Ethical? Quantifying the Impact of Web Crawling Opt-Outs**|Dongyang Fan et.al.|[2504.06219](http://arxiv.org/abs/2504.06219)|null|
|**2025-04-08**|**TxGemma: Efficient and Agentic LLMs for Therapeutics**|Eric Wang et.al.|[2504.06196](http://arxiv.org/abs/2504.06196)|null|
|**2025-04-09**|**Navigating the Rabbit Hole: Emergent Biases in LLM-Generated Attack Narratives Targeting Mental Health Groups**|Rijul Magu et.al.|[2504.06160](http://arxiv.org/abs/2504.06160)|null|
|**2025-04-08**|**ARLO: A Tailorable Approach for Transforming Natural Language Software Requirements into Architecture using LLMs**|Tooraj Helmi et.al.|[2504.06143](http://arxiv.org/abs/2504.06143)|null|
|**2025-04-08**|**QGen Studio: An Adaptive Question-Answer Generation, Training and Evaluation Platform**|Movina Moses et.al.|[2504.06136](http://arxiv.org/abs/2504.06136)|null|
|**2025-04-07**|**Truthful or Fabricated? Using Causal Attribution to Mitigate Reward Hacking in Explanations**|Pedro Ferreira et.al.|[2504.05294](http://arxiv.org/abs/2504.05294)|null|
|**2025-04-07**|**The challenge of uncertainty quantification of large language models in medicine**|Zahra Atf et.al.|[2504.05278](http://arxiv.org/abs/2504.05278)|null|
|**2025-04-07**|**Enhancing LLM-Based Short Answer Grading with Retrieval-Augmented Generation**|Yucheng Chu et.al.|[2504.05276](http://arxiv.org/abs/2504.05276)|null|
|**2025-04-07**|**Do PhD-level LLMs Truly Grasp Elementary Addition? Probing Rule Learning vs. Memorization in Large Language Models**|Yang Yan et.al.|[2504.05262](http://arxiv.org/abs/2504.05262)|null|
|**2025-04-07**|**Learning to Reason Over Time: Timeline Self-Reflection for Improved Temporal Reasoning in Language Models**|Adrián Bazaga et.al.|[2504.05258](http://arxiv.org/abs/2504.05258)|null|
|**2025-04-07**|**LLM-based Automated Grading with Human-in-the-Loop**|Hang Li et.al.|[2504.05239](http://arxiv.org/abs/2504.05239)|null|
|**2025-04-08**|**Leveraging LLMs for Utility-Focused Annotation: Reducing Manual Effort for Retrieval and RAG**|Hengran Zhang et.al.|[2504.05220](http://arxiv.org/abs/2504.05220)|null|
|**2025-04-07**|**Unleashing the Power of LLMs in Dense Retrieval with Query Likelihood Modeling**|Hengran Zhang et.al.|[2504.05216](http://arxiv.org/abs/2504.05216)|null|
|**2025-04-07**|**Post-Training Language Models for Continual Relation Extraction**|Sefika Efeoglu et.al.|[2504.05214](http://arxiv.org/abs/2504.05214)|null|
|**2025-04-07**|**Quantum Program Linting with LLMs: Emerging Results from a Comparative Study**|Seung Yeob Shin et.al.|[2504.05204](http://arxiv.org/abs/2504.05204)|null|
|**2025-04-04**|**Do Larger Language Models Imply Better Reasoning? A Pretraining Scaling Law for Reasoning**|Xinyi Wang et.al.|[2504.03635](http://arxiv.org/abs/2504.03635)|null|
|**2025-04-04**|**Align to Structure: Aligning Large Language Models with Structural Information**|Zae Myung Kim et.al.|[2504.03622](http://arxiv.org/abs/2504.03622)|null|
|**2025-04-04**|**Multilingual Retrieval-Augmented Generation for Knowledge-Intensive Task**|Leonardo Ranaldi et.al.|[2504.03616](http://arxiv.org/abs/2504.03616)|null|
|**2025-04-04**|**AIR: A Systematic Analysis of Annotations, Instructions, and Response Pairs in Preference Dataset**|Bingxiang He et.al.|[2504.03612](http://arxiv.org/abs/2504.03612)|null|
|**2025-04-04**|**EnrichIndex: Using LLMs to Enrich Retrieval Indices Offline**|Peter Baile Chen et.al.|[2504.03598](http://arxiv.org/abs/2504.03598)|null|
|**2025-04-04**|**Agentic Knowledgeable Self-awareness**|Shuofei Qiao et.al.|[2504.03553](http://arxiv.org/abs/2504.03553)|**[link](https://github.com/zjunlp/knowself)**|
|**2025-04-04**|**Neutralizing the Narrative: AI-Powered Debiasing of Online News Articles**|Chen Wei Kuo et.al.|[2504.03520](http://arxiv.org/abs/2504.03520)|null|
|**2025-04-04**|**LLMSched: Uncertainty-Aware Workload Scheduling for Compound LLM Applications**|Botao Zhu et.al.|[2504.03444](http://arxiv.org/abs/2504.03444)|null|
|**2025-04-04**|**Know What You do Not Know: Verbalized Uncertainty Estimation Robustness on Corrupted Images in Vision-Language Models**|Mirko Borszukovszki et.al.|[2504.03440](http://arxiv.org/abs/2504.03440)|null|
|**2025-04-04**|**Locations of Characters in Narratives: Andersen and Persuasion Datasets**|Batuhan Ozyurt et.al.|[2504.03434](http://arxiv.org/abs/2504.03434)|**[link](https://github.com/batuhan-ozyurt/location-of-characters-in-narratives-andersen-and-persuasion-datasets)**|
|**2025-04-03**|**Sparse Autoencoders Learn Monosemantic Features in Vision-Language Models**|Mateusz Pach et.al.|[2504.02821](http://arxiv.org/abs/2504.02821)|**[link](https://github.com/explainableml/sae-for-vlm)**|
|**2025-04-03**|**Generative Evaluation of Complex Reasoning in Large Language Models**|Haowei Lin et.al.|[2504.02810](http://arxiv.org/abs/2504.02810)|**[link](https://github.com/linhaowei1/kumo)**|
|**2025-04-03**|**MegaMath: Pushing the Limits of Open Math Corpora**|Fan Zhou et.al.|[2504.02807](http://arxiv.org/abs/2504.02807)|**[link](https://github.com/llm360/megamath)**|
|**2025-04-04**|**A Survey of Large Language Models in Mental Health Disorder Detection on Social Media**|Zhuohan Ge et.al.|[2504.02800](http://arxiv.org/abs/2504.02800)|null|
|**2025-04-03**|**A Framework for Robust Cognitive Evaluation of LLMs**|Karin de Langis et.al.|[2504.02789](http://arxiv.org/abs/2504.02789)|null|
|**2025-04-03**|**From Consumption to Collaboration: Measuring Interaction Patterns to Augment Human Cognition in Open-Ended Tasks**|Joshua Holstein et.al.|[2504.02780](http://arxiv.org/abs/2504.02780)|null|
|**2025-04-03**|**BT-ACTION: A Test-Driven Approach for Modular Understanding of User Instruction Leveraging Behaviour Trees and LLMs**|Alexander Leszczynski et.al.|[2504.02779](http://arxiv.org/abs/2504.02779)|**[link](https://github.com/1eggbert7/bt_llm)**|
|**2025-04-03**|**How Deep Do Large Language Models Internalize Scientific Literature and Citation Practices?**|Andres Algaba et.al.|[2504.02767](http://arxiv.org/abs/2504.02767)|**[link](https://github.com/andresalgaba/llms_scientific_literature)**|
|**2025-04-03**|**Enhancing LLM Robustness to Perturbed Instructions: An Empirical Study**|Aryan Agrawal et.al.|[2504.02733](http://arxiv.org/abs/2504.02733)|**[link](https://github.com/ary4n99/llm-robustness)**|
|**2025-04-04**|**Why do LLMs attend to the first token?**|Federico Barbero et.al.|[2504.02732](http://arxiv.org/abs/2504.02732)|null|
|**2025-04-02**|**Critical Thinking: Which Kinds of Complexity Govern Optimal Reasoning Length?**|Celine Lee et.al.|[2504.01935](http://arxiv.org/abs/2504.01935)|**[link](https://github.com/celine-lee/critical_thinking)**|
|**2025-04-02**|**Gen-C: Populating Virtual Worlds with Generative Crowds**|Andreas Panayiotou et.al.|[2504.01924](http://arxiv.org/abs/2504.01924)|null|
|**2025-04-03**|**Bridging the Linguistic Divide: A Survey on Leveraging Large Language Models for Machine Translation**|Baban Gain et.al.|[2504.01919](http://arxiv.org/abs/2504.01919)|null|
|**2025-04-02**|**Advancing AI-Scientist Understanding: Making LLM Think Like a Physicist with Interpretable Reasoning**|Yinggan Xu et.al.|[2504.01911](http://arxiv.org/abs/2504.01911)|null|
|**2025-04-02**|**TransientTables: Evaluating LLMs' Reasoning on Temporally Evolving Semi-structured Tables**|Abhilash Shankarampeta et.al.|[2504.01879](http://arxiv.org/abs/2504.01879)|null|
|**2025-04-02**|**From Code Generation to Software Testing: AI Copilot with Context-Based RAG**|Yuchen Wang et.al.|[2504.01866](http://arxiv.org/abs/2504.01866)|null|
|**2025-04-02**|**Cross-Lingual Consistency: A Novel Inference Framework for Advancing Reasoning in Large Language Models**|Zhiwei Yu et.al.|[2504.01857](http://arxiv.org/abs/2504.01857)|null|
|**2025-04-02**|**Code Red! On the Harmfulness of Applying Off-the-shelf Large Language Models to Programming Tasks**|Ali Al-Kaswan et.al.|[2504.01850](http://arxiv.org/abs/2504.01850)|null|
|**2025-04-02**|**LARGE: Legal Retrieval Augmented Generation Evaluation Tool**|Minhu Park et.al.|[2504.01840](http://arxiv.org/abs/2504.01840)|**[link](https://github.com/hoorangyee/lrage)**|
|**2025-04-02**|**YourBench: Easy Custom Evaluation Sets for Everyone**|Sumuk Shashidhar et.al.|[2504.01833](http://arxiv.org/abs/2504.01833)|**[link](https://github.com/huggingface/yourbench)**|
|**2025-03-31**|**Harnessing the Reasoning Economy: A Survey of Efficient Reasoning for Large Language Models**|Rui Wang et.al.|[2503.24377](http://arxiv.org/abs/2503.24377)|**[link](https://github.com/devoallen/awesome-reasoning-economy-papers)**|
|**2025-03-31**|**Exploring the Effect of Reinforcement Learning on Video Understanding: Insights from SEED-Bench-R1**|Yi Chen et.al.|[2503.24376](http://arxiv.org/abs/2503.24376)|**[link](https://github.com/tencentarc/seed-bench-r1)**|
|**2025-03-31**|**Effectively Controlling Reasoning Models through Thinking Intervention**|Tong Wu et.al.|[2503.24370](http://arxiv.org/abs/2503.24370)|null|
|**2025-03-31**|**ORAL: Prompting Your Large-Scale LoRAs via Conditional Recurrent Diffusion**|Rana Muhammad Shahroz Khan et.al.|[2503.24354](http://arxiv.org/abs/2503.24354)|null|
|**2025-03-31**|**BEATS: Bias Evaluation and Assessment Test Suite for Large Language Models**|Alok Abhishek et.al.|[2503.24310](http://arxiv.org/abs/2503.24310)|null|
|**2025-03-31**|**A Systematic Evaluation of LLM Strategies for Mental Health Text Analysis: Fine-tuning vs. Prompt Engineering vs. RAG**|Arshia Kermani et.al.|[2503.24307](http://arxiv.org/abs/2503.24307)|null|
|**2025-03-31**|**Rec-R1: Bridging Generative Large Language Models and User-Centric Recommendation Systems via Reinforcement Learning**|Jiacheng Lin et.al.|[2503.24289](http://arxiv.org/abs/2503.24289)|**[link](https://github.com/linjc16/Rec-R1)**|
|**2025-03-31**|**Evaluating and Designing Sparse Autoencoders by Approximating Quasi-Orthogonality**|Sewoong Lee et.al.|[2503.24277](http://arxiv.org/abs/2503.24277)|**[link](https://github.com/sewoonglee/top-afa-sae)**|
|**2025-03-31**|**Enhancing Large Language Models (LLMs) for Telecommunications using Knowledge Graphs and Retrieval-Augmented Generation**|Dun Yuan et.al.|[2503.24245](http://arxiv.org/abs/2503.24245)|null|
|**2025-03-31**|**What, How, Where, and How Well? A Survey on Test-Time Scaling in Large Language Models**|Qiyuan Zhang et.al.|[2503.24235](http://arxiv.org/abs/2503.24235)|**[link](https://github.com/testtimescaling/testtimescaling.github.io)**|
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
|**2025-03-18**|**Aligning Multimodal LLM with Human Preference: A Survey**|Tao Yu et.al.|[2503.14504](http://arxiv.org/abs/2503.14504)|**[link](https://github.com/bradyfu/awesome-multimodal-large-language-models)**|
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
|**2025-03-11**|**Randomness, Not Representation: The Unreliability of Evaluating Cultural Alignment in LLMs**|Ariba Khan et.al.|[2503.08688](http://arxiv.org/abs/2503.08688)|**[link](https://github.com/ariba-k/llm-cultural-alignment-evaluation)**|
|**2025-03-11**|**Self-Taught Self-Correction for Small Language Models**|Viktor Moskvoretskii et.al.|[2503.08681](http://arxiv.org/abs/2503.08681)|null|
|**2025-03-11**|**Exploring the Word Sense Disambiguation Capabilities of Large Language Models**|Pierpaolo Basile et.al.|[2503.08662](http://arxiv.org/abs/2503.08662)|null|
|**2025-03-11**|**EMMOE: A Comprehensive Benchmark for Embodied Mobile Manipulation in Open Environments**|Dongping Li et.al.|[2503.08604](http://arxiv.org/abs/2503.08604)|**[link](https://github.com/silence143/EMMOE)**|
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
|**2025-02-28**|**FANformer: Improving Large Language Models Through Effective Periodicity Modeling**|Yihong Dong et.al.|[2502.21309](http://arxiv.org/abs/2502.21309)|**[link](https://github.com/yihongdong/fanformer)**|
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
|**2025-02-27**|**Bridging Legal Knowledge and AI: Retrieval-Augmented Generation with Vector Stores, Knowledge Graphs, and Hierarchical Non-negative Matrix Factorization**|Ryan C. Barron et.al.|[2502.20364](http://arxiv.org/abs/2502.20364)|**[link](https://github.com/lanl/t-elf)**|
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
|**2025-02-21**|**Machine-generated text detection prevents language model collapse**|George Drayson et.al.|[2502.15654](http://arxiv.org/abs/2502.15654)|**[link](https://github.com/georgedrayson/model_collapse)**|
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
|**2025-02-14**|**Large Language Models and Synthetic Data for Monitoring Dataset Mentions in Research Papers**|Aivin V. Solatorio et.al.|[2502.10263](http://arxiv.org/abs/2502.10263)|**[link](https://github.com/worldbank/ai4data-use)**|
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
|**2025-01-14**|**Addressing the sustainable AI trilemma: a case study on LLM agents and RAG**|Hui Wu et.al.|[2501.08262](http://arxiv.org/abs/2501.08262)|**[link](https://github.com/huiwxing/llmagent_trilemma)**|
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
|**2024-12-18**|**Digestion Algorithm in Hierarchical Symbolic Forests: A Fast Text Normalization Algorithm and Semantic Parsing Framework for Specific Scenarios and Lightweight Deployment**|Kevin You et.al.|[2412.14054](http://arxiv.org/abs/2412.14054)|**[link](https://github.com/Magic-Abracadabra/AI-Chinese-Scripting-Language)**|
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
|**2024-12-16**|**Cost-Effective Label-free Node Classification with LLMs**|Taiyan Zhang et.al.|[2412.11983](http://arxiv.org/abs/2412.11983)|**[link](https://github.com/hkbu-lagas/locle)**|
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
|**2024-12-12**|**AI Predicts AGI: Leveraging AGI Forecasting and Peer Review to Explore LLMs' Complex Reasoning Capabilities**|Fabrizio Davide et.al.|[2412.09385](http://arxiv.org/abs/2412.09385)|**[link](https://github.com/LeonardoErcolani/AGILab-Peer-Review)**|
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
|**2024-12-03**|**PrefixLLM: LLM-aided Prefix Circuit Design**|Weihua Xiao et.al.|[2412.02594](http://arxiv.org/abs/2412.02594)|**[link](https://github.com/FCHXWH823/PrefixGPT)**|
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
|**2024-11-26**|**Toward High-Performance LLM Serving: A Simulation-Based Approach for Identifying Optimal Parallelism**|Yi-Chien Lin et.al.|[2411.17651](http://arxiv.org/abs/2411.17651)|**[link](https://github.com/microsoft/apex_plus)**|
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
|**2024-11-14**|**Spider: Any-to-Many Multimodal LLM**|Jinxiang Lai et.al.|[2411.09439](http://arxiv.org/abs/2411.09439)|**[link](https://github.com/Layjins/Spider)**|
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
|**2024-11-08**|**Recycled Attention: Efficient inference for long-context language models**|Fangyuan Xu et.al.|[2411.05787](http://arxiv.org/abs/2411.05787)|**[link](https://github.com/carriex/recycled-attention)**|
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

<p align=right>(<a href=#updated-on-20250525>back to top</a>)</p>

## moe

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-05-22**|**DriveMoE: Mixture-of-Experts for Vision-Language-Action Model in End-to-End Autonomous Driving**|Zhenjie Yang et.al.|[2505.16278](http://arxiv.org/abs/2505.16278)|null|端到端自动驾驶（E2E-AD）需要有效处理多视角感知数据，并稳健地应对多样化和复杂的驾驶场景，特别是激进转弯等罕见操作。最近在大型语言模型（LLMs）中成功应用的混合专家（MoE）架构表明，参数的专业化能够实现强大的可扩展性。在这项工作中，我们提出了DriveMoE，一种基于MoE的新型E2E-AD框架，包含场景专业化视觉MoE和技能专业化动作MoE。DriveMoE基于我们的 $\pi_0$视觉-语言-动作（VLA）基线（最初来自具身AI领域），称为Drive-$\pi_0$。具体来说，我们通过训练一个路由器来根据驾驶上下文动态选择相关摄像头，从而将视觉MoE添加到Drive-$\pi_0$中。这种设计模仿了人类驾驶认知，即驾驶员选择性地关注关键视觉线索，而不是详尽处理所有视觉信息。此外，我们通过训练另一个路由器来激活针对不同驾驶行为的专业模块，从而添加动作MoE。通过明确的行为专业化，DriveMoE能够在不遭受现有模型常见的模式平均问题的情况下处理多样化的场景。在Bench2Drive闭环评估实验中，DriveMoE达到了最先进的性能，展示了结合视觉和动作MoE在自动驾驶任务中的有效性。我们将发布DriveMoE和Drive-$\pi_0$ 的代码和模型。|
|**2025-05-21**|**Not All Models Suit Expert Offloading: On Local Routing Consistency of Mixture-of-Expert Models**|Jingcong Liang et.al.|[2505.16056](http://arxiv.org/abs/2505.16056)|null|混合专家（MoE）通过在推理过程中稀疏激活专家，实现了大规模语言模型（LLMs）的有效扩展。为了在内存受限的设备上有效部署大型MoE模型，许多系统引入了*专家卸载*技术，该技术将一部分专家缓存在快速内存中，而其他专家则保留在慢速内存中，运行于CPU或按需加载。虽然一些研究已经利用了专家激活的局部性，即连续的token会激活相似的专家，但这种**局部路由一致性**的程度在不同模型之间有所不同，并且尚未得到充分研究。在这篇论文中，我们提出了两个度量指标来衡量MoE模型的局部路由一致性：(1) **段路由最佳性能（SRP）**，评估一组固定的专家能够多好地满足一段token的需求；(2) **段缓存最佳命中率（SCH）**，在给定缓存大小限制下测量最优的段级缓存命中率。我们分析了20个具有不同规模和架构的MoE LLMs，发现那些在每一层都应用MoE并且不使用共享专家的模型表现出最高的局部路由一致性。我们进一步表明，领域专业化专家比词汇专业化专家对路由一致性贡献更大，并且大多数模型可以在大约2倍活跃专家数量的缓存大小下平衡缓存效果与效率。这些发现为设计和部署内存高效的MoE铺平了道路，同时不会牺牲推理速度。我们发布了复现实验的代码，地址为https://github.com/ljcleo/moe-lrc。|
|**2025-05-21**|**CoLA: Collaborative Low-Rank Adaptation**|Yiyun Zhou et.al.|[2505.15471](http://arxiv.org/abs/2505.15471)|**[link](https://github.com/zyy-2001/cola)**|**大型语言模型（LLMs）的扩展法则揭示了一种幂律关系，表明随着模型规模的增加，性能提升逐渐减小。虽然从头开始训练LLMs非常耗费资源，但针对特定任务对预训练模型进行微调已成为一种实用的替代方案。全参数微调（FFT）可以实现强大的性能；然而，它计算成本高且效率低下。为了应对这些挑战，提出了参数高效微调（PEFT）方法，如LoRA，通过冻结预训练模型并添加轻量级的任务特定模块来解决这些问题。特别是LoRA已被证明有效，但在多任务场景中的应用受到任务间干扰的限制。最近的方法，如Mixture-of-Experts (MOE) 和非对称LoRA，旨在缓解这些问题，但由于其固定结构，仍然难以处理样本稀缺和噪声干扰问题。为此，我们提出了一种更灵活的LoRA架构CoLA，具有高效的初始化方案，并引入了三种协作策略，通过更好地利用矩阵A和B之间的定量关系来提高性能。我们的实验表明，CoLA在有效性及鲁棒性方面优于现有的PEFT方法，特别是在低样本场景中表现尤为出色。我们的数据和代码完全公开，可在https://github.com/zyy-2001/CoLA获取。**|
|**2025-05-22**|**Hunyuan-TurboS: Advancing Large Language Models through Mamba-Transformer Synergy and Adaptive Chain-of-Thought**|Tencent Hunyuan Team et.al.|[2505.15431](http://arxiv.org/abs/2505.15431)|null|随着大型语言模型（LLM）的迅速发展，我们推出了Hunyuan-TurboS，这是一种新颖的大规模混合Transformer-Mamba专家混合模型（MoE）。它将Mamba处理长序列的高效性与Transformer卓越的上下文理解能力相结合。Hunyuan-TurboS具有自适应的长短链式思维机制，能够根据查询的复杂度动态切换快速响应和深度“思考”模式，从而优化计算资源。该模型在激活状态下有560亿参数中的560亿被激活，采用128层结构（Mamba2、注意力机制、前馈网络），并使用创新的AMF/MF块模式。更快的Mamba2确保了线性复杂度，分组查询注意力机制减少了KV缓存，而前馈网络则采用了MoE结构。该模型在16万亿高质量令牌上进行了预训练，支持256K上下文长度，并且是首个工业部署的大规模Mamba模型。我们的全面后训练策略通过监督微调（3百万条指令）、一种新的自适应长短链式思维融合方法、多轮审议学习以实现迭代改进以及针对STEM和一般指令跟随任务的两阶段大规模强化学习过程来增强其能力。评估显示，Hunyuan-TurboS表现强劲：在LMSYS Chatbot Arena上的总排名为第7位，得分为1356，超过了Gemini-2.0-Flash-001（1352）和o4-mini-2025-04-16（1345）等领先模型。TurboS还在23个自动化基准测试中达到了平均77.9%的成绩。Hunyuan-TurboS在高性能与效率之间取得了平衡，在推理成本低于许多推理模型的情况下提供了显著的能力，为高效的大型预训练模型树立了新范例。|
|**2025-05-21**|**Efficient Data Driven Mixture-of-Expert Extraction from Trained Networks**|Uranik Berisha et.al.|[2505.15414](http://arxiv.org/abs/2505.15414)|null|视觉变换器在各种计算机视觉任务中已成为最先进的模型，但其高计算和资源需求带来了显著的挑战。虽然混合专家（MoE）可以使这些模型更高效，但它们通常需要昂贵的重新训练甚至从零开始训练。最近的发展旨在通过利用预训练网络来减少这些计算成本。这些方法已被证明能够在编码器块的多层感知机（MLPs）中产生稀疏激活模式，从而允许仅对每个样本的相关子网络进行条件激活。基于这一想法，我们提出了一种从预训练模型构建MoE变体的新方法。我们的方法在训练后从模型的MLP层中分两个阶段提取专家子网络。首先，我们聚类输出激活以识别不同的激活模式。在第二阶段，我们使用这些聚类来提取负责生成这些模式的相应子网络。在ImageNet-1k识别任务上，我们展示了这些提取出的专家可以直接表现出令人惊讶的良好性能，并且只需要少量微调即可恢复到原始性能的98%，同时减少了多达36%的MACs和32%的模型大小。|
|**2025-05-21**|**Time Tracker: Mixture-of-Experts-Enhanced Foundation Time Series Forecasting Model with Decoupled Training Pipelines**|Xiaohou Shi et.al.|[2505.15151](http://arxiv.org/abs/2505.15151)|null|在过去的几年中，时间序列基础模型已经取得了卓越的预测准确性。然而，现实世界的时间序列在其时间跨度和领域上表现出显著的多样性，这使得单一模型架构难以适应所有复杂场景。此外，时间序列数据可能包含多个变量，这些变量之间存在复杂的相互关系。近期主流的研究工作主要集中在以通道独立的方式对预训练和微调阶段的时间序列进行建模，忽略了有价值的序列间依赖性。为此，我们提出了**Time Tracker**，以更好地预测多变量时间序列数据。首先，我们在Transformer中利用稀疏混合专家（MoE）来处理多样时间序列模式的建模，从而缓解单一模型的学习困难并提高其泛化能力。此外，我们提出了Any-variate Attention，使统一的模型结构能够无缝处理单变量和多变量时间序列，支持预训练阶段的通道独立建模和微调阶段的通道混合建模。进一步地，我们设计了一个图学习模块，从频域特征中构建序列之间的关系，为捕捉通道混合建模中的序列间依赖性提供更精确的指导。基于这些改进，Time Tracker在预测准确性、模型泛化能力和适应性方面达到了最先进的性能。|
|**2025-05-20**|**Balanced and Elastic End-to-end Training of Dynamic LLMs**|Mohamed Wahib et.al.|[2505.14864](http://arxiv.org/abs/2505.14864)|null|为了降低大型语言模型（LLMs）的计算和内存成本，出现了诸如专家混合（MoEs）、参数剪枝、层冻结、稀疏注意力、早期令牌退出和深度混合（MoDs）等动态工作负载减少方案。然而，这些方法引入了严重的工作负载不平衡问题，限制了它们在大规模分布式训练中的实用性。我们提出了DynMo，这是一种自主的动态负载均衡解决方案，能够在使用流水线并行进行动态模型训练时确保最佳的计算分布。DynMo能够自适应地平衡工作负载，动态地将任务打包到更少的工作节点中以释放闲置资源，并支持多GPU单节点和多节点系统。与静态训练方法（如Megatron-LM、DeepSpeed）相比，DynMo在加速训练方面表现优异：对于MoEs可加速至1.23倍，对于剪枝可加速至3.18倍，对于层冻结可加速至2.23倍，对于稀疏注意力可加速至4.02倍，对于早期退出可加速至4.52倍，对于MoDs可加速至1.17倍。DynMo可以在https://anonymous.4open.science/r/DynMo-4D04/获取。|
|**2025-05-20**|**Two Experts Are All You Need for Steering Thinking: Reinforcing Cognitive Effort in MoE Reasoning Models Without Additional Training**|Mengru Wang et.al.|[2505.14681](http://arxiv.org/abs/2505.14681)|null|在大型推理模型（LRMs）中，基于专家混合（MoE）架构通过选择性激活专家来促进结构化的认知过程，已经实现了令人印象深刻的推理能力。尽管取得了显著进展，现有的推理模型通常会遭受认知效率低下的问题，如过度思考和思考不足。为了解决这些局限性，我们引入了一种新的推理时引导方法，称为强化认知专家（RICE），旨在不增加额外训练或复杂启发式的情况下提高推理性能。利用归一化点互信息（nPMI），我们系统地识别出专门的专家，称为“认知专家”，它们负责由诸如“<think>”之类的标记特征化的元级推理操作。通过领先的基于MoE的LRMs（DeepSeek-R1和Qwen3-235B）在严格的定量和科学推理基准上的实证评估表明，在推理准确性、认知效率和跨域泛化方面都有明显且一致的改进。重要的是，我们的轻量级方法在保持模型通用指令跟随技能的同时，显著优于流行的推理引导技术，如提示设计和解码约束。这些结果强调了强化认知专家作为一种有前景、实用且可解释的方向，以增强先进推理模型中的认知效率。|
|**2025-05-21**|**Scaling and Enhancing LLM-based AVSR: A Sparse Mixture of Projectors Approach**|Umberto Cappellazzo et.al.|[2505.14336](http://arxiv.org/abs/2505.14336)|null|音频视觉语音识别（AVSR）通过整合视觉线索增强了在嘈杂环境中的鲁棒性。尽管最近的进展将大型语言模型（LLMs）集成到AVSR中，但其高昂的计算成本阻碍了在资源受限环境中的部署。为了解决这个问题，我们提出了Llama-SMoP，这是一种高效的多模态LLM，它采用稀疏投影混合（SMoP）模块来扩展模型容量而不增加推理成本。通过结合稀疏门控混合专家（MoE）投影器，Llama-SMoP能够在使用较小的LLM的同时保持强大的性能。我们探索了三种SMoP配置，并表明使用模态特定路由器和专家的Llama-SMoP DEDR（独立专家，独立路由器）在ASR、VSR和AVSR任务上实现了优越性能。消融研究表明，它在专家激活、可扩展性和噪声鲁棒性方面具有有效性。|
|**2025-05-20**|**FuxiMT: Sparsifying Large Language Models for Chinese-Centric Multilingual Machine Translation**|Shaolin Zhu et.al.|[2505.14256](http://arxiv.org/abs/2505.14256)|null|在本文中，我们介绍了FuxiMT，这是一种基于稀疏化大语言模型（LLM）的新型以中文为中心的多语言机器翻译模型。我们采用两阶段策略来训练FuxiMT。首先在大规模中文语料库上进行预训练，然后在一个涵盖65种语言的大规模平行数据集上进行多语言微调。FuxiMT结合了专家混合（MoEs）机制，并采用了课程学习策略，以实现在不同资源水平下的稳健性能。实验结果表明，FuxiMT显著优于包括最先进的大语言模型和机器翻译模型在内的强大基线，特别是在低资源场景下。此外，FuxiMT在未见过的语言对上表现出卓越的零样本翻译能力，表明其在平行数据稀缺或不可用的情况下具有潜在的沟通桥梁作用。|
|**2025-05-20**|**THOR-MoE: Hierarchical Task-Guided and Context-Responsive Routing for Neural Machine Translation**|Yunlong Liang et.al.|[2505.14173](http://arxiv.org/abs/2505.14173)|null|
|**2025-05-20**|**Multimodal Mixture of Low-Rank Experts for Sentiment Analysis and Emotion Recognition**|Shuo Zhang et.al.|[2505.14143](http://arxiv.org/abs/2505.14143)|null|
|**2025-05-20**|**Local Mixtures of Experts: Essentially Free Test-Time Training via Model Merging**|Ryo Bertolissi et.al.|[2505.14136](http://arxiv.org/abs/2505.14136)|null|
|**2025-05-20**|**U-SAM: An audio language Model for Unified Speech, Audio, and Music Understanding**|Ziqian Wang et.al.|[2505.13880](http://arxiv.org/abs/2505.13880)|**[link](https://github.com/honee-w/u-sam)**|
|**2025-05-20**|**EfficientLLM: Efficiency in Large Language Models**|Zhengqing Yuan et.al.|[2505.13840](http://arxiv.org/abs/2505.13840)|null|
|**2025-05-19**|**Occult: Optimizing Collaborative Communication across Experts for Accelerated Parallel MoE Training and Inference**|Shuqing Luo et.al.|[2505.13345](http://arxiv.org/abs/2505.13345)|**[link](https://github.com/unites-lab/occult)**|
|**2025-05-19**|**Model Selection for Gaussian-gated Gaussian Mixture of Experts Using Dendrograms of Mixing Measures**|Tuan Thai et.al.|[2505.13052](http://arxiv.org/abs/2505.13052)|null|
|**2025-05-20**|**Model Merging in Pre-training of Large Language Models**|Yunshui Li et.al.|[2505.12082](http://arxiv.org/abs/2505.12082)|null|
|**2025-05-19**|**MegaScale-MoE: Large-Scale Communication-Efficient Training of Mixture-of-Experts Models in Production**|Chao Jin et.al.|[2505.11432](http://arxiv.org/abs/2505.11432)|null|
|**2025-05-16**|**MoE-CAP: Benchmarking Cost, Accuracy and Performance of Sparse Mixture-of-Experts Systems**|Yinsicheng Jiang et.al.|[2505.11415](http://arxiv.org/abs/2505.11415)|null|
|**2025-05-16**|**On DeepSeekMoE: Statistical Benefits of Shared Experts and Normalized Sigmoid Gating**|Huy Nguyen et.al.|[2505.10860](http://arxiv.org/abs/2505.10860)|null|
|**2025-05-14**|**PT-MoE: An Efficient Finetuning Framework for Integrating Mixture-of-Experts into Prompt Tuning**|Zongqian Li et.al.|[2505.09519](http://arxiv.org/abs/2505.09519)|**[link](https://github.com/zongqianli/pt-moe)**|
|**2025-05-14**|**Qwen3 Technical Report**|An Yang et.al.|[2505.09388](http://arxiv.org/abs/2505.09388)|**[link](https://github.com/qwenlm/qwen3)**|
|**2025-05-14**|**Insights into DeepSeek-V3: Scaling Challenges and Reflections on Hardware for AI Architectures**|Chenggang Zhao et.al.|[2505.09343](http://arxiv.org/abs/2505.09343)|null|
|**2025-05-13**|**Toward Cost-Efficient Serving of Mixture-of-Experts with Asynchrony**|Shaoyu Wang et.al.|[2505.08944](http://arxiv.org/abs/2505.08944)|null|
|**2025-05-13**|**AM-Thinking-v1: Advancing the Frontier of Reasoning at 32B Scale**|Yunjie Ji et.al.|[2505.08311](http://arxiv.org/abs/2505.08311)|null|
|**2025-05-12**|**UMoE: Unifying Attention and FFN with Shared Experts**|Yuanhang Yang et.al.|[2505.07260](http://arxiv.org/abs/2505.07260)|null|
|**2025-05-11**|**Seed1.5-VL Technical Report**|Dong Guo et.al.|[2505.07062](http://arxiv.org/abs/2505.07062)|null|
|**2025-05-11**|**FreqMoE: Dynamic Frequency Enhancement for Neural PDE Solvers**|Tianyu Chen et.al.|[2505.06858](http://arxiv.org/abs/2505.06858)|null|
|**2025-05-11**|**The power of fine-grained experts: Granularity boosts expressivity in Mixture of Experts**|Enric Boix-Adsera et.al.|[2505.06839](http://arxiv.org/abs/2505.06839)|null|
|**2025-05-10**|**Gated Attention for Large Language Models: Non-linearity, Sparsity, and Attention-Sink-Free**|Zihan Qiu et.al.|[2505.06708](http://arxiv.org/abs/2505.06708)|**[link](https://github.com/qiuzh20/gated_attention)**|
|**2025-05-10**|**Emotion-Qwen: Training Hybrid Experts for Unified Emotion and General Vision-Language Understanding**|Dawei Huang et.al.|[2505.06685](http://arxiv.org/abs/2505.06685)|null|
|**2025-05-10**|**QoS-Efficient Serving of Multiple Mixture-of-Expert LLMs Using Partial Runtime Reconfiguration**|HamidReza Imani et.al.|[2505.06481](http://arxiv.org/abs/2505.06481)|null|
|**2025-05-12**|**FloE: On-the-Fly MoE Inference on Memory-constrained GPU**|Yuxin Zhou et.al.|[2505.05950](http://arxiv.org/abs/2505.05950)|null|
|**2025-05-09**|**MxMoE: Mixed-precision Quantization for MoE with Accuracy and Performance Co-Design**|Haojie Duanmu et.al.|[2505.05799](http://arxiv.org/abs/2505.05799)|null|
|**2025-05-08**|**Divide-and-Conquer: Cold-Start Bundle Recommendation via Mixture of Diffusion Experts**|Ming Li et.al.|[2505.05035](http://arxiv.org/abs/2505.05035)|null|
|**2025-05-07**|**Pangu Ultra MoE: How to Train Your Big MoE on Ascend NPUs**|Yehui Tang et.al.|[2505.04519](http://arxiv.org/abs/2505.04519)|null|
|**2025-05-07**|**SToLa: Self-Adaptive Touch-Language Framework with Tactile Commonsense Reasoning in Open-Ended Scenarios**|Ning Cheng et.al.|[2505.04201](http://arxiv.org/abs/2505.04201)|null|
|**2025-05-02**|**MoEQuant: Enhancing Quantization for Mixture-of-Experts Large Language Models via Expert-Balanced Sampling and Affinity Guidance**|Xing Hu et.al.|[2505.03804](http://arxiv.org/abs/2505.03804)|null|
|**2025-05-06**|**Faster MoE LLM Inference for Extremely Large Models**|Haoqi Yang et.al.|[2505.03531](http://arxiv.org/abs/2505.03531)|null|
|**2025-05-06**|**3D Gaussian Splatting Data Compression with Mixture of Priors**|Lei Liu et.al.|[2505.03310](http://arxiv.org/abs/2505.03310)|null|
|**2025-05-05**|**Finger Pose Estimation for Under-screen Fingerprint Sensor**|Xiongjun Guan et.al.|[2505.02481](http://arxiv.org/abs/2505.02481)|**[link](https://github.com/xiongjunguan/draco)**|
|**2025-05-05**|**Multimodal Deep Learning-Empowered Beam Prediction in Future THz ISAC Systems**|Kai Zhang et.al.|[2505.02381](http://arxiv.org/abs/2505.02381)|null|
|**2025-05-04**|**Learning Heterogeneous Mixture of Scene Experts for Large-scale Neural Radiance Fields**|Zhenxing Mi et.al.|[2505.02005](http://arxiv.org/abs/2505.02005)|**[link](https://github.com/MiZhenxing/Switch-NeRF)**|
|**2025-05-03**|**Backdoor Attacks Against Patch-based Mixture of Experts**|Cedric Chan et.al.|[2505.01811](http://arxiv.org/abs/2505.01811)|**[link](https://github.com/geefmegeld/pmoe-backdoor)**|
|**2025-05-01**|**MoxE: Mixture of xLSTM Experts with Entropy-Aware Routing for Efficient Language Modeling**|Abdoul Majid O. Thiombiano et.al.|[2505.01459](http://arxiv.org/abs/2505.01459)|null|
|**2025-05-02**|**CoCoAFusE: Beyond Mixtures of Experts via Model Fusion**|Aurelio Raffa Ugolini et.al.|[2505.01105](http://arxiv.org/abs/2505.01105)|null|
|**2025-05-01**|**CICADA: Cross-Domain Interpretable Coding for Anomaly Detection and Adaptation in Multivariate Time Series**|Tian Lan et.al.|[2505.00415](http://arxiv.org/abs/2505.00415)|null|
|**2025-05-01**|**Mixture of Sparse Attention: Content-Based Learnable Sparse Attention via Expert-Choice Routing**|Piotr Piękos et.al.|[2505.00315](http://arxiv.org/abs/2505.00315)|**[link](https://github.com/piotrpiekos/MoSA)**|
|**2025-04-29**|**Token-Level Prompt Mixture with Parameter-Free Routing for Federated Domain Generalization**|Shuai Gong et.al.|[2504.21063](http://arxiv.org/abs/2504.21063)|null|
|**2025-04-26**|**PICO: Secure Transformers via Robust Prompt Isolation and Cybersecurity Oversight**|Ben Goertzel et.al.|[2504.21029](http://arxiv.org/abs/2504.21029)|null|
|**2025-04-29**|**MicarVLMoE: A Modern Gated Cross-Aligned Vision-Language Mixture of Experts Model for Medical Image Captioning and Report Generation**|Amaan Izhar et.al.|[2504.20343](http://arxiv.org/abs/2504.20343)|**[link](https://github.com/AI-14/micar-vl-moe)**|
|**2025-04-28**|**Accelerating Mixture-of-Experts Training with Adaptive Expert Replication**|Athinagoras Skiadopoulos et.al.|[2504.19925](http://arxiv.org/abs/2504.19925)|null|
|**2025-04-28**|**Decentralization of Generative AI via Mixture of Experts for Wireless Networks: A Comprehensive Survey**|Yunting Xu et.al.|[2504.19660](http://arxiv.org/abs/2504.19660)|null|
|**2025-05-04**|**ARTEMIS: Autoregressive End-to-End Trajectory Planning with Mixture of Experts for Autonomous Driving**|Renju Feng et.al.|[2504.19580](http://arxiv.org/abs/2504.19580)|**[link](https://github.com/Lg0914/ARTEMIS)**|
|**2025-04-29**|**BadMoE: Backdooring Mixture-of-Experts LLMs via Optimizing Routing Triggers and Infecting Dormant Experts**|Qingyue Wang et.al.|[2504.18598](http://arxiv.org/abs/2504.18598)|null|
|**2025-04-22**|**Compass-V2 Technical Report**|Sophia Maria et.al.|[2504.15527](http://arxiv.org/abs/2504.15527)|null|
|**2025-04-17**|**D $^{2}$ MoE: Dual Routing and Dynamic Scheduling for Efficient On-Device MoE-based LLM Serving**|Haodong Wang et.al.|[2504.15299](http://arxiv.org/abs/2504.15299)|null|
|**2025-04-23**|**MoE Parallel Folding: Heterogeneous Parallelism Mappings for Efficient Large-Scale MoE Model Training with Megatron Core**|Dennis Liu et.al.|[2504.14960](http://arxiv.org/abs/2504.14960)|null|
|**2025-04-22**|**Seed-Thinking-v1.5: Advancing Superb Reasoning Models with Reinforcement Learning**|ByteDance Seed et.al.|[2504.13914](http://arxiv.org/abs/2504.13914)|null|
|**2025-04-18**|**Dense Backpropagation Improves Training for Sparse Mixture-of-Experts**|Ashwinee Panda et.al.|[2504.12463](http://arxiv.org/abs/2504.12463)|**[link](https://github.com/vatsal0/default-moe)**|
|**2025-04-14**|**Correlative and Discriminative Label Grouping for Multi-Label Visual Prompt Tuning**|LeiLei Ma et.al.|[2504.09990](http://arxiv.org/abs/2504.09990)|null|
|**2025-04-13**|**Mixture-of-Shape-Experts (MoSE): End-to-End Shape Dictionary Framework to Prompt SAM for Generalizable Medical Segmentation**|Jia Wei et.al.|[2504.09601](http://arxiv.org/abs/2504.09601)|null|
|**2025-04-12**|**MoE-Lens: Towards the Hardware Limit of High-Throughput MoE LLM Serving Under Resource Constraints**|Yichao Yuan et.al.|[2504.09345](http://arxiv.org/abs/2504.09345)|null|
|**2025-04-12**|**Mixture of Group Experts for Learning Invariant Representations**|Lei Kang et.al.|[2504.09265](http://arxiv.org/abs/2504.09265)|null|
|**2025-04-22**|**RouterKT: Mixture-of-Experts for Knowledge Tracing**|Han Liao et.al.|[2504.08989](http://arxiv.org/abs/2504.08989)|**[link](https://github.com/ringotc/RouterKT)**|
|**2025-04-10**|**C3PO: Critical-Layer, Core-Expert, Collaborative Pathway Optimization for Test-Time Expert Re-Mixing**|Zhongyang Li et.al.|[2504.07964](http://arxiv.org/abs/2504.07964)|**[link](https://github.com/tianyi-lab/c3po)**|
|**2025-04-11**|**Scaling Laws for Native Multimodal Models**|Mustafa Shukor et.al.|[2504.07951](http://arxiv.org/abs/2504.07951)|null|
|**2025-04-10**|**Cluster-Driven Expert Pruning for Mixture-of-Experts Large Language Models**|Hongcheng Guo et.al.|[2504.07807](http://arxiv.org/abs/2504.07807)|**[link](https://github.com/fighoture/moe_unsupervised_pruning)**|
|**2025-04-15**|**Kimi-VL Technical Report**|Kimi Team et.al.|[2504.07491](http://arxiv.org/abs/2504.07491)|**[link](https://github.com/moonshotai/kimi-vl)**|
|**2025-04-09**|**MoEDiff-SR: Mixture of Experts-Guided Diffusion Model for Region-Adaptive MRI Super-Resolution**|Zhe Wang et.al.|[2504.07308](http://arxiv.org/abs/2504.07308)|**[link](https://github.com/zwang78/moediff-sr)**|
|**2025-04-11**|**Holistic Capability Preservation: Towards Compact Yet Comprehensive Reasoning Models**|Ling Team et.al.|[2504.07158](http://arxiv.org/abs/2504.07158)|null|
|**2025-04-09**|**Domain-Specific Pruning of Large Mixture-of-Experts Models with Few-shot Demonstrations**|Zican Dong et.al.|[2504.06792](http://arxiv.org/abs/2504.06792)|null|
|**2025-04-09**|**FedMerge: Federated Personalization via Model Merging**|Shutong Chen et.al.|[2504.06768](http://arxiv.org/abs/2504.06768)|null|
|**2025-04-08**|**S'MoRE: Structural Mixture of Residual Experts for LLM Fine-tuning**|Hanqing Zeng et.al.|[2504.06426](http://arxiv.org/abs/2504.06426)|null|
|**2025-04-08**|**HybriMoE: Hybrid CPU-GPU Scheduling and Cache Management for Efficient MoE Inference**|Shuzhang Zhong et.al.|[2504.05897](http://arxiv.org/abs/2504.05897)|**[link](https://github.com/pku-sec-lab/hybrimoe)**|
|**2025-04-08**|**Adaptive Substructure-Aware Expert Model for Molecular Property Prediction**|Tianyi Jiang et.al.|[2504.05844](http://arxiv.org/abs/2504.05844)|null|
|**2025-04-07**|**SUEDE:Shared Unified Experts for Physical-Digital Face Attack Detection Enhancement**|Zuying Xie et.al.|[2504.04818](http://arxiv.org/abs/2504.04818)|null|
|**2025-04-04**|**HeterMoE: Efficient Training of Mixture-of-Experts Models on Heterogeneous GPUs**|Yongji Wu et.al.|[2504.03871](http://arxiv.org/abs/2504.03871)|null|
|**2025-04-01**|**Detecting Financial Fraud with Hybrid Deep Learning: A Mix-of-Experts Approach to Sequential and Anomalous Patterns**|Diego Vallarino et.al.|[2504.03750](http://arxiv.org/abs/2504.03750)|null|
|**2025-04-01**|**A Unified Virtual Mixture-of-Experts Framework:Enhanced Inference and Hallucination Mitigation in Single-Model System**|Mingyan Liu et.al.|[2504.03739](http://arxiv.org/abs/2504.03739)|null|
|**2025-04-04**|**RingMoE: Mixture-of-Modality-Experts Multi-Modal Foundation Models for Universal Remote Sensing Image Interpretation**|Hanbo Bi et.al.|[2504.03166](http://arxiv.org/abs/2504.03166)|null|
|**2025-04-07**|**MiLo: Efficient Quantized MoE Inference with Mixture of Low-Rank Compensators**|Beichen Huang et.al.|[2504.02658](http://arxiv.org/abs/2504.02658)|**[link](https://github.com/supercomputing-system-ai-lab/milo)**|
|**2025-04-07**|**MegaScale-Infer: Serving Mixture-of-Experts at Scale with Disaggregated Expert Parallelism**|Ruidong Zhu et.al.|[2504.02263](http://arxiv.org/abs/2504.02263)|null|
|**2025-04-02**|**Advancing MoE Efficiency: A Collaboration-Constrained Routing (C2R) Strategy for Better Expert Parallelism Design**|Mohan Zhang et.al.|[2504.01337](http://arxiv.org/abs/2504.01337)|null|
|**2025-04-01**|**Mixture-of-Experts for Distributed Edge Computing with Channel-Aware Gating Function**|Qiuchen Song et.al.|[2504.00819](http://arxiv.org/abs/2504.00819)|null|
|**2025-04-01**|**DynMoLE: Boosting Mixture of LoRA Experts Fine-Tuning with a Hybrid Routing Mechanism**|Dengchun Li et.al.|[2504.00661](http://arxiv.org/abs/2504.00661)|**[link](https://github.com/mikecovlee/DynMoLE)**|
|**2025-03-30**|**Mixture of Routers**|Jia-Chen Zhang et.al.|[2503.23362](http://arxiv.org/abs/2503.23362)|null|
|**2025-03-29**|**Beyond Standard MoE: Mixture of Latent Experts for Resource-Efficient Language Models**|Zehua Liu et.al.|[2503.23100](http://arxiv.org/abs/2503.23100)|null|
|**2025-03-26**|**Reasoning Beyond Limits: Advances and Open Problems for LLMs**|Mohamed Amine Ferrag et.al.|[2503.22732](http://arxiv.org/abs/2503.22732)|null|
|**2025-04-01**|**Exploiting Mixture-of-Experts Redundancy Unlocks Multimodal Generative Abilities**|Raman Dutt et.al.|[2503.22517](http://arxiv.org/abs/2503.22517)|null|
|**2025-03-27**|**iMedImage Technical Report**|Ran Wei et.al.|[2503.21836](http://arxiv.org/abs/2503.21836)|null|
|**2025-03-27**|**LLaVA-CMoE: Towards Continual Mixture of Experts for Large Vision-Language Models**|Hengyuan Zhao et.al.|[2503.21227](http://arxiv.org/abs/2503.21227)|null|
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
|**2025-02-26**|**Make LoRA Great Again: Boosting LoRA with Adaptive Singular Values and Mixture-of-Experts Optimization Alignment**|Chenghao Fan et.al.|[2502.16894](http://arxiv.org/abs/2502.16894)|**[link](https://github.com/facico/goat-peft)**|
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
|**2025-02-12**|**Heterogeneous Mixture of Experts for Remote Sensing Image Super-Resolution**|Bowen Chen et.al.|[2502.09654](http://arxiv.org/abs/2502.09654)|**[link](https://github.com/mr-bamboo/mfg-hmoe)**|
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
|**2025-02-02**|**UniGraph2: Learning a Unified Embedding Space to Bind Multimodal Graphs**|Yufei He et.al.|[2502.00806](http://arxiv.org/abs/2502.00806)|**[link](https://github.com/yf-he/unigraph2)**|
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

<p align=right>(<a href=#updated-on-20250525>back to top</a>)</p>

## SSMs

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-05-21**|**FR-Mamba: Time-Series Physical Field Reconstruction Based on State Space Model**|Jiahuan Long et.al.|[2505.16083](http://arxiv.org/abs/2505.16083)|null|物理场重建（PFR）旨在根据有限的传感器测量值预测物理量（如速度、压力和温度）的状态分布。它在流体动力学和热力学等领域中起着关键作用。然而，现有的深度学习方法往往无法捕捉长时序依赖性，导致在时间演变的物理系统上的性能不佳。为了解决这一问题，我们提出了FR-Mamba，这是一种基于状态空间建模的新型时空流场重建框架。具体来说，我们设计了一种混合神经网络架构，结合了傅里叶神经算子（FNO）和状态空间模型（SSM），以捕捉全局空间特征和长时序依赖性。我们采用了最近提出的高效SSM架构Mamba，以线性时间复杂度建模长时序依赖性。同时，FNO通过利用频域变换来捕捉非局部空间特征。由这两个组件提取的时空表示随后被融合，以重建物理系统的全场分布。广泛的实验表明，我们的方法在流场重建任务中显著优于现有的PFR方法，在长序列上实现了高精度性能。|
|**2025-05-21**|**Directional Non-Commutative Monoidal Structures for Compositional Embeddings in Machine Learning**|Mahesh Godavarti et.al.|[2505.15507](http://arxiv.org/abs/2505.15507)|null|我们介绍了一种新的多维组合嵌入的代数结构，该结构基于方向性非交换幺半群算子。这项工作的核心贡献是这一新颖框架，它展示了吸引人的理论性质（沿每个维度的结合律以及确保全局一致性的交换律），同时与现代机器学习架构兼容。我们的构造为每个轴i定义了一个不同的组合算子circ_i，确保了沿每个轴的结合组合，而不施加全局交换性。重要的是，所有特定于轴的算子彼此之间都是可交换的，强制执行一个全局交换律，使跨轴组合保持一致。据我们所知，这是第一个提供通用基础的方法，将经典的序列建模范式（例如，结构化状态空间模型（SSM）和变压器自注意力机制）推广到统一的多维框架中。例如，我们框架的一维具体实例可以恢复熟悉的仿射变换代数、普通的自注意力机制和SSM风格的递归。高维泛化自然支持嵌入空间中的递归、结构感知操作。我们概述了这种结构解锁的几个潜在应用，包括变压器中的结构化位置编码、方向性图像嵌入以及序列或网格的符号建模，表明它可以指导未来的深度学习模型设计。我们正式建立了框架的代数性质，并讨论了高效的实现方法。最后，由于我们的重点是理论上的，这里不包含实验，将实证验证留待未来的工作，我们计划进行这些工作。|
|**2025-05-21**|**Mechanistic evaluation of Transformers and state space models**|Aryaman Arora et.al.|[2505.15105](http://arxiv.org/abs/2505.15105)|null|状态空间模型（SSM）在语言建模方面有望成为二次注意力Transformer的有效且高性能的替代方案，但在从上下文中回忆基本信息方面表现不一。虽然像关联记忆（AR）这样的合成任务性能可以指出这种不足，但行为指标很少提供关于某些架构为何失败而其他架构成功的机制层面的信息。为了解决这个问题，我们在AR上进行了实验，发现只有Transformer和Based SSM模型完全成功完成了AR任务，Mamba紧随其后排名第三，而其他SSM（H3、Hyena）则失败了。然后我们使用因果干预来解释原因。我们发现，Transformer和Based通过归纳头学习在上下文中存储键值关联。相比之下，SSM仅在最后一个状态计算这些关联，只有Mamba因其短卷积组件而成功。为了扩展和深化这些发现，我们引入了关联树调用（ATR），这是一种基于PCFG归纳的与AR类似的合成任务。ATR将类似语言的层次结构引入到AR设置中。我们发现所有架构都学习了与AR相同的机制，并且同样是这三种模型成功完成了任务。这些结果揭示了具有相似准确性的架构可能仍然存在实质性差异，从而推动了对机制评估的采用。|
|**2025-05-20**|**STree: Speculative Tree Decoding for Hybrid State-Space Models**|Yangchao Wu et.al.|[2505.14969](http://arxiv.org/abs/2505.14969)|null|推测解码是一种利用硬件并行性来提高大规模自回归（AR）Transformer模型效率的技术，它通过单次前向传递实现多个步骤的令牌生成。状态空间模型（SSMs）比AR Transformers更高效，因为它们的状态可以总结所有过去的数据，而无需在滑动窗口上下文中缓存或重新处理令牌。然而，它们的状态也可能包含数千个令牌；因此，推测解码最近被扩展到了SSMs上。然而，现有的方法并没有利用基于树的验证方法，因为当前的SSMs缺乏有效计算令牌树的方法。我们提出了第一个可扩展的算法，用于在状态空间模型（SSMs）和SSM与Transformer层的混合架构中执行基于树的推测解码。我们利用累积状态转移矩阵的结构来促进基于树的推测解码，同时对当前SSM状态更新实现的开销最小。通过该算法，我们描述了一个硬件感知的实现，这改进了将AR Transformer基于树的推测解码方法直接应用于SSMs时的朴素应用。此外，在三个不同的基准测试中，即使使用基线草稿模型和树结构，我们的方法也优于纯推测解码的SSMs，为SSM和混合模型推理提供了进一步加速的机会。代码将在论文接受后发布。|
|**2025-05-19**|**Mamba-Adaptor: State Space Model Adaptor for Visual Recognition**|Fei Xie et.al.|[2505.12685](http://arxiv.org/abs/2505.12685)|null|最近的状态空间模型（SSM），特别是Mamba，在视觉建模方面表现出色，并且具有优越的模型效率。然而，由于序列模型中存在的三个主要限制，Mamba在视觉任务中的应用表现较差：1）因果计算无法访问全局上下文；2）在计算当前隐藏状态时出现长距离遗忘；3）由于输入被转换为序列形式，导致空间结构建模能力较弱。为了解决这些问题，我们研究了一种简单但强大的适用于Mamba模型的视觉任务适配器，该适配器由两个功能模块组成：Adaptor-T和Adaptor-S。在解决SSM的隐藏状态时，我们应用了一个轻量级预测模块Adaptor-T来选择一组可学习的位置作为记忆增强，以缓解长距离遗忘问题。此外，我们利用由多尺度扩张卷积核组成的Adaptor-S来增强空间建模，并将图像归纳偏差引入特征输出中。这两个模块都可以扩大因果计算中的上下文建模范围，因为输出通过不可访问的特征得到了增强。我们探索了Mamba-适配器的三种使用方式：作为各种视觉任务的一般视觉骨干网络；作为一个提升预训练骨干网络性能的增强模块；以及作为一个高效的微调模块，用于适应基础模型进行迁移学习任务。广泛的实验验证了Mamba-适配器在这三种设置下的有效性。值得注意的是，我们的Mamba-适配器在ImageNet和COCO基准测试上达到了最先进的性能。|
|**2025-05-18**|**MTIL: Encoding Full History with Mamba for Temporal Imitation Learning**|Yulin Zhou et.al.|[2505.12410](http://arxiv.org/abs/2505.12410)|**[link](https://github.com/yulinzhouzyl/mtil)**|**标准的模仿学习（IL）方法在机器人领域已经取得了相当大的成功，但通常依赖于马尔可夫假设，这限制了它们在需要历史上下文来消除当前观察模糊性的任务中的应用。这种局限性阻碍了在长时序操作任务中的表现，因为在这些任务中，正确的动作取决于过去事件，而这些事件不能完全通过当前状态捕捉。为了解决这一根本挑战，我们引入了Mamba时序模仿学习（MTIL），这是一种新颖的方法，利用了状态空间模型（SSMs）中固有的循环状态动态，特别是Mamba架构。MTIL将整个轨迹历史编码到一个压缩的隐藏状态中，并基于这个全面的时间上下文以及当前多模态观测来条件化动作预测。通过对模拟基准测试（ACT数据集任务、Robomimic、LIBERO）和专门设计用于探测时间依赖性的实际顺序操作任务进行广泛的实验，MTIL显著优于最先进的方法如ACT和扩散策略。我们的研究结果证实了完整时间上下文对于鲁棒的序列决策的重要性，并验证了MTIL作为一种强大方法能够超越马尔可夫模仿学习的内在限制。**|
|**2025-05-17**|**Learning to Dissipate Energy in Oscillatory State-Space Models**|Jared Boyer et.al.|[2505.12171](http://arxiv.org/abs/2505.12171)|**[link](https://github.com/jaredbmit/damped-linoss)**|**状态空间模型（SSM）是一类用于序列学习的网络，其固定的状态大小和相对于序列长度的线性复杂度与典型的注意力机制的二次缩放形成对比。受到神经科学观察的启发，线性振荡状态空间模型（LinOSS）是最近提出的一类SSM，由离散化的强迫谐波振荡器层构成。尽管这些模型表现出色，通过在对角递归矩阵上进行快速并行扫描，在序列长度达到50k的任务中实现了最先进的性能，但LinOSS模型依赖于与状态演化时间尺度固有耦合的刚性能量耗散（“遗忘”）机制。由于遗忘是长距离推理的关键机制，我们展示了这些模型的表示限制，并引入了阻尼线性振荡状态空间模型（D-LinOSS），这是一种更通用的振荡SSM，能够在多个时间尺度上学习潜态能量的耗散。我们分析了模型递归矩阵的谱分布，并证明了在简单、灵活的参数化下，SSM层表现出稳定的动力学。D-LinOSS在长距离学习任务上始终优于之前的LinOSS方法，而没有引入额外的复杂性，并且同时将超参数搜索空间减少了50%。**|
|**2025-05-17**|**WaLRUS: Wavelets for Long-range Representation Using SSMs**|Hossein Babaei et.al.|[2505.12161](http://arxiv.org/abs/2505.12161)|null|状态空间模型（SSM）已被证明是处理序列数据中长距离依赖关系的强大工具。尽管最近的方法HiPPO已经展示了强大的性能，并且成为机器学习模型S4和Mamba的基础，但它仍然受限于仅能使用少数具有良好封闭形式解的特定基。SaFARi框架推广了这种方法，能够从任意框架构建SSM，包括非正交和冗余框架，从而允许在SSM家族中存在无限多样的“种类”。在这篇论文中，我们介绍了WaLRUS（基于小波的长距离表示使用SSM），这是一种基于Daubechies小波实现的SaFARi新方法。|
|**2025-05-16**|**Regularity and Stability Properties of Selective SSMs with Discontinuous Gating**|Nikola Zubić et.al.|[2505.11602](http://arxiv.org/abs/2505.11602)|null|深度选择性状态空间模型（SSMs），以其输入依赖的、时变的参数为特征，提供了显著的表现力，但在稳定性分析方面带来了挑战，尤其是对于不连续的门控信号。本文通过被动性和输入到状态稳定性（ISS）的角度，研究了连续时间选择性SSMs的稳定性和规律性属性。我们证明了内在的能量耗散保证了过去状态的指数遗忘。关键的是，我们证明了无外力系统动力学具有一个基本的二次能量函数，其定义矩阵表现出稳健的 $\text{AUC}_{\text{loc}}$ 规律性，能够适应不连续的门控。此外，假设一个通用的二次存储函数确保了所有输入下的被动性，我们推导出了参数化的LMI条件和核约束，限制了门控机制，形式化了循环模型的“不可逆遗忘”。最后，我们提供了全局ISS的充分条件，将均匀局部耗散性与整体系统鲁棒性联系起来。我们的发现为理解和设计稳定可靠的深度选择性SSMs提供了一个严格的框架。|
|**2025-05-16**|**Hybrid-Emba3D: Geometry-Aware and Cross-Path Feature Hybrid Enhanced State Space Model for Point Cloud Classification**|Bin Liu et.al.|[2505.11099](http://arxiv.org/abs/2505.11099)|**[link](https://github.com/l1277471578/hybrid-emba3d)**|**点云分类任务面临着高效提取局部几何特征同时保持模型复杂性的双重挑战。Mamba架构利用状态空间模型（SSM）的线性复杂度优势克服了Transformer的计算瓶颈，同时平衡了全局建模能力。然而，其单向依赖性和点云无序性质之间的固有矛盾阻碍了局部邻域内空间相关性的建模，从而限制了几何特征的提取。本文提出了Hybrid-Emba3D，这是一种通过几何特征耦合和跨路径特征混合增强的双向Mamba模型。局部几何池化与几何特征耦合机制通过局部中心点与其邻域之间几何信息的协调传播和动态聚合，显著增强了局部特征的判别力，而无需引入额外参数。设计的协作特征增强器采用双路径混合，有效处理局部突变和稀疏关键信号，突破了传统SSM长程建模的局限。实验结果表明，所提出的模型在ModelNet40数据集上仅增加0.03M参数就达到了95.99%的新SOTA分类精度。**|
|**2025-05-14**|**Dyadic Mamba: Long-term Dyadic Human Motion Synthesis**|Julian Tanke et.al.|[2505.09827](http://arxiv.org/abs/2505.09827)|null|
|**2025-05-13**|**Block-Biased Mamba for Long-Range Sequence Processing**|Annan Yu et.al.|[2505.09022](http://arxiv.org/abs/2505.09022)|null|
|**2025-05-13**|**DyGSSM: Multi-view Dynamic Graph Embeddings with State Space Model Gradient Update**|Bizhan Alipour Pijan et.al.|[2505.09017](http://arxiv.org/abs/2505.09017)|null|
|**2025-05-13**|**SaFARi: State-Space Models for Frame-Agnostic Representation**|Hossein Babaei et.al.|[2505.08977](http://arxiv.org/abs/2505.08977)|null|
|**2025-05-13**|**Efficient Unstructured Pruning of Mamba State-Space Models for Resource-Constrained Environments**|Ibne Farabi Shihab et.al.|[2505.08299](http://arxiv.org/abs/2505.08299)|null|
|**2025-05-08**|**PillarMamba: Learning Local-Global Context for Roadside Point Cloud via Hybrid State Space Model**|Zhang Zhang et.al.|[2505.05397](http://arxiv.org/abs/2505.05397)|null|
|**2025-05-08**|**EDmamba: A Simple yet Effective Event Denoising Method with State Space Model**|Ciyu Ruan et.al.|[2505.05391](http://arxiv.org/abs/2505.05391)|null|
|**2025-05-04**|**Learning Local Causal World Models with State Space Models and Attention**|Francesco Petri et.al.|[2505.02074](http://arxiv.org/abs/2505.02074)|null|
|**2025-05-02**|**BiGSCoder: State Space Model for Code Understanding**|Shweta Verma et.al.|[2505.01475](http://arxiv.org/abs/2505.01475)|null|
|**2025-05-03**|**Vision Mamba in Remote Sensing: A Comprehensive Survey of Techniques, Applications and Outlook**|Muyi Bao et.al.|[2505.00630](http://arxiv.org/abs/2505.00630)|**[link](https://github.com/baobao0926/awesome-mamba-in-remote-sensing)**|
|**2025-04-24**|**Fine-Grained Fusion: The Missing Piece in Area-Efficient State Space Model Acceleration**|Robin Geens et.al.|[2504.17333](http://arxiv.org/abs/2504.17333)|null|
|**2025-04-22**|**LongMamba: Enhancing Mamba's Long Context Capabilities via Training-Free Receptive Field Enlargement**|Zhifan Ye et.al.|[2504.16053](http://arxiv.org/abs/2504.16053)|**[link](https://github.com/gatech-eic/longmamba)**|
|**2025-04-20**|**VM-BHINet:Vision Mamba Bimanual Hand Interaction Network for 3D Interacting Hand Mesh Recovery From a Single RGB Image**|Han Bi et.al.|[2504.14618](http://arxiv.org/abs/2504.14618)|null|
|**2025-04-19**|**Empirical Evaluation of Knowledge Distillation from Transformers to Subquadratic Language Models**|Patrick Haller et.al.|[2504.14366](http://arxiv.org/abs/2504.14366)|null|
|**2025-04-18**|**CacheFormer: High Attention-Based Segment Caching**|Sushant Singh et.al.|[2504.13981](http://arxiv.org/abs/2504.13981)|null|
|**2025-04-17**|**Hierarchical Feature Learning for Medical Point Clouds via State Space Model**|Guoqing Zhang et.al.|[2504.13015](http://arxiv.org/abs/2504.13015)|**[link](https://github.com/wlsdzyzl/flemme)**|
|**2025-04-16**|**Dynamics and Computational Principles of Echo State Networks: A Mathematical Perspective**|Pradeep Singh et.al.|[2504.11757](http://arxiv.org/abs/2504.11757)|null|
|**2025-04-15**|**Efficient Hybrid Language Model Compression through Group-Aware SSM Pruning**|Ali Taghibakhshi et.al.|[2504.11409](http://arxiv.org/abs/2504.11409)|null|
|**2025-04-12**|**Stochastic Claims Reserving Using State Space Modeling**|Rajesh Selukar et.al.|[2504.09292](http://arxiv.org/abs/2504.09292)|null|
|**2025-04-07**|**Leveraging State Space Models in Long Range Genomics**|Matvei Popov et.al.|[2504.06304](http://arxiv.org/abs/2504.06304)|null|
|**2025-04-08**|**DefMamba: Deformable Visual State Space Model**|Leiye Liu et.al.|[2504.05794](http://arxiv.org/abs/2504.05794)|null|
|**2025-04-06**|**GAMBAS: Generalised-Hilbert Mamba for Super-resolution of Paediatric Ultra-Low-Field MRI**|Levente Baljer et.al.|[2504.04523](http://arxiv.org/abs/2504.04523)|**[link](https://github.com/levente-1/GAMBAS)**|
|**2025-04-04**|**Pyramid-based Mamba Multi-class Unsupervised Anomaly Detection**|Nasar Iqbal et.al.|[2504.03442](http://arxiv.org/abs/2504.03442)|null|
|**2025-04-03**|**State-Space Model Inspired Multiple-Input Multiple-Output Spiking Neurons**|Sanja Karilanova et.al.|[2504.02591](http://arxiv.org/abs/2504.02591)|null|
|**2025-04-09**|**Mesh Mamba: A Unified State Space Model for Saliency Prediction in Non-Textured and Textured Meshes**|Kaiwei Zhang et.al.|[2504.01466](http://arxiv.org/abs/2504.01466)|**[link](https://github.com/kaviezhang/meshmamba)**|
|**2025-04-01**|**Scaling Up Resonate-and-Fire Networks for Fast Deep Learning**|Thomas E. Huber et.al.|[2504.00719](http://arxiv.org/abs/2504.00719)|**[link](https://github.com/thomasehuber/s5-rf)**|
|**2025-04-01**|**ParallelFlow: Parallelizing Linear Transformers via Flow Discretization**|Nicola Muca Cirone et.al.|[2504.00492](http://arxiv.org/abs/2504.00492)|null|
|**2025-03-31**|**TransMamba: Flexibly Switching between Transformer and Mamba**|Yixing Li et.al.|[2503.24067](http://arxiv.org/abs/2503.24067)|null|
|**2025-03-31**|**Free Parametrization of L2-bounded State Space Models**|Leonardo Massai et.al.|[2503.23818](http://arxiv.org/abs/2503.23818)|**[link](https://github.com/DecodEPFL/SSM)**|
|**2025-03-29**|**Fast Training of Recurrent Neural Networks with Stationary State Feedbacks**|Paul Caillon et.al.|[2503.23104](http://arxiv.org/abs/2503.23104)|**[link](https://github.com/p0lcai/dsf)**|
|**2025-03-29**|**SSM-RDU: A Reconfigurable Dataflow Unit for Long-Sequence State-Space Models**|Sho Ko et.al.|[2503.22937](http://arxiv.org/abs/2503.22937)|null|
|**2025-04-03**|**Quamba2: A Robust and Scalable Post-training Quantization Framework for Selective State Space Models**|Hung-Yueh Chiang et.al.|[2503.22879](http://arxiv.org/abs/2503.22879)|**[link](https://github.com/enyac-group/quamba)**|
|**2025-04-02**|**Q-MambaIR: Accurate Quantized Mamba for Efficient Image Restoration**|Yujie Chen et.al.|[2503.21970](http://arxiv.org/abs/2503.21970)|null|
|**2025-03-27**|**vGamba: Attentive State Space Bottleneck for efficient Long-range Dependencies in Visual Recognition**|Yunusa Haruna et.al.|[2503.21262](http://arxiv.org/abs/2503.21262)|**[link](https://github.com/yunusa2k2/vGamba)**|
|**2025-03-26**|**ReverBERT: A State Space Model for Efficient Text-Driven Speech Style Transfer**|Michael Brown et.al.|[2503.20992](http://arxiv.org/abs/2503.20992)|null|
|**2025-03-25**|**A Comprehensive Analysis of Mamba for 3D Volumetric Medical Image Segmentation**|Chaohan Wang et.al.|[2503.19308](http://arxiv.org/abs/2503.19308)|null|
|**2025-03-22**|**A Survey on Structured State Space Sequence (S4) Models**|Shriyank Somvanshi et.al.|[2503.18970](http://arxiv.org/abs/2503.18970)|null|
|**2025-03-24**|**Exploring State Space Model in Wavelet Domain: An Infrared and Visible Image Fusion Network via Wavelet Transform and State Space Model**|Tianpei Zhang et.al.|[2503.18378](http://arxiv.org/abs/2503.18378)|null|
|**2025-03-23**|**GLADMamba: Unsupervised Graph-Level Anomaly Detection Powered by Selective State Space Model**|Yali Fu et.al.|[2503.17903](http://arxiv.org/abs/2503.17903)|**[link](https://github.com/yali-f/gladmamba)**|
|**2025-03-21**|**MM-UNet: Meta Mamba UNet for Medical Image Segmentation**|Bin Xie et.al.|[2503.17540](http://arxiv.org/abs/2503.17540)|null|
|**2025-03-24**|**An Energy-Adaptive Elastic Equivariant Transformer Framework for Protein Structure Representation**|Zhongyue Zhang et.al.|[2503.16996](http://arxiv.org/abs/2503.16996)|null|
|**2025-03-20**|**SaMam: Style-aware State Space Model for Arbitrary Image Style Transfer**|Hongda Liu et.al.|[2503.15934](http://arxiv.org/abs/2503.15934)|**[link](https://github.com/Chernobyllight/SaMam)**|
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
|**2025-02-12**|**SS4Rec: Continuous-Time Sequential Recommendation with State Space Models**|Wei Xiao et.al.|[2502.08132](http://arxiv.org/abs/2502.08132)|**[link](https://github.com/XiaoWei-i/SS4Rec)**|
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

<p align=right>(<a href=#updated-on-20250525>back to top</a>)</p>

## Communication Intelligence

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-09-21**|**LLM Agents as 6G Orchestrator: A Paradigm for Task-Oriented Physical-Layer Automation**|Zhuoran Xiao et.al.|[2410.03688](http://arxiv.org/abs/2410.03688)|null|生成式预训练模型的快速发展正在推动技术进步从基本应用（如聊天机器人）向更复杂的基于代理的系统转变。将6G系统与大型语言模型（LLM）代理和数字孪生（DT）相结合，具有巨大的潜力和必要性，以管理具有新出现功能（如原生AI服务和感知）的高度复杂通信系统。借助面向6G的代理，基站可以理解各种动态上层任务的传输需求，自动编排最优系统工作流程。通过持续从6G DT获得反馈进行强化，代理最终可以相应地提高实际系统的性能。与现有的为通用应用设计的LLM代理不同，面向6G的代理旨在利用大量额外的专业知识进行高度严谨和精确的规划，这不可避免地需要从模型训练到实现的特定系统设计。本文提出了一种构建面向任务的6G LLM代理的新颖综合方法。我们首先提出了一种两阶段持续预训练和微调方案，以构建领域基础模型和多样化的专业专家模型，以满足各种应用场景的需求。此外，还提出了一种基于语义检索的新颖推理框架，以利用现有的通信相关功能。实验结果表明，对于诸如物理层任务分解等示例任务，所提出的范式是可行且有效的。|

<p align=right>(<a href=#updated-on-20250525>back to top</a>)</p>

## RAG

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-05-22**|**R1-Searcher++: Incentivizing the Dynamic Knowledge Acquisition of LLMs via Reinforcement Learning**|Huatong Song et.al.|[2505.17005](http://arxiv.org/abs/2505.17005)|null|大型语言模型（LLM）虽然强大，但容易因静态知识而产生幻觉。检索增强生成（RAG）通过注入外部信息来帮助解决这一问题，但当前的方法往往成本高昂、泛化能力差或忽视了模型的内部知识。在本文中，我们介绍了R1-Searcher++，这是一种新颖的框架，旨在训练LLM自适应地利用内部和外部知识源。R1-Searcher++采用两阶段训练策略：初始的SFT冷启动阶段用于初步格式学习，随后是动态知识获取的强化学习（RL）阶段。RL阶段使用结果监督来鼓励探索，结合了一种奖励机制以促进内部知识的利用，并集成了一种记忆机制以持续吸收检索到的信息，从而丰富模型的内部知识。通过利用内部知识和外部搜索引擎，模型不断改进其能力，实现高效的检索增强推理。我们的实验表明，R1-Searcher++优于以往的RAG和推理方法，并实现了高效的检索。代码可在https://github.com/RUCAIBox/R1-Searcher-plus获取。|
|**2025-05-22**|**Code Graph Model (CGM): A Graph-Integrated Large Language Model for Repository-Level Software Engineering Tasks**|Hongyuan Tao et.al.|[2505.16901](http://arxiv.org/abs/2505.16901)|null|最近在大型语言模型（LLMs）方面的进展在函数级代码生成方面显示出潜力，但仓库级的软件工程任务仍然具有挑战性。当前的解决方案主要依赖于专有LLM代理，这引入了不可预测性并限制了可访问性，引发了关于数据隐私和模型定制的担忧。本文探讨了开源LLMs是否能够在不采用基于代理的方法的情况下有效解决仓库级任务。我们通过使LLMs能够理解代码库中的函数和文件的语义信息和结构依赖关系来证明这是可能的。为此，我们引入了代码图模型（CGMs），将仓库代码图结构整合到LLM的注意力机制中，并使用专门适配器将节点属性映射到LLM的输入空间。当与无代理的图RAG框架结合时，我们的方法在使用开源Qwen2.5-72B模型的情况下，在SWE-bench Lite基准测试中达到了43.00%的解决率。这一表现位列开源权重模型之首，在具有开源系统的方案中排名第二，总体上排名第八，超过了之前最好的基于开源模型方法12.33%。|
|**2025-05-22**|**Walk&Retrieve: Simple Yet Effective Zero-shot Retrieval-Augmented Generation via Knowledge Graph Walks**|Martin Böckling et.al.|[2505.16849](http://arxiv.org/abs/2505.16849)|**[link](https://github.com/MartinBoeckling/KGRag)**|**大型语言模型（LLM）展示了令人印象深刻的推理能力，但往往存在幻觉或知识过时的问题。基于知识图谱（KG）的检索增强生成（RAG）通过将LLM的响应基于外部结构化信息库进行接地，来解决这些不足。然而，许多基于KG的RAG方法在（i）对齐KG和文本表示、（ii）平衡检索准确性和效率以及（iii）适应动态更新的KG方面遇到困难。在这项工作中，我们引入了Walk&Retrieve，这是一个简单而有效的基于KG的框架，它利用基于行走的图遍历和知识口头化来为零样本RAG生成语料库。该方法围绕高效的KG行走构建，不需要针对特定领域的数据进行微调，从而能够无缝适应KG更新，减少计算开销，并允许与任何现成的基础LLM集成。尽管其简单，Walk&Retrieve在响应准确性和减少幻觉方面表现出色，经常优于现有的RAG系统。此外，它还展示了较低的查询延迟和对大规模KG的强大可扩展性，突显了轻量级检索策略作为未来RAG研究强有力基准的潜力。**|
|**2025-05-22**|**SimpleDeepSearcher: Deep Information Seeking via Web-Powered Reasoning Trajectory Synthesis**|Shuang Sun et.al.|[2505.16834](http://arxiv.org/abs/2505.16834)|null|检索增强生成（RAG）系统在需要多步推理和迭代信息检索的复杂深度搜索场景中提升了大型语言模型（LLMs）的能力。然而，现有方法面临关键限制，如缺乏高质量的训练轨迹、模拟环境中的分布不匹配以及实际部署时的计算成本过高。本文介绍了一种轻量而有效的框架SimpleDeepSearcher，通过策略性数据工程而不是复杂的训练范式来弥合这一差距。我们的方法通过在实时网络搜索环境中模拟真实的用户交互，并结合优化输入和输出多样性和质量的多标准筛选策略，合成高质量的训练数据。在五个不同领域的基准测试中，仅对871个精选样本进行监督微调（SFT），就显著优于基于强化学习的基线。我们的工作通过系统地解决数据稀缺瓶颈，确立了SFT作为可行路径的地位，为高效的深度搜索系统提供了实用见解。我们的代码可在https://github.com/RUCAIBox/SimpleDeepSearcher获取。|
|**2025-05-22**|**Beyond LLMs: An Exploration of Small Open-source Language Models in Logging Statement Generation**|Renyi Zhong et.al.|[2505.16590](http://arxiv.org/abs/2505.16590)|null|有效的软件维护在很大程度上依赖于高质量的日志记录语句，但手动日志记录具有挑战性、容易出错且标准化不足，经常导致日志质量不一致。虽然大型语言模型在自动日志记录方面显示出潜力，但它们引入了隐私、资源消耗和适应特定企业需求方面的担忧。为了解决这些限制，本文通过实证研究探讨小型开源语言模型（SOLMs）是否可以通过适当利用成为可行的替代方案。具体而言，我们对四个著名的小型开源语言模型进行了大规模的实证研究，系统地评估了各种交互策略、参数高效微调技术、模型大小和模型类型在自动日志记录中的影响。我们的主要发现表明，检索增强生成显著提高了性能，而LoRA是一种非常有效的参数高效微调技术。尽管较大的SOLMs往往表现更好，但这涉及计算资源的权衡，且经过指令微调的SOLMs通常优于其基础版本。值得注意的是，经过微调的SOLMs，特别是Qwen2.5-coder-14B，在准确预测日志位置和生成高质量语句方面超过了现有的专用工具和大型语言模型基线，这一结论得到了传统评估指标和LLM作为评判者的评估的支持。此外，SOLMs还展示了在多样化且未见过的代码库中的强大泛化能力。|
|**2025-05-22**|**CUB: Benchmarking Context Utilisation Techniques for Language Models**|Lovisa Hagström et.al.|[2505.16518](http://arxiv.org/abs/2505.16518)|null|在知识密集型任务中，如问答和事实核查，整合外部知识至关重要。然而，语言模型（LMs）可能会忽略与过时参数记忆相矛盾的相关信息，或者被不相关的上下文所干扰。虽然最近提出了许多鼓励或抑制上下文利用的上下文利用操作技术（CMTs）来缓解这些问题，但很少有系统性的比较。在这篇论文中，我们开发了CUB（上下文利用基准），以帮助检索增强生成（RAG）领域的从业者识别最适合他们需求的CMT。CUB允许对三种不同的上下文类型进行严格测试，这些类型涵盖了现实世界中上下文利用场景的关键挑战。通过这个基准，我们在三个多样化的数据集和任务上评估了七种最先进的方法，这些方法代表了CMTs的主要类别，并应用于九个语言模型。我们的结果显示，大多数现有的CMTs难以处理在实际检索增强场景中可能遇到的所有类型的上下文。此外，我们发现许多CMTs在简单的合成数据集上的表现优于更真实的自然样本数据集。总的来说，我们的结果表明需要对CMTs进行全面测试，并开发能够处理多种上下文类型的CMTs。|
|**2025-05-22**|**Benchmarking Retrieval-Augmented Multimomal Generation for Document Question Answering**|Kuicai Dong et.al.|[2505.16470](http://arxiv.org/abs/2505.16470)|null|文档视觉问答（DocVQA）在处理长篇多模态文档（文本、图像、表格）和进行跨模态推理时面临双重挑战。当前的文档检索增强生成（DocRAG）方法因其以文本为中心的方式而受到限制，经常遗漏关键的视觉信息。该领域还缺乏强大的基准来评估多模态证据选择和整合。我们引入了MMDocRAG，这是一个全面的基准，包含4,055个专家标注的问答对，具有多页、跨模态的证据链。我们的框架引入了创新的指标来评估多模态引用选择，并允许答案中穿插文本与相关的视觉元素。通过对60种视觉语言模型/大型语言模型和14种检索系统的大量实验，我们发现了在多模态证据检索、选择和整合方面的持续性挑战。主要发现表明，先进的专有视觉语言模型比开源替代方案表现出更优的性能。此外，它们在使用多模态输入时比仅使用文本输入显示出适度的优势，而开源替代方案则表现出显著的性能下降。值得注意的是，经过微调的大型语言模型在使用详细的图像描述时取得了显著改进。MMDocRAG建立了一个严格的测试平台，并为开发更强大的多模态DocVQA系统提供了可操作的见解。我们的基准和代码可在https://mmdocrag.github.io/MMDocRAG/获取。|
|**2025-05-22**|**Attributing Response to Context: A Jensen-Shannon Divergence Driven Mechanistic Study of Context Attribution in Retrieval-Augmented Generation**|Ruizhe Li et.al.|[2505.16415](http://arxiv.org/abs/2505.16415)|null|检索增强生成（RAG）利用大型语言模型（LLM）结合外部上下文来提高生成响应的准确性和可靠性。然而，由于当前方法通常需要大量的微调或人工标注，可靠地将生成内容归因于特定上下文段落（即上下文归因）仍然具有挑战性。在这项工作中，我们引入了一种基于Jensen-Shannon散度的方法来归因响应到上下文（ARC-JSD），该方法能够在不进行额外微调或替代建模的情况下，高效且准确地识别关键的上下文句子。通过对TyDi QA、Hotpot QA和Musique等广泛的RAG基准测试以及不同规模的指令调优LLM进行评估，结果显示，与之前的基于替代模型的方法相比，我们的方法在准确性上表现出色，并且在计算效率上有显著提升。此外，我们的机制分析揭示了负责上下文归因的具体注意力头和多层感知器（MLP）层，为理解RAG模型内部工作原理提供了有价值的见解。|
|**2025-05-22**|**Chain-of-Thought Poisoning Attacks against R1-based Retrieval-Augmented Generation Systems**|Hongru Song et.al.|[2505.16367](http://arxiv.org/abs/2505.16367)|null|检索增强生成（RAG）系统可以有效缓解大型语言模型（LLMs）的幻觉问题，但它们也存在固有的脆弱性。在大规模实际部署RAG系统之前识别这些弱点非常重要，因为这为未来构建更安全和鲁棒的RAG系统奠定了基础。现有的对抗攻击方法通常利用知识库污染来探测RAG系统的漏洞，这种方法可以有效地欺骗标准的RAG模型。然而，随着现代LLMs深度推理能力的迅速进步，仅注入错误知识的方法在攻击具有深度推理能力的RAG系统时已显得不足。受LLMs深度思考能力的启发，本文从基于R1的RAG系统中提取推理过程模板，使用这些模板将错误知识包装成对抗性文档，并将其注入知识库以攻击RAG系统。我们方法的关键思想是，通过模拟与模型训练信号一致的思维链模式，对抗性文档可能被模型误解为真实的过往推理过程，从而增加其被引用的可能性。在MS MARCO段落排名数据集上进行的实验表明了我们提出方法的有效性。|
|**2025-05-22**|**Ask, Retrieve, Summarize: A Modular Pipeline for Scientific Literature Summarization**|Pierre Achkar et.al.|[2505.16349](http://arxiv.org/abs/2505.16349)|null|科学出版物的指数级增长使得研究人员越来越难以保持更新并有效地综合知识。本文介绍了XSum，这是一种使用检索增强生成（RAG）的科学领域多文档摘要（MDS）模块化流水线。该流水线包括两个核心组件：问题生成模块和编辑模块。问题生成模块根据输入的论文动态生成问题，确保检索到相关且准确的信息。编辑模块将检索到的内容综合成连贯且结构良好的摘要，符合学术标准的正确引用。在SurveySum数据集上的评估显示，XSum在CheckEval、G-Eval和Ref-F1等指标上相比现有方法取得了显著改进。这项工作提供了一个透明、可适应的科学摘要框架，并在广泛领域中具有潜在应用。代码可在https://github.com/webis-de/scolia25-xsum获取。|
|**2025-05-21**|**Scalable Defense against In-the-wild Jailbreaking Attacks with Safety Context Retrieval**|Taiye Chen et.al.|[2505.15753](http://arxiv.org/abs/2505.15753)|null|
|**2025-05-21**|**HDLxGraph: Bridging Large Language Models and HDL Repositories via HDL Graph Databases**|Pingqing Zheng et.al.|[2505.15701](http://arxiv.org/abs/2505.15701)|**[link](https://github.com/nick-zheng-q/hdlxgraph)**|
|**2025-05-21**|**Listen to the Context: Towards Faithful Large Language Models for Retrieval Augmented Generation on Climate Questions**|David Thulke et.al.|[2505.15633](http://arxiv.org/abs/2505.15633)|null|
|**2025-05-21**|**Do RAG Systems Suffer From Positional Bias?**|Florin Cuconasu et.al.|[2505.15561](http://arxiv.org/abs/2505.15561)|null|
|**2025-05-21**|**Single LLM, Multiple Roles: A Unified Retrieval-Augmented Generation Framework Using Role-Specific Token Optimization**|Yutao Zhu et.al.|[2505.15444](http://arxiv.org/abs/2505.15444)|null|
|**2025-05-21**|**Silent Leaks: Implicit Knowledge Extraction Attack on RAG Systems through Benign Queries**|Yuhao Wang et.al.|[2505.15420](http://arxiv.org/abs/2505.15420)|null|
|**2025-05-21**|**Reranking with Compressed Document Representation**|Hervé Déjean et.al.|[2505.15394](http://arxiv.org/abs/2505.15394)|null|
|**2025-05-21**|**Adaptive Plan-Execute Framework for Smart Contract Security Auditing**|Zhiyuan Wei et.al.|[2505.15242](http://arxiv.org/abs/2505.15242)|null|
|**2025-05-21**|**Deliberation on Priors: Trustworthy Reasoning of Large Language Models on Knowledge Graphs**|Jie Ma et.al.|[2505.15210](http://arxiv.org/abs/2505.15210)|**[link](https://github.com/reml-group/deliberation-on-priors)**|
|**2025-05-21**|**RAG or Fine-tuning? A Comparative Study on LCMs-based Code Completion in Industry**|Chaozheng Wang et.al.|[2505.15179](http://arxiv.org/abs/2505.15179)|null|
|**2025-05-20**|**BugRepro: Enhancing Android Bug Reproduction with Domain-Specific Knowledge Integration**|Hongrong Yin et.al.|[2505.14528](http://arxiv.org/abs/2505.14528)|null|
|**2025-05-20**|**RAVENEA: A Benchmark for Multimodal Retrieval-Augmented Visual Culture Understanding**|Jiaang Li et.al.|[2505.14462](http://arxiv.org/abs/2505.14462)|**[link](https://github.com/yfyuan01/ravenea)**|
|**2025-05-20**|**Causal Cartographer: From Mapping to Reasoning Over Counterfactual Worlds**|Gaël Gendron et.al.|[2505.14396](http://arxiv.org/abs/2505.14396)|**[link](https://github.com/ggendro/causal-cartographer)**|
|**2025-05-20**|**SCAN: Semantic Document Layout Analysis for Textual and Visual Retrieval-Augmented Generation**|Yuyang Dong et.al.|[2505.14381](http://arxiv.org/abs/2505.14381)|null|
|**2025-05-20**|**Automatic Dataset Generation for Knowledge Intensive Question Answering Tasks**|Sizhe Yuen et.al.|[2505.14212](http://arxiv.org/abs/2505.14212)|null|
|**2025-05-20**|**s3: You Don't Need That Much Data to Train a Search Agent via RL**|Pengcheng Jiang et.al.|[2505.14146](http://arxiv.org/abs/2505.14146)|**[link](https://github.com/pat-jj/s3)**|
|**2025-05-20**|**MultiHal: Multilingual Dataset for Knowledge-Graph Grounded Evaluation of LLM Hallucinations**|Ernests Lavrinovics et.al.|[2505.14101](http://arxiv.org/abs/2505.14101)|null|
|**2025-05-20**|**Beyond Chains: Bridging Large Language Models and Knowledge Bases in Complex Question Answering**|Yihua Zhu et.al.|[2505.14099](http://arxiv.org/abs/2505.14099)|null|
|**2025-05-20**|**Process vs. Outcome Reward: Which is Better for Agentic RAG Reinforcement Learning**|Wenlin Zhang et.al.|[2505.14069](http://arxiv.org/abs/2505.14069)|null|
|**2025-05-20**|**Divide by Question, Conquer by Agent: SPLIT-RAG with Question-Driven Graph Partitioning**|Ruiyi Yang et.al.|[2505.13994](http://arxiv.org/abs/2505.13994)|null|
|**2025-05-19**|**OPA-Pack: Object-Property-Aware Robotic Bin Packing**|Jia-Hui Pan et.al.|[2505.13339](http://arxiv.org/abs/2505.13339)|null|
|**2025-05-19**|**Effective and Transparent RAG: Adaptive-Reward Reinforcement Learning for Decision Traceability**|Jingyi Ren et.al.|[2505.13258](http://arxiv.org/abs/2505.13258)|null|
|**2025-05-19**|**Agentic Publications: An LLM-Driven Framework for Interactive Scientific Publishing, Supplementing Traditional Papers with AI-Powered Knowledge Systems**|Roberto Pugliese et.al.|[2505.13246](http://arxiv.org/abs/2505.13246)|null|
|**2025-05-19**|**A Case Study of Cross-Lingual Zero-Shot Generalization for Classical Languages in LLMs**|V. S. D. S. Mahesh Akavarapu et.al.|[2505.13173](http://arxiv.org/abs/2505.13173)|**[link](https://github.com/mahesh-ak/SktQA)**|
|**2025-05-19**|**Optimizing Retrieval Augmented Generation for Object Constraint Language**|Kevin Chenhao Li et.al.|[2505.13129](http://arxiv.org/abs/2505.13129)|null|
|**2025-05-19**|**Evaluating the Performance of RAG Methods for Conversational AI in the Airport Domain**|Yuyang Li et.al.|[2505.13006](http://arxiv.org/abs/2505.13006)|null|
|**2025-05-19**|**TinyAlign: Boosting Lightweight Vision-Language Models by Mitigating Modal Alignment Bottlenecks**|Yuanze Hu et.al.|[2505.12884](http://arxiv.org/abs/2505.12884)|null|
|**2025-05-19**|**Re-identification of De-identified Documents with Autoregressive Infilling**|Lucas Georges Gabriel Charpentier et.al.|[2505.12859](http://arxiv.org/abs/2505.12859)|null|
|**2025-05-19**|**PsyMem: Fine-grained psychological alignment and Explicit Memory Control for Advanced Role-Playing LLMs**|Xilong Cheng et.al.|[2505.12814](http://arxiv.org/abs/2505.12814)|null|
|**2025-05-19**|**Accelerating Adaptive Retrieval Augmented Generation via Instruction-Driven Representation Reduction of Retrieval Overlaps**|Jie Ou et.al.|[2505.12731](http://arxiv.org/abs/2505.12731)|null|
|**2025-05-16**|**Semantic Caching of Contextual Summaries for Efficient Question-Answering with Language Models**|Camille Couturier et.al.|[2505.11271](http://arxiv.org/abs/2505.11271)|null|
|**2025-05-16**|**mmRAG: A Modular Benchmark for Retrieval-Augmented Generation over Text, Tables, and Knowledge Graphs**|Chuan Xu et.al.|[2505.11180](http://arxiv.org/abs/2505.11180)|**[link](https://github.com/nju-websoft/mmrag)**|
|**2025-05-16**|**RAGSynth: Synthetic Data for Robust and Faithful RAG Component Optimization**|Haiyang Shen et.al.|[2505.10989](http://arxiv.org/abs/2505.10989)|**[link](https://github.com/eachsheep/ragsynth)**|
|**2025-05-16**|**SubGCache: Accelerating Graph-based RAG with Subgraph-level KV Cache**|Qiuyu Zhu et.al.|[2505.10951](http://arxiv.org/abs/2505.10951)|null|
|**2025-05-16**|**Explain What You Mean: Intent Augmented Knowledge Graph Recommender Built With LLM**|Wenqing Zheng et.al.|[2505.10900](http://arxiv.org/abs/2505.10900)|null|
|**2025-05-16**|**Enhancing Low-Resource Minority Language Translation with LLMs and Retrieval-Augmented Generation for Cultural Nuances**|Chen-Chi Chang et.al.|[2505.10829](http://arxiv.org/abs/2505.10829)|null|
|**2025-05-19**|**Finetune-RAG: Fine-Tuning Language Models to Resist Hallucination in Retrieval-Augmented Generation**|Zhan Peng Lee et.al.|[2505.10792](http://arxiv.org/abs/2505.10792)|**[link](https://github.com/Pints-AI/Finetune-Bench-RAG)**|
|**2025-05-15**|**MMLongBench: Benchmarking Long-Context Vision-Language Models Effectively and Thoroughly**|Zhaowei Wang et.al.|[2505.10610](http://arxiv.org/abs/2505.10610)|**[link](https://github.com/edinburghnlp/mmlongbench)**|
|**2025-05-15**|**CL-RAG: Bridging the Gap in Retrieval-Augmented Generation with Curriculum Learning**|Shaohan Wang et.al.|[2505.10493](http://arxiv.org/abs/2505.10493)|null|
|**2025-05-16**|**AI Agents vs. Agentic AI: A Conceptual Taxonomy, Applications and Challenges**|Ranjan Sapkota et.al.|[2505.10468](http://arxiv.org/abs/2505.10468)|null|
|**2025-05-15**|**Hierarchical Document Refinement for Long-context Retrieval-augmented Generation**|Jiajie Jin et.al.|[2505.10413](http://arxiv.org/abs/2505.10413)|**[link](https://github.com/ignorejjj/longrefiner)**|
|**2025-05-15**|**GE-Chat: A Graph Enhanced RAG Framework for Evidential Response Generation of LLMs**|Longchao Da et.al.|[2505.10143](http://arxiv.org/abs/2505.10143)|null|
|**2025-05-15**|**XRAG: Cross-lingual Retrieval-Augmented Generation**|Wei Liu et.al.|[2505.10089](http://arxiv.org/abs/2505.10089)|null|
|**2025-05-16**|**Leveraging Graph Retrieval-Augmented Generation to Support Learners' Understanding of Knowledge Concepts in MOOCs**|Mohamed Abdelmagied et.al.|[2505.10074](http://arxiv.org/abs/2505.10074)|null|
|**2025-05-15**|**CAFE: Retrieval Head-based Coarse-to-Fine Information Seeking to Enhance Multi-Document QA Capability**|Han Peng et.al.|[2505.10063](http://arxiv.org/abs/2505.10063)|null|
|**2025-05-15**|**Personalizing Large Language Models using Retrieval Augmented Generation and Knowledge Graph**|Deeksha Prahlad et.al.|[2505.09945](http://arxiv.org/abs/2505.09945)|**[link](https://github.com/asu-kim/personal-llm-kg)**|
|**2025-05-14**|**Do Large Language Models Know Conflict? Investigating Parametric vs. Non-Parametric Knowledge of LLMs for Conflict Forecasting**|Apollinaire Poli Nemkova et.al.|[2505.09852](http://arxiv.org/abs/2505.09852)|null|
|**2025-05-14**|**A Multimodal Multi-Agent Framework for Radiology Report Generation**|Ziruo Yi et.al.|[2505.09787](http://arxiv.org/abs/2505.09787)|null|
|**2025-05-14**|**CXMArena: Unified Dataset to benchmark performance in realistic CXM Scenarios**|Raghav Garg et.al.|[2505.09436](http://arxiv.org/abs/2505.09436)|**[link](https://github.com/kapilsprinklr/cxmarena)**|
|**2025-05-14**|**RAG-Enabled Intent Reasoning for Application-Network Interaction**|Salwa Mostafa et.al.|[2505.09339](http://arxiv.org/abs/2505.09339)|**[link](https://github.com/SalwaMostafa/RAG-Enabled-Intent-Reasoning-for-Application-Network-Interaction)**|
|**2025-05-14**|**Scent of Knowledge: Optimizing Search-Enhanced Reasoning with Information Foraging**|Hongjin Qian et.al.|[2505.09316](http://arxiv.org/abs/2505.09316)|null|
|**2025-05-13**|**Improving the Reliability of LLMs: Combining CoT, RAG, Self-Consistency, and Self-Verification**|Adarsh Kumar et.al.|[2505.09031](http://arxiv.org/abs/2505.09031)|null|
|**2025-05-13**|**Securing RAG: A Risk Assessment and Mitigation Framework**|Lukas Ammann et.al.|[2505.08728](http://arxiv.org/abs/2505.08728)|null|
|**2025-05-13**|**Adaptive Schema-aware Event Extraction with Retrieval-Augmented Generation**|Sheng Liang et.al.|[2505.08690](http://arxiv.org/abs/2505.08690)|null|
|**2025-05-13**|**Scaling Context, Not Parameters: Training a Compact 7B Language Model for Efficient Long-Context Processing**|Chen Wu et.al.|[2505.08651](http://arxiv.org/abs/2505.08651)|null|
|**2025-05-13**|**WixQA: A Multi-Dataset Benchmark for Enterprise Retrieval-Augmented Generation**|Dvir Cohen et.al.|[2505.08643](http://arxiv.org/abs/2505.08643)|null|
|**2025-05-13**|**Enhancing Thyroid Cytology Diagnosis with RAG-Optimized LLMs and Pa-thology Foundation Models**|Hussien Al-Asi et.al.|[2505.08590](http://arxiv.org/abs/2505.08590)|null|
|**2025-05-13**|**TrialMatchAI: An End-to-End AI-powered Clinical Trial Recommendation System to Streamline Patient-to-Trial Matching**|Majd Abdallah et.al.|[2505.08508](http://arxiv.org/abs/2505.08508)|null|
|**2025-05-13**|**IterKey: Iterative Keyword Generation with LLMs for Enhanced Retrieval Augmented Generation**|Kazuki Hayashi et.al.|[2505.08450](http://arxiv.org/abs/2505.08450)|null|
|**2025-05-13**|**Optimizing Retrieval-Augmented Generation: Analysis of Hyperparameter Impact on Performance and Efficiency**|Adel Ammar et.al.|[2505.08445](http://arxiv.org/abs/2505.08445)|null|
|**2025-05-14**|**Hakim: Farsi Text Embedding Model**|Mehran Sarmadi et.al.|[2505.08435](http://arxiv.org/abs/2505.08435)|null|
|**2025-05-13**|**Enhancing Cache-Augmented Generation (CAG) with Adaptive Contextual Compression for Scalable Knowledge Integration**|Rishabh Agrawal et.al.|[2505.08261](http://arxiv.org/abs/2505.08261)|null|
|**2025-05-13**|**OnPrem.LLM: A Privacy-Conscious Document Intelligence Toolkit**|Arun S. Maiya et.al.|[2505.07672](http://arxiv.org/abs/2505.07672)|**[link](https://github.com/amaiya/onprem)**|
|**2025-05-12**|**Benchmarking Retrieval-Augmented Generation for Chemistry**|Xianrui Zhong et.al.|[2505.07671](http://arxiv.org/abs/2505.07671)|null|
|**2025-05-12**|**Chronocept: Instilling a Sense of Time in Machines**|Krish Goel et.al.|[2505.07637](http://arxiv.org/abs/2505.07637)|**[link](https://github.com/krishgoel/chronocept-baseline-models)**|
|**2025-05-12**|**KAQG: A Knowledge-Graph-Enhanced RAG for Difficulty-Controlled Question Generation**|Ching Han Chen et.al.|[2505.07618](http://arxiv.org/abs/2505.07618)|null|
|**2025-05-12**|**Reinforced Internal-External Knowledge Synergistic Reasoning for Efficient Adaptive Search Agent**|Ziyang Huang et.al.|[2505.07596](http://arxiv.org/abs/2505.07596)|null|
|**2025-05-12**|**Towards Requirements Engineering for RAG Systems**|Tor Sporsem et.al.|[2505.07553](http://arxiv.org/abs/2505.07553)|null|
|**2025-05-12**|**GRADA: Graph-based Reranker against Adversarial Documents Attack**|Jingjie Zheng et.al.|[2505.07546](http://arxiv.org/abs/2505.07546)|**[link](https://github.com/agrzheng/GRADA)**|
|**2025-05-12**|**SEReDeEP: Hallucination Detection in Retrieval-Augmented Models via Semantic Entropy and Context-Parameter Fusion**|Lei Wang et.al.|[2505.07528](http://arxiv.org/abs/2505.07528)|null|
|**2025-05-12**|**Why Uncertainty Estimation Methods Fall Short in RAG: An Axiomatic Analysis**|Heydar Soudani et.al.|[2505.07459](http://arxiv.org/abs/2505.07459)|null|
|**2025-05-12**|**DynamicRAG: Leveraging Outputs of Large Language Model as Feedback for Dynamic Reranking in Retrieval-Augmented Generation**|Jiashuo Sun et.al.|[2505.07233](http://arxiv.org/abs/2505.07233)|**[link](https://github.com/gasolsun36/dynamicrag)**|
|**2025-05-09**|**Query-driven Document-level Scientific Evidence Extraction from Biomedical Studies**|Massimiliano Pronesti et.al.|[2505.06186](http://arxiv.org/abs/2505.06186)|null|
|**2025-05-09**|**ArtRAG: Retrieval-Augmented Generation with Structured Context for Visual Art Understanding**|Shuai Wang et.al.|[2505.06020](http://arxiv.org/abs/2505.06020)|null|
|**2025-05-09**|**NeoQA: Evidence-based Question Answering with Generated News Events**|Max Glockner et.al.|[2505.05949](http://arxiv.org/abs/2505.05949)|**[link](https://github.com/amazon-science/neoqa)**|
|**2025-05-09**|**Multimodal Integrated Knowledge Transfer to Large Language Models through Preference Optimization with Biomedical Applications**|Da Wu et.al.|[2505.05736](http://arxiv.org/abs/2505.05736)|**[link](https://github.com/wglab/mint-llm)**|
|**2025-05-08**|**Lost in OCR Translation? Vision-Based Approaches to Robust Document Retrieval**|Alexander Most et.al.|[2505.05666](http://arxiv.org/abs/2505.05666)|null|
|**2025-05-08**|**VR-RAG: Open-vocabulary Species Recognition with RAG-Assisted Large Multi-Modal Models**|Faizan Farooq Khan et.al.|[2505.05635](http://arxiv.org/abs/2505.05635)|null|
|**2025-05-08**|**KG-HTC: Integrating Knowledge Graphs into LLMs for Effective Zero-shot Hierarchical Text Classification**|Qianbo Zang et.al.|[2505.05583](http://arxiv.org/abs/2505.05583)|**[link](https://github.com/qianbozang/kg-htc)**|
|**2025-05-08**|**QualBench: Benchmarking Chinese LLMs with Localized Professional Qualifications for Vertical Domain Evaluation**|Mengze Hong et.al.|[2505.05225](http://arxiv.org/abs/2505.05225)|null|
|**2025-05-08**|**Stealthy LLM-Driven Data Poisoning Attacks Against Embedding-Based Retrieval-Augmented Recommender Systems**|Fatemeh Nazary et.al.|[2505.05196](http://arxiv.org/abs/2505.05196)|null|
|**2025-05-08**|**Towards Mitigating API Hallucination in Code Generated by LLMs with Hierarchical Dependency Aware**|Yujia Chen et.al.|[2505.05057](http://arxiv.org/abs/2505.05057)|**[link](https://github.com/yujiachen99/apimitigation)**|
|**2025-05-08**|**LSRP: A Leader-Subordinate Retrieval Framework for Privacy-Preserving Cloud-Device Collaboration**|Yingyi Zhang et.al.|[2505.05031](http://arxiv.org/abs/2505.05031)|**[link](https://github.com/zhang-yingyi/lsrp)**|
|**2025-05-08**|**An Open-Source Dual-Loss Embedding Model for Semantic Retrieval in Higher Education**|Ramteja Sajja et.al.|[2505.04916](http://arxiv.org/abs/2505.04916)|null|
|**2025-05-08**|**From First Draft to Final Insight: A Multi-Agent Approach for Feedback Generation**|Jie Cao et.al.|[2505.04869](http://arxiv.org/abs/2505.04869)|null|
|**2025-05-07**|**Benchmarking LLM Faithfulness in RAG with Evolving Leaderboards**|Manveer Singh Tamber et.al.|[2505.04847](http://arxiv.org/abs/2505.04847)|null|
|**2025-05-07**|**HiPerRAG: High-Performance Retrieval Augmented Generation for Scientific Insights**|Ozan Gokdemir et.al.|[2505.04846](http://arxiv.org/abs/2505.04846)|null|
|**2025-05-07**|**Osiris: A Lightweight Open-Source Hallucination Detection System**|Alex Shan et.al.|[2505.04844](http://arxiv.org/abs/2505.04844)|null|
|**2025-05-07**|**A Proposal for Evaluating the Operational Risk for ChatBots based on Large Language Models**|Pedro Pinacho-Davidson et.al.|[2505.04784](http://arxiv.org/abs/2505.04784)|null|
|**2025-05-07**|**The Aloe Family Recipe for Open and Specialized Healthcare LLMs**|Dario Garcia-Gasulla et.al.|[2505.04388](http://arxiv.org/abs/2505.04388)|null|
|**2025-05-07**|**CDE-Mapper: Using Retrieval-Augmented Language Models for Linking Clinical Data Elements to Controlled Vocabularies**|Komal Gilani et.al.|[2505.04365](http://arxiv.org/abs/2505.04365)|null|
|**2025-05-07**|**LLM-Independent Adaptive RAG: Let the Question Speak for Itself**|Maria Marina et.al.|[2505.04253](http://arxiv.org/abs/2505.04253)|null|
|**2025-05-07**|**AutoPatch: Multi-Agent Framework for Patching Real-World CVE Vulnerabilities**|Minjae Seo et.al.|[2505.04195](http://arxiv.org/abs/2505.04195)|**[link](https://github.com/ai-llm-research/autopatch)**|
|**2025-05-07**|**DOTA: Deformable Optimized Transformer Architecture for End-to-End Text Recognition with Retrieval-Augmented Generation**|Naphat Nithisopa et.al.|[2505.04175](http://arxiv.org/abs/2505.04175)|null|
|**2025-05-07**|**Shadow Wireless Intelligence: Large Language Model-Driven Reasoning in Covert Communications**|Yuanai Xie et.al.|[2505.04068](http://arxiv.org/abs/2505.04068)|null|
|**2025-05-06**|**A Reasoning-Focused Legal Retrieval Benchmark**|Lucia Zheng et.al.|[2505.03970](http://arxiv.org/abs/2505.03970)|null|
|**2025-05-06**|**A Comprehensive Survey of Large AI Models for Future Communications: Foundations, Applications and Challenges**|Feibo Jiang et.al.|[2505.03556](http://arxiv.org/abs/2505.03556)|**[link](https://github.com/jiangfeibo/comlam)**|
|**2025-05-06**|**An Analysis of Hyper-Parameter Optimization Methods for Retrieval Augmented Generation**|Matan Orbach et.al.|[2505.03452](http://arxiv.org/abs/2505.03452)|null|
|**2025-05-06**|**Lightweight Clinical Decision Support System using QLoRA-Fine-Tuned LLMs and Retrieval-Augmented Generation**|Mohammad Shoaib Ansari et.al.|[2505.03406](http://arxiv.org/abs/2505.03406)|null|
|**2025-05-06**|**Capability-Driven Skill Generation with LLMs: A RAG-Based Approach for Reusing Existing Libraries and Interfaces**|Luis Miguel Vieira da Silva et.al.|[2505.03295](http://arxiv.org/abs/2505.03295)|null|
|**2025-05-06**|**RAG-MCP: Mitigating Prompt Bloat in LLM Tool Selection via Retrieval-Augmented Generation**|Tiantian Gan et.al.|[2505.03275](http://arxiv.org/abs/2505.03275)|null|
|**2025-05-05**|**Direct Retrieval-augmented Optimization: Synergizing Knowledge Selection and Language Models**|Zhengliang Shi et.al.|[2505.03075](http://arxiv.org/abs/2505.03075)|**[link](https://github.com/mangopy/direct-rag-learning)**|
|**2025-05-05**|**Knowing You Don't Know: Learning When to Continue Search in Multi-round RAG through Self-Practicing**|Diji Yang et.al.|[2505.02811](http://arxiv.org/abs/2505.02811)|**[link](https://github.com/ucscirkm/sim-rag)**|
|**2025-05-05**|**SymbioticRAG: Enhancing Document Intelligence Through Human-LLM Symbiotic Collaboration**|Qiang Sun et.al.|[2505.02418](http://arxiv.org/abs/2505.02418)|null|
|**2025-05-05**|**From Course to Skill: Evaluating LLM Performance in Curricular Analytics**|Zhen Xu et.al.|[2505.02324](http://arxiv.org/abs/2505.02324)|**[link](https://github.com/aequitas-lab/evaluation-of-llm-in-ca-aied-2025)**|
|**2025-05-05**|**Generative Sign-description Prompts with Multi-positive Contrastive Learning for Sign Language Recognition**|Siyu Liang et.al.|[2505.02304](http://arxiv.org/abs/2505.02304)|null|
|**2025-05-04**|**Real-time Spatial Retrieval Augmented Generation for Urban Environments**|David Nazareno Campo et.al.|[2505.02271](http://arxiv.org/abs/2505.02271)|null|
|**2025-05-04**|**A New HOPE: Domain-agnostic Automatic Evaluation of Text Chunking**|Henrik Brådland et.al.|[2505.02171](http://arxiv.org/abs/2505.02171)|null|
|**2025-05-04**|**Incorporating Legal Structure in Retrieval-Augmented Generation: A Case Study on Copyright Fair Use**|Justin Ho et.al.|[2505.02164](http://arxiv.org/abs/2505.02164)|**[link](https://github.com/justinhjy1004/fairuselegalbot)**|
|**2025-05-04**|**Enhancing LLM Code Generation: A Systematic Evaluation of Multi-Agent Collaboration and Runtime Debugging for Improved Accuracy, Reliability, and Latency**|Nazmus Ashrafi et.al.|[2505.02133](http://arxiv.org/abs/2505.02133)|**[link](https://github.com/nazmus-ashrafi/multiagent_vs_debugger)**|
|**2025-05-04**|**Retrieval-augmented in-context learning for multimodal large language models in disease classification**|Zaifu Zhan et.al.|[2505.02087](http://arxiv.org/abs/2505.02087)|null|
|**2025-05-03**|**Harnessing the Power of LLMs, Informers and Decision Transformers for Intent-driven RAN Management in 6G**|Md Arafat Habib et.al.|[2505.01841](http://arxiv.org/abs/2505.01841)|null|
|**2025-05-02**|**Document Retrieval Augmented Fine-Tuning (DRAFT) for safety-critical software assessments**|Regan Bolton et.al.|[2505.01307](http://arxiv.org/abs/2505.01307)|null|
|**2025-05-02**|**CaGR-RAG: Context-aware Query Grouping for Disk-based Vector Search in RAG Systems**|Yeonwoo Jeong et.al.|[2505.01164](http://arxiv.org/abs/2505.01164)|null|
|**2025-05-02**|**Retrieval-Augmented Generation in Biomedicine: A Survey of Technologies, Datasets, and Clinical Applications**|Jiawei He et.al.|[2505.01146](http://arxiv.org/abs/2505.01146)|null|
|**2025-05-02**|**Retrieval Augmented Learning: A Retrial-based Large Language Model Self-Supervised Learning and Autonomous Knowledge Generation**|Zongyuan Li et.al.|[2505.01073](http://arxiv.org/abs/2505.01073)|null|
|**2025-05-01**|**HalluMix: A Task-Agnostic, Multi-Domain Benchmark for Real-World Hallucination Detection**|Deanna Emery et.al.|[2505.00506](http://arxiv.org/abs/2505.00506)|null|
|**2025-05-01**|**Distributed Retrieval-Augmented Generation**|Chenhao Xu et.al.|[2505.00443](http://arxiv.org/abs/2505.00443)|**[link](https://github.com/xuchenhao001/drag)**|
|**2025-05-01**|**EnronQA: Towards Personalized RAG over Private Documents**|Michael J. Ryan et.al.|[2505.00263](http://arxiv.org/abs/2505.00263)|null|
|**2025-05-02**|**Empowering Agentic Video Analytics Systems with Video Language Models**|Yuxuan Yan et.al.|[2505.00254](http://arxiv.org/abs/2505.00254)|null|
|**2025-04-30**|**Optimization of embeddings storage for RAG systems using quantization and dimensionality reduction techniques**|Naamán Huerga-Pérez et.al.|[2505.00105](http://arxiv.org/abs/2505.00105)|null|
|**2025-04-30**|**LLM-Empowered Embodied Agent for Memory-Augmented Task Planning in Household Robotics**|Marc Glocker et.al.|[2504.21716](http://arxiv.org/abs/2504.21716)|**[link](https://github.com/marc1198/chat-hsr)**|
|**2025-04-30**|**Hoist with His Own Petard: Inducing Guardrails to Facilitate Denial-of-Service Attacks on Retrieval-Augmented Generation of LLMs**|Pan Suo et.al.|[2504.21680](http://arxiv.org/abs/2504.21680)|null|
|**2025-04-30**|**Traceback of Poisoning Attacks to Retrieval-Augmented Generation**|Baolei Zhang et.al.|[2504.21668](http://arxiv.org/abs/2504.21668)|null|
|**2025-04-30**|**Homa at SemEval-2025 Task 5: Aligning Librarian Records with OntoAligner for Subject Tagging**|Hadi Bayrami Asl Tekanlou et.al.|[2504.21474](http://arxiv.org/abs/2504.21474)|null|
|**2025-04-30**|**Talk Before You Retrieve: Agent-Led Discussions for Better RAG in Medical QA**|Xuanzhao Dong et.al.|[2504.21252](http://arxiv.org/abs/2504.21252)|**[link](https://github.com/llm-vlm-gsl/discuss-rag)**|
|**2025-04-30**|**Memorization and Knowledge Injection in Gated LLMs**|Xu Pan et.al.|[2504.21239](http://arxiv.org/abs/2504.21239)|null|
|**2025-04-29**|**Detecting Manipulated Contents Using Knowledge-Grounded Inference**|Mark Huasong Meng et.al.|[2504.21165](http://arxiv.org/abs/2504.21165)|**[link](https://github.com/cyberooo/manicod)**|
|**2025-04-29**|**CBM-RAG: Demonstrating Enhanced Interpretability in Radiology Report Generation with Multi-Agent RAG and Concept Bottleneck Models**|Hasan Md Tusfiqur Alam et.al.|[2504.20898](http://arxiv.org/abs/2504.20898)|**[link](https://github.com/tifat58/enhanced-interpretable-report-generation-demo)**|
|**2025-04-29**|**UniversalRAG: Retrieval-Augmented Generation over Multiple Corpora with Diverse Modalities and Granularities**|Woongyeong Yeo et.al.|[2504.20734](http://arxiv.org/abs/2504.20734)|**[link](https://github.com/wgcyeo/UniversalRAG)**|
|**2025-04-29**|**ComplexVCoder: An LLM-Driven Framework for Systematic Generation of Complex Verilog Code**|Jian Zuo et.al.|[2504.20653](http://arxiv.org/abs/2504.20653)|null|
|**2025-04-29**|**Information Retrieval in the Age of Generative AI: The RGB Model**|Michele Garetto et.al.|[2504.20610](http://arxiv.org/abs/2504.20610)|**[link](https://github.com/franco-galante/rgb-model)**|
|**2025-04-29**|**ReasonIR: Training Retrievers for Reasoning Tasks**|Rulin Shao et.al.|[2504.20595](http://arxiv.org/abs/2504.20595)|**[link](https://github.com/facebookresearch/reasonir)**|
|**2025-04-29**|**ARCS: Agentic Retrieval-Augmented Code Synthesis with Iterative Refinement**|Manish Bhattarai et.al.|[2504.20434](http://arxiv.org/abs/2504.20434)|null|
|**2025-04-29**|**AKIBoards: A Structure-Following Multiagent System for Predicting Acute Kidney Injury**|David Gordon et.al.|[2504.20368](http://arxiv.org/abs/2504.20368)|null|
|**2025-04-28**|**Can LLMs Be Trusted for Evaluating RAG Systems? A Survey of Methods and Datasets**|Lorenz Brehme et.al.|[2504.20119](http://arxiv.org/abs/2504.20119)|null|
|**2025-04-28**|**Chatbot Arena Meets Nuggets: Towards Explanations and Diagnostics in the Evaluation of LLM Responses**|Sahel Sharifymoghaddam et.al.|[2504.20006](http://arxiv.org/abs/2504.20006)|null|
|**2025-04-28**|**Reconstructing Context: Evaluating Advanced Chunking Strategies for Retrieval-Augmented Generation**|Carlo Merola et.al.|[2504.19754](http://arxiv.org/abs/2504.19754)|**[link](https://github.com/disi-unibo-nlp/rag-when-how-chunk)**|
|**2025-04-28**|**Context-Guided Dynamic Retrieval for Improving Generation Quality in RAG Models**|Jacky He et.al.|[2504.19436](http://arxiv.org/abs/2504.19436)|null|
|**2025-04-28**|**Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory**|Prateek Chhikara et.al.|[2504.19413](http://arxiv.org/abs/2504.19413)|null|
|**2025-04-27**|**Privacy-Preserving Federated Embedding Learning for Localized Retrieval-Augmented Generation**|Qianren Mao et.al.|[2504.19101](http://arxiv.org/abs/2504.19101)|null|
|**2025-04-26**|**MTCSC: Retrieval-Augmented Iterative Refinement for Chinese Spelling Correction**|Junhong Liang et.al.|[2504.18938](http://arxiv.org/abs/2504.18938)|null|
|**2025-04-26**|**Building Scalable AI-Powered Applications with Cloud Databases: Architectures, Best Practices and Performance Considerations**|Santosh Bhupathi et.al.|[2504.18793](http://arxiv.org/abs/2504.18793)|null|
|**2025-04-25**|**LLMpatronous: Harnessing the Power of LLMs For Vulnerability Detection**|Rajesh Yarra et.al.|[2504.18423](http://arxiv.org/abs/2504.18423)|null|
|**2025-04-25**|**ThreMoLIA: Threat Modeling of Large Language Model-Integrated Applications**|Felix Viktor Jedrzejewski et.al.|[2504.18369](http://arxiv.org/abs/2504.18369)|null|
|**2025-04-25**|**Even Small Reasoners Should Quote Their Sources: Introducing the Pleias-RAG Model Family**|Pierre-Carl Langlais et.al.|[2504.18225](http://arxiv.org/abs/2504.18225)|null|
|**2025-04-25**|**Automating Function-Level TARA for Automotive Full-Lifecycle Security**|Yuqiao Yang et.al.|[2504.18083](http://arxiv.org/abs/2504.18083)|null|
|**2025-04-25**|**PropRAG: Guiding Retrieval with Beam Search over Proposition Paths**|Jingjin Wang et.al.|[2504.18070](http://arxiv.org/abs/2504.18070)|null|
|**2025-04-25**|**RAG LLMs are Not Safer: A Safety Analysis of Retrieval-Augmented Generation for Large Language Models**|Bang An et.al.|[2504.18041](http://arxiv.org/abs/2504.18041)|null|
|**2025-04-25**|**SMARTFinRAG: Interactive Modularized Financial RAG Benchmark**|Yiwei Zha et.al.|[2504.18024](http://arxiv.org/abs/2504.18024)|**[link](https://github.com/jonathanzha47/smartfinrag)**|
|**2025-04-25**|**Self-Balancing, Memory Efficient, Dynamic Metric Space Data Maintenance, for Rapid Multi-Kernel Estimation**|Aditya S Ellendula et.al.|[2504.18003](http://arxiv.org/abs/2504.18003)|null|
|**2025-04-24**|**A Comprehensive Survey of Knowledge-Based Vision Question Answering Systems: The Lifecycle of Knowledge in Visual Reasoning Task**|Jiaqi Deng et.al.|[2504.17547](http://arxiv.org/abs/2504.17547)|null|
|**2025-04-24**|**A RAG-Based Multi-Agent LLM System for Natural Hazard Resilience and Adaptation**|Yangxinyu Xie et.al.|[2504.17200](http://arxiv.org/abs/2504.17200)|null|
|**2025-04-23**|**MIRAGE: A Metric-Intensive Benchmark for Retrieval-Augmented Generation Evaluation**|Chanhee Park et.al.|[2504.17137](http://arxiv.org/abs/2504.17137)|null|
|**2025-04-23**|**Enhancing Critical Thinking with AI: A Tailored Warning System for RAG Models**|Xuyang Zhu et.al.|[2504.16883](http://arxiv.org/abs/2504.16883)|null|
|**2025-04-23**|**LLM-assisted Graph-RAG Information Extraction from IFC Data**|Sima Iranmanesh et.al.|[2504.16813](http://arxiv.org/abs/2504.16813)|null|
|**2025-04-23**|**Credible plan-driven RAG method for Multi-hop Question Answering**|Ningning Zhang et.al.|[2504.16787](http://arxiv.org/abs/2504.16787)|null|
|**2025-04-23**|**Detecting and Understanding Hateful Contents in Memes Through Captioning and Visual Question-Answering**|Ali Anaissi et.al.|[2504.16723](http://arxiv.org/abs/2504.16723)|null|
|**2025-04-23**|**DTVM: Revolutionizing Smart Contract Execution with Determinism and Compatibility**|Wei Zhou et.al.|[2504.16552](http://arxiv.org/abs/2504.16552)|null|
|**2025-04-24**|**Synergizing RAG and Reasoning: A Systematic Review**|Yunfan Gao et.al.|[2504.15909](http://arxiv.org/abs/2504.15909)|null|
|**2025-04-23**|**FinDER: Financial Dataset for Question Answering and Evaluating Retrieval-Augmented Generation**|Chanyeol Choi et.al.|[2504.15800](http://arxiv.org/abs/2504.15800)|null|
|**2025-04-22**|**Grounded in Context: Retrieval-Based Method for Hallucination Detection**|Assaf Gerner et.al.|[2504.15771](http://arxiv.org/abs/2504.15771)|null|
|**2025-04-22**|**The Viability of Crowdsourcing for RAG Evaluation**|Lukas Gienapp et.al.|[2504.15689](http://arxiv.org/abs/2504.15689)|null|
|**2025-04-22**|**CiteFix: Enhancing RAG Accuracy Through Post-Processing Citation Correction**|Harsh Maheshwari et.al.|[2504.15629](http://arxiv.org/abs/2504.15629)|null|
|**2025-04-23**|**A LoRA-Based Approach to Fine-Tuning LLMs for Educational Guidance in Resource-Constrained Settings**|Md Millat Hosen et.al.|[2504.15610](http://arxiv.org/abs/2504.15610)|**[link](https://github.com/codermillat/StudyAbroadGPT)**|
|**2025-04-21**|**TVR: Automotive System Requirement Traceability Validation and Recovery Through Retrieval-Augmented Generation**|Feifei Niu et.al.|[2504.15427](http://arxiv.org/abs/2504.15427)|null|
|**2025-04-21**|**Support Evaluation for the TREC 2024 RAG Track: Comparing Human versus LLM Judges**|Nandan Thakur et.al.|[2504.15205](http://arxiv.org/abs/2504.15205)|null|
|**2025-04-21**|**The Great Nugget Recall: Automating Fact Extraction and RAG Evaluation with Large Language Models**|Ronak Pradeep et.al.|[2504.15068](http://arxiv.org/abs/2504.15068)|null|
|**2025-04-21**|**LLMs as Data Annotators: How Close Are We to Human Performance**|Muhammad Uzair Ul Haq et.al.|[2504.15022](http://arxiv.org/abs/2504.15022)|null|
|**2025-04-21**|**Efficient Document Retrieval with G-Retriever**|Manthankumar Solanki et.al.|[2504.14955](http://arxiv.org/abs/2504.14955)|**[link](https://github.com/manthan2305/Efficient-G-Retriever)**|
|**2025-04-22**|**WindVE: Collaborative CPU-NPU Vector Embedding**|Jinqi Huang et.al.|[2504.14941](http://arxiv.org/abs/2504.14941)|null|
|**2025-04-21**|**POLYRAG: Integrating Polyviews into Retrieval-Augmented Generation for Medical Applications**|Chunjing Gan et.al.|[2504.14917](http://arxiv.org/abs/2504.14917)|null|
|**2025-04-21**|**Retrieval Augmented Generation Evaluation in the Era of Large Language Models: A Comprehensive Survey**|Aoran Gan et.al.|[2504.14891](http://arxiv.org/abs/2504.14891)|null|
|**2025-04-21**|**AlignRAG: An Adaptable Framework for Resolving Misalignments in Retrieval-Aware Reasoning of RAG**|Jiaqi Wei et.al.|[2504.14858](http://arxiv.org/abs/2504.14858)|**[link](https://github.com/qqw-ing/rag-reasonalignment)**|
|**2025-04-21**|**Transparentize the Internal and External Knowledge Utilization in LLMs with Trustworthy Citation**|Jiajun Shen et.al.|[2504.14856](http://arxiv.org/abs/2504.14856)|null|
|**2025-04-20**|**Towards Optimal Circuit Generation: Multi-Agent Collaboration Meets Collective Intelligence**|Haiyan Qin et.al.|[2504.14625](http://arxiv.org/abs/2504.14625)|**[link](https://github.com/buaa-clab/circuitmind)**|
|**2025-04-18**|**Detecting Malicious Source Code in PyPI Packages with LLMs: Does RAG Come in Handy?**|Motunrayo Ibiyo et.al.|[2504.13769](http://arxiv.org/abs/2504.13769)|null|
|**2025-04-18**|**RAG Without the Lag: Interactive Debugging for Retrieval-Augmented Generation Pipelines**|Quentin Romero Lauro et.al.|[2504.13587](http://arxiv.org/abs/2504.13587)|null|
|**2025-04-18**|**CoT-RAG: Integrating Chain of Thought and Retrieval-Augmented Generation to Enhance Reasoning in Large Language Models**|Feiyang Li et.al.|[2504.13534](http://arxiv.org/abs/2504.13534)|null|
|**2025-04-18**|**Secure Multifaceted-RAG for Enterprise: Hybrid Knowledge Retrieval with Security Filtering**|Grace Byun et.al.|[2504.13425](http://arxiv.org/abs/2504.13425)|null|
|**2025-04-17**|**FreshStack: Building Realistic Benchmarks for Evaluating Retrieval on Technical Documents**|Nandan Thakur et.al.|[2504.13128](http://arxiv.org/abs/2504.13128)|null|
|**2025-04-17**|**Uncertainty-Aware Trajectory Prediction via Rule-Regularized Heteroscedastic Deep Classification**|Kumar Manas et.al.|[2504.13111](http://arxiv.org/abs/2504.13111)|null|
|**2025-04-17**|**Retrieval-Augmented Generation with Conflicting Evidence**|Han Wang et.al.|[2504.13079](http://arxiv.org/abs/2504.13079)|**[link](https://github.com/hannight/ramdocs)**|
|**2025-04-17**|**InstructRAG: Leveraging Retrieval-Augmented Generation on Instruction Graphs for LLM-Based Task Planning**|Zheng Wang et.al.|[2504.13032](http://arxiv.org/abs/2504.13032)|null|
|**2025-04-17**|**Accommodate Knowledge Conflicts in Retrieval-augmented LLMs: Towards Reliable Response Generation in the Wild**|Jiatai Wang et.al.|[2504.12982](http://arxiv.org/abs/2504.12982)|null|
|**2025-04-17**|**Estimating Optimal Context Length for Hybrid Retrieval-augmented Multi-document Summarization**|Adithya Pratapa et.al.|[2504.12972](http://arxiv.org/abs/2504.12972)|**[link](https://github.com/adithya7/hybrid-rag)**|
|**2025-04-17**|**Explainable AI in Usable Privacy and Security: Challenges and Opportunities**|Vincent Freiberger et.al.|[2504.12931](http://arxiv.org/abs/2504.12931)|null|
|**2025-04-17**|**Can LLMs reason over extended multilingual contexts? Towards long-context evaluation beyond retrieval and haystacks**|Amey Hengle et.al.|[2504.12845](http://arxiv.org/abs/2504.12845)|**[link](https://github.com/AmeyHengle/multilingual-long-context-reasoning)**|
|**2025-04-17**|**ACoRN: Noise-Robust Abstractive Compression in Retrieval-Augmented Language Models**|Singon Kim et.al.|[2504.12673](http://arxiv.org/abs/2504.12673)|null|
|**2025-04-17**|**CDF-RAG: Causal Dynamic Feedback for Adaptive Retrieval-Augmented Generation**|Elahe Khatibi et.al.|[2504.12560](http://arxiv.org/abs/2504.12560)|**[link](https://github.com/elakhatibi/cdf-rag)**|
|**2025-04-16**|**ARCeR: an Agentic RAG for the Automated Definition of Cyber Ranges**|Matteo Lupinacci et.al.|[2504.12143](http://arxiv.org/abs/2504.12143)|null|
|**2025-04-16**|**A Visual RAG Pipeline for Few-Shot Fine-Grained Product Classification**|Bianca Lamm et.al.|[2504.11838](http://arxiv.org/abs/2504.11838)|null|
|**2025-04-16**|**Shared Disk KV Cache Management for Efficient Multi-Instance Inference in RAG-Powered LLMs**|Hyungwoo Lee et.al.|[2504.11765](http://arxiv.org/abs/2504.11765)|null|
|**2025-04-16**|**A Library of LLM Intrinsics for Retrieval-Augmented Generation**|Marina Danilevsky et.al.|[2504.11704](http://arxiv.org/abs/2504.11704)|null|
|**2025-04-15**|**NodeRAG: Structuring Graph-based RAG with Heterogeneous Nodes**|Tianyang Xu et.al.|[2504.11544](http://arxiv.org/abs/2504.11544)|null|
|**2025-04-15**|**Enhancing Autonomous Driving Systems with On-Board Deployed Large Language Models**|Nicolas Baumann et.al.|[2504.11514](http://arxiv.org/abs/2504.11514)|**[link](https://github.com/ForzaETH/LLMxRobot)**|
|**2025-04-15**|**Towards Automated Safety Requirements Derivation Using Agent-based RAG**|Balahari Vignesh Balu et.al.|[2504.11243](http://arxiv.org/abs/2504.11243)|null|
|**2025-04-16**|**Efficient Distributed Retrieval-Augmented Generation for Enhancing Language Model Performance**|Shangyu Liu et.al.|[2504.11197](http://arxiv.org/abs/2504.11197)|null|
|**2025-04-15**|**ReZero: Enhancing LLM search ability by trying one-more-time**|Alan Dao et.al.|[2504.11001](http://arxiv.org/abs/2504.11001)|null|
|**2025-04-17**|**Exploring the Role of Knowledge Graph-Based RAG in Japanese Medical Question Answering with Small-Scale LLMs**|Yingjian Chen et.al.|[2504.10982](http://arxiv.org/abs/2504.10982)|null|
|**2025-04-15**|**ARise: Towards Knowledge-Augmented Reasoning via Risk-Adaptive Search**|Yize Zhang et.al.|[2504.10893](http://arxiv.org/abs/2504.10893)|null|
|**2025-04-15**|**Ai2 Scholar QA: Organized Literature Synthesis with Attribution**|Amanpreet Singh et.al.|[2504.10861](http://arxiv.org/abs/2504.10861)|**[link](https://github.com/allenai/ai2-scholarqa-lib)**|
|**2025-04-15**|**LayoutCoT: Unleashing the Deep Reasoning Potential of Large Language Models for Layout Generation**|Hengyu Shi et.al.|[2504.10829](http://arxiv.org/abs/2504.10829)|null|
|**2025-04-14**|**Smooth sailing or ragged climb? -- Increasing the robustness of power spectrum de-wiggling and ShapeFit parameter compression**|Katayoon Ghaemi et.al.|[2504.10578](http://arxiv.org/abs/2504.10578)|null|
|**2025-04-14**|**SymRTLO: Enhancing RTL Code Optimization with LLMs and Neuron-Inspired Symbolic Reasoning**|Yiting Wang et.al.|[2504.10369](http://arxiv.org/abs/2504.10369)|null|
|**2025-04-14**|**SlowFastVAD: Video Anomaly Detection via Integrating Simple Detector and RAG-Enhanced Vision-Language Model**|Zongcan Ding et.al.|[2504.10320](http://arxiv.org/abs/2504.10320)|null|
|**2025-04-14**|**AutoStyle-TTS: Retrieval-Augmented Generation based Automatic Style Matching Text-to-Speech Synthesis**|Dan Luo et.al.|[2504.10309](http://arxiv.org/abs/2504.10309)|null|
|**2025-04-14**|**XY-Cut++: Advanced Layout Ordering via Hierarchical Mask Mechanism on a Novel Benchmark**|Shuai Liu et.al.|[2504.10258](http://arxiv.org/abs/2504.10258)|**[link](https://github.com/liushuai35/PaddleXrc)**|
|**2025-04-14**|**GNN-ACLP: Graph Neural Networks based Analog Circuit Link Prediction**|Guanyuan Pan et.al.|[2504.10240](http://arxiv.org/abs/2504.10240)|null|
|**2025-04-14**|**DioR: Adaptive Cognitive Detection and Contextual Retrieval Optimization for Dynamic Retrieval-Augmented Generation**|Hanghui Guo et.al.|[2504.10198](http://arxiv.org/abs/2504.10198)|null|
|**2025-04-14**|**HalluSearch at SemEval-2025 Task 3: A Search-Enhanced RAG Pipeline for Hallucination Detection**|Mohamed A. Abdallah et.al.|[2504.10168](http://arxiv.org/abs/2504.10168)|null|
|**2025-04-14**|**A Survey of Personalization: From RAG to Agent**|Xiaopeng Li et.al.|[2504.10147](http://arxiv.org/abs/2504.10147)|**[link](https://github.com/Applied-Machine-Learning-Lab/Awesome-Personalized-RAG-Agent)**|
|**2025-04-15**|**MMKB-RAG: A Multi-Modal Knowledge-Based Retrieval-Augmented Generation Framework**|Zihan Ling et.al.|[2504.10074](http://arxiv.org/abs/2504.10074)|null|
|**2025-04-14**|**Hallucination Detection in LLMs via Topological Divergence on Attention Graphs**|Alexandra Bazarova et.al.|[2504.10063](http://arxiv.org/abs/2504.10063)|null|
|**2025-04-11**|**TP-RAG: Benchmarking Retrieval-Augmented Large Language Model Agents for Spatiotemporal-Aware Travel Planning**|Hang Ni et.al.|[2504.08694](http://arxiv.org/abs/2504.08694)|null|
|**2025-04-11**|**Adopting Large Language Models to Automated System Integration**|Robin D. Pesl et.al.|[2504.08490](http://arxiv.org/abs/2504.08490)|null|
|**2025-04-11**|**PCA-RAG: Principal Component Analysis for Efficient Retrieval-Augmented Generation**|Arman Khaledian et.al.|[2504.08386](http://arxiv.org/abs/2504.08386)|null|
|**2025-04-11**|**RAG-VR: Leveraging Retrieval-Augmented Generation for 3D Question Answering in VR Environments**|Shiyi Ding et.al.|[2504.08256](http://arxiv.org/abs/2504.08256)|**[link](https://github.com/sding11/RAG-VR)**|
|**2025-04-11**|**Out of Style: RAG's Fragility to Linguistic Variation**|Tianyu Cao et.al.|[2504.08231](http://arxiv.org/abs/2504.08231)|**[link](https://github.com/springcty/rag-fragility-to-linguistic-variation)**|
|**2025-04-11**|**DRAFT-ing Architectural Design Decisions using LLMs**|Rudra Dhar et.al.|[2504.08207](http://arxiv.org/abs/2504.08207)|**[link](https://github.com/sa4s-serc/llm4adr)**|
|**2025-04-10**|**A System for Comprehensive Assessment of RAG Frameworks**|Mattia Rengo et.al.|[2504.07803](http://arxiv.org/abs/2504.07803)|**[link](https://github.com/eustema-s-p-a/scarf)**|
|**2025-04-10**|**Plan-and-Refine: Diverse and Comprehensive Retrieval-Augmented Generation**|Alireza Salemi et.al.|[2504.07794](http://arxiv.org/abs/2504.07794)|**[link](https://github.com/alirezasalemi7/pr-rag)**|
|**2025-04-10**|**Automated Construction of a Knowledge Graph of Nuclear Fusion Energy for Effective Elicitation and Retrieval of Information**|A. Loreti et.al.|[2504.07738](http://arxiv.org/abs/2504.07738)|null|
|**2025-04-10**|**MRD-RAG: Enhancing Medical Diagnosis with Multi-Round Retrieval-Augmented Generation**|Yixiang Chen et.al.|[2504.07724](http://arxiv.org/abs/2504.07724)|**[link](https://github.com/yixiangch/mrd-rag)**|
|**2025-04-10**|**PR-Attack: Coordinated Prompt-RAG Attacks on Retrieval-Augmented Generation in Large Language Models via Bilevel Optimization**|Yang Jiao et.al.|[2504.07717](http://arxiv.org/abs/2504.07717)|null|
|**2025-04-10**|**CollEX -- A Multimodal Agentic RAG System Enabling Interactive Exploration of Scientific Collections**|Florian Schneider et.al.|[2504.07643](http://arxiv.org/abs/2504.07643)|null|
|**2025-04-10**|**ConceptFormer: Towards Efficient Use of Knowledge-Graph Embeddings in Large Language Models**|Joel Barmettler et.al.|[2504.07624](http://arxiv.org/abs/2504.07624)|null|
|**2025-04-10**|**REANIMATOR: Reanimate Retrieval Test Collections with Extracted and Synthetic Resources**|Björn Engelmann et.al.|[2504.07584](http://arxiv.org/abs/2504.07584)|**[link](https://github.com/irgroup/Reanimator)**|
|**2025-04-10**|**LLM4Ranking: An Easy-to-use Framework of Utilizing Large Language Models for Document Reranking**|Qi Liu et.al.|[2504.07439](http://arxiv.org/abs/2504.07439)|**[link](https://github.com/liuqi6777/llm4ranking)**|
|**2025-04-10**|**AgentAda: Skill-Adaptive Data Analytics for Tailored Insight Discovery**|Amirhossein Abaskohi et.al.|[2504.07421](http://arxiv.org/abs/2504.07421)|**[link](https://github.com/servicenow/agentada)**|
|**2025-04-09**|**Evaluating Retrieval Augmented Generative Models for Document Queries in Transportation Safety**|Chad Melton et.al.|[2504.07022](http://arxiv.org/abs/2504.07022)|null|
|**2025-04-09**|**Review of Case-Based Reasoning for LLM Agents: Theoretical Foundations, Architectural Components, and Cognitive Integration**|Kostas Hatalis et.al.|[2504.06943](http://arxiv.org/abs/2504.06943)|null|
|**2025-04-08**|**Don't Let It Hallucinate: Premise Verification via Retrieval-Augmented Logical Reasoning**|Yuehan Qin et.al.|[2504.06438](http://arxiv.org/abs/2504.06438)|null|
|**2025-04-08**|**Decentralizing AI Memory: SHIMI, a Semantic Hierarchical Memory Index for Scalable Agent Reasoning**|Tooraj Helmi et.al.|[2504.06135](http://arxiv.org/abs/2504.06135)|null|
|**2025-04-08**|**PathGPT: Leveraging Large Language Models for Personalized Route Generation**|Steeve Cuthbert Marcelyn et.al.|[2504.05846](http://arxiv.org/abs/2504.05846)|null|
|**2025-04-08**|**Retrieval Augmented Generation with Collaborative Filtering for Personalized Text Generation**|Teng Shi et.al.|[2504.05731](http://arxiv.org/abs/2504.05731)|**[link](https://github.com/TengShi-RUC/CFRAG)**|
|**2025-04-08**|**Simplifying Data Integration: SLM-Driven Systems for Unified Semantic Queries Across Heterogeneous Databases**|Teng Lin et.al.|[2504.05634](http://arxiv.org/abs/2504.05634)|null|
|**2025-04-08**|**MicroNN: An On-device Disk-resident Updatable Vector Database**|Jeffrey Pound et.al.|[2504.05573](http://arxiv.org/abs/2504.05573)|null|
|**2025-04-07**|**Bridging Industrial Expertise and XR with LLM-Powered Conversational Agents**|Despina Tomkou et.al.|[2504.05527](http://arxiv.org/abs/2504.05527)|null|
|**2025-04-07**|**GraphRAFT: Retrieval Augmented Fine-Tuning for Knowledge Graphs on Graph Databases**|Alfred Clemedtson et.al.|[2504.05478](http://arxiv.org/abs/2504.05478)|**[link](https://github.com/AlfredClemedtson/graphraft)**|
|**2025-04-07**|**Enhancing LLM-Based Short Answer Grading with Retrieval-Augmented Generation**|Yucheng Chu et.al.|[2504.05276](http://arxiv.org/abs/2504.05276)|null|
|**2025-04-08**|**Leveraging LLMs for Utility-Focused Annotation: Reducing Manual Effort for Retrieval and RAG**|Hengran Zhang et.al.|[2504.05220](http://arxiv.org/abs/2504.05220)|null|
|**2025-04-07**|**Evaluating Knowledge Graph Based Retrieval Augmented Generation Methods under Knowledge Incompleteness**|Dongzhuoran Zhou et.al.|[2504.05163](http://arxiv.org/abs/2504.05163)|null|
|**2025-04-07**|**AI for Climate Finance: Agentic Retrieval and Multi-Step Reasoning for Early Warning System Investments**|Saeid Ario Vaghefi et.al.|[2504.05104](http://arxiv.org/abs/2504.05104)|null|
|**2025-04-07**|**RS-RAG: Bridging Remote Sensing Imagery and Comprehensive Knowledge with a Multi-Modal Dataset and Retrieval-Augmented Generation Model**|Congcong Wen et.al.|[2504.04988](http://arxiv.org/abs/2504.04988)|null|
|**2025-04-07**|**Collab-RAG: Boosting Retrieval-Augmented Generation for Complex Question Answering via White-Box and Black-Box LLM Collaboration**|Ran Xu et.al.|[2504.04915](http://arxiv.org/abs/2504.04915)|**[link](https://github.com/ritaranx/collab-rag)**|
|**2025-04-07**|**Don't Lag, RAG: Training-Free Adversarial Detection Using RAG**|Roie Kazoom et.al.|[2504.04858](http://arxiv.org/abs/2504.04858)|null|
|**2025-04-07**|**Improving Multilingual Retrieval-Augmented Language Models through Dialectic Reasoning Argumentations**|Leonardo Ranaldi et.al.|[2504.04771](http://arxiv.org/abs/2504.04771)|null|
|**2025-04-06**|**Hierarchical Planning for Complex Tasks with Knowledge Graph-RAG and Symbolic Verification**|Cristina Cornelio et.al.|[2504.04578](http://arxiv.org/abs/2504.04578)|null|
|**2025-04-06**|**KnowsLM: A framework for evaluation of small language models for knowledge augmentation and humanised conversations**|Chitranshu Harbola et.al.|[2504.04569](http://arxiv.org/abs/2504.04569)|null|
|**2025-04-04**|**Multilingual Retrieval-Augmented Generation for Knowledge-Intensive Task**|Leonardo Ranaldi et.al.|[2504.03616](http://arxiv.org/abs/2504.03616)|null|
|**2025-04-04**|**Talk2X -- An Open-Source Toolkit Facilitating Deployment of LLM-Powered Chatbots on the Web**|Lars Krupp et.al.|[2504.03343](http://arxiv.org/abs/2504.03343)|**[link](https://github.com/aiondemand/aiod-chatbot)**|
|**2025-04-04**|**Rotation Invariance in Floor Plan Digitization using Zernike Moments**|Marius Graumann et.al.|[2504.03241](http://arxiv.org/abs/2504.03241)|null|
|**2025-04-04**|**Efficient Dynamic Clustering-Based Document Compression for Retrieval-Augmented-Generation**|Weitao Li et.al.|[2504.03165](http://arxiv.org/abs/2504.03165)|**[link](https://github.com/tsinghua-dhy/edc-2-rag)**|
|**2025-04-04**|**DeepResearcher: Scaling Deep Research via Reinforcement Learning in Real-world Environments**|Yuxiang Zheng et.al.|[2504.03160](http://arxiv.org/abs/2504.03160)|**[link](https://github.com/gair-nlp/deepresearcher)**|
|**2025-04-03**|**HyperRAG: Enhancing Quality-Efficiency Tradeoffs in Retrieval-Augmented Generation with Reranker KV-Cache Reuse**|Yuwei An et.al.|[2504.02921](http://arxiv.org/abs/2504.02921)|null|
|**2025-04-03**|**TeleMoM: Consensus-Driven Telecom Intelligence via Mixture of Models**|Xinquan Wang et.al.|[2504.02712](http://arxiv.org/abs/2504.02712)|null|
|**2025-04-03**|**Retrieval-Augmented Purifier for Robust LLM-Empowered Recommendation**|Liangbo Ning et.al.|[2504.02458](http://arxiv.org/abs/2504.02458)|null|
|**2025-04-03**|**Adapting Large Language Models for Multi-Domain Retrieval-Augmented-Generation**|Alexandre Misrahi et.al.|[2504.02411](http://arxiv.org/abs/2504.02411)|null|
|**2025-04-02**|**One Pic is All it Takes: Poisoning Visual Document Retrieval Augmented Generation with a Single Image**|Ezzeldin Shereen et.al.|[2504.02132](http://arxiv.org/abs/2504.02132)|null|
|**2025-04-02**|**CoRAG: Collaborative Retrieval-Augmented Generation**|Aashiq Muhamed et.al.|[2504.01883](http://arxiv.org/abs/2504.01883)|**[link](https://github.com/aashiqmuhamed/CoRAG)**|
|**2025-04-02**|**From Code Generation to Software Testing: AI Copilot with Context-Based RAG**|Yuchen Wang et.al.|[2504.01866](http://arxiv.org/abs/2504.01866)|null|
|**2025-04-02**|**LARGE: Legal Retrieval Augmented Generation Evaluation Tool**|Minhu Park et.al.|[2504.01840](http://arxiv.org/abs/2504.01840)|**[link](https://github.com/hoorangyee/lrage)**|
|**2025-04-02**|**Reasoning LLMs for User-Aware Multimodal Conversational Agents**|Hamed Rahimi et.al.|[2504.01700](http://arxiv.org/abs/2504.01700)|null|
|**2025-04-02**|**PROPHET: An Inferable Future Forecasting Benchmark with Causal Intervened Likelihood Estimation**|Zhengwei Tao et.al.|[2504.01509](http://arxiv.org/abs/2504.01509)|**[link](https://github.com/TZWwww/PROPHET)**|
|**2025-04-03**|**GeoRAG: A Question-Answering Approach from a Geographical Perspective**|Jian Wang et.al.|[2504.01458](http://arxiv.org/abs/2504.01458)|null|
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
|**2025-03-27**|**ReaRAG: Knowledge-guided Reasoning Enhances Factuality of Large Reasoning Models with Iterative Retrieval Augmented Generation**|Zhicheng Lee et.al.|[2503.21729](http://arxiv.org/abs/2503.21729)|**[link](https://github.com/thu-keg/rearag)**|
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
|**2025-03-20**|**FutureGen: LLM-RAG Approach to Generate the Future Work of Scientific Article**|Ibrahim Al Azher et.al.|[2503.16561](http://arxiv.org/abs/2503.16561)|**[link](https://github.com/IbrahimAlAzhar/FutureWorkGeneration)**|
|**2025-03-20**|**Towards Lighter and Robust Evaluation for Retrieval Augmented Generation**|Alex-Razvan Ispas et.al.|[2503.16161](http://arxiv.org/abs/2503.16161)|**[link](https://github.com/razvanip13/towards_lighter_and_robust_evaluation)**|
|**2025-03-20**|**Tuning LLMs by RAG Principles: Towards LLM-native Memory**|Jiale Wei et.al.|[2503.16071](http://arxiv.org/abs/2503.16071)|**[link](https://github.com/mindverse/rag-tuned-llm)**|
|**2025-03-20**|**Parameters vs. Context: Fine-Grained Control of Knowledge Reliance in Language Models**|Baolong Bi et.al.|[2503.15888](http://arxiv.org/abs/2503.15888)|**[link](https://github.com/byronbbl/ck-plug)**|
|**2025-03-21**|**Typed-RAG: Type-aware Multi-Aspect Decomposition for Non-Factoid Question Answering**|DongGeon Lee et.al.|[2503.15879](http://arxiv.org/abs/2503.15879)|**[link](https://github.com/teamnlp/typed-rag)**|
|**2025-03-20**|**DroidTTP: Mapping Android Applications with TTP for Cyber Threat Intelligence**|Dincy R Arikkat et.al.|[2503.15866](http://arxiv.org/abs/2503.15866)|**[link](https://github.com/OPTIMA-CTI/DroidTTP)**|
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
|**2025-03-11**|**Privacy-Enhancing Paradigms within Federated Multi-Agent Systems**|Zitong Shi et.al.|[2503.08175](http://arxiv.org/abs/2503.08175)|**[link](https://github.com/zitongshi/epeagent)**|
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
|**2025-02-27**|**Bridging Legal Knowledge and AI: Retrieval-Augmented Generation with Vector Stores, Knowledge Graphs, and Hierarchical Non-negative Matrix Factorization**|Ryan C. Barron et.al.|[2502.20364](http://arxiv.org/abs/2502.20364)|**[link](https://github.com/lanl/t-elf)**|
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
|**2025-02-24**|**Mitigating Bias in RAG: Controlling the Embedder**|Taeyoun Kim et.al.|[2502.17390](http://arxiv.org/abs/2502.17390)|**[link](https://github.com/danielkty/debiasing-rag)**|
|**2025-02-24**|**Benchmarking Retrieval-Augmented Generation in Multi-Modal Contexts**|Zhenghao Liu et.al.|[2502.17297](http://arxiv.org/abs/2502.17297)|**[link](https://github.com/neuir/m2rag)**|
|**2025-02-24**|**MEMERAG: A Multilingual End-to-End Meta-Evaluation Benchmark for Retrieval Augmented Generation**|María Andrea Cruz Blandón et.al.|[2502.17163](http://arxiv.org/abs/2502.17163)|**[link](https://github.com/amazon-science/memerag)**|
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
|**2025-02-10**|**Combining Large Language Models with Static Analyzers for Code Review Generation**|Imen Jaoua et.al.|[2502.06633](http://arxiv.org/abs/2502.06633)|**[link](https://github.com/imenjaoua/hybrid-code-review)**|
|**2025-02-10**|**C-3PO: Compact Plug-and-Play Proxy Optimization to Achieve Human-like Retrieval-Augmented Generation**|Guoxin Chen et.al.|[2502.06205](http://arxiv.org/abs/2502.06205)|null|
|**2025-02-10**|**Optimizing Knowledge Integration in Retrieval-Augmented Generation with Self-Selection**|Yan Weng et.al.|[2502.06148](http://arxiv.org/abs/2502.06148)|null|
|**2025-02-11**|**RALLRec: Improving Retrieval Augmented Large Language Model Recommendation with Representation Learning**|Jian Xu et.al.|[2502.06101](http://arxiv.org/abs/2502.06101)|**[link](https://github.com/jianxu95/rallrec)**|
|**2025-02-09**|**MetaChain: A Fully-Automated and Zero-Code Framework for LLM Agents**|Jiabin Tang et.al.|[2502.05957](http://arxiv.org/abs/2502.05957)|**[link](https://github.com/hkuds/autoagent)**|
|**2025-02-11**|**Enhancing Financial Time-Series Forecasting with Retrieval-Augmented Large Language Models**|Mengxi Xiao et.al.|[2502.05878](http://arxiv.org/abs/2502.05878)|null|
|**2025-02-09**|**Quality Assurance for LLM-RAG Systems: Empirical Insights from Tourism Application Testing**|Bestoun S. Ahmed et.al.|[2502.05782](http://arxiv.org/abs/2502.05782)|null|
|**2025-02-08**|**AI-Driven Electronic Health Records System for Enhancing Patient Data Management and Diagnostic Support in Egypt**|Arwa Alorbany et.al.|[2502.05603](http://arxiv.org/abs/2502.05603)|null|
|**2025-02-08**|**APE: Faster and Longer Context-Augmented Generation via Adaptive Parallel Encoding**|Xinyu Yang et.al.|[2502.05431](http://arxiv.org/abs/2502.05431)|**[link](https://github.com/infini-ai-lab/ape)**|
|**2025-02-07**|**Enhancing Health Information Retrieval with RAG by Prioritizing Topical Relevance and Factual Accuracy**|Rishabh Uapadhyay et.al.|[2502.04666](http://arxiv.org/abs/2502.04666)|null|
|**2025-02-07**|**Agentic Reasoning: Reasoning LLMs with Tools for the Deep Research**|Junde Wu et.al.|[2502.04644](http://arxiv.org/abs/2502.04644)|**[link](https://github.com/theworldofagents/agentic-reasoning)**|
|**2025-02-06**|**MedRAG: Enhancing Retrieval-augmented Generation with Knowledge Graph-Elicited Reasoning for Healthcare Copilot**|Xuejiao Zhao et.al.|[2502.04413](http://arxiv.org/abs/2502.04413)|**[link](https://github.com/snowteam2023/medrag)**|
|**2025-02-05**|**MARAGE: Transferable Multi-Model Adversarial Attack for Retrieval-Augmented Generation Data Extraction**|Xiao Hu et.al.|[2502.04360](http://arxiv.org/abs/2502.04360)|null|
|**2025-02-04**|**Open Foundation Models in Healthcare: Challenges, Paradoxes, and Opportunities with GenAI Driven Personalized Prescription**|Mahdi Alkaeed et.al.|[2502.04356](http://arxiv.org/abs/2502.04356)|null|
|**2025-02-06**|**MRAMG-Bench: A BeyondText Benchmark for Multimodal Retrieval-Augmented Multimodal Generation**|Qinhan Yu et.al.|[2502.04176](http://arxiv.org/abs/2502.04176)|**[link](https://github.com/mramg-bench/mramg)**|
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
|**2025-01-20**|**RACCOON: A Retrieval-Augmented Generation Approach for Location Coordinate Capture from News Articles**|Jonathan Lin et.al.|[2501.11440](http://arxiv.org/abs/2501.11440)|**[link](https://github.com/jonlin223/raccoon-geocoding)**|
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
|**2025-01-14**|**Addressing the sustainable AI trilemma: a case study on LLM agents and RAG**|Hui Wu et.al.|[2501.08262](http://arxiv.org/abs/2501.08262)|**[link](https://github.com/huiwxing/llmagent_trilemma)**|
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
|**2024-12-29**|**Understanding the Impact of Confidence in Retrieval Augmented Generation: A Case Study in the Medical Domain**|Shintaro Ozaki et.al.|[2412.20309](http://arxiv.org/abs/2412.20309)|**[link](https://github.com/naist-nlp/CC_RAG)**|
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
|**2024-12-07**|**KG-Retriever: Efficient Knowledge Indexing for Retrieval-Augmented Large Language Models**|Weijie Chen et.al.|[2412.05547](http://arxiv.org/abs/2412.05547)|**[link](https://github.com/bai-lab/kg-retriever)**|
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
|**2024-11-17**|**ForPKG-1.0: A Framework for Constructing Forestry Policy Knowledge Graph and Application Analysis**|Jingyun Sun et.al.|[2411.11090](http://arxiv.org/abs/2411.11090)|**[link](https://github.com/luozhongze/ForPKG)**|
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

<p align=right>(<a href=#updated-on-20250525>back to top</a>)</p>

## text2sql

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-05-08**|**HEXGEN-TEXT2SQL: Optimizing LLM Inference Request Scheduling for Agentic Text-to-SQL Workflow**|You Peng et.al.|[2505.05286](http://arxiv.org/abs/2505.05286)|**[link](https://github.com/relaxed-system-lab/hexgen-flow)**|**最近在利用大型语言模型（LLM）的代理范式方面的进展显著增强了Text-to-SQL的能力，使不具备专门数据库知识的用户也能直观地查询数据。然而，在生产环境中部署这些基于代理LLM的Text-to-SQL系统面临重大挑战，原因在于其固有的多阶段工作流程、严格的延迟要求以及企业环境中可能存在的异构GPU基础设施。当前的LLM服务框架缺乏有效处理相互依赖的推理任务、动态延迟变化和资源异质性的机制，导致性能不佳和服务水平目标（SLO）频繁违规。在本文中，我们引入了HEXGEN-TEXT2SQL，这是一个专为在异构GPU集群上调度和执行基于代理的多阶段LLM Text-to-SQL工作流而设计的新框架，能够处理多租户端到端查询。HEXGEN-TEXT2SQL提出了一种分层调度方法，结合全局负载均衡的任务调度和本地自适应紧急度优先排序，该方法由对代理Text-to-SQL工作流的系统分析指导。此外，我们还提出了一种轻量级的基于仿真的方法来调整关键调度超参数，进一步增强系统的鲁棒性和适应性。我们在现实的Text-to-SQL基准测试中的广泛评估表明，HEXGEN-TEXT2SQL显著优于最先进的LLM服务框架。具体而言，与vLLM相比，HEXGEN-TEXT2SQL在多样化的现实工作负载条件下将延迟截止时间减少了高达1.67倍（平均1.41倍），并将系统吞吐量提高了高达1.75倍（平均1.65倍）。我们的代码可在https://github.com/Relaxed-System-Lab/Hexgen-Flow获取。**|
|**2025-05-08**|**Text2Cypher: Data Pruning using Hard Example Selection**|Makbule Gulcin Ozsoy et.al.|[2505.05122](http://arxiv.org/abs/2505.05122)|null|数据库查询语言如关系型数据库的SQL和图数据库的Cypher已被广泛采用。最近，大型语言模型（LLMs）的发展使得通过Text2SQL和Text2Cypher等模型用自然语言与数据库进行交互成为可能。通常，微调这些模型需要包含非平凡示例的大规模多样化数据集。然而，随着数据集规模的增加，微调的成本也随之上升。这使得较小但高质量的数据集对于减少成本同时保持相同或更好的性能变得至关重要。在本文中，我们提出了五种难例选择技术来精简Text2Cypher数据集，旨在保持或提高性能的同时减少资源使用。我们的结果表明，这些难例选择方法可以将训练时间和成本减半，并且对性能的影响极小，证明了难例选择提供了一种成本效益高的解决方案。|
|**2025-05-02**|**Sparks of Tabular Reasoning via Text2SQL Reinforcement Learning**|Josefa Lia Stoisser et.al.|[2505.00016](http://arxiv.org/abs/2505.00016)|null|这项工作将Text-to-SQL任务重新定义为教授大型语言模型（LLMs）对表格数据进行推理和操作的途径，超越了传统的查询生成重点。我们提出了一个两阶段框架，利用SQL监督来开发可迁移的表格推理能力。首先，我们从现实世界的SQL查询中合成详细的思维链（CoT）追踪，提供逐条、逐子句级别的监督，教导模型如何遍历、过滤和聚合表格字段。其次，我们引入了一种组相对策略优化（GRPO）强化学习目标，该目标通过鼓励超出特定任务语法并能在不同数据集间迁移的步骤，将SQL执行准确性与通用推理联系起来。实验结果表明，我们的方法在标准的Text-to-SQL基准测试上提高了性能，并且在诸如BIRD和CRT-QA等需要大量推理的数据集上取得了显著进步，展示了增强的泛化能力和可解释性。具体来说，经过Text-to-SQL任务训练后，蒸馏量化版的LLaMA模型实现了33.9%的相对准确率提升，而Qwen则实现了14.5%的相对准确率提升。这些结果表明，SQL不仅可以作为一种目标形式主义，还可以作为学习强健且可迁移的结构化数据推理的有效支架。|
|**2025-04-24**|**High-Fidelity And Complex Test Data Generation For Real-World SQL Code Generation Services**|Shivasankari Kannan et.al.|[2504.17203](http://arxiv.org/abs/2504.17203)|null|在工业环境中，对高保真测试数据的需求至关重要，因为访问生产数据通常受到严格限制。传统数据生成方法往往难以满足需求，尤其是在生成能够模拟复杂数据结构和语义关系的高质量数据方面，这对于测试复杂的SQL代码生成服务（如自然语言到SQL）尤为重要。本文针对为包含嵌套结构列的复杂模式生成语法正确且语义“有意义”的模拟数据这一迫切需求进行了探讨。我们指出了现有生产中使用的方法的局限性，特别是它们无法处理大规模和复杂的模式，以及缺乏语义连贯的测试数据，这导致了测试覆盖率不足。我们展示了通过利用大型语言模型（LLMs）并结合策略性的预处理和后处理步骤，可以生成符合复杂结构约束并保持与测试目标（SQL查询/函数）语义完整性的现实高保真测试数据。这种方法支持对涉及连接、聚合甚至深度嵌套子查询的复杂SQL查询进行全面测试，确保了对SQL代码生成服务（如NL2SQL和SQL代码助手服务）的稳健评估。我们的结果表明，基于开箱即用的大型语言模型（gemini）的测试数据生成方法，在工业SQL代码生成服务中具有实际应用价值，特别是在由于生产数据集经常不可用而需要生成现实测试数据的情况下。|
|**2025-04-27**|**Think2SQL: Reinforce LLM Reasoning Capabilities for Text2SQL**|Simone Papicchio et.al.|[2504.15077](http://arxiv.org/abs/2504.15077)|null|大型语言模型（LLM）在将关于关系数据库的自然语言问题转换为SQL查询方面展示了令人印象深刻的能力。尽管最近有所改进，但在零样本学习（ZSL）设置下，小型LLM在处理涉及多个表和复杂SQL模式的问题时仍存在困难。监督微调（SFT）部分弥补了预训练模型的知识缺陷，但在处理需要多跳推理的查询时仍然不足。为了弥合这一差距，提出了不同的LLM训练策略来增强推理能力，包括在ZSL中利用思维过程、在SFT中包含任务特定的推理痕迹，或采用强化学习（RL）策略。然而，推理对Text2SQL性能的影响仍很大程度上未被探索。本文研究了LLM推理能力对其在四个基准数据集上的Text2SQL性能的影响程度。为此，考虑了以下LLM设置：(1) ZSL，包括是否使用通用推理；(2) SFT，有无任务特定的推理痕迹；(3) RL，探索使用不同的奖励函数，既包括已建立的执行准确性（EX），也包括结合了精确度、召回率和部分正确答案基数的细粒度指标；(4) SFT+RL，即结合SFT和RL的两阶段方法。结果显示，在处理复杂的Text2SQL案例时，ZSL下的通用推理被证明是无效的。小型LLM从带有推理的SFT中获益远大于大型LLM。RL总体上对所有测试模型和数据集都是有益的。使用细粒度指标被证明是最有效的RL策略。得益于RL和新的Text2SQL奖励，7B Qwen-Coder-2.5模型在Bird数据集上的表现与400+Billion级别的模型（包括gpt-4o）相当。|
|**2025-04-16**|**A New Paradigm of User-Centric Wireless Communication Driven by Large Language Models**|Kuiyuan Ding et.al.|[2504.11696](http://arxiv.org/abs/2504.11696)|null|下一代无线通信旨在将人工智能（AI）与以用户为中心的通信网络深度融合，目标是开发出能够更准确满足用户需求的AI原生网络。大型语言模型（LLM）的快速发展为实现这些目标提供了巨大潜力。然而，现有利用LLM进行无线通信的努力往往忽视了人类自然语言与实际通信系统复杂性之间的巨大差距，未能充分利用LLM的能力。为解决这一问题，我们提出了一种新颖的基于LLM驱动的无线通信范式，创新地结合了自然语言到结构化查询语言（NL2SQL）工具。具体而言，在这一范式中，用户个人需求是主要关注点。在接收到用户请求后，LLM首先根据相关通信指标和系统参数分析用户意图。随后，生成一个结构化查询语言（SQL）语句从高性能实时数据库中检索特定参数值。我们进一步利用LLM根据用户请求和检索到的参数来制定并解决优化问题。该优化问题的解用于调整通信系统以满足用户需求。为了验证所提范式的可行性，我们展示了一个原型系统。在这个原型系统中，我们考虑了以用户请求为中心的语义通信（URC-SC）系统，其中物理层上的动态语义表示网络会根据用户需求自适应其编码深度。此外，还使用了两个LLM分别用于分析用户请求和生成SQL语句。仿真结果表明了该方法的有效性。|
|**2025-05-12**|**SQL-R1: Training Natural Language to SQL Reasoning Model By Reinforcement Learning**|Peixian Ma et.al.|[2504.08600](http://arxiv.org/abs/2504.08600)|**[link](https://github.com/IDEA-FinAI/SQL-R1)**|**自然语言到SQL（NL2SQL）通过将自然语言查询转换为结构化的SQL语句，实现了与数据库的直观交互。尽管在增强数据库应用程序中人机交互方面取得了最新进展，但在涉及多表连接和嵌套查询等复杂场景下的推理性能仍然存在重大挑战。当前方法主要利用监督微调（SFT）来训练NL2SQL模型，这可能限制了其在新环境（如金融和医疗保健）中的适应性和可解释性。为了提高NL2SQL模型在上述复杂情况下的推理性能，我们引入了SQL-R1，这是一种使用强化学习（RL）算法训练的新型NL2SQL推理模型。我们设计了一种专门针对NL2SQL任务的基于RL的奖励函数，并讨论了冷启动对密集训练有效性的影响。此外，我们仅使用少量合成的NL2SQL数据进行增强训练就达到了竞争性的准确性，并进一步探索了用于RL的数据工程。在现有的实验中，SQL-R1在基准测试Spider和BIRD上分别达到了88.6%和66.6%的执行准确率，仅使用7B基础模型。**|
|**2025-04-03**|**LearNAT: Learning NL2SQL with AST-guided Task Decomposition for Large Language Models**|Weibin Liao et.al.|[2504.02327](http://arxiv.org/abs/2504.02327)|null|自然语言到SQL（NL2SQL）已成为实现与数据库无缝交互的关键任务。最近，大型语言模型（LLMs）在这一领域展示了卓越的性能。然而，现有的NL2SQL方法主要依赖于通过提示工程利用闭源LLMs，而开源模型通常需要微调以获得特定领域的知识。尽管做出了这些努力，开源LLMs在处理复杂的NL2SQL任务时仍然面临挑战，因为用户查询目标的间接表达以及用户查询与数据库模式之间的语义差距。受到强化学习在数学问题解决中鼓励LLMs逐步推理的应用启发，我们提出了LearNAT（基于AST引导的任务分解的学习NL2SQL），这是一种通过任务分解和强化学习来提高开源LLMs在复杂NL2SQL任务上表现的新框架。LearNAT引入了三个关键组件：(1) 分解合成程序，利用抽象语法树（ASTs）指导高效搜索和剪枝策略进行任务分解；(2) 边界感知强化学习，通过具有AST边界的DPO进行细粒度步骤级优化；(3) 自适应示例推理，一种动态选择相关示例以增强分解能力的机制。在两个基准数据集Spider和BIRD上的广泛实验表明，LearNAT使一个70亿参数的开源LLM能够达到与GPT-4相当的表现，同时提供了更高的效率和可访问性。|
|**2025-04-05**|**Review, Refine, Repeat: Understanding Iterative Decoding of AI Agents with Dynamic Evaluation and Selection**|Souradip Chakraborty et.al.|[2504.01931](http://arxiv.org/abs/2504.01931)|null|尽管AI代理在各种任务中表现出色，但在复杂的多模态应用、结构化生成和战略规划方面仍存在困难。通过标准微调进行改进通常是不切实际的，因为解决代理任务通常依赖于黑盒API访问，而无法控制模型参数。像Best-of-N（BON）采样这样的推理时间方法提供了一种简单而有效的方法来提高性能。然而，BON缺乏迭代反馈整合机制。因此，我们提出了迭代代理解码（IAD），它结合了迭代细化和由验证器指导的动态候选评估与选择。IAD在如何设计和集成反馈方面有所不同，特别优化以从奖励分数中提取最大信号。我们在Sketch2Code、Text2SQL和Webshop上进行了详细的基线比较，结果表明IAD在关键指标上始终优于基线，在Sketch2Code和Text2SQL（无论是否有大语言模型裁判）上实现了3-6%的绝对增益，在Webshop上的多个指标上实现了8-10%的增益。为了更好地理解IAD的增益来源，我们进行了受控实验以分离自适应反馈与随机采样的影响，并发现IAD的改进主要由验证器引导的细化驱动，而不仅仅是采样多样性。我们还展示了当由最优验证器指导时，IAD和BON都表现出随着计算增加而在推理时间内的扩展性。我们的分析强调了验证器质量在有效推理时间优化中的关键作用，并探讨了噪声和稀疏奖励对扩展行为的影响。这些发现共同提供了关于有效推理时间优化的权衡和原则的关键见解。|
|**2025-03-30**|**Distill-C: Enhanced NL2SQL via Distilled Customization with LLMs**|Cong Duy Vu Hoang et.al.|[2504.00048](http://arxiv.org/abs/2504.00048)|**[link](https://github.com/clemencelanfranchi/distill-c)**|**随着大型语言模型（LLMs）在商业应用中的日益普及，人们对自然语言到SQL（NL2SQL）解决方案的兴趣也越来越大，其中高性能和高效率的需求相互竞争。特定领域和客户的具体要求进一步复杂化了这一问题。为了解决这一难题，我们引入了Distill-C，这是一种针对NL2SQL任务量身定制的精简框架。Distill-C利用大型教师LLM通过一个强大且可扩展的管道生成高质量的合成数据。通过对这些合成数据进行微调，较小且开源的LLM能够与大十倍的教师模型相匹敌甚至超越。在多个具有挑战性的基准测试中，Distill-C相比来自三个不同LLM家族的基础模型，在执行准确率上平均提高了36%。此外，在三个内部客户基准测试中，Distill-C相较于基础模型表现出了22.6%的性能提升。我们的结果表明，Distill-C是一种有效、高性能且通用的方法，用于部署轻量级但功能强大的NL2SQL模型，能够在保持低计算成本的同时提供卓越的准确性。**|
|**2025-03-22**|**Feather-SQL: A Lightweight NL2SQL Framework with Dual-Model Collaboration Paradigm for Small Language Models**|Wenqi Pei et.al.|[2503.17811](http://arxiv.org/abs/2503.17811)|null|
|**2025-03-15**|**NL2SQL-BUGs: A Benchmark for Detecting Semantic Errors in NL2SQL Translation**|Xinyu Liu et.al.|[2503.11984](http://arxiv.org/abs/2503.11984)|null|
|**2025-03-04**|**NLI4DB: A Systematic Review of Natural Language Interfaces for Databases**|Mengyi Liu et.al.|[2503.02435](http://arxiv.org/abs/2503.02435)|null|
|**2025-02-23**|**SQLong: Enhanced NL2SQL for Longer Contexts with LLMs**|Dai Quoc Nguyen et.al.|[2502.16747](http://arxiv.org/abs/2502.16747)|null|
|**2025-03-23**|**Balancing Content Size in RAG-Text2SQL System**|Prakhar Gurawa et.al.|[2502.15723](http://arxiv.org/abs/2502.15723)|null|
|**2025-02-17**|**SQL-o1: A Self-Reward Heuristic Dynamic Search Method for Text-to-SQL**|Shuai Lyu et.al.|[2502.11741](http://arxiv.org/abs/2502.11741)|**[link](https://github.com/shuailyu0110/sql-o1)**|
|**2025-01-30**|**Fundamental Challenges in Evaluating Text2SQL Solutions and Detecting Their Limitations**|Cedric Renggli et.al.|[2501.18197](http://arxiv.org/abs/2501.18197)|null|
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

<p align=right>(<a href=#updated-on-20250525>back to top</a>)</p>

## PPC

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-05-22**|**Redefining Clustered Federated Learning for System Identification: The Path of ClusterCraft**|Ertuğrul Keçeci et.al.|[2505.16857](http://arxiv.org/abs/2505.16857)|null|本文在联邦学习框架下解决了系统辨识（SYSID）问题。我们引入了一种新颖的算法，即基于增量聚类的联邦学习方法用于系统辨识（IC-SYSID），旨在解决多个数据源中的系统辨识挑战，且无需事先了解数据集。IC-SYSID利用了一种名为ClusterCraft（CC）的增量聚类方法，消除了对数据集先验知识的依赖。CC从单一聚类模型开始，并通过动态增加聚类数量将相似的本地工作者分配到同一聚类中。为了减少CC生成的聚类数量，我们引入了ClusterMerge，其中相似的聚类模型会被合并。此外，我们还引入了增强版ClusterCraft，以减少训练过程中生成相似聚类模型的数量。IC-SYSID通过在损失函数中加入正则化项并使用缩放的Glorot初始化来解决聚类模型不稳定性的问题。它还利用小批量深度学习方法来处理大规模SYSID数据集在本地训练中的管理。通过在一个代表性的实际SYSID问题上进行实验，即一组车辆协同学习车辆动力学，我们展示了IC-SYSID在防止学习不稳定聚类的同时实现了高SYSID性能。|
|**2025-05-22**|**ATR-Bench: A Federated Learning Benchmark for Adaptation, Trust, and Reasoning**|Tajamul Ashraf et.al.|[2505.16850](http://arxiv.org/abs/2505.16850)|null|联邦学习（FL）作为一种有前景的范式，能够在保护分散参与者数据隐私的同时进行协作模型训练。随着FL的采用日益增多，已经提出了许多技术来解决其实际挑战。然而，由于缺乏在关键维度上的标准化评估，阻碍了FL方法的系统性进展和公平比较。在这项工作中，我们引入了ATR-Bench，这是一个通过三个基础维度——适应性、信任性和推理——来分析联邦学习的统一框架。我们深入探讨了每个主题的概念基础、任务表述和开放的研究挑战。我们广泛地对代表性的方法和数据集进行了基准测试，以适应异构客户端并在对抗或不可靠环境中保持可信度。由于联邦学习中缺乏可靠的推理度量和模型，我们仅对此维度提供了文献驱动的见解。ATR-Bench为具有现实意义的联邦学习的系统化和全面评估奠定了基础。我们将公开我们的完整代码库，并维护一个持续跟踪FL文献中新发展和研究的精选资料库。|
|**2025-05-22**|**Data-Driven Breakthroughs and Future Directions in AI Infrastructure: A Comprehensive Review**|Beyazit Bestami Yuksel et.al.|[2505.16771](http://arxiv.org/abs/2505.16771)|null|本文全面综合了过去十五年人工智能（AI）的主要突破，结合历史、理论和技术视角。通过追踪计算资源、数据访问和算法创新的融合，确定了AI演进的关键转折点。分析强调了研究人员如何实现基于GPU的模型训练，通过ImageNet引发以数据为中心的转变，通过Transformer简化架构，并通过GPT系列扩展建模能力。本文并未将这些进展视为孤立的里程碑，而是将其作为更深层次范式转变的标志。通过应用统计学习理论中的样本复杂度和数据效率等概念，本文解释了研究人员如何将突破转化为可扩展的解决方案，以及为什么该领域现在必须拥抱以数据为中心的方法。面对日益增长的隐私担忧和监管收紧，本文评估了联邦学习、隐私增强技术（PETs）和数据站点模式等新兴解决方案，这些方案重新定义了数据访问和安全。在现实世界数据仍不可访问的情况下，本文还评估了模拟和合成数据生成的效用和限制。通过将技术见解与不断发展的数据基础设施相结合，本研究为未来的人工智能研究和政策制定提供了战略指导。|
|**2025-05-22**|**WikiDBGraph: Large-Scale Database Graph of Wikidata for Collaborative Learning**|Zhaomin Wu et.al.|[2505.16635](http://arxiv.org/abs/2505.16635)|null|表格数据无处不在且信息丰富，是深度表示学习日益关注的焦点。然而，研究通常集中在单一表格或孤立的数据库上，这由于数据规模限制了模型的能力。虽然联邦学习、迁移学习、分割学习和表格基础模型等协作学习方法旨在从多个相关数据库中学习，但它们受到现实世界互联表格资源稀缺的挑战。当前的数据湖和语料库主要由缺乏定义的跨数据库关联的孤立数据库组成。为了解决这个问题，我们引入了WikiDBGraph，这是一个大规模图，包含来自WikiData的10万个现实世界的表格数据库，通过1700万条边连接，并由其数据库模式和数据分布派生出13个节点属性和12个边属性来表征。WikiDBGraph的加权边识别实例和特征重叠的数据库。在这些新识别的数据库上的实验确认了协作学习可以带来更好的性能，从而为结构化基础模型训练提供了巨大潜力，同时也揭示了从互联表格数据学习的关键挑战和未来方向。|
|**2025-05-22**|**From Local Patterns to Global Understanding: Cross-Stock Trend Integration for Enhanced Predictive Modeling**|Yi Hu et.al.|[2505.16573](http://arxiv.org/abs/2505.16573)|null|股票价格预测是金融预测中的一个关键领域，传统上通过使用个股的历史价格数据来训练模型。虽然这些模型能够有效地捕捉单个股票的模式，但它们未能利用股票趋势之间的潜在关联性，而这可能提高预测性能。当前的单股票学习方法因此在提供对多只股票价格动态的更广泛理解方面存在局限。为了解决这个问题，我们提出了一种新的方法，通过跨股票模式整合将局部模式合并成全局理解。我们的策略受到联邦学习（FL）范式的启发，这是一种为分布式数据集设计的去中心化模型训练方法。FL能够在不共享原始数据的情况下促进跨分布式数据集的协作学习，从而在保留数据隐私的同时促进全局洞察的聚合。在我们的适应中，我们在个体股票数据上训练模型，并迭代地将它们合并以创建一个统一的全局模型。然后，这个全局模型会在特定股票数据上进行微调，以保持本地相关性。所提出的策略使个体股票模型的并行训练成为可能，促进了计算资源的有效利用并减少了总体训练时间。我们进行了广泛的实验来评估所提出的方法，结果表明它优于基准模型，并增强了最先进方法的预测能力。我们的研究结果突出了跨股票趋势整合（CSTI）在推进股票价格预测方面的有效性，为传统的单股票学习方法提供了一个强大的替代方案。|
|**2025-05-22**|**Performance Guaranteed Poisoning Attacks in Federated Learning: A Sliding Mode Approach**|Huazi Pan et.al.|[2505.16403](http://arxiv.org/abs/2505.16403)|null|本地训练数据和本地更新的操纵，即投毒攻击，是联邦学习（FL）范式协作性质带来的主要威胁。大多数现有的投毒攻击旨在以导致拒绝服务（DoS）问题的方式操纵本地数据/模型。在本文中，我们介绍了一种新的攻击方法，名为联邦学习滑动攻击（FedSA）方案，其目标是以一种微妙且可控的方式精确引入投毒程度。它基于预定义的目标进行操作，例如将全局模型的预测准确率降低10%。FedSA将鲁棒非线性控制—滑模控制（SMC）理论与模型投毒攻击相结合。它可以操纵恶意客户端的更新，使全局模型逐渐趋向于受损状态，并以可控而不显眼的速度实现这一目标。此外，利用FedSA的鲁棒控制特性可以精确控制收敛边界，使攻击者能够将被投毒模型的全局准确率设置为任何期望的水平。实验结果表明，FedSA可以使用更少的恶意客户端准确达到预设的全局准确率，同时保持高水平的隐蔽性和可调的学习率。|
|**2025-05-22**|**Privacy-Aware Cyberterrorism Network Analysis using Graph Neural Networks and Federated Learning**|Anas Ali et.al.|[2505.16371](http://arxiv.org/abs/2505.16371)|null|网络恐怖主义对数字基础设施构成了巨大威胁，随着对加密和去中心化平台依赖的增加，威胁行为者的活动变得越来越隐蔽。为了解决在分析此类对抗性网络时保护分布式情报数据隐私的问题，我们提出了一种隐私感知的联邦图神经网络（PA-FGNN）框架。PA-FGNN将图注意力网络、差分隐私和同态加密集成到一个针对网络恐怖主义网络分析定制的强大联邦学习流水线中。每个客户端在敏感图数据上进行本地训练，并与中央聚合器交换加密的、添加噪声的模型更新，该聚合器执行安全聚合并广播全局更新。我们实现了异常检测来标记高风险节点，并加入了针对梯度投毒攻击的防御措施。在模拟暗网和网络情报图上的实验评估表明，PA-FGNN达到了超过91%的分类准确率，在20%的对抗性客户端行为下保持了鲁棒性，并且通信开销不到18%。我们的结果表明，隐私保护的GNN可以在不牺牲实用性、隐私或鲁棒性的前提下支持大规模网络威胁检测。|
|**2025-05-22**|**Enhancing Federated Survival Analysis through Peer-Driven Client Reputation in Healthcare**|Navid Seidi et.al.|[2505.16190](http://arxiv.org/abs/2505.16190)|null|联邦学习（FL）通过在不损害患者数据隐私的情况下实现协作模型训练，在数字健康领域展现出巨大潜力。然而，机构间的异质性、缺乏持续的声誉以及不可靠的贡献仍然是主要挑战。在本文中，我们提出了一种针对联邦医疗保健的稳健的、基于同行驱动的声誉机制，该机制采用混合通信模型，将去中心化的同行反馈与基于聚类的噪声处理相结合，以增强模型聚合。关键的是，我们的方法通过在共享给同行评估之前对客户端模型更新应用差分隐私，将联邦聚合和声誉机制解耦。这确保了在声誉计算过程中敏感信息得到保护，而未修改的更新则发送到服务器进行全局模型训练。使用Cox比例风险模型对多个联邦节点进行生存分析，我们的框架通过动态调整基于局部性能改进（通过一致性指数测量）的信任分数来解决数据异质性和声誉不足的问题。在合成数据集和SEER数据集上的实验评估表明，我们的方法能够持续获得高且稳定的一致性指数值，有效降低了噪声客户端更新的影响，并优于缺乏声誉系统的联邦学习方法。|
|**2025-05-22**|**Multimodal Online Federated Learning with Modality Missing in Internet of Things**|Heqiang Wang et.al.|[2505.16138](http://arxiv.org/abs/2505.16138)|null|物联网生态系统从传感器、摄像头和麦克风等异构源生成大量多模态数据。随着边缘智能的不断发展，物联网设备已经从简单的数据收集单元演进为能够执行复杂计算任务的节点。这种演变需要采用分布式学习策略，以有效处理物联网环境中的多模态数据。此外，数据收集的实时性和物联网边缘设备有限的本地存储空间要求采用在线学习范式。为应对这些挑战，我们引入了多模态在线联邦学习（MMO-FL）的概念，这是一种为动态和去中心化的物联网环境设计的新框架。在此基础上，我们进一步考虑了边缘设备固有的不稳定性，这经常导致在学习过程中出现缺失模态的情况。我们在完整和缺失模态场景下进行了全面的理论分析，提供了关于缺失模态导致性能下降的见解。为了减轻缺失模态的影响，我们提出了原型模态缓解（PMM）算法，该算法利用原型学习有效地补偿缺失模态。在两个多模态数据集上的实验结果进一步证明了PMM相比基准方法的优越性能。|
|**2025-05-21**|**Federated Learning with Unlabeled Clients: Personalization Can Happen in Low Dimensions**|Hossein Zakerinia et.al.|[2505.15579](http://arxiv.org/abs/2505.15579)|null|个性化联邦学习已成为在持有统计异质数据的设备（称为客户端）上进行训练的一种流行方法。然而，大多数现有方法要求客户端拥有带标签的数据以进行训练或微调，从而获得自己的个性化模型。在这篇论文中，我们提出了一种名为FLowDUP的新方法，该方法仅使用未标记数据的前向传播即可生成个性化模型。生成的模型参数位于低维子空间内，从而实现高效的通信和计算。FLowDUP的学习目标由我们新的归纳多任务PAC-Bayesian泛化界理论驱动，为未标记数据的客户端提供性能保证。该目标结构允许既有带标签数据的客户端也有仅含未标记数据的客户端共同参与训练过程。为了补充我们的理论结果，我们对FLowDUP进行了全面的实验评估，在不同类型的统计异质客户端的各种数据集上展示了强大的实证表现。通过大量的消融研究，我们测试了该方法各个组件的有效性。|
|**2025-05-21**|**Federated Learning-Enhanced Blockchain Framework for Privacy-Preserving Intrusion Detection in Industrial IoT**|Anas Ali et.al.|[2505.15376](http://arxiv.org/abs/2505.15376)|null|
|**2025-05-21**|**Distributionally Robust Federated Learning with Client Drift Minimization**|Mounssif Krouka et.al.|[2505.15371](http://arxiv.org/abs/2505.15371)|null|
|**2025-05-21**|**Reliable Vertical Federated Learning in 5G Core Network Architecture**|Mohamad Mestoukirdi et.al.|[2505.15244](http://arxiv.org/abs/2505.15244)|**[link](https://github.com/merce-fra/Reliable-VFL-in-5G-Core-NW-Arch)**|
|**2025-05-21**|**A Survey On Secure Machine Learning**|Taobo Liao et.al.|[2505.15124](http://arxiv.org/abs/2505.15124)|null|
|**2025-05-20**|**Efficient Privacy-Preserving Cross-Silo Federated Learning with Multi-Key Homomorphic Encryption**|Abdullah Al Omar et.al.|[2505.14797](http://arxiv.org/abs/2505.14797)|null|
|**2025-05-20**|**Federated prediction for scalable and privacy-preserved knowledge-based planning in radiotherapy**|Jingyun Chen et.al.|[2505.14507](http://arxiv.org/abs/2505.14507)|null|
|**2025-05-20**|**Federated learning in low-resource settings: A chest imaging study in Africa -- Challenges and lessons learned**|Jorge Fabila et.al.|[2505.14217](http://arxiv.org/abs/2505.14217)|null|
|**2025-05-20**|**Personalized Bayesian Federated Learning with Wasserstein Barycenter Aggregation**|Ting Wei et.al.|[2505.14161](http://arxiv.org/abs/2505.14161)|null|
|**2025-05-20**|**FedGraM: Defending Against Untargeted Attacks in Federated Learning via Embedding Gram Matrix**|Di Wu et.al.|[2505.14024](http://arxiv.org/abs/2505.14024)|null|
|**2025-05-19**|**Optimal Client Sampling in Federated Learning with Client-Level Heterogeneous Differential Privacy**|Jiahao Xu et.al.|[2505.13655](http://arxiv.org/abs/2505.13655)|null|
|**2025-05-19**|**Traceable Black-box Watermarks for Federated Learning**|Jiahao Xu et.al.|[2505.13651](http://arxiv.org/abs/2505.13651)|null|
|**2025-05-19**|**FedCTTA: A Collaborative Approach to Continual Test-Time Adaptation in Federated Learning**|Rakibul Hasan Rajib et.al.|[2505.13643](http://arxiv.org/abs/2505.13643)|null|
|**2025-05-20**|**SVAFD: A Secure and Verifiable Co-Aggregation Protocol for Federated Distillation**|Tian Wen et.al.|[2505.13319](http://arxiv.org/abs/2505.13319)|null|
|**2025-05-19**|**Cross-Cloud Data Privacy Protection: Optimizing Collaborative Mechanisms of AI Systems by Integrating Federated Learning and LLMs**|Huaiying Luo et.al.|[2505.13292](http://arxiv.org/abs/2505.13292)|null|
|**2025-05-19**|**RIFLES: Resource-effIcient Federated LEarning via Scheduling**|Sara Alosaime et.al.|[2505.13169](http://arxiv.org/abs/2505.13169)|null|
|**2025-05-19**|**FLTG: Byzantine-Robust Federated Learning via Angle-Based Defense and Non-IID-Aware Weighting**|Yanhua Wen et.al.|[2505.12851](http://arxiv.org/abs/2505.12851)|null|
|**2025-05-19**|**FedSVD: Adaptive Orthogonalization for Private Federated Learning with LoRA**|Seanie Lee et.al.|[2505.12805](http://arxiv.org/abs/2505.12805)|null|
|**2025-05-18**|**$γ$ -FedHT: Stepsize-Aware Hard-Threshold Gradient Compression in Federated Learning**|Rongwei Lu et.al.|[2505.12479](http://arxiv.org/abs/2505.12479)|null|
|**2025-05-18**|**SecEmb: Sparsity-Aware Secure Federated Learning of On-Device Recommender System with Large Embedding**|Peihua Mai et.al.|[2505.12453](http://arxiv.org/abs/2505.12453)|**[link](https://github.com/nusioraprivacy/secemb)**|
|**2025-05-17**|**FL-PLAS: Federated Learning with Partial Layer Aggregation for Backdoor Defense Against High-Ratio Malicious Clients**|Jianyi Zhang et.al.|[2505.12019](http://arxiv.org/abs/2505.12019)|null|
|**2025-05-17**|**Incentivize Contribution and Learn Parameters Too: Federated Learning with Strategic Data Owners**|Drashthi Doshi et.al.|[2505.12010](http://arxiv.org/abs/2505.12010)|null|
|**2025-05-17**|**FedHQ: Hybrid Runtime Quantization for Federated Learning**|Zihao Zheng et.al.|[2505.11982](http://arxiv.org/abs/2505.11982)|null|
|**2025-05-16**|**Heterogeneity-Aware Client Sampling: A Unified Solution for Consistent Federated Learning**|Shudi Weng et.al.|[2505.11304](http://arxiv.org/abs/2505.11304)|null|
|**2025-05-16**|**Multi-Modal Multi-Task (M3T) Federated Foundation Models for Embodied AI: Potentials and Challenges for Edge Integration**|Kasra Borazjani et.al.|[2505.11191](http://arxiv.org/abs/2505.11191)|null|
|**2025-05-16**|**FedDuA: Doubly Adaptive Federated Learning**|Shokichi Takakura et.al.|[2505.11126](http://arxiv.org/abs/2505.11126)|null|
|**2025-05-16**|**Deep Latent Variable Model based Vertical Federated Learning with Flexible Alignment and Labeling Scenarios**|Kihun Hong et.al.|[2505.11035](http://arxiv.org/abs/2505.11035)|null|
|**2025-05-16**|**Nosy Layers, Noisy Fixes: Tackling DRAs in Federated Learning Systems using Explainable AI**|Meghali Nandi et.al.|[2505.10942](http://arxiv.org/abs/2505.10942)|null|
|**2025-05-16**|**Random Client Selection on Contrastive Federated Learning for Tabular Data**|Achmad Ginanjar et.al.|[2505.10759](http://arxiv.org/abs/2505.10759)|null|
|**2025-05-15**|**Defending the Edge: Representative-Attention for Mitigating Backdoor Attacks in Federated Learning**|Chibueze Peace Obioma et.al.|[2505.10297](http://arxiv.org/abs/2505.10297)|null|
|**2025-05-15**|**Cutting Through Privacy: A Hyperplane-Based Data Reconstruction Attack in Federated Learning**|Francesco Diana et.al.|[2505.10264](http://arxiv.org/abs/2505.10264)|null|
|**2025-05-15**|**Robust Federated Learning on Edge Devices with Domain Heterogeneity**|Huy Q. Le et.al.|[2505.10128](http://arxiv.org/abs/2505.10128)|null|
|**2025-05-18**|**Enhancing the Performance of Global Model by Improving the Adaptability of Local Models in Federated Learning**|Wujun Zhou et.al.|[2505.10125](http://arxiv.org/abs/2505.10125)|null|
|**2025-05-15**|**Sybil-based Virtual Data Poisoning Attacks in Federated Learning**|Changxun Zhu et.al.|[2505.09983](http://arxiv.org/abs/2505.09983)|null|
|**2025-05-14**|**Chisme: Fully Decentralized Differentiated Deep Learning for Edge Intelligence**|Harikrishna Kuttivelil et.al.|[2505.09854](http://arxiv.org/abs/2505.09854)|null|
|**2025-05-14**|**Robust Federated Learning with Confidence-Weighted Filtering and GAN-Based Completion under Noisy and Incomplete Data**|Alpaslan Gokcen et.al.|[2505.09733](http://arxiv.org/abs/2505.09733)|null|
|**2025-05-14**|**Energy-Efficient Federated Learning for AIoT using Clustering Methods**|Roberto Pereira et.al.|[2505.09704](http://arxiv.org/abs/2505.09704)|**[link](https://github.com/robertomatheuspp/clustering_ee_fl)**|
|**2025-05-14**|**Toward Fair Federated Learning under Demographic Disparities and Data Imbalance**|Qiming Wu et.al.|[2505.09295](http://arxiv.org/abs/2505.09295)|**[link](https://github.com/qimingwu/fedida)**|
|**2025-05-14**|**Ranking-Based At-Risk Student Prediction Using Federated Learning and Differential Features**|Shunsuke Yoneda et.al.|[2505.09287](http://arxiv.org/abs/2505.09287)|**[link](https://github.com/limu-research/2025-edm-fl)**|
|**2025-05-14**|**Toward Malicious Clients Detection in Federated Learning**|Zhihao Dou et.al.|[2505.09110](http://arxiv.org/abs/2505.09110)|null|
|**2025-05-13**|**Federated Large Language Models: Feasibility, Robustness, Security and Future Directions**|Wenhao Jiang et.al.|[2505.08830](http://arxiv.org/abs/2505.08830)|null|
|**2025-05-13**|**Modular Federated Learning: A Meta-Framework Perspective**|Frederico Vicente et.al.|[2505.08646](http://arxiv.org/abs/2505.08646)|null|
|**2025-05-13**|**FedRS-Bench: Realistic Federated Learning Datasets and Benchmarks in Remote Sensing**|Haodong Zhao et.al.|[2505.08325](http://arxiv.org/abs/2505.08325)|null|
|**2025-05-13**|**Privacy-Preserving Analytics for Smart Meter (AMI) Data: A Hybrid Approach to Comply with CPUC Privacy Regulations**|Benjamin Westrich et.al.|[2505.08237](http://arxiv.org/abs/2505.08237)|null|
|**2025-05-13**|**Multi-Layer Hierarchical Federated Learning with Quantization**|Seyed Mohammad Azimi-Abarghouyi et.al.|[2505.08145](http://arxiv.org/abs/2505.08145)|null|
|**2025-05-12**|**Sharp Gaussian approximations for Decentralized Federated Learning**|Soham Bonnerjee et.al.|[2505.08125](http://arxiv.org/abs/2505.08125)|null|
|**2025-05-12**|**A Federated Random Forest Solution for Secure Distributed Machine Learning**|Alexandre Cotorobai et.al.|[2505.08085](http://arxiv.org/abs/2505.08085)|**[link](https://github.com/ieeta-pt/fed_rf)**|
|**2025-05-12**|**Demo: A Practical Testbed for Decentralized Federated Learning on Physical Edge Devices**|Chao Feng et.al.|[2505.08033](http://arxiv.org/abs/2505.08033)|null|
|**2025-05-12**|**Enhancing Federated Learning with Kolmogorov-Arnold Networks: A Comparative Study Across Diverse Aggregation Strategies**|Yizhou Ma et.al.|[2505.07629](http://arxiv.org/abs/2505.07629)|null|
|**2025-05-12**|**Personalized Federated Learning under Model Dissimilarity Constraints**|Samuel Erickson et.al.|[2505.07575](http://arxiv.org/abs/2505.07575)|null|
|**2025-05-12**|**Adaptive Latent-Space Constraints in Personalized FL**|Sana Ayromlou et.al.|[2505.07525](http://arxiv.org/abs/2505.07525)|**[link](https://github.com/vectorinstitute/fl4health)**|
|**2025-05-12**|**FedIFL: A federated cross-domain diagnostic framework for motor-driven systems with inconsistent fault modes**|Zexiao Wang et.al.|[2505.07315](http://arxiv.org/abs/2505.07315)|null|
|**2025-05-12**|**Securing Genomic Data Against Inference Attacks in Federated Learning Environments**|Chetan Pathade et.al.|[2505.07188](http://arxiv.org/abs/2505.07188)|null|
|**2025-05-12**|**Empowering the Grid: Collaborative Edge Artificial Intelligence for Decentralized Energy Systems**|Eddie de Paula Jr et.al.|[2505.07170](http://arxiv.org/abs/2505.07170)|null|
|**2025-05-11**|**AugMixCloak: A Defense against Membership Inference Attacks via Image Transformation**|Heqing Ren et.al.|[2505.07149](http://arxiv.org/abs/2505.07149)|null|
|**2025-05-11**|**Standing Firm in 5G: A Single-Round, Dropout-Resilient Secure Aggregation for Federated Learning**|Yiwei Zhang et.al.|[2505.07148](http://arxiv.org/abs/2505.07148)|null|
|**2025-05-11**|**Empirical Analysis of Asynchronous Federated Learning on Heterogeneous Devices: Efficiency, Fairness, and Privacy Trade-offs**|Samaneh Mohammadi et.al.|[2505.07041](http://arxiv.org/abs/2505.07041)|null|
|**2025-05-11**|**Federated Learning with LoRA Optimized DeiT and Multiscale Patch Embedding for Secure Eye Disease Recognition**|Md. Naimur Asif Borno et.al.|[2505.06982](http://arxiv.org/abs/2505.06982)|null|
|**2025-05-09**|**Self-Supervised Federated GNSS Spoofing Detection with Opportunistic Data**|Wenjie Liu et.al.|[2505.06171](http://arxiv.org/abs/2505.06171)|null|
|**2025-05-09**|**Safe-EF: Error Feedback for Nonsmooth Constrained Optimization**|Rustem Islamov et.al.|[2505.06053](http://arxiv.org/abs/2505.06053)|null|
|**2025-05-09**|**DaringFed: A Dynamic Bayesian Persuasion Pricing for Online Federated Learning under Two-sided Incomplete Information**|Yun Xin et.al.|[2505.05842](http://arxiv.org/abs/2505.05842)|null|
|**2025-05-09**|**Efficient Full-Stack Private Federated Deep Learning with Post-Quantum Security**|Yiwei Zhang et.al.|[2505.05751](http://arxiv.org/abs/2505.05751)|null|
|**2025-05-08**|**Adaptive Biased User Scheduling for Heterogeneous Wireless Federate Learning Network**|Changxiang Wu et.al.|[2505.05231](http://arxiv.org/abs/2505.05231)|null|
|**2025-05-08**|**QualBench: Benchmarking Chinese LLMs with Localized Professional Qualifications for Vertical Domain Evaluation**|Mengze Hong et.al.|[2505.05225](http://arxiv.org/abs/2505.05225)|null|
|**2025-05-08**|**FedTDP: A Privacy-Preserving and Unified Framework for Trajectory Data Preparation via Federated Learning**|Zhihao Zeng et.al.|[2505.05155](http://arxiv.org/abs/2505.05155)|null|
|**2025-05-08**|**CacheFL: Efficient Federated Cache Model Fine-Tuning for Vision-Language Models**|Mengjun Yi et.al.|[2505.05130](http://arxiv.org/abs/2505.05130)|null|
|**2025-05-08**|**Balancing Client Participation in Federated Learning Using AoI**|Alireza Javani et.al.|[2505.05099](http://arxiv.org/abs/2505.05099)|null|
|**2025-05-11**|**Federated Deconfounding and Debiasing Learning for Out-of-Distribution Generalization**|Zhuang Qi et.al.|[2505.04979](http://arxiv.org/abs/2505.04979)|null|
|**2025-05-08**|**DFPL: Decentralized Federated Prototype Learning Across Heterogeneous Data Distributions**|Hongliang Zhang et.al.|[2505.04947](http://arxiv.org/abs/2505.04947)|null|
|**2025-05-08**|**FedRE: Robust and Effective Federated Learning with Privacy Preference**|Tianzhe Xiao et.al.|[2505.04889](http://arxiv.org/abs/2505.04889)|null|
|**2025-05-08**|**Federated Learning for Cyber Physical Systems: A Comprehensive Survey**|Minh K. Quan et.al.|[2505.04873](http://arxiv.org/abs/2505.04873)|null|
|**2025-05-07**|**Communication-Efficient Federated Fine-Tuning of Language Models via Dynamic Update Schedules**|Michail Theologitis et.al.|[2505.04535](http://arxiv.org/abs/2505.04535)|**[link](https://github.com/miketheologitis/FDA-Opt)**|
|**2025-05-07**|**FedBWO: Enhancing Communication Efficiency in Federated Learning**|Vahideh Hayyolalam et.al.|[2505.04435](http://arxiv.org/abs/2505.04435)|null|
|**2025-05-07**|**FRAIN to Train: A Fast-and-Reliable Solution for Decentralized Federated Learning**|Sanghyeon Park et.al.|[2505.04223](http://arxiv.org/abs/2505.04223)|**[link](https://github.com/BRAIN-chain/FRAIN)**|
|**2025-05-07**|**Privacy Challenges In Image Processing Applications**|Maneesha et.al.|[2505.04181](http://arxiv.org/abs/2505.04181)|null|
|**2025-05-06**|**Small-Scale-Fading-Aware Resource Allocation in Wireless Federated Learning**|Jiacheng Wang et.al.|[2505.03533](http://arxiv.org/abs/2505.03533)|null|
|**2025-05-05**|**Energy, Scalability, Data and Security in Massive IoT: Current Landscape and Future Directions**|Imane Cheikh et.al.|[2505.03036](http://arxiv.org/abs/2505.03036)|null|
|**2025-05-05**|**HSplitLoRA: A Heterogeneous Split Parameter-Efficient Fine-Tuning Framework for Large Language Models**|Zheng Lin et.al.|[2505.02795](http://arxiv.org/abs/2505.02795)|null|
|**2025-05-05**|**Lazy But Effective: Collaborative Personalized Federated Learning with Heterogeneous Data**|Ljubomir Rokvic et.al.|[2505.02540](http://arxiv.org/abs/2505.02540)|null|
|**2025-05-05**|**Bayesian Robust Aggregation for Federated Learning**|Aleksandr Karakulev et.al.|[2505.02490](http://arxiv.org/abs/2505.02490)|**[link](https://github.com/sciml-fl/bra-fl)**|
|**2025-05-05**|**Incentivizing Inclusive Contributions in Model Sharing Markets**|Enpei Zhang et.al.|[2505.02462](http://arxiv.org/abs/2505.02462)|null|
|**2025-05-05**|**Towards One-shot Federated Learning: Advances, Challenges, and Future Directions**|Flora Amato et.al.|[2505.02426](http://arxiv.org/abs/2505.02426)|**[link](https://github.com/Xtra-Computing/NIID-Bench)**|
|**2025-05-05**|**Sampling-based federated inference for M-estimators with non-smooth objective functions**|Xiudi Li et.al.|[2505.02356](http://arxiv.org/abs/2505.02356)|null|
|**2025-05-04**|**Bayesian Federated Cause-of-Death Classification and Quantification Under Distribution Shift**|Yu Zhu et.al.|[2505.02257](http://arxiv.org/abs/2505.02257)|null|
|**2025-05-04**|**A Survey on Privacy Risks and Protection in Large Language Models**|Kang Chen et.al.|[2505.01976](http://arxiv.org/abs/2505.01976)|null|
|**2025-05-03**|**Towards Trustworthy Federated Learning with Untrusted Participants**|Youssef Allouah et.al.|[2505.01874](http://arxiv.org/abs/2505.01874)|null|
|**2025-05-03**|**PQS-BFL: A Post-Quantum Secure Blockchain-based Federated Learning Framework**|Daniel Commey et.al.|[2505.01866](http://arxiv.org/abs/2505.01866)|null|
|**2025-05-02**|**A Self-Healing and Fault-Tolerant Cloud-based Digital Twin Processing Management Model**|Deepika Saxena et.al.|[2505.01215](http://arxiv.org/abs/2505.01215)|null|
|**2025-05-02**|**Secure Cluster-Based Hierarchical Federated Learning in Vehicular Networks**|M. Saeid HaghighiFard et.al.|[2505.01186](http://arxiv.org/abs/2505.01186)|null|
|**2025-05-02**|**Federated Adapter on Foundation Models: An Out-Of-Distribution Approach**|Yiyuan Yang et.al.|[2505.01075](http://arxiv.org/abs/2505.01075)|null|
|**2025-05-02**|**SemSpaceFL: A Collaborative Hierarchical Federated Learning Framework for Semantic Communication in 6G LEO Satellites**|Loc X. Nguyen et.al.|[2505.00966](http://arxiv.org/abs/2505.00966)|null|
|**2025-05-01**|**Open-Source LLM-Driven Federated Transformer for Predictive IoV Management**|Yazan Otoum et.al.|[2505.00651](http://arxiv.org/abs/2505.00651)|null|
|**2025-05-01**|**Communication-Efficient Wireless Federated Fine-Tuning for Large-Scale AI Models**|Bumjun Kim et.al.|[2505.00333](http://arxiv.org/abs/2505.00333)|null|
|**2025-05-01**|**FedEMA: Federated Exponential Moving Averaging with Negative Entropy Regularizer in Autonomous Driving**|Wei-Bin Kou et.al.|[2505.00318](http://arxiv.org/abs/2505.00318)|null|
|**2025-04-30**|**Online Federation For Mixtures of Proprietary Agents with Black-Box Encoders**|Xuwei Yang et.al.|[2505.00216](http://arxiv.org/abs/2505.00216)|null|
|**2025-04-30**|**Learning Heterogeneous Performance-Fairness Trade-offs in Federated Learning**|Rongguang Ye et.al.|[2504.21775](http://arxiv.org/abs/2504.21775)|null|
|**2025-04-30**|**Bilateral Differentially Private Vertical Federated Boosted Decision Trees**|Bokang Zhang et.al.|[2504.21739](http://arxiv.org/abs/2504.21739)|null|
|**2025-04-30**|**Whispers of Data: Unveiling Label Distributions in Federated Learning Through Virtual Client Simulation**|Zhixuan Ma et.al.|[2504.21436](http://arxiv.org/abs/2504.21436)|null|
|**2025-04-30**|**A Generalized Meta Federated Learning Framework with Theoretical Convergence Guarantees**|Mohammad Vahid Jamali et.al.|[2504.21327](http://arxiv.org/abs/2504.21327)|null|
|**2025-04-29**|**FedHERO: A Federated Learning Approach for Node Classification Task on Heterophilic Graphs**|Zihan Chen et.al.|[2504.21206](http://arxiv.org/abs/2504.21206)|null|
|**2025-04-29**|**Artificial Intelligence for Personalized Prediction of Alzheimer's Disease Progression: A Survey of Methods, Data Challenges, and Future Directions**|Gulsah Hancerliogullari Koksalmis et.al.|[2504.21189](http://arxiv.org/abs/2504.21189)|null|
|**2025-04-29**|**Federated One-Shot Learning with Data Privacy and Objective-Hiding**|Maximilian Egger et.al.|[2504.21182](http://arxiv.org/abs/2504.21182)|null|
|**2025-04-29**|**Relaxed Choices in Bottom-Up Asynchronous Multiparty Session Types**|Ivan Prokić et.al.|[2504.21108](http://arxiv.org/abs/2504.21108)|null|
|**2025-04-29**|**A Survey on Parameter-Efficient Fine-Tuning for Foundation Models in Federated Learning**|Jieming Bian et.al.|[2504.21099](http://arxiv.org/abs/2504.21099)|null|
|**2025-04-29**|**Hubs and Spokes Learning: Efficient and Scalable Collaborative Machine Learning**|Atul Sharma et.al.|[2504.20988](http://arxiv.org/abs/2504.20988)|null|
|**2025-04-29**|**FedMVP: Federated Multi-modal Visual Prompt Tuning for Vision-Language Models**|Mainak Singha et.al.|[2504.20860](http://arxiv.org/abs/2504.20860)|null|
|**2025-04-29**|**Federated learning, ethics, and the double black box problem in medical AI**|Joshua Hatherley et.al.|[2504.20656](http://arxiv.org/abs/2504.20656)|null|
|**2025-04-29**|**Learning and Generalization with Mixture Data**|Harsh Vardhan et.al.|[2504.20651](http://arxiv.org/abs/2504.20651)|null|
|**2025-04-29**|**ReCIT: Reconstructing Full Private Data from Gradient in Parameter-Efficient Fine-Tuning of Large Language Models**|Jin Xie et.al.|[2504.20570](http://arxiv.org/abs/2504.20570)|null|
|**2025-04-29**|**Clustering-Based Evolutionary Federated Multiobjective Optimization and Learning**|Chengui Xiao et.al.|[2504.20346](http://arxiv.org/abs/2504.20346)|null|
|**2025-04-28**|**FedCCL: Federated Clustered Continual Learning Framework for Privacy-focused Energy Forecasting**|Michael A. Helcig et.al.|[2504.20282](http://arxiv.org/abs/2504.20282)|null|
|**2025-04-28**|**Financial Data Analysis with Robust Federated Logistic Regression**|Kun Yang et.al.|[2504.20250](http://arxiv.org/abs/2504.20250)|**[link](https://github.com/kun0906/flr)**|
|**2025-04-28**|**Robust Federated Personalised Mean Estimation for the Gaussian Mixture Model**|Malhar A. Managoli et.al.|[2504.19955](http://arxiv.org/abs/2504.19955)|null|
|**2025-04-28**|**Convergence Analysis of Asynchronous Federated Learning with Gradient Compression for Non-Convex Optimization**|Diying Yang et.al.|[2504.19903](http://arxiv.org/abs/2504.19903)|null|
|**2025-04-28**|**Federated Out-of-Distribution Generalization: A Causal Augmentation View**|Runhui Zhang et.al.|[2504.19882](http://arxiv.org/abs/2504.19882)|null|
|**2025-04-28**|**A Unified Benchmark of Federated Learning with Kolmogorov-Arnold Networks for Medical Imaging**|Youngjoon Lee et.al.|[2504.19639](http://arxiv.org/abs/2504.19639)|**[link](https://github.com/yjlee22/fkan)**|
|**2025-04-28**|**Soft-Label Caching and Sharpening for Communication-Efficient Federated Distillation**|Kitsuya Azuma et.al.|[2504.19602](http://arxiv.org/abs/2504.19602)|**[link](https://github.com/kitsuyaazuma/scarlet)**|
|**2025-04-27**|**Harmonizing Generalization and Personalization in Ring-topology Decentralized Federated Learning**|Shunxin Guo et.al.|[2504.19103](http://arxiv.org/abs/2504.19103)|null|
|**2025-04-27**|**Privacy-Preserving Federated Embedding Learning for Localized Retrieval-Augmented Generation**|Qianren Mao et.al.|[2504.19101](http://arxiv.org/abs/2504.19101)|null|
|**2025-04-26**|**Federated Learning-based Semantic Segmentation for Lane and Object Detection in Autonomous Driving**|Gharbi Khamis Alshammari et.al.|[2504.18939](http://arxiv.org/abs/2504.18939)|null|
|**2025-04-26**|**UnifyFL: Enabling Decentralized Cross-Silo Federated Learning**|Sarang S et.al.|[2504.18916](http://arxiv.org/abs/2504.18916)|**[link](https://github.com/dash-lab-csis/unifyfl)**|
|**2025-04-25**|**Intelligent Attacks and Defense Methods in Federated Learning-enabled Energy-Efficient Wireless Networks**|Han Zhang et.al.|[2504.18519](http://arxiv.org/abs/2504.18519)|null|
|**2025-04-25**|**Switch-Based Multi-Part Neural Network**|Surajit Majumder et.al.|[2504.18241](http://arxiv.org/abs/2504.18241)|null|
|**2025-04-25**|**Privacy-Preserving Personalized Federated Learning for Distributed Photovoltaic Disaggregation under Statistical Heterogeneity**|Xiaolu Chen et.al.|[2504.18078](http://arxiv.org/abs/2504.18078)|null|
|**2025-04-25**|**Federated Client-tailored Adapter for Medical Image Segmentation**|Guyue Hu et.al.|[2504.18020](http://arxiv.org/abs/2504.18020)|null|
|**2025-04-25**|**Differential Privacy-Driven Framework for Enhancing Heart Disease Prediction**|Yazan Otoum et.al.|[2504.18007](http://arxiv.org/abs/2504.18007)|null|
|**2025-04-24**|**Federated Learning: A Survey on Privacy-Preserving Collaborative Intelligence**|Edward Collins et.al.|[2504.17703](http://arxiv.org/abs/2504.17703)|null|
|**2025-04-24**|**Decentralized Time Series Classification with ROCKET Features**|Bruno Casella et.al.|[2504.17617](http://arxiv.org/abs/2504.17617)|null|
|**2025-04-24**|**TACO: Tackling Over-correction in Federated Learning with Tailored Adaptive Correction**|Weijie Liu et.al.|[2504.17528](http://arxiv.org/abs/2504.17528)|null|
|**2025-04-23**|**An Adaptive ML Framework for Power Converter Monitoring via Federated Transfer Learning**|Panagiotis Kakosimos et.al.|[2504.16866](http://arxiv.org/abs/2504.16866)|null|
|**2025-04-23**|**Simplified Swarm Learning Framework for Robust and Scalable Diagnostic Services in Cancer Histopathology**|Yanjie Wu et.al.|[2504.16732](http://arxiv.org/abs/2504.16732)|null|
|**2025-04-23**|**Efficient Data Valuation Approximation in Federated Learning: A Sampling-based Approach**|Shuyue Wei et.al.|[2504.16668](http://arxiv.org/abs/2504.16668)|null|
|**2025-04-23**|**Federated EndoViT: Pretraining Vision Transformers via Federated Learning on Endoscopic Image Collections**|Max Kirchner et.al.|[2504.16612](http://arxiv.org/abs/2504.16612)|null|
|**2025-04-23**|**Federated Learning of Low-Rank One-Shot Image Detection Models in Edge Devices with Scalable Accuracy and Compute Complexity**|Abdul Hannaan et.al.|[2504.16515](http://arxiv.org/abs/2504.16515)|null|
|**2025-04-23**|**Private Federated Learning using Preference-Optimized Synthetic Data**|Charlie Hou et.al.|[2504.16438](http://arxiv.org/abs/2504.16438)|**[link](https://github.com/meiyuw/popri)**|
|**2025-04-23**|**DP2FL: Dual Prompt Personalized Federated Learning in Foundation Models**|Ying Chang et.al.|[2504.16357](http://arxiv.org/abs/2504.16357)|null|
|**2025-04-22**|**Towards a Distributed Federated Learning Aggregation Placement using Particle Swarm Intelligence**|Amir Ali-Pour et.al.|[2504.16227](http://arxiv.org/abs/2504.16227)|null|
|**2025-04-22**|**LLMs meet Federated Learning for Scalable and Secure IoT Management**|Yazan Otoum et.al.|[2504.16032](http://arxiv.org/abs/2504.16032)|null|
|**2025-04-22**|**OPUS-VFL: Incentivizing Optimal Privacy-Utility Tradeoffs in Vertical Federated Learning**|Sindhuja Madabushi et.al.|[2504.15995](http://arxiv.org/abs/2504.15995)|null|
|**2025-04-22**|**Achieving Distributive Justice in Federated Learning via Uncertainty Quantification**|Alycia Carey et.al.|[2504.15924](http://arxiv.org/abs/2504.15924)|**[link](https://github.com/alycia-noel/udj-fl)**|
|**2025-04-22**|**CARE: Compatibility-Aware Incentive Mechanisms for Federated Learning with Budgeted Requesters**|Xiang Liu et.al.|[2504.15847](http://arxiv.org/abs/2504.15847)|null|
|**2025-04-22**|**Collaborative Split Federated Learning with Parallel Training and Aggregation**|Yiannis Papageorgiou et.al.|[2504.15724](http://arxiv.org/abs/2504.15724)|null|
|**2025-04-22**|**Trusted Compute Units: A Framework for Chained Verifiable Computations**|Fernando Castillo et.al.|[2504.15717](http://arxiv.org/abs/2504.15717)|null|
|**2025-04-22**|**TrojanDam: Detection-Free Backdoor Defense in Federated Learning through Proactive Model Robustification utilizing OOD Data**|Yanbo Dai et.al.|[2504.15674](http://arxiv.org/abs/2504.15674)|null|
|**2025-04-22**|**Federated Latent Factor Learning for Recovering Wireless Sensor Networks Signal with Privacy-Preserving**|Chengjun Yu et.al.|[2504.15525](http://arxiv.org/abs/2504.15525)|null|
|**2025-04-21**|**FedFetch: Faster Federated Learning with Adaptive Downstream Prefetching**|Qifan Yan et.al.|[2504.15366](http://arxiv.org/abs/2504.15366)|**[link](https://github.com/distributedml/fedfetch)**|
|**2025-04-21**|**Bayesian Federated Learning for Continual Training**|Usevalad Milasheuski et.al.|[2504.15328](http://arxiv.org/abs/2504.15328)|null|
|**2025-04-21**|**Federated Latent Factor Model for Bias-Aware Recommendation with Privacy-Preserving**|Junxiang Gao et.al.|[2504.15090](http://arxiv.org/abs/2504.15090)|null|
|**2025-04-21**|**Aligning Beam with Imbalanced Multi-modality: A Generative Federated Learning Approach**|Jiahui Liang et.al.|[2504.14835](http://arxiv.org/abs/2504.14835)|null|
|**2025-04-20**|**Learning Critically: Selective Self Distillation in Federated Learning on Non-IID Data**|Yuting He et.al.|[2504.14694](http://arxiv.org/abs/2504.14694)|null|
|**2025-04-20**|**Efficient Federated Split Learning for Large Language Models over Communication Networks**|Kai Zhao et.al.|[2504.14667](http://arxiv.org/abs/2504.14667)|null|
|**2025-04-20**|**GENE-FL: Gene-Driven Parameter-Efficient Dynamic Federated Learning**|Shunxin Guo et.al.|[2504.14628](http://arxiv.org/abs/2504.14628)|null|
|**2025-04-19**|**PEFT A2Z: Parameter-Efficient Fine-Tuning Survey for Large Language and Vision Models**|Nusrat Jahan Prottasha et.al.|[2504.14117](http://arxiv.org/abs/2504.14117)|null|
|**2025-04-18**|**SFL-LEO: Asynchronous Split-Federated Learning Design for LEO Satellite-Ground Network Framework**|Jiasheng Wu et.al.|[2504.13479](http://arxiv.org/abs/2504.13479)|null|
|**2025-04-18**|**Stratify: Rethinking Federated Learning for Non-IID Data through Balanced Sampling**|Hui Yeok Wong et.al.|[2504.13462](http://arxiv.org/abs/2504.13462)|null|
|**2025-04-17**|**VLLFL: A Vision-Language Model Based Lightweight Federated Learning Framework for Smart Agriculture**|Long Li et.al.|[2504.13365](http://arxiv.org/abs/2504.13365)|null|
|**2025-04-21**|**A Client-level Assessment of Collaborative Backdoor Poisoning in Non-IID Federated Learning**|Phung Lai et.al.|[2504.12875](http://arxiv.org/abs/2504.12875)|null|
|**2025-04-19**|**FedX: Adaptive Model Decomposition and Quantization for IoT Federated Learning**|Phung Lai et.al.|[2504.12849](http://arxiv.org/abs/2504.12849)|null|
|**2025-04-17**|**Decentralized Nonconvex Composite Federated Learning with Gradient Tracking and Momentum**|Yuan Zhou et.al.|[2504.12742](http://arxiv.org/abs/2504.12742)|null|
|**2025-04-18**|**The Athenian Academy: A Seven-Layer Architecture Model for Multi-Agent Systems**|Lidong Zhai et.al.|[2504.12735](http://arxiv.org/abs/2504.12735)|null|
|**2025-04-17**|**Local Data Quantity-Aware Weighted Averaging for Federated Learning with Dishonest Clients**|Leming Wu et.al.|[2504.12577](http://arxiv.org/abs/2504.12577)|null|
|**2025-04-16**|**Communication Optimization for Decentralized Learning atop Bandwidth-limited Edge Networks**|Tingyang Sun et.al.|[2504.12210](http://arxiv.org/abs/2504.12210)|null|
|**2025-04-16**|**Battery-aware Cyclic Scheduling in Energy-harvesting Federated Learning**|Eunjeong Jeong et.al.|[2504.12181](http://arxiv.org/abs/2504.12181)|null|
|**2025-04-16**|**FedEPA: Enhancing Personalization and Modality Alignment in Multimodal Federated Learning**|Yu Zhang et.al.|[2504.12025](http://arxiv.org/abs/2504.12025)|null|
|**2025-04-16**|**FedCanon: Non-Convex Composite Federated Learning with Efficient Proximal Operation on Heterogeneous Data**|Yuan Zhou et.al.|[2504.11903](http://arxiv.org/abs/2504.11903)|null|
|**2025-04-16**|**Benchmarking Mutual Information-based Loss Functions in Federated Learning**|Sarang S et.al.|[2504.11877](http://arxiv.org/abs/2504.11877)|null|
|**2025-04-16**|**Federated Spectral Graph Transformers Meet Neural Ordinary Differential Equations for Non-IID Graphs**|Kishan Gurumurthy et.al.|[2504.11808](http://arxiv.org/abs/2504.11808)|**[link](https://github.com/springwiz11/fed-gnodeformer)**|
|**2025-04-17**|**Selective Attention Federated Learning: Improving Privacy and Efficiency for Clinical Text Classification**|Yue Li et.al.|[2504.11793](http://arxiv.org/abs/2504.11793)|null|
|**2025-04-15**|**Diversity-Driven Learning: Tackling Spurious Correlations and Data Heterogeneity in Federated Models**|Gergely D. Németh et.al.|[2504.11216](http://arxiv.org/abs/2504.11216)|null|
|**2025-04-15**|**FLSSM: A Federated Learning Storage Security Model with Homomorphic Encryption**|Yang Li et.al.|[2504.11088](http://arxiv.org/abs/2504.11088)|null|
|**2025-04-15**|**ICAFS: Inter-Client-Aware Feature Selection for Vertical Federated Learning**|Ruochen Jin et.al.|[2504.10851](http://arxiv.org/abs/2504.10851)|null|
|**2025-04-15**|**FHBench: Towards Efficient and Personalized Federated Learning for Multimodal Healthcare**|Penghao Wang et.al.|[2504.10817](http://arxiv.org/abs/2504.10817)|**[link](https://github.com/wph6/fhbench)**|
|**2025-04-14**|**Optimising Intrusion Detection Systems in Cloud-Edge Continuum with Knowledge Distillation for Privacy-Preserving and Efficient Communication**|Soad Almabdy et.al.|[2504.10698](http://arxiv.org/abs/2504.10698)|null|
|**2025-04-14**|**Privacy-Preserving Distributed Link Predictions Among Peers in Online Classrooms Using Federated Learning**|Anurata Prabha Hridi et.al.|[2504.10456](http://arxiv.org/abs/2504.10456)|null|
|**2025-04-14**|**Satellite Federated Fine-Tuning for Foundation Models in Space Computing Power Networks**|Yan zhu et.al.|[2504.10403](http://arxiv.org/abs/2504.10403)|null|
|**2025-04-14**|**Undermining Federated Learning Accuracy in EdgeIoT via Variational Graph Auto-Encoders**|Kai Li et.al.|[2504.10067](http://arxiv.org/abs/2504.10067)|null|
|**2025-04-14**|**FedRecon: Missing Modality Reconstruction in Distributed Heterogeneous Environments**|Junming Liu et.al.|[2504.09941](http://arxiv.org/abs/2504.09941)|null|
|**2025-04-14**|**Accelerating Differentially Private Federated Learning via Adaptive Extrapolation**|Shokichi Takakura et.al.|[2504.09850](http://arxiv.org/abs/2504.09850)|null|
|**2025-04-14**|**Multi-task Federated Learning with Encoder-Decoder Structure: Enabling Collaborative Learning Across Different Tasks**|Jingxuan Zhou et.al.|[2504.09800](http://arxiv.org/abs/2504.09800)|null|
|**2025-04-13**|**SegOTA: Accelerating Over-the-Air Federated Learning with Segmented Transmission**|Chong Zhang et.al.|[2504.09745](http://arxiv.org/abs/2504.09745)|null|
|**2025-04-13**|**FSSUAVL: A Discriminative Framework using Vision Models for Federated Self-Supervised Audio and Image Understanding**|Yasar Abbas Ur Rehman et.al.|[2504.09516](http://arxiv.org/abs/2504.09516)|null|
|**2025-04-12**|**Query-based Knowledge Transfer for Heterogeneous Learning Environments**|Norah Alballa et.al.|[2504.09205](http://arxiv.org/abs/2504.09205)|null|
|**2025-04-12**|**Deploying Large AI Models on Resource-Limited Devices with Split Federated Learning**|Xianke Qiang et.al.|[2504.09114](http://arxiv.org/abs/2504.09114)|null|
|**2025-04-11**|**Boosting multi-demographic federated learning for chest x-ray analysis using general-purpose self-supervised representations**|Mahshad Lotfinia et.al.|[2504.08584](http://arxiv.org/abs/2504.08584)|null|
|**2025-04-11**|**Explainability and Continual Learning meet Federated Learning at the Network Edge**|Thomas Tsouparopoulos et.al.|[2504.08536](http://arxiv.org/abs/2504.08536)|null|
|**2025-04-11**|**An Adaptive Clustering Scheme for Client Selections in Communication-Efficient Federated Learning**|Yan-Ann Chen et.al.|[2504.08356](http://arxiv.org/abs/2504.08356)|null|
|**2025-04-11**|**The More is not the Merrier: Investigating the Effect of Client Size on Federated Learning**|Eleanor Wallach et.al.|[2504.08198](http://arxiv.org/abs/2504.08198)|**[link](https://github.com/eleanor-w/kci_for_fl)**|
|**2025-04-10**|**Traversal Learning Coordination For Lossless And Efficient Distributed Learning**|Erdenebileg Batbaatar et.al.|[2504.07471](http://arxiv.org/abs/2504.07471)|null|
|**2025-04-09**|**FedMerge: Federated Personalization via Model Merging**|Shutong Chen et.al.|[2504.06768](http://arxiv.org/abs/2504.06768)|null|
|**2025-04-08**|**Federated Neural Architecture Search with Model-Agnostic Meta Learning**|Xinyuan Huang et.al.|[2504.06457](http://arxiv.org/abs/2504.06457)|null|
|**2025-04-08**|**Decentralized Federated Domain Generalization with Style Sharing: A Formal Modeling and Convergence Analysis**|Shahryar Zehtabi et.al.|[2504.06235](http://arxiv.org/abs/2504.06235)|null|
|**2025-04-08**|**FedFeat+: A Robust Federated Learning Framework Through Federated Aggregation and Differentially Private Feature-Based Classifier Retraining**|Mrityunjoy Gain et.al.|[2504.06004](http://arxiv.org/abs/2504.06004)|null|
|**2025-04-08**|**Federated Unlearning Made Practical: Seamless Integration via Negated Pseudo-Gradients**|Alessio Mora et.al.|[2504.05822](http://arxiv.org/abs/2504.05822)|**[link](https://github.com/alessiomora/puf_unlearning)**|
|**2025-04-08**|**FedEFC: Federated Learning Using Enhanced Forward Correction Against Noisy Labels**|Seunghun Yu et.al.|[2504.05615](http://arxiv.org/abs/2504.05615)|null|
|**2025-04-07**|**Federated Hierarchical Reinforcement Learning for Adaptive Traffic Signal Control**|Yongjie Fu et.al.|[2504.05553](http://arxiv.org/abs/2504.05553)|null|
|**2025-04-07**|**Embedded Federated Feature Selection with Dynamic Sparse Training: Balancing Accuracy-Cost Tradeoffs**|Afsaneh Mahanipour et.al.|[2504.05245](http://arxiv.org/abs/2504.05245)|null|
|**2025-04-07**|**Federated Learning for Medical Image Classification: A Comprehensive Benchmark**|Zhekai Zhou et.al.|[2504.05238](http://arxiv.org/abs/2504.05238)|null|
|**2025-04-07**|**SparsyFed: Sparse Adaptive Federated Training**|Adriano Guastella et.al.|[2504.05153](http://arxiv.org/abs/2504.05153)|**[link](https://github.com/aguastella/sparsyfed)**|
|**2025-04-08**|**Towards Optimal Heterogeneous Client Sampling in Multi-Model Federated Learning**|Haoran Zhang et.al.|[2504.05138](http://arxiv.org/abs/2504.05138)|null|
|**2025-04-07**|**Decentralized Semantic Federated Learning for Real-Time Public Safety Tasks: Challenges, Methods, and Directions**|Baosheng Li et.al.|[2504.05107](http://arxiv.org/abs/2504.05107)|null|
|**2025-04-07**|**FedSAUC: A Similarity-Aware Update Control for Communication-Efficient Federated Learning in Edge Computing**|Ming-Lun Lee et.al.|[2504.04867](http://arxiv.org/abs/2504.04867)|null|
|**2025-04-07**|**Federated Learning over 5G, WiFi, and Ethernet: Measurements and Evaluation**|Robert J. Hayek et.al.|[2504.04678](http://arxiv.org/abs/2504.04678)|**[link](https://github.com/Net-X-Research-Group/federated_learning_testbed)**|
|**2025-04-06**|**A Novel Algorithm for Personalized Federated Learning: Knowledge Distillation with Weighted Combination Loss**|Hengrui Hu et.al.|[2504.04642](http://arxiv.org/abs/2504.04642)|null|
|**2025-04-06**|**WeiDetect: Weibull Distribution-Based Defense against Poisoning Attacks in Federated Learning for Network Intrusion Detection Systems**|Sameera K. M. et.al.|[2504.04367](http://arxiv.org/abs/2504.04367)|null|
|**2025-04-05**|**Scaling Federated Learning Solutions with Kubernetes for Synthesizing Histopathology Images**|Andrei-Alexandru Preda et.al.|[2504.04130](http://arxiv.org/abs/2504.04130)|**[link](https://github.com/pandrei7/paper-synthesizing-histopathology)**|
|**2025-04-04**|**Hierarchical Knowledge Structuring for Effective Federated Learning in Heterogeneous Environments**|Wai Fong Tam et.al.|[2504.03505](http://arxiv.org/abs/2504.03505)|null|
|**2025-04-04**|**PPFPL: Cross-silo Privacy-preserving Federated Prototype Learning Against Data Poisoning Attacks on Non-IID Data**|Hongliang Zhang et.al.|[2504.03173](http://arxiv.org/abs/2504.03173)|null|
|**2025-04-03**|**Integrating Identity-Based Identification against Adaptive Adversaries in Federated Learning**|Jakub Kacper Szelag et.al.|[2504.03077](http://arxiv.org/abs/2504.03077)|null|
|**2025-04-03**|**Improving Efficiency in Federated Learning with Optimized Homomorphic Encryption**|Feiran Yang et.al.|[2504.03002](http://arxiv.org/abs/2504.03002)|null|
|**2025-04-03**|**Enhancing Air Quality Monitoring: A Brief Review of Federated Learning Advances**|Sara Yarham et.al.|[2504.02909](http://arxiv.org/abs/2504.02909)|null|
|**2025-04-03**|**Tree-based Models for Vertical Federated Learning: A Survey**|Bingchen Qian et.al.|[2504.02285](http://arxiv.org/abs/2504.02285)|null|
|**2025-04-03**|**Secure Generalization through Stochastic Bidirectional Parameter Updates Using Dual-Gradient Mechanism**|Shourya Goel et.al.|[2504.02213](http://arxiv.org/abs/2504.02213)|null|
|**2025-04-02**|**Like Oil and Water: Group Robustness Methods and Poisoning Defenses May Be at Odds**|Michael-Andrei Panaitescu-Liess et.al.|[2504.02142](http://arxiv.org/abs/2504.02142)|null|
|**2025-04-02**|**On Model Protection in Federated Learning against Eavesdropping Attacks**|Dipankar Maity et.al.|[2504.02114](http://arxiv.org/abs/2504.02114)|null|
|**2025-04-02**|**Efficient Federated Learning Tiny Language Models for Mobile Network Feature Prediction**|Daniel Becking et.al.|[2504.01947](http://arxiv.org/abs/2504.01947)|null|
|**2025-04-02**|**Client Selection in Federated Learning with Data Heterogeneity and Network Latencies**|Harsh Vardhan et.al.|[2504.01921](http://arxiv.org/abs/2504.01921)|null|
|**2025-04-02**|**CO-DEFEND: Continuous Decentralized Federated Learning for Secure DoH-Based Threat Detection**|Diego Cajaraville-Aboy et.al.|[2504.01882](http://arxiv.org/abs/2504.01882)|**[link](https://gitlab.com/compromise3/co-defend)**|
|**2025-04-02**|**A Randomized Zeroth-Order Hierarchical Framework for Heterogeneous Federated Learning**|Yuyang Qiu et.al.|[2504.01839](http://arxiv.org/abs/2504.01839)|null|
|**2025-04-02**|**A Two-Timescale Approach for Wireless Federated Learning with Parameter Freezing and Power Control**|Jinhao Ouyang et.al.|[2504.01752](http://arxiv.org/abs/2504.01752)|null|
|**2025-04-02**|**Sky of Unlearning (SoUL): Rewiring Federated Machine Unlearning via Selective Pruning**|Md Mahabub Uz Zaman et.al.|[2504.01705](http://arxiv.org/abs/2504.01705)|null|
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
|**2025-03-28**|**Route-and-Aggregate Decentralized Federated Learning Under Communication Errors**|Weicai Li et.al.|[2503.22186](http://arxiv.org/abs/2503.22186)|**[link](https://github.com/jasminebear2024/RouteAndAggregate)**|
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
|**2025-03-26**|**AIGC-assisted Federated Learning for Edge Intelligence: Architecture Design, Research Challenges and Future Directions**|Xianke Qiang et.al.|[2503.20166](http://arxiv.org/abs/2503.20166)|**[link](https://github.com/XiankeQiang/AdaptiveSplitFederatedLearning)**|
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
|**2025-03-20**|**FedAWA: Adaptive Optimization of Aggregation Weights in Federated Learning Using Client Vectors**|Changlong Shi et.al.|[2503.15842](http://arxiv.org/abs/2503.15842)|**[link](https://github.com/changlongshi/fedawa)**|
|**2025-03-20**|**Energy-Efficient Federated Learning and Migration in Digital Twin Edge Networks**|Yuzhi Zhou et.al.|[2503.15822](http://arxiv.org/abs/2503.15822)|null|
|**2025-03-20**|**Communication Efficient Federated Learning with Linear Convergence on Heterogeneous Data**|Jie Liu et.al.|[2503.15804](http://arxiv.org/abs/2503.15804)|null|
|**2025-03-19**|**Reducing Communication Overhead in Federated Learning for Network Anomaly Detection with Adaptive Client Selection**|William Marfo et.al.|[2503.15448](http://arxiv.org/abs/2503.15448)|null|
|**2025-03-19**|**Federated Continual 3D Segmentation With Single-round Communication**|Can Peng et.al.|[2503.15414](http://arxiv.org/abs/2503.15414)|null|
|**2025-03-19**|**FedSCA: Federated Tuning with Similarity-guided Collaborative Aggregation for Heterogeneous Medical Image Segmentation**|Yumin Zhang et.al.|[2503.15390](http://arxiv.org/abs/2503.15390)|null|
|**2025-03-19**|**FedBEns: One-Shot Federated Learning based on Bayesian Ensemble**|Jacopo Talpini et.al.|[2503.15367](http://arxiv.org/abs/2503.15367)|null|
|**2025-03-19**|**Online federated learning framework for classification**|Wenxing Guo et.al.|[2503.15210](http://arxiv.org/abs/2503.15210)|null|
|**2025-03-19**|**Global Group Fairness in Federated Learning via Function Tracking**|Yves Rychener et.al.|[2503.15163](http://arxiv.org/abs/2503.15163)|**[link](https://github.com/yvesrychener/Fair-FL)**|
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
|**2025-03-03**|**GRAIN: Exact Graph Reconstruction from Gradients**|Maria Drencheva et.al.|[2503.01838](http://arxiv.org/abs/2503.01838)|**[link](https://github.com/insait-institute/grain)**|
|**2025-03-03**|**FLAME: A Federated Learning Benchmark for Robotic Manipulation**|Santiago Bou Betran et.al.|[2503.01729](http://arxiv.org/abs/2503.01729)|null|
|**2025-03-03**|**Heterogeneity Matters even More in Distributed Learning: Study from Generalization Perspective**|Masoud Kavian et.al.|[2503.01598](http://arxiv.org/abs/2503.01598)|null|
|**2025-03-03**|**MoCFL: Mobile Cluster Federated Learning Framework for Highly Dynamic Network**|Kai Fang et.al.|[2503.01557](http://arxiv.org/abs/2503.01557)|null|
|**2025-03-03**|**MAB-Based Channel Scheduling for Asynchronous Federated Learning in Non-Stationary Environments**|Zhiyin Li et.al.|[2503.01324](http://arxiv.org/abs/2503.01324)|null|
|**2025-03-02**|**Patient-Level Anatomy Meets Scanning-Level Physics: Personalized Federated Low-Dose CT Denoising Empowered by Large Language Model**|Ziyuan Yang et.al.|[2503.00908](http://arxiv.org/abs/2503.00908)|null|
|**2025-02-28**|**QFAL: Quantum Federated Adversarial Learning**|Walid El Maouaki et.al.|[2502.21171](http://arxiv.org/abs/2502.21171)|null|
|**2025-02-28**|**FedDyMem: Efficient Federated Learning with Dynamic Memory and Memory-Reduce for Unsupervised Image Anomaly Detection**|Silin Chen et.al.|[2502.21012](http://arxiv.org/abs/2502.21012)|null|
|**2025-02-28**|**Managing Federated Learning on Decentralized Infrastructures as a Reputation-based Collaborative Workflow**|Yuandou Wang et.al.|[2502.20882](http://arxiv.org/abs/2502.20882)|**[link](https://github.com/CWL-FLOps/DecentralizedFL-CWL)**|
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
|**2025-02-06**|**Generative Autoregressive Transformers for Model-Agnostic Federated MRI Reconstruction**|Valiyeh A. Nezhad et.al.|[2502.04521](http://arxiv.org/abs/2502.04521)|**[link](https://github.com/icon-lab/FedGAT)**|
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
|**2024-12-04**|**Beyond Local Sharpness: Communication-Efficient Global Sharpness-aware Minimization for Federated Learning**|Debora Caldarola et.al.|[2412.03752](http://arxiv.org/abs/2412.03752)|**[link](https://github.com/pietrocagnasso/fedgloss)**|
|**2024-12-04**|**Adaptive Personalized Over-the-Air Federated Learning with Reflecting Intelligent Surfaces**|Jiayu Mao et.al.|[2412.03514](http://arxiv.org/abs/2412.03514)|null|
|**2024-12-04**|**Reactive Orchestration for Hierarchical Federated Learning Under a Communication Cost Budget**|Ivan Čilić et.al.|[2412.03385](http://arxiv.org/abs/2412.03385)|**[link](https://github.com/AIoTwin/fl-orchestrator)**|
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
|**2024-11-19**|**Attribute Inference Attacks for Federated Regression Tasks**|Francesco Diana et.al.|[2411.12697](http://arxiv.org/abs/2411.12697)|**[link](https://github.com/francescodiana99/fedkit-learn)**|
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
|**2024-11-09**|**TinyML NLP Approach for Semantic Wireless Sentiment Classification**|Ahmed Y. Radwan et.al.|[2411.06291](http://arxiv.org/abs/2411.06291)|**[link](https://github.com/ahmedradwan02/tinyeco2ai-nlp)**|
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
|**2024-11-06**|**FedRISE: Rating Induced Sign Election of Gradients for Byzantine Tolerant Federated Aggregation**|Joseph Geo Benjamin et.al.|[2411.03861](http://arxiv.org/abs/2411.03861)|**[link](https://github.com/josephgeobenjamin/fedseca-byzantinetolerance)**|
|**2024-11-06**|**Overcoming label shift in targeted federated learning**|Edvin Listo Zec et.al.|[2411.03799](http://arxiv.org/abs/2411.03799)|null|
|**2024-11-06**|**Optimal Defenses Against Gradient Reconstruction Attacks**|Yuxiao Chen et.al.|[2411.03746](http://arxiv.org/abs/2411.03746)|**[link](https://github.com/cyx78/optimal_defenses_against_gradient_reconstruction_attacks)**|
|**2024-11-06**|**NeurIPS 2023 Competition: Privacy Preserving Federated Learning Document VQA**|Marlon Tobaben et.al.|[2411.03730](http://arxiv.org/abs/2411.03730)|null|
|**2024-11-06**|**Domain Generalization for Cross-Receiver Radio Frequency Fingerprint Identification**|Ying Zhang et.al.|[2411.03636](http://arxiv.org/abs/2411.03636)|null|
|**2024-11-06**|**Towards Personalized Federated Learning via Comprehensive Knowledge Distillation**|Pengju Wang et.al.|[2411.03569](http://arxiv.org/abs/2411.03569)|null|

<p align=right>(<a href=#updated-on-20250525>back to top</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[contributors-url]: https://github.com/Vincentqyw/cv-arxiv-daily/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[forks-url]: https://github.com/Vincentqyw/cv-arxiv-daily/network/members
[stars-shield]: https://img.shields.io/github/stars/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[stars-url]: https://github.com/Vincentqyw/cv-arxiv-daily/stargazers
[issues-shield]: https://img.shields.io/github/issues/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[issues-url]: https://github.com/Vincentqyw/cv-arxiv-daily/issues

