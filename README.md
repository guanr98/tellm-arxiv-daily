[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## Updated on 2025.02.24
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
|**2025-02-20**|**I-MCTS: Enhancing Agentic AutoML via Introspective Monte Carlo Tree Search**|Zujie Liang et.al.|[2502.14693](http://arxiv.org/abs/2502.14693)|null|最近在大型语言模型（LLM）方面的进展显示出在自动化机器学习任务中的巨大潜力。然而，现有的基于LLM的代理在代码生成方面往往存在多样性低和质量不佳的问题。虽然近期的研究引入了蒙特卡洛树搜索（MCTS）来解决这些问题，但在生成思想的质量和多样性以及用于节点选择的标量值反馈机制方面仍然存在局限性。在这项研究中，我们提出了一种新的方法——内省式蒙特卡洛树搜索（I-MCTS），该方法通过一个内省过程迭代地扩展树节点，仔细分析来自父节点和兄弟节点的解决方案和结果。这促进了搜索树中节点的持续改进，从而增强了整体决策过程。此外，我们集成了一个基于大型语言模型（LLM）的价值模型，以便在进行全面计算展开之前直接评估每个节点的解决方案。我们实现了一种混合奖励机制，可以无缝地将Q值从LLM估计分数转换为实际性能分数，从而使高质量的节点能够更早被遍历。应用于各种机器学习任务时，我们的方法相比强大的开源AutoML代理展示了6%的绝对性能提升，证明了其在增强自动代理AutoML系统方面的有效性。|
|**2025-02-20**|**InstructAgent: Building User Controllable Recommender via LLM Agent**|Wujiang Xu et.al.|[2502.14662](http://arxiv.org/abs/2502.14662)|null|传统的推荐系统通常采用用户-平台模式，在这种模式下，用户直接暴露在平台推荐算法的控制之下。然而，推荐算法的缺陷可能使用户在这种模式下处于非常脆弱的位置。首先，许多复杂的模型通常是基于商业目标设计的，侧重于平台的利益，这可能妨碍它们保护和捕捉用户真实兴趣的能力。其次，这些模型通常使用所有用户的数据进行优化，可能会忽视个别用户的偏好。由于这些缺点，用户在传统用户-平台直接曝光模式下可能会遇到多种不利情况，如对推荐系统的缺乏控制、可能受到平台操纵、回音室效应或因活跃用户在协同学习中的主导地位而导致较少活跃用户的个性化不足。因此，迫切需要开发一种新的模式来保护用户利益并缓解这些问题。最近，一些研究人员引入了大语言模型代理来模拟用户行为，但这些方法主要旨在优化平台侧的表现，未能解决推荐系统的核心问题。为了解决这些局限性，我们提出了一种新的用户-代理-平台模式，在这种模式下，代理作为用户与推荐系统之间的保护屏障，实现间接曝光。为此，我们首先构建了四个推荐数据集，记作 $\dataset$ ，并为每条记录提供了用户指令。|
|**2025-02-20**|**Plan-over-Graph: Towards Parallelable LLM Agent Schedule**|Shiqi Zhang et.al.|[2502.14563](http://arxiv.org/abs/2502.14563)|null|大型语言模型（LLM）在任务规划的推理方面展现了卓越的能力。然而，在并行调度方面的挑战仍然未被充分探索。本文介绍了一种新的范式，即基于图的规划，其中模型首先将现实生活中的文本任务分解为可执行的子任务，并构建一个抽象的任务图。然后，模型将该任务图作为输入进行理解，并生成一个并行执行的计划。为了增强复杂且可扩展图的规划能力，我们设计了一个自动化且可控的流程来生成合成图，并提出了一种两阶段训练方案。实验结果表明，我们的基于图的规划方法显著提高了基于API的LLM和可训练开源LLM的任务性能。通过将复杂任务标准化为图，我们的方法自然支持并行执行，展示了全局效率。代码和数据可在https://github.com/zsq259/Plan-over-Graph获取。|
|**2025-02-20**|**MLGym: A New Framework and Benchmark for Advancing AI Research Agents**|Deepak Nathani et.al.|[2502.14499](http://arxiv.org/abs/2502.14499)|null|我们介绍了Meta MLGym和MLGym-Bench，这是一个新的框架和基准，用于评估和发展在AI研究任务上的大型语言模型（LLM）代理。这是第一个针对机器学习（ML）任务的Gym环境，使研究强化学习（RL）算法以训练此类代理成为可能。MLGym-bench包括13个来自不同领域的多样化且开放式的AI研究任务，如计算机视觉、自然语言处理、强化学习和博弈论。解决这些任务需要现实世界中的AI研究技能，例如生成新想法和假设、创建和处理数据、实现ML方法、训练模型、运行实验、分析结果，并通过这一过程迭代以改进给定任务。我们在我们的基准上评估了一些前沿的大规模语言模型，如Claude-3.5-Sonnet、Llama-3.1 405B、GPT-4o、o1-preview和Gemini-1.5 Pro。我们的MLGym框架使得添加新任务、集成和评估模型或代理、大规模生成合成数据以及开发用于训练代理执行AI研究任务的新学习算法变得容易。我们发现当前的前沿模型可以在给定基线上有所改进，通常是通过找到更好的超参数，但它们不会生成新颖的假设、算法、架构或实质性的改进。我们将我们的框架和基准开源，以促进未来关于提升LLM代理的AI研究能力的研究。|
|**2025-02-20**|**Enhancing Language Multi-Agent Learning with Multi-Agent Credit Re-Assignment for Interactive Environment Generalization**|Zhitao He et.al.|[2502.14496](http://arxiv.org/abs/2502.14496)|null|基于大语言模型的代理在交互式环境（如移动操作和网页浏览）以及其他非计算机使用领域取得了显著进展。当前的多代理系统普遍在性能上优于单个代理，但在跨环境泛化方面由于预定义的角色和不充分的通用化策略而遇到困难。实现强大性能与良好泛化性的挑战阻碍了交互式环境中多代理系统的发展。为了解决这些问题，我们提出了CollabUIAgents，这是一种多代理强化学习框架，采用了一种新颖的多代理信用重新分配（CR）策略，通过大语言模型而非特定环境奖励来分配过程奖励，并利用合成偏好数据进行学习，以促进无角色代理策略之间的可泛化协作行为。实证结果表明，我们的框架提高了多代理系统的性能和跨环境泛化能力。此外，我们70亿参数的系统达到了与强大的闭源模型相当或超越的结果，以及指导CR的大语言模型。我们还提供了有效使用细粒度CR奖励以实现环境泛化的见解，以及如何在多代理系统中容纳训练好的大语言模型。|
|**2025-02-20**|**FlowAgent: Achieving Compliance and Flexibility for Workflow Agents**|Yuchen Shi et.al.|[2502.14345](http://arxiv.org/abs/2502.14345)|null|将工作流与大型语言模型（LLM）集成，使基于LLM的代理能够执行预定义的程序，从而增强现实世界应用中的自动化。传统的基于规则的方法往往限制了LLM的固有灵活性，因为其预定义的执行路径在遇到意外的、超出工作流（OOW）查询时会限制模型的动作空间。相反，基于提示的方法允许LLM完全控制流程，但这可能导致程序合规性的减弱。为了解决这些挑战，我们引入了FlowAgent，这是一种旨在保持合规性和灵活性的新代理框架。我们提出了过程描述语言（PDL），它结合了自然语言的适应性和代码的精确性来制定工作流。在此基础上，我们开发了一个全面的框架，使LLM能够有效地管理OOW查询，同时保持执行路径受到一组控制器的监督。此外，我们提出了一种新的评估方法，以严格评估LLM代理处理OOW场景的能力，超越了现有基准测试中仅关注常规流程合规性的局限。在三个数据集上的实验表明，FlowAgent不仅遵循工作流，还能有效管理OOW查询，突显了其在合规性和灵活性方面的双重优势。代码可在https://github.com/Lightblues/FlowAgent获取。|
|**2025-02-20**|**STeCa: Step-level Trajectory Calibration for LLM Agent Learning**|Hanlin Wang et.al.|[2502.14276](http://arxiv.org/abs/2502.14276)|**[link](https://github.com/WangHanLinHenry/STeCa)**|**基于大型语言模型（LLM）的代理通过与环境动态交互在处理复杂任务方面显示出潜力。现有工作主要集中在从专家演示中进行行为克隆和通过探索性轨迹采样进行偏好学习。然而，这些方法在长周期任务中往往表现不佳，其中次优动作逐步累积，导致代理偏离正确的任务轨迹。为了解决这个问题，我们强调了及时校准的重要性，并提出了自动构建校准轨迹以训练代理的需求。我们提出了一种新的LLM代理学习框架——Step-Level Trajectory Calibration (STeCa)。具体来说，STeCa通过在探索过程中进行步骤级奖励比较来识别次优动作。它利用LLM驱动的反思构建校准轨迹，使代理能够从改进的决策过程中学习。这些校准轨迹以及成功的轨迹数据被用于强化训练。广泛的实验表明，STeCa显著优于现有方法。进一步的分析表明，步骤级校准使代理能够以更高的鲁棒性完成任务。我们的代码和数据可以在https://github.com/WangHanLinHenry/STeCa获取。**|
|**2025-02-19**|**Investigating Non-Transitivity in LLM-as-a-Judge**|Yi Xu et.al.|[2502.14074](http://arxiv.org/abs/2502.14074)|null|基于大型语言模型（LLMs）的自动评估方法正逐渐成为评估基于LLM的代理指令遵循能力的标准工具。这种范式中最常见的方法是与基线模型进行成对比较，该方法严重依赖于传递性偏好的假设。然而，这一假设的有效性尚未得到充分探索。在本研究中，我们调查了AlpacaEval框架中存在的非传递性偏好，并分析了其对模型排名的影响。我们发现，LLM评判者表现出非传递性偏好，导致排名对基线模型的选择非常敏感。为了解决这个问题，我们展示了结合Bradley-Terry偏好模型的循环赛可以产生更可靠的排名。值得注意的是，我们的方法提高了与Chatbot Arena之间的Spearman相关性和Kendall相关性（分别从95.0%提高到96.4%，从82.1%提高到86.3%）。为了应对循环赛带来的计算成本问题，我们提出了Swiss-Wise迭代配对（Swim）锦标赛，采用动态匹配策略来捕捉循环赛的好处，同时保持计算效率。|
|**2025-02-19**|**Autellix: An Efficient Serving Engine for LLM Agents as General Programs**|Michael Luo et.al.|[2502.13965](http://arxiv.org/abs/2502.13965)|null|大型语言模型（LLM）应用正在从简单的聊天机器人演进为动态的、通用的代理程序，这些程序通过扩展LLM调用和输出令牌来帮助AI代理进行推理、探索和解决复杂任务。然而，现有的LLM服务系统忽略了程序与调用之间的依赖关系，错失了重要的优化机会。我们的分析显示，提交给LLM服务引擎的程序经历了很长的累积等待时间，这主要是由于在单个LLM请求和程序层面都存在头部阻塞现象。为了解决这一问题，我们引入了Autellix，这是一种将程序视为首要对象以最小化其端到端延迟的LLM服务系统。Autellix拦截程序提交的LLM调用，通过程序级上下文丰富调度器。我们提出了两种调度算法——分别针对单线程和分布式程序——根据程序先前完成的调用来抢占和优先处理LLM调用。评估表明，在不同的LLM和代理工作负载下，与最先进的系统（如vLLM）相比，Autellix在相同延迟的情况下提高了4-15倍的程序吞吐量。|
|**2025-02-19**|**DataSciBench: An LLM Agent Benchmark for Data Science**|Dan Zhang et.al.|[2502.13897](http://arxiv.org/abs/2502.13897)|**[link](https://github.com/thudm/datascibench)**|**本文介绍了DataSciBench，这是一个全面的基准测试工具，用于评估大型语言模型（LLM）在数据科学方面的能力。最近的相关基准测试主要集中在单一任务、易于获取的事实依据和简单的评估指标上，这限制了可评估的任务范围。相比之下，DataSciBench基于一个更全面且精心策划的自然且具有挑战性的提示集合构建，这些提示针对不确定的事实依据和评估指标。我们开发了一种半自动化的管道来生成事实依据并验证评估指标。该管道利用并实现了一种基于LLM的自一致性策略和人工验证策略，通过利用收集到的提示、预定义的任务类型和聚合函数（指标）来生成准确的事实依据。此外，我们提出了一种创新的任务-函数-代码（TFC）框架，根据精确定义的指标和程序规则评估每个代码执行结果。我们的实验框架涉及使用我们收集的各种提示对6个基于API的模型、8个开源通用模型和9个开源代码生成模型进行测试。这种方法旨在提供对数据科学领域中的LLM更全面和严格的评估，揭示它们的优点和缺点。实验结果表明，在所有指标上，基于API的模型优于开源模型，而Deepseek-Coder-33B-Instruct在开源模型中得分最高。我们在https://github.com/THUDM/DataSciBench上发布了所有的代码和数据。**|
|**2025-02-19**|**AI Software Engineer: Programming with Trust**|Abhik Roychoudhury et.al.|[2502.13767](http://arxiv.org/abs/2502.13767)|null|
|**2025-02-19**|**An LLM-based Agent for Reliable Docker Environment Configuration**|Ruida Hu et.al.|[2502.13681](http://arxiv.org/abs/2502.13681)|null|
|**2025-02-18**|**Demonstrating specification gaming in reasoning models**|Alexander Bondarenko et.al.|[2502.13295](http://arxiv.org/abs/2502.13295)|null|
|**2025-02-18**|**Interactive Agents to Overcome Ambiguity in Software Engineering**|Sanidhya Vijayvargiya et.al.|[2502.13069](http://arxiv.org/abs/2502.13069)|**[link](https://github.com/sani903/interactivesweagents)**|
|**2025-02-18**|**Towards a Design Guideline for RPA Evaluation: A Survey of Large Language Model-Based Role-Playing Agents**|Chaoran Chen et.al.|[2502.13012](http://arxiv.org/abs/2502.13012)|null|
|**2025-02-18**|**Towards more Contextual Agents: An extractor-Generator Optimization Framework**|Mourad Aouini et.al.|[2502.12926](http://arxiv.org/abs/2502.12926)|null|
|**2025-02-18**|**Towards Adaptive Feedback with AI: Comparing the Feedback Quality of LLMs and Teachers on Experimentation Protocols**|Kathrin Seßler et.al.|[2502.12842](http://arxiv.org/abs/2502.12842)|null|
|**2025-02-18**|**DemonAgent: Dynamically Encrypted Multi-Backdoor Implantation Attack on LLM-based Agent**|Pengyu Zhu et.al.|[2502.12575](http://arxiv.org/abs/2502.12575)|**[link](https://github.com/whfelingyu/demonagent)**|
|**2025-02-18**|**UXAgent: An LLM Agent-Based Usability Testing Framework for Web Design**|Yuxuan Lu et.al.|[2502.12561](http://arxiv.org/abs/2502.12561)|null|
|**2025-02-18**|**CityEQA: A Hierarchical LLM Agent on Embodied Question Answering Benchmark in City Space**|Yong Zhao et.al.|[2502.12532](http://arxiv.org/abs/2502.12532)|null|
|**2025-02-18**|**EDGE: Efficient Data Selection for LLM Agents via Guideline Effectiveness**|Yunxiao Zhang et.al.|[2502.12494](http://arxiv.org/abs/2502.12494)|null|
|**2025-02-18**|**EPO: Explicit Policy Optimization for Strategic Reasoning in LLMs via Reinforcement Learning**|Xiaoqian Liu et.al.|[2502.12486](http://arxiv.org/abs/2502.12486)|null|
|**2025-02-18**|**Investigating and Extending Homans' Social Exchange Theory with Large Language Model based Agents**|Lei Wang et.al.|[2502.12450](http://arxiv.org/abs/2502.12450)|null|
|**2025-02-17**|**HARBOR: Exploring Persona Dynamics in Multi-Agent Competition**|Kenan Jiang et.al.|[2502.12149](http://arxiv.org/abs/2502.12149)|null|
|**2025-02-17**|**Scaling Autonomous Agents via Automatic Reward Modeling And Planning**|Zhenfang Chen et.al.|[2502.12130](http://arxiv.org/abs/2502.12130)|null|
|**2025-02-17**|**A-MEM: Agentic Memory for LLM Agents**|Wujiang Xu et.al.|[2502.12110](http://arxiv.org/abs/2502.12110)|null|
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

<p align=right>(<a href=#updated-on-20250224>back to top</a>)</p>

## llm

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-02-20**|**LServe: Efficient Long-sequence LLM Serving with Unified Sparse Attention**|Shang Yang et.al.|[2502.14866](http://arxiv.org/abs/2502.14866)|null|大型语言模型（LLM）在处理长序列方面展现了显著的潜力，但在预填充阶段由于注意力机制的二次计算复杂度以及解码阶段KV缓存的大量内存占用，高效地服务这些长上下文模型仍然是一个挑战。为了解决这些问题，我们引入了LServe系统，通过混合稀疏注意力来加速长序列LLM的服务。该方法将不同硬件友好的结构化稀疏模式统一到一个框架中，在预填充和解码阶段以块的形式跳过对不重要标记的计算。LServe展示了静态和动态稀疏性在长上下文LLM注意力中的兼容性。这种设计通过结合这些优化实现了乘法级的速度提升。具体来说，我们在预填充和解码阶段都将近一半的注意力头转换为几乎免费的流式头。此外，我们发现无论上下文长度如何，只需要固定数量的KV页就能保持长上下文能力。然后，我们设计了一种基于查询中心相似性的分层KV页选择策略，以动态修剪KV页。平均而言，与vLLM相比，LServe在LLM预填充上加速了最高2.9倍，在解码上加速了1.3-2.1倍，同时保持了长上下文准确性。代码发布于https://github.com/mit-han-lab/omniserve。|
|**2025-02-20**|**Aligning LLMs to Ask Good Questions A Case Study in Clinical Reasoning**|Shuyue Stella Li et.al.|[2502.14860](http://arxiv.org/abs/2502.14860)|null|大型语言模型（LLM）在面对不确定性时往往无法提出有效的问题，这使得它们在需要主动收集信息进行决策的领域中不可靠。我们提出了ALFA框架，该框架通过以下方式改进了LLM提问能力：(i) 将“好”问题的概念分解为一组基于理论的属性（例如，清晰度、相关性），(ii) 可控地合成特定于属性的问题变体，以及(iii) 通过基于偏好的优化对齐模型，使其能够沿着这些细粒度的属性明确学习如何提出更好的问题。以临床推理作为案例研究，我们引入了MediQ-AskDocs数据集，其中包含17,000个现实世界的临床互动，并附有80,000个针对特定属性的后续问题偏好对，以及一个新颖的专家注释交互式医疗问答任务来评估提问能力。与最先进的指令调优LLM相比，使用ALFA对齐的模型在MediQ-AskDocs上的诊断错误减少了56.6%，问题层面的胜率为64.4%，并且具有很强的泛化能力。我们的发现表明，在专家应用领域中，通过结构化的细粒度属性明确指导提问提供了一条改进LLM的可扩展路径。|
|**2025-02-20**|**FR-Spec: Accelerating Large-Vocabulary Language Models via Frequency-Ranked Speculative Sampling**|Weilin Zhao et.al.|[2502.14856](http://arxiv.org/abs/2502.14856)|null|推测性采样已成为通过利用先草稿后验证机制在每次前向传递中生成多个标记来加速大型语言模型（LLMs）自回归生成过程的重要技术。虽然最先进的推测性采样方法仅使用单层和语言建模（LM）头作为草稿模型以实现令人印象深刻的层压缩，但对于具有大词汇量的LLM（如词汇量为128k的Llama-3-8B），其效率增益显著降低。为了解决这个问题，我们提出了FR-Spec，这是一种基于频率排名的推测性采样框架，通过词汇空间压缩优化草稿候选选择。通过将草稿搜索限制在优先考虑频率的标记子集中，我们的方法减少了75%的LM头部计算开销，同时确保最终输出分布的一致性。跨多个数据集的实验表明，与最先进的推测性采样方法EAGLE-2相比，平均速度提高了1.12倍。|
|**2025-02-20**|**Prompt-to-Leaderboard**|Evan Frick et.al.|[2502.14855](http://arxiv.org/abs/2502.14855)|null|大型语言模型（LLM）的评估通常依赖于像准确率或人类偏好这样的聚合指标，这些指标是通过对用户和提示进行平均计算得出的。这种平均方法掩盖了模型性能在用户和提示方面的具体差异。为了解决这个问题，我们提出了Prompt-to-Leaderboard (P2L) 方法，该方法能够生成特定于提示的排行榜。其核心思想是训练一个接受自然语言提示作为输入的语言模型，输出Bradley-Terry系数向量，然后使用这些系数来预测人类偏好的投票结果。由此产生的依赖于提示的排行榜允许进行无监督的任务特定评估、查询到模型的最佳路由、个性化以及自动评估模型的优势和劣势。来自Chatbot Arena的数据表明，P2L比平均排行榜更能捕捉到语言模型性能的细微差别。此外，我们的研究发现，P2L产生特定于提示的评估能力遵循类似于在LLM中观察到的幂律缩放规律。2025年1月，基于此方法训练的路由器在Chatbot Arena排行榜上取得了第一名的位置。我们的代码可以在以下GitHub链接获取：https://github.com/lmarena/p2l。|
|**2025-02-20**|**GATE: Graph-based Adaptive Tool Evolution Across Diverse Tasks**|Jianwen Luo et.al.|[2502.14848](http://arxiv.org/abs/2502.14848)|null|大型语言模型（LLM）在工具制作方面展现出了巨大潜力，但现有的框架往往难以高效构建可靠的工具集，并且局限于单一任务设置。为了解决这些挑战，我们提出了GATE（基于图的自适应工具进化），这是一种自适应框架，能够动态构建和进化跨多个场景的层次化可重用工具图。我们在开放式任务（Minecraft）、基于代理的任务（TextCraft、DABench）以及代码生成任务（MATH、Date、TabMWP）上对GATE进行了评估。结果显示，与之前的最先进方法相比，GATE在Minecraft中完成里程碑的速度快了4.3倍，并在代码生成任务中平均提高了9.23%，在代理任务中平均提高了10.03%。GATE展示了自适应进化的强大能力，在保持高效率的同时平衡了工具的数量、复杂性和功能。代码和数据可以在https://github.com/ayanami2003/GATE获取。|
|**2025-02-20**|**Scaling Text-Rich Image Understanding via Code-Guided Synthetic Multimodal Data Generation**|Yue Yang et.al.|[2502.14846](http://arxiv.org/abs/2502.14846)|null|关于图像和丰富文本（如图表和文档）的推理是视觉-语言模型（VLMs）的一个关键应用。然而，由于缺乏多样化的文本丰富的视觉-语言数据，VLMs在这些领域中常常表现不佳。为了解决这一挑战，我们提出了CoSyn框架，该框架利用纯文本大型语言模型（LLMs）的编码能力自动生成合成的文本丰富多模态数据。给定描述目标领域的输入文本（例如，“营养成分标签”），CoSyn会提示LLM生成用于渲染合成图像的代码（Python、HTML、LaTeX等）。通过将底层代码作为合成图像的文本表示，CoSyn可以生成高质量的指令调优数据，再次依赖于纯文本LLM。使用CoSyn，我们构建了一个包含40万张图像和270万行视觉-语言指令调优数据的数据集。在七个基准测试上的全面实验表明，使用我们的合成数据训练的模型在竞争性的开源模型中达到了最先进的性能，包括Llama 3.2，并且超越了专有模型如GPT-4V和Gemini 1.5 Flash。此外，CoSyn还可以生成合成指针数据，使VLMs能够在输入图像中定位信息，展示了其开发能够作用于真实环境中的多模态代理的潜力。|
|**2025-02-20**|**A Survey of Model Architectures in Information Retrieval**|Zhichao Xu et.al.|[2502.14822](http://arxiv.org/abs/2502.14822)|null|该调查研究了信息检索（IR）中模型架构的演变，重点关注两个关键方面：用于特征提取的基础模型和用于相关性估计的端到端系统架构。本综述有意将架构考虑与训练方法分开，以集中分析IR系统中的结构创新。我们追溯了从传统的基于术语的方法到现代神经网络方法的发展过程，特别是强调了基于Transformer的模型及其后续的大规模语言模型（LLM）的影响。最后，我们讨论了新兴的挑战和未来方向，包括针对性能和可扩展性的架构优化、处理多模态和多语言数据以及适应传统搜索范式之外的新应用领域。|
|**2025-02-20**|**eC-Tab2Text: Aspect-Based Text Generation from e-Commerce Product Tables**|Luis Antonio Gutiérrez Guanilo et.al.|[2502.14820](http://arxiv.org/abs/2502.14820)|null|大型语言模型（LLMs）在各个领域展现了出色的多功能性，但在电子商务中的应用仍然较少探索，主要是因为缺乏特定领域的数据集。为了解决这一问题，我们引入了eC-Tab2Text，这是一个旨在捕捉电子商务复杂性的新数据集，包括详细的产品属性和用户特定的查询。利用eC-Tab2Text，我们专注于从产品表格生成文本，使LLMs能够从结构化的表格数据中生成高质量、属性特定的产品评论。经过微调的模型使用标准的Table2Text指标进行了严格的评估，并对正确性、忠实性和流畅性进行了评估。我们的结果表明，在生成上下文准确的评论方面有了显著改进，突显了定制数据集和微调方法在优化电子商务工作流程中的变革潜力。这项工作强调了LLMs在电子商务工作流程中的潜力以及特定领域数据集在应对行业特定挑战中的重要作用。|
|**2025-02-20**|**Dynamic Low-Rank Sparse Adaptation for Large Language Models**|Weizhong Huang et.al.|[2502.14816](http://arxiv.org/abs/2502.14816)|null|尽管网络稀疏性在缓解大型语言模型（LLMs）部署压力方面效果显著，但它仍然存在显著的性能下降问题。将低秩适应（LoRA）应用于稀疏LLM的微调提供了一种直观的方法来解决这一困境，但这种方法存在以下不足：1）无法在训练后将LoRA权重集成到稀疏LLM中；2）在高稀疏率下性能恢复不足。本文提出了一种新的方法——动态低秩稀疏适应（LoSA），该方法在一个统一框架内无缝地将低秩适应集成到LLM稀疏性中，从而在不增加推理延迟的情况下增强稀疏LLM的性能。具体而言，LoSA在微调过程中根据相应的稀疏权重动态稀疏化LoRA的结果，从而确保LoRA模块可以在训练后集成到稀疏LLM中。此外，LoSA利用表示互信息（RMI）作为指标来确定各层的重要性，从而在微调过程中有效地确定层级别的稀疏率。基于此，LoSA根据层间重建误差的变化调整LoRA模块的秩，为每一层分配适当的微调以减少密集和稀疏LLM之间的输出差异。大量实验表明，LoSA能够在几小时内有效提升稀疏LLM的效能，且不会引入任何额外的推理负担。例如，LoSA将稀疏LLaMA-2-7B的困惑度降低了68.73，并将零样本准确率提高了16.32%，在CPU上实现了2.60倍的速度提升，在GPU上实现了2.23倍的速度提升，仅需在单个NVIDIA A100 80GB GPU上进行45分钟的微调。代码可在https://github.com/wzhuang-xmu/LoSA获取。|
|**2025-02-20**|**From RAG to Memory: Non-Parametric Continual Learning for Large Language Models**|Bernal Jiménez Gutiérrez et.al.|[2502.14802](http://arxiv.org/abs/2502.14802)|**[link](https://github.com/osu-nlp-group/hipporag)**|**我们持续获取、组织和利用知识的能力是人类智能的一个关键特征，AI系统必须接近这一能力才能发挥其全部潜力。鉴于大型语言模型（LLM）在持续学习方面面临的挑战，检索增强生成（RAG）已成为引入新信息的主要方式。然而，它对向量检索的依赖阻碍了其模仿人类长期记忆的动态性和互联性。最近的RAG方法通过将向量嵌入与知识图谱等结构结合来解决这些差距，特别是意义理解和关联性。然而，它们在基本的事实记忆任务上的表现显著低于标准RAG。为了解决这种意外的性能下降，我们提出了HippoRAG 2框架，该框架在事实记忆、意义理解以及关联记忆任务上全面优于标准RAG。HippoRAG 2基于HippoRAG中使用的个性化PageRank算法，并通过更深层次的段落整合和更有效的在线使用LLM进行增强。这种组合使这个RAG系统更接近人类长期记忆的有效性，在关联记忆任务上比最先进的嵌入模型提高了7%，同时在事实知识和意义理解记忆能力方面也表现出色。这项工作为LLM的非参数持续学习铺平了道路。我们的代码和数据将在https://github.com/OSU-NLP-Group/HippoRAG发布。**|
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
|**2025-02-18**|**RuozhiBench: Evaluating LLMs with Logical Fallacies and Misleading Premises**|Zenan Zhai et.al.|[2502.13125](http://arxiv.org/abs/2502.13125)|null|
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
|**2025-02-17**|**A-MEM: Agentic Memory for LLM Agents**|Wujiang Xu et.al.|[2502.12110](http://arxiv.org/abs/2502.12110)|null|
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
|**2025-02-11**|**DarwinLM: Evolutionary Structured Pruning of Large Language Models**|Shengkun Tang et.al.|[2502.07780](http://arxiv.org/abs/2502.07780)|null|
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
|**2025-02-10**|**Large Language Models Meet Symbolic Provers for Logical Reasoning Evaluation**|Chengwen Qi et.al.|[2502.06563](http://arxiv.org/abs/2502.06563)|null|
|**2025-02-10**|**Is API Access to LLMs Useful for Generating Private Synthetic Tabular Data?**|Marika Swanberg et.al.|[2502.06555](http://arxiv.org/abs/2502.06555)|null|
|**2025-02-07**|**NoLiMa: Long-Context Evaluation Beyond Literal Matching**|Ali Modarressi et.al.|[2502.05167](http://arxiv.org/abs/2502.05167)|null|
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

<p align=right>(<a href=#updated-on-20250224>back to top</a>)</p>

## moe

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-02-20**|**Ray-Tracing for Conditionally Activated Neural Networks**|Claudio Gallicchio et.al.|[2502.14788](http://arxiv.org/abs/2502.14788)|null|在本文中，我们介绍了一种新颖的条件激活神经网络架构，该架构结合了多层混合专家（MoEs）的层次结构与一种采样机制，这种机制能够逐步收敛到优化的专家激活配置。此方法使网络架构能够动态展开，从而促进高效的路径特定训练。实验结果表明，该方法在保持与传统基线相当的准确率的同时，显著减少了推理所需的参数数量。值得注意的是，参数减少的程度与输入模式的复杂性相关，这一特性自然地从网络的操作动态中产生，无需引入显式的辅助惩罚函数。|
|**2025-02-19**|**Unraveling the Localized Latents: Learning Stratified Manifold Structures in LLM Embedding Space with Sparse Mixture-of-Experts**|Xin Li et.al.|[2502.13577](http://arxiv.org/abs/2502.13577)|null|然而，现实世界的数据通常表现出复杂的局部结构，这对于基于平滑全局流形的单一模型方法来说是难以解析的。在这项工作中，我们推测在这些大型语言模型的潜在空间中，嵌入向量存在于一种具有不同维度的局部流形结构中，这种结构取决于输入数据的困惑度和领域，通常被称为分层流形结构，这些结构共同形成一个称为分层空间的结构化空间。为了验证这一结构性假设的有效性，我们提出了一种基于专家混合（MoE）模型的分析框架，其中每个专家都通过不同稀疏水平下的简单字典学习算法来实现。通过结合基于注意力机制的软门控网络，我们验证了我们的模型能够为一组输入数据源学习专门化的子流形，这反映了LLM嵌入空间中的语义分层。我们进一步分析了这些分层子流形的内在维度，并提供了关于专家分配、门控熵和专家间距离的广泛统计数据。我们的实验结果表明，我们的方法不仅验证了LLM嵌入空间中存在分层流形结构的假设，而且还提供了与输入数据内在语义变化相一致的可解释聚类。|
|**2025-02-18**|**MoBA: Mixture of Block Attention for Long-Context LLMs**|Enzhe Lu et.al.|[2502.13189](http://arxiv.org/abs/2502.13189)|**[link](https://github.com/moonshotai/moba)**|**扩展有效上下文长度对于推动大型语言模型（LLMs）向通用人工智能（AGI）发展至关重要。然而，传统注意力机制固有的计算复杂度二次增长带来了巨大的开销。现有的方法要么引入强偏置结构，如特定任务的sink或窗口注意力，要么将注意力机制彻底修改为线性近似，其在复杂推理任务中的表现尚未得到充分探索。在这项工作中，我们提出了一种遵循“少结构”原则的解决方案，允许模型自主决定关注点，而不是引入预定义的偏置。我们引入了块注意力混合（MoBA），这是一种创新的方法，它将专家混合（MoE）的原则应用于注意力机制。这种新颖的架构在长上下文任务中表现出色，并具有一个关键优势：能够在全注意力和稀疏注意力之间无缝切换，提高效率而不牺牲性能。MoBA已经部署用于支持Kimi的长上下文请求，并在LLMs的有效注意力计算方面展示了显著的进步。我们的代码可以在https://github.com/MoonshotAI/MoBA获取。**|
|**2025-02-18**|**Every Expert Matters: Towards Effective Knowledge Distillation for Mixture-of-Experts Language Models**|Gyeongman Kim et.al.|[2502.12947](http://arxiv.org/abs/2502.12947)|null|随着混合专家模型（MoE）的出现，模型规模的有效扩展加速了近年来大型语言模型的发展。然而，它们对内存的高要求阻碍了其在资源受限环境中的应用。尽管知识蒸馏（KD）已被证明是模型压缩的有效方法，但其在MoE教师模型上的应用仍较少被探索。通过我们的研究，我们发现MoE模型中未激活的专家拥有对学生模型有益的宝贵知识。我们进一步表明，现有的KD方法并不适合压缩MoE模型，因为它们无法有效利用这些知识。为了解决这个问题，我们首次提出了两种直观的针对MoE的知识蒸馏方法：知识增强（KA）和学生感知路由（SAR），这两种方法都旨在从所有专家中有效提取知识。具体来说，KA通过多次采样专家来增强知识，而SAR则使用所有专家并通过路由训练调整专家权重以提供最佳知识。广泛的实验表明，我们的方法优于传统的KD方法，展示了它们在MoE教师模型上的有效性。|
|**2025-02-17**|**Accurate Expert Predictions in MoE Inference via Cross-Layer Gate**|Zhiyuan Fang et.al.|[2502.12224](http://arxiv.org/abs/2502.12224)|null|大型语言模型（LLM）在各种任务中表现出色，其在边缘场景中的应用也引起了广泛关注。然而，适用于边缘场景的稀疏激活混合专家（MoE）模型由于其高内存需求而受到较少关注。为了解决这一挑战，提出了基于卸载的方法，但这些方法在专家预测方面遇到了困难。不准确的专家预测会导致推理延迟增加。为了促进MoE模型在边缘场景中的应用，我们提出了Fate，这是一种专为MoE模型设计的卸载系统，旨在资源受限环境中实现高效的推理。Fate的核心思想是利用相邻层的门控输入进行专家预取，从而在不增加GPU开销的情况下实现高预测精度。此外，Fate采用了一种浅层优先的专家缓存策略，将专家命中率提高到99%。Fate还集成了针对缓存优化和IO效率定制的量化策略。实验结果表明，与按需加载和基于专家激活路径的方法相比，Fate在预填充速度上最高可达到4.5倍和1.9倍的速度提升，在解码速度上最高可达到4.1倍和2.2倍的速度提升，同时保持了推理质量。此外，Fate的性能改进在不同的内存预算下具有良好的可扩展性。|
|**2025-02-16**|**ClimateLLM: Efficient Weather Forecasting via Frequency-Aware Large Language Models**|Shixuan Li et.al.|[2502.11059](http://arxiv.org/abs/2502.11059)|null|天气预报对于公共安全、灾害预防和缓解、农业生产以及能源管理至关重要，具有全球相关性。尽管深度学习在天气预测方面取得了显著进展，但当前的方法仍面临一些关键限制：(i) 它们通常难以同时捕捉动态时间依赖性和短期突变，使得极端天气建模变得困难；(ii) 由于需要大量训练和资源，它们会带来高昂的计算成本；(iii) 它们对多尺度频率的适应能力有限，导致在全球趋势与局部波动分离时遇到挑战。为了解决这些问题，我们提出了ClimateLLM，这是一种用于天气预报的基础模型。它通过一个跨时间和跨空间的协作建模框架来捕捉时空依赖性，该框架将基于傅里叶的频率分解与大型语言模型（LLMs）结合，以增强空间和时间建模。我们的框架使用了一种混合专家（MoE）机制，能够自适应地处理不同的频率组件，从而有效应对全局信号和局部极端事件。此外，我们引入了一种跨时间和跨空间的动态提示机制，使LLMs能够有效地整合多个尺度的气象模式。在真实数据集上的广泛实验表明，ClimateLLM在准确性和效率方面优于现有最先进方法，成为一种可扩展的全球天气预报解决方案。|
|**2025-02-15**|**Semantic Specialization in MoE Appears with Scale: A Study of DeepSeek R1 Expert Specialization**|Matthew Lyle Olson et.al.|[2502.10928](http://arxiv.org/abs/2502.10928)|null|DeepSeek-R1是最大的开源混合专家（MoE）模型，其推理能力可与专有前沿模型相媲美。先前的研究探索了MoE模型中的专家路由机制，但发现专家选择往往是基于单个词而不是语义驱动的。鉴于DeepSeek-R1增强的推理能力，我们研究其路由机制是否比之前的MoE模型展现出更高的语义专业化。为此，我们进行了两项关键实验：(1) 词语意义消歧任务，我们检查具有不同意义的词语在专家激活模式上的差异；(2) 认知推理分析，在DiscoveryWorld的交互式任务设置中评估DeepSeek-R1的结构化思维过程。我们的结论是DeepSeek-R1的路由机制更具语义意识，并且它能够进行结构化的认知处理。|
|**2025-02-11**|**MoHAVE: Mixture of Hierarchical Audio-Visual Experts for Robust Speech Recognition**|Sungnyun Kim et.al.|[2502.10447](http://arxiv.org/abs/2502.10447)|null|
|**2025-02-12**|**Heterogeneous Mixture of Experts for Remote Sensing Image Super-Resolution**|Bowen Chen et.al.|[2502.09654](http://arxiv.org/abs/2502.09654)|null|遥感图像超分辨率（SR）旨在从低分辨率输入中重建高分辨率的遥感图像，从而解决传感器和成像条件带来的限制。然而，遥感图像固有的特性，包括多样化的地物类型和复杂的细节，给高质量重建带来了显著挑战。现有的方法通常采用统一的结构来处理各种类型的地物，没有进行区分，难以适应遥感图像的复杂特性。为了解决这一问题，我们引入了混合专家（MoE）模型，并设计了一组异构专家。这些专家被组织成多个专家组，每个组内的专家是同质的，而不同组之间的专家是异质的。这种设计确保可以使用专门的激活参数有效地处理地物的多样性和复杂细节。为了更好地适应异构专家，我们提出了一种多级特征聚合策略来指导路由过程。此外，我们开发了一种双路由机制，以自适应地为每个像素选择最优专家。在UCMerced和AID数据集上的实验表明，我们提出的方法在SR重建精度方面优于最先进的方法。代码将在https://github.com/Mr-Bamboo/MFG-HMoE上提供。|
|**2025-02-12**|**The MoE-Empowered Edge LLMs Deployment: Architecture, Challenges, and Opportunities**|Ning Li et.al.|[2502.08381](http://arxiv.org/abs/2502.08381)|null|大型语言模型（LLM）的强大性能表明，为了满足6G的泛在智能需求，在终端、边缘和云端部署具有不同规模和架构的各种LLM以适应异构硬件是关键途径。然而，LLM的大规模参数对边缘设备的部署提出了巨大挑战，主要是由于其对计算和存储资源的高需求。鉴于专家混合（MoE）中的稀疏激活对于边缘环境下的计算和通信资源可扩展性和动态分配非常有效，本文提出了一种新的基于MoE赋能的边缘LLM协作部署框架，称为CoEL。该框架充分利用了MoE架构的特点，并涵盖四个关键方面：感知、部署、压缩与更新。边缘服务器向邻近设备广播其资源状态以及LLM的具体资源需求。然后，利用这些数据，提出两种先进的部署策略来满足不同的模型规模，确保每个模型都能得到有效部署。一种是在单个边缘设备上通过设备内资源协作部署LLM，另一种则是通过设备间资源协作实现跨多个边缘设备的分布式部署。此外，通过对模型进行量化压缩和采用令牌融合及剪枝技术减少中间数据量，进一步减少了内存占用。最后，考虑到网络拓扑、资源状态和用户需求的变化，定期更新部署策略以保持其相关性和有效性。本文还概述了边缘LLM部署所面临的挑战和潜在的研究方向。|
|**2025-02-12**|**Mixture of Decoupled Message Passing Experts with Entropy Constraint for General Node Classification**|Xuanze Chen et.al.|[2502.08083](http://arxiv.org/abs/2502.08083)|null|在现实世界的图中，不同程度的同质性和异质性持续限制了图神经网络（GNNs）在节点分类任务中的通用性。从数据为中心的角度出发，本研究揭示了不同图对不同的消息编码方案有内在偏好：同质性图倾向于局部传播，而异质性图则表现出对传播和变换灵活组合的偏好。为了解决这一问题，我们提出了基于专家混合机制（MoE）的通用节点分类框架GNNMoE。该框架首先通过细粒度编码算子的重组构建多种消息传递专家，然后设计软门控层和硬门控层来为每个节点表示学习分配最合适的专业网络，从而提高模型的表达能力和对多样化图的适应性。此外，考虑到软门控可能在同质性场景下引入编码噪声，我们引入了一个熵约束来指导软门控的锐化，实现了加权组合与Top-K选择的有机整合。大量实验表明，GNNMoE在节点分类性能和跨多样图数据集的通用性方面显著优于主流GNN、异质性GNN和图变换器。|
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

<p align=right>(<a href=#updated-on-20250224>back to top</a>)</p>

## SSMs

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-02-18**|**DAMamba: Vision State Space Model with Dynamic Adaptive Scan**|Tanzhe Li et.al.|[2502.12627](http://arxiv.org/abs/2502.12627)|null|状态空间模型（SSMs）在计算机视觉领域最近受到了广泛关注。然而，由于图像数据的独特特性，将自然语言处理中的SSMs适应到计算机视觉并没有超过目前最先进的卷积神经网络（CNNs）和视觉变换器（ViTs）。现有的视觉SSMs主要利用手动设计的扫描方式将图像块局部或全局地展平为序列。这种方法破坏了图像原有的语义空间邻近性，并且缺乏灵活性，难以捕捉复杂的图像结构。为了解决这一局限性，我们提出了动态自适应扫描（DAS），这是一种数据驱动的方法，能够自适应地分配扫描顺序和区域。这使得模型具有更灵活的建模能力，同时保持线性的计算复杂度和全局建模能力。基于DAS，我们进一步提出了视觉骨干网络DAMamba，在图像分类、目标检测、实例分割和语义分割等视觉任务上显著优于当前最先进的视觉Mamba模型。值得注意的是，它还超过了某些最新的先进CNNs和ViTs。代码将在https://github.com/ltzovo/DAMamba发布。|
|**2025-02-12**|**From Layers to States: A State Space Model Perspective to Deep Neural Network Layer Dynamics**|Qinshuo Liu et.al.|[2502.10463](http://arxiv.org/abs/2502.10463)|null|神经网络的深度是其能力的一个关键因素，通常更深的模型表现出更优的性能。基于这一点，人们在增强层聚合方面做出了大量努力——重用来自先前层的信息以更好地提取当前层的特征，从而提高深层神经网络的表现力。然而，以往的工作主要从离散状态的角度来解决这个问题，这在层数增加时并不适用。本文创新性地将各层的输出视为连续过程的状态，并考虑利用状态空间模型（SSM）来设计非常深的神经网络中的层聚合。此外，受到其在建模长序列方面的进展启发，选择性状态空间模型（S6）被用来设计一个新的模块，称为选择性状态空间模型层聚合（S6LA）。该模块旨在将传统的CNN或Transformer架构结合在一个顺序框架中，增强最先进的视觉网络的表现力。广泛的实验表明，S6LA在图像分类和检测任务上都带来了显著的改进，突显了将SSM与当代深度学习技术相结合的潜力。|
|**2025-02-12**|**SS4Rec: Continuous-Time Sequential Recommendation with State Space Models**|Wei Xiao et.al.|[2502.08132](http://arxiv.org/abs/2502.08132)|null|顺序推荐是推荐系统领域的一个关键方向，旨在基于用户具有不规则时间间隔的历史交互序列来建模用户兴趣。尽管先前基于循环神经网络和注意力机制的方法取得了显著成果，但由于其离散特性，在捕捉系统连续性方面存在局限。在连续时间建模的背景下，状态空间模型（SSM）提供了一种潜在解决方案，因为它能够有效地捕捉用户兴趣随时间的动态演变。然而，现有的基于SSM的方法忽略了历史用户交互中不规则时间间隔的影响，这使得在序列中建模复杂的用户-项目转换变得困难。为了解决这个问题，我们提出了一种混合SSM模型SS4Rec用于连续时间顺序推荐。SS4Rec集成了一个时间感知的SSM来处理不规则的时间间隔，以及一个关系感知的SSM来建模上下文依赖关系，使其能够从时间和序列两个角度推断用户兴趣。在训练过程中，根据用户交互时间间隔和输入数据，时间感知的SSM和关系感知的SSM分别通过可变步长进行离散化。这有助于捕捉来自不规则时间间隔的连续依赖，并提供特定时间的个性化推荐。在五个基准数据集上的实验研究表明了SS4Rec的优势和有效性。|
|**2025-02-14**|**Implicit Language Models are RNNs: Balancing Parallelization and Expressivity**|Mark Schöne et.al.|[2502.07827](http://arxiv.org/abs/2502.07827)|null|状态空间模型（SSM）和变换器主导了语言建模领域。然而，它们的计算复杂度低于传统的递归神经网络（RNN），这限制了它们的表现力。相比之下，RNN在训练过程中缺乏并行化，引发了关于并行化与表现力之间权衡的基本问题。我们提出了隐式SSM，它通过迭代一个转换直到收敛到固定点。理论上，我们证明隐式SSM实现了RNN的非线性状态转换。实验上，我们发现仅需要近似的固定点收敛就足够了，这使得可以设计出一种大规模的训练课程，大部分保留了并行化，而只有少量的标记需要完全收敛。我们的方法在规则语言的状态跟踪能力上优于变换器和SSM。我们将隐式SSM扩展到自然语言推理任务以及大型语言模型的预训练，参数规模达到13亿，在2070亿个标记上进行训练——据我们所知，这是迄今为止训练的最大规模的隐式模型。值得注意的是，我们的隐式模型在标准基准测试中优于其显式对应模型。|
|**2025-02-11**|**A Survey on Mamba Architecture for Vision Applications**|Fady Ibrahim et.al.|[2502.07161](http://arxiv.org/abs/2502.07161)|null|Transformer 已成为对象检测、语义分割和视频理解等视觉任务的基础，但其注意力机制的二次复杂度带来了可扩展性挑战。为了解决这些限制，Mamba 架构利用状态空间模型（SSM）实现了线性可扩展性、高效处理和增强的上下文感知能力。本文研究了 Mamba 架构在视觉领域的应用及其最新进展，包括 Vision Mamba (ViM) 和 VideoMamba，它们引入了双向扫描、选择性扫描机制和时空处理，以增强图像和视频的理解。诸如位置嵌入、跨扫描模块和分层设计等架构创新进一步优化了 Mamba 框架，用于全局和局部特征提取。这些进步使 Mamba 成为计算机视觉研究和应用中一个有前景的架构。|
|**2025-02-18**|**XAMBA: Enabling Efficient State Space Models on Resource-Constrained Neural Processing Units**|Arghadip Das et.al.|[2502.06924](http://arxiv.org/abs/2502.06924)|**[link](https://github.com/arghadippurdue/xamba)**|**状态空间模型（SSM）已成为处理序列数据任务的有效替代方案，提供了与序列长度成线性或接近线性的可扩展性，使其非常适合自然语言处理、视觉和边缘AI中的长序列应用，包括实时转录、翻译和上下文搜索。这些应用需要轻量级、高性能的模型，以便部署在资源受限的设备上，如笔记本电脑和个人电脑。为每一种新兴神经网络设计专用加速器成本高昂且不切实际；相反，优化现有AI个人电脑中的NPU提供了一种可扩展的解决方案。为此，我们提出了XAMBA，这是首个在商业现成（COTS）最先进（SOTA）NPU上启用并优化SSM的框架。XAMBA遵循三步方法：（1）在NPU上启用SSM，（2）优化性能以满足KPI要求，以及（3）通过牺牲精度来换取额外的性能提升。在NPU上启用SSM后，XAMBA使用CumBA和ReduBA缓解关键瓶颈，将顺序的CumSum和ReduceSum操作替换为基于矩阵的计算，显著提高了执行速度和内存效率。此外，ActiBA通过使用分段线性映射近似昂贵的激活函数（例如Swish、Softplus），减少了延迟，同时保持最小的精度损失。在Intel Core Ultra Series 2 AI PC上的评估表明，XAMBA相比基线实现了高达2.6倍的速度提升。我们的实现可在https://github.com/arghadippurdue/XAMBA获取。**|
|**2025-02-08**|**TrackDiffuser: Nearly Model-Free Bayesian Filtering with Diffusion Model**|Yangguang He et.al.|[2502.05629](http://arxiv.org/abs/2502.05629)|null|状态估计仍然是众多领域中的一个基本挑战，从自动驾驶、飞机跟踪到量子系统控制。尽管贝叶斯滤波一直是解决这一问题的基石方法，但其传统的基于模型的范式面临着两大局限：它难以应对不准确的状态空间模型（SSM），并且需要对噪声特性有广泛的先验知识。我们提出了TrackDiffuser，这是一种生成框架，通过将贝叶斯滤波重新表述为条件扩散模型来解决这两个挑战。我们的方法通过从数据中隐式学习系统动力学来减轻不准确SSM的影响，同时通过建立测量与状态之间的直接关系，绕过了对显式测量模型和噪声先验的需求。通过一种隐式的预测与更新机制，TrackDiffuser保持了传统基于模型的滤波方法的可解释性优势。大量实验表明，我们的框架在具有挑战性的非线性场景中，特别是在涉及非高斯噪声的情况下，显著优于经典和当代混合方法。值得注意的是，TrackDiffuser在面对SSM不准确性时表现出极高的鲁棒性，为现实世界中的状态估计问题提供了一种实用解决方案，在这些问题中完美的模型和先验知识是不可获得的。|
|**2025-02-07**|**CMamba: Learned Image Compression with State Space Models**|Zhuojie Wu et.al.|[2502.04988](http://arxiv.org/abs/2502.04988)|null|学习图像压缩（LIC）已经探索了各种架构，例如卷积神经网络（CNNs）和变换器，以建模图像内容分布，从而实现有效的压缩。然而，在保持低计算复杂度（即参数、FLOPs和延迟）的同时达到高率失真性能仍然是一个挑战。在本文中，我们提出了一种基于卷积和状态空间模型（SSMs）的混合图像压缩框架，称为CMamba，以实现具有低计算复杂度的优越率失真性能。具体来说，CMamba引入了两个关键组件：内容自适应SSM（CA-SSM）模块和上下文感知熵（CAE）模块。首先，我们观察到SSMs在建模整体内容方面表现出色，但往往会丢失高频细节。相比之下，CNNs擅长捕捉局部细节。受此启发，我们提出了CA-SSM模块，该模块可以在编码和解码阶段动态融合由SSM块提取的全局内容和由CNN块捕获的局部细节。因此，在压缩过程中重要图像内容得到了很好的保留。其次，我们提出的CAE模块旨在减少编码后潜在表示中的空间和通道冗余。具体而言，我们的CAE利用SSMs对潜在表示中的空间内容进行参数化。得益于SSMs，CAE显著提高了空间压缩效率，同时减少了空间内容冗余。此外，在通道维度上，CAE通过自回归方式减少潜在表示的通道间冗余，可以充分利用先前通道的先验知识而不牺牲效率。实验结果表明，CMamba实现了卓越的率失真性能。|
|**2025-02-07**|**SSMLoRA: Enhancing Low-Rank Adaptation with State Space Model**|Jiayang Yu et.al.|[2502.04958](http://arxiv.org/abs/2502.04958)|**[link](https://github.com/yuhkalhic/ssmlora)**|**微调是使语言模型适应特定下游任务的关键方法，但随着模型规模的增加，更新所有模型参数变得不切实际。参数高效微调（PEFT）方法，如低秩适应（LoRA），通过在预训练权重矩阵中引入额外的适应参数来解决这一挑战。然而，LoRA 的性能在模型内的不同插入点之间存在差异，这表明由于不必要的插入可能导致参数效率低下。为此，我们提出了 SSMLoRA（状态空间模型低秩适应），这是 LoRA 的扩展，它结合了状态空间模型（SSM）以连接低秩矩阵。SSMLoRA 即使在更稀疏的插入情况下也能保持性能。SSMLoRA 不仅可以将输入映射到低秩空间以实现更好的特征提取，还可以利用前一个低秩空间中的计算结果。我们的方法在通用语言理解评估（GLUE）基准上达到了与 LoRA 相当的性能，同时使用的参数数量仅为后者的一半。此外，由于其结构，SSMLoRA 在处理较长输入序列的任务方面也显示出潜力。您可以在以下链接找到我们的代码：https://github.com/yuhkalhic/SSMLoRA。**|
|**2025-02-07**|**A Foundational Brain Dynamics Model via Stochastic Optimal Control**|Joonhyeong Park et.al.|[2502.04892](http://arxiv.org/abs/2502.04892)|null|我们介绍了一种基于随机最优控制（SOC）和摊销推理的脑动力学基础模型。该方法采用连续-离散状态空间模型（SSM），能够稳健地处理功能磁共振成像（fMRI）信号的复杂性和噪声。为了解决计算限制，我们在SOC框架的基础上实施了一种近似策略。此外，我们提出了一种无模拟的潜动态方法，利用局部线性近似，实现高效且可扩展的推理。为了有效的表示学习，我们从SOC公式中推导出了证据下界（ELBO），这与自监督学习（SSL）的最新进展无缝集成，从而促进鲁棒和可迁移的表示。在大规模数据集如UKB上预训练后，我们的模型在各种下游任务中取得了最先进的结果，包括人口统计预测、特质分析、疾病诊断和预后。此外，在HCP-A、ABIDE和ADHD200等外部数据集上的评估进一步验证了其在不同人口统计和临床分布中的卓越能力和鲁棒性。我们的基础模型提供了一种可扩展和高效的解码脑动力学的方法，为神经科学领域的众多应用打开了大门。|
|**2025-02-01**|**Multilingual State Space Models for Structured Question Answering in Indic Languages**|Arpita Vats et.al.|[2502.01673](http://arxiv.org/abs/2502.01673)|null|
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

<p align=right>(<a href=#updated-on-20250224>back to top</a>)</p>

## Communication Intelligence

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-09-21**|**LLM Agents as 6G Orchestrator: A Paradigm for Task-Oriented Physical-Layer Automation**|Zhuoran Xiao et.al.|[2410.03688](http://arxiv.org/abs/2410.03688)|null|生成式预训练模型的快速发展正在推动技术进步从基础应用如聊天机器人向更复杂的基于代理的系统转变。将6G系统与大型语言模型（LLM）代理和数字孪生（DT）相结合，对于管理具有新出现特性（如原生AI服务和感知）的高度复杂通信系统具有巨大的潜力和必要性。通过6G导向的代理，基站可以理解各种动态上层任务的传输需求，自动编排最优系统工作流程。通过不断从6G DT获取反馈进行强化，代理最终能够相应地提高实际系统的性能。不同于现有的为通用应用设计的LLM代理，6G导向的代理旨在利用大量的额外专业知识进行高度严谨和精确的规划，这不可避免地需要从模型训练到实施的特定系统设计。本文提出了一种构建面向任务的6G LLM代理的新综合方法。我们首先提出了一种两阶段持续预训练和微调方案，以建立领域基础模型和多样化的专业专家模型，以满足各种应用场景的需求。此外，我们还提出了一种基于语义检索的新推理框架，用于利用现有的通信相关功能。物理层任务分解等示例任务的实验结果表明了所提范式的可行性和有效性。|

<p align=right>(<a href=#updated-on-20250224>back to top</a>)</p>

## RAG

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-02-20**|**Benchmarking Multimodal RAG through a Chart-based Document Question-Answering Generation Framework**|Yuming Yang et.al.|[2502.14864](http://arxiv.org/abs/2502.14864)|null|多模态检索增强生成（MRAG）通过整合外部知识来增强推理能力。然而，现有的基准测试主要关注简单的图像-文本交互，忽视了在实际应用中普遍存在的复杂视觉格式，如图表。在这项工作中，我们引入了一个新任务——基于图表的MRAG，以解决这一局限性。为了半自动生成高质量的评估样本，我们提出了一个名为CHARGE的框架，该框架通过结构化关键点提取、跨模态验证和基于关键点的生成来生成评估数据。结合CHARGE与专家验证，我们构建了Chart-MRAG Bench，这是一个全面的基于图表的MRAG评估基准，包含来自真实文档8个领域的4738个问答对。我们的评估揭示了当前方法中的三个关键限制：（1）统一的多模态嵌入检索方法在基于图表的场景中表现不佳，（2）即使使用真实检索结果，最先进的MLLM也只能达到58.19%的正确性和73.87%的覆盖率得分，（3）MLLM在基于图表的MRAG推理过程中表现出一致的文本优于视觉模态偏见。CHARGE和Chart-MRAG Bench已在https://github.com/Nomothings/CHARGE.git上发布。|
|**2025-02-20**|**From RAG to Memory: Non-Parametric Continual Learning for Large Language Models**|Bernal Jiménez Gutiérrez et.al.|[2502.14802](http://arxiv.org/abs/2502.14802)|**[link](https://github.com/osu-nlp-group/hipporag)**|**我们不断获取、组织和利用知识的能力是人类智能的一个关键特征，AI系统必须接近这一能力才能发挥其全部潜力。鉴于大型语言模型（LLM）在持续学习方面面临的挑战，检索增强生成（RAG）已成为引入新信息的主要方式。然而，它对向量检索的依赖阻碍了其模仿人类长期记忆动态和互联性质的能力。最近的RAG方法通过结合知识图谱等结构来解决这些问题，特别是意义理解和关联性。然而，它们在基本的事实记忆任务上的表现明显低于标准RAG。我们解决了这种意外的退化问题，并提出了HippoRAG 2框架，该框架在事实记忆、意义理解和关联记忆任务上全面优于标准RAG。HippoRAG 2基于HippoRAG中使用的个性化PageRank算法，并通过更深层次的段落整合和更有效的在线使用LLM进行了增强。这种组合使该RAG系统更接近于人类长期记忆的有效性，在关联记忆任务上比最先进的嵌入模型提高了7%，同时也表现出卓越的事实知识和意义理解记忆能力。这项工作为LLM的非参数持续学习铺平了道路。我们的代码和数据将在https://github.com/OSU-NLP-Group/HippoRAG发布。**|
|**2025-02-20**|**On the Influence of Context Size and Model Choice in Retrieval-Augmented Generation Systems**|Juraj Vladika et.al.|[2502.14759](http://arxiv.org/abs/2502.14759)|null|检索增强生成（RAG）作为一种方法，通过减少大型语言模型（LLMs）对静态知识的依赖并提高答案的事实准确性来增强这些模型。RAG 通过检索相关上下文片段，并基于这些片段生成答案。尽管 RAG 在工业应用中越来越广泛，但对于其组件的系统性探索仍然不足，特别是在提供上下文的理想大小、基础 LLM 的选择以及检索方法方面。为了帮助开发稳健的 RAG 系统，我们评估了不同大小的上下文、BM25 和语义搜索作为检索器，以及八个基础 LLM。不同于通常使用简短答案进行 RAG 评估的方式，我们在两个领域中探索了更具挑战性的长篇问答，其中好的答案必须利用整个上下文。我们的研究发现表明，最终的问答性能在多达15个片段时稳步提升，但超过这个数量后则趋于停滞或下降。最后，我们展示了在生物医学领域和百科全书式领域中表现优异的通用 LLM 是不同的，并且在大型语料库中进行开放域证据检索是具有挑战性的。|
|**2025-02-20**|**WavRAG: Audio-Integrated Retrieval Augmented Generation for Spoken Dialogue Models**|Yifu Chen et.al.|[2502.14727](http://arxiv.org/abs/2502.14727)|null|检索增强生成（RAG）由于其能够使大型语言模型（LLMs）整合外部知识的能力而得到了广泛的应用。然而，现有的RAG框架主要是为基于文本的LLMs设计的，并依赖于自动语音识别来处理语音输入，这不仅丢失了重要的音频信息，还存在转录错误的风险以及增加了计算开销。因此，我们引入了WavRAG，这是第一个具有原生端到端音频支持的检索增强生成框架。WavRAG提供了两个关键特性：1) 绕过ASR，WavRAG直接处理原始音频用于嵌入和检索。2) WavRAG将音频和文本集成到了一个统一的知识表示中。具体来说，我们提出了WavRetriever来促进从文本-音频混合知识库中的检索，并通过整合链式思维推理进一步增强了口语对话模型的情境能力。与最先进的ASR-文本RAG管道相比，WavRAG在达到相当检索性能的同时实现了10倍的速度提升。此外，WavRAG独特的文本-音频混合检索能力将RAG的应用扩展到了音频领域。|
|**2025-02-20**|**FIND: Fine-grained Information Density Guided Adaptive Retrieval-Augmented Generation for Disease Diagnosis**|Mingyi Jia et.al.|[2502.14614](http://arxiv.org/abs/2502.14614)|null|检索增强的大规模语言模型（LLMs），通过将外部知识整合到LLMs中，在包括临床诊断在内的多个医学领域展现出了卓越的性能。然而，现有的RAG方法在有效评估任务难度以做出检索决策方面存在困难，因此无法满足临床对于平衡效率和准确性要求。在这篇论文中，我们提出了FIND（细粒度信息密度指导自适应RAG）这一新框架，旨在提高RAG在疾病诊断场景中的可靠性。FIND引入了一个细粒度自适应控制模块，根据输入的信息密度来判断是否需要进行检索。通过对检索过程的优化以及实现知识过滤模块，FIND确保了检索更符合临床应用场景的需求。在三个中文电子病历数据集上的实验表明，FIND显著优于各种基线方法，突显了其在临床诊断任务中的有效性。|
|**2025-02-20**|**EpMAN: Episodic Memory AttentioN for Generalizing to Longer Contexts**|Subhajit Chaudhury et.al.|[2502.14280](http://arxiv.org/abs/2502.14280)|null|最近，大型语言模型（LLMs）在许多语言任务上取得了令人瞩目的成功。然而，使用LLMs高效处理长上下文仍然是一个重大挑战。我们引入了**EpMAN**——一种利用*情景记忆*模块处理长上下文的方法，同时*整体关注*语义相关的上下文片段。*情景注意力*的输出随后用于在训练和生成过程中重新调整解码器对存储在KV缓存中的上下文的自注意力权重。当使用**EpMAN**训练LLM解码器时，其在多个具有挑战性的单跳长上下文回忆和问答基准测试中的表现，在16k到256k令牌范围内比仅使用自注意力训练的基线解码器以及流行的检索增强生成框架更加强大和稳健。|
|**2025-02-20**|**Fact or Guesswork? Evaluating Large Language Model's Medical Knowledge with Structured One-Hop Judgment**|Jiaxi Li et.al.|[2502.14275](http://arxiv.org/abs/2502.14275)|null|大型语言模型（LLM）已在各种下游任务领域得到广泛应用。然而，它们直接回忆和应用医学事实知识的能力尚未得到充分探索。现有的大多数医学问答基准评估的是复杂的推理或多跳推理，这使得很难将LLM的固有医学知识与其推理能力区分开来。鉴于医学应用的高风险性，错误信息可能带来严重后果，因此评估LLM编码、保留和回忆基本医学事实的能力至关重要。为了解决这一问题，我们引入了医学知识判断（MKJ），这是一个专门设计用于测量LLM单跳医学事实知识的数据集。MKJ构建自统一医学语言系统（UMLS），这是一个大规模标准化生物医学词汇和知识图谱的存储库。我们将知识评估构建成一个二元判断任务，要求LLM验证从可靠和结构化的知识来源中提取的医学陈述的正确性。  我们的实验表明，LLM在医学事实知识保留方面存在困难，在不同的语义类别上表现出显著的性能差异，特别是对于罕见的医学状况。此外，LLM显示出较差的校准度，经常对错误答案过于自信。为了缓解这些问题，我们探讨了增强检索生成方法，证明其在提高事实准确性以及减少医学决策中的不确定性方面的有效性。|
|**2025-02-20**|**PaperHelper: Knowledge-Based LLM QA Paper Reading Assistant**|Congrui Yin et.al.|[2502.14271](http://arxiv.org/abs/2502.14271)|null|在本文中，我们介绍了一种论文阅读助手PaperHelper，这是一种旨在提高研究人员高效浏览和理解科学文献能力的强大工具。通过利用检索增强生成（RAG）框架，PaperHelper有效地减少了大型语言模型（LLMs）中常见的幻觉现象，优化了准确、高质量知识的提取。采用诸如RAFT和RAG Fusion等先进技术显著提升了基于LLMs的文献综述过程的性能、准确性和可靠性。此外，PaperHelper具有用户友好的界面，便于批量下载文档，并使用Mermaid格式来展示文档之间的结构关系。实验结果表明，基于微调后的GPT-4 API的PaperHelper达到了60.04的F1分数，延迟仅为5.8秒，比基本RAG模型在F1分数上高出7%。|
|**2025-02-19**|**Collaborative Retrieval for Large Language Model-based Conversational Recommender Systems**|Yaochen Zhu et.al.|[2502.14137](http://arxiv.org/abs/2502.14137)|null|对话推荐系统（CRS）旨在通过与用户的交互式对话提供个性化推荐。虽然大型语言模型（LLM）凭借其对上下文感知用户偏好的卓越理解能力增强了CRS，但它们通常难以利用行为数据，而这些数据对于基于经典协同过滤（CF）的方法来说非常重要。为此，我们提出了CRAG，即用于LLM基础的CRS的协作检索增强生成方法。据我们所知，CRAG是首个将最先进的LLM与CF结合用于对话推荐的方法。我们在两个公开的电影对话推荐数据集上的实验，即一个精炼的Reddit数据集（我们称之为Reddit-v2）以及Redial数据集，展示了CRAG在项目覆盖率和推荐性能方面优于多个CRS基线。此外，我们观察到改进主要体现在对新上映电影的推荐准确性上。代码和数据可在https://github.com/yaochenzhu/CRAG获取。|
|**2025-02-19**|**Towards Context-Robust LLMs: A Gated Representation Fine-tuning Approach**|Shenglai Zeng et.al.|[2502.14100](http://arxiv.org/abs/2502.14100)|null|大型语言模型（LLM）通过检索增强生成（RAG）等方法结合外部上下文时，常常面临处理不完美证据的挑战。它们往往过度依赖外部知识，这使得它们容易受到误导和无用上下文的影响。为了解决这一问题，我们提出了上下文鲁棒的LLM概念，这种模型能够有效地平衡内部知识与外部上下文，类似于人类的认知过程。具体来说，上下文鲁棒的LLM应该只在缺乏内部知识时依赖外部上下文，识别内部和外部知识之间的矛盾，并忽略无用的上下文。为了实现这一目标，我们引入了Grft，这是一种轻量级且即插即用的门控表示微调方法。Grft包括两个关键组件：一个用于检测和过滤问题输入的门控机制，以及用于调整隐藏表示的低秩表示适配器。通过在不到200个样本上训练仅占模型大小0.0004%的轻量级干预函数，Grft可以有效地使LLM表现出上下文鲁棒的行为。|
|**2025-02-19**|**RAG-Gym: Optimizing Reasoning and Search Agents with Process Supervision**|Guangzhi Xiong et.al.|[2502.13957](http://arxiv.org/abs/2502.13957)|null|
|**2025-02-19**|**DH-RAG: A Dynamic Historical Context-Powered Retrieval-Augmented Generation Method for Multi-Turn Dialogue**|Feiyuan Zhang et.al.|[2502.13847](http://arxiv.org/abs/2502.13847)|null|
|**2025-02-19**|**In-Place Updates of a Graph Index for Streaming Approximate Nearest Neighbor Search**|Haike Xu et.al.|[2502.13826](http://arxiv.org/abs/2502.13826)|null|
|**2025-02-19**|**TrustRAG: An Information Assistant with Retrieval Augmented Generation**|Yixing Fan et.al.|[2502.13719](http://arxiv.org/abs/2502.13719)|null|
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
|**2025-02-05**|**Rankify: A Comprehensive Python Toolkit for Retrieval, Re-Ranking, and Retrieval-Augmented Generation**|Abdelrahman Abdallah et.al.|[2502.02464](http://arxiv.org/abs/2502.02464)|null|
|**2025-02-04**|**Personalization Toolkit: Training Free Personalization of Large Vision Language Models**|Soroush Seifi et.al.|[2502.02452](http://arxiv.org/abs/2502.02452)|null|
|**2025-02-04**|**Conversation AI Dialog for Medicare powered by Finetuning and Retrieval Augmented Generation**|Atharva Mangeshkumar Agrawal et.al.|[2502.02249](http://arxiv.org/abs/2502.02249)|null|
|**2025-02-04**|**LLMSecConfig: An LLM-Based Approach for Fixing Software Container Misconfigurations**|Ziyang Ye et.al.|[2502.02009](http://arxiv.org/abs/2502.02009)|null|
|**2025-02-04**|**MPIC: Position-Independent Multimodal Context Caching System for Efficient MLLM Serving**|Shiju Zhao et.al.|[2502.01960](http://arxiv.org/abs/2502.01960)|null|
|**2025-02-03**|**Position: Towards a Responsible LLM-empowered Multi-Agent Systems**|Jinwei Hu et.al.|[2502.01714](http://arxiv.org/abs/2502.01714)|null|
|**2025-02-03**|**VideoRAG: Retrieval-Augmented Generation with Extreme Long-Context Videos**|Xubin Ren et.al.|[2502.01549](http://arxiv.org/abs/2502.01549)|null|
|**2025-02-03**|**CondAmbigQA: A Benchmark and Dataset for Conditional Ambiguous Question Answering**|Zongxi Li et.al.|[2502.01523](http://arxiv.org/abs/2502.01523)|null|
|**2025-02-03**|**Topic-FlipRAG: Topic-Orientated Adversarial Opinion Manipulation Attacks to Retrieval-Augmented Generation Models**|Yuyang Gong et.al.|[2502.01386](http://arxiv.org/abs/2502.01386)|null|
|**2025-01-28**|**SafeRAG: Benchmarking Security in Retrieval-Augmented Generation of Large Language Model**|Xun Liang et.al.|[2501.18636](http://arxiv.org/abs/2501.18636)|**[link](https://github.com/iaar-shanghai/saferag)**|
|**2025-01-30**|**Can we Retrieve Everything All at Once? ARM: An Alignment-Oriented LLM-based Retrieval Method**|Peter Baile Chen et.al.|[2501.18539](http://arxiv.org/abs/2501.18539)|null|
|**2025-01-30**|**RbFT: Robust Fine-tuning for Retrieval-Augmented Generation against Retrieval Defects**|Yiteng Tu et.al.|[2501.18365](http://arxiv.org/abs/2501.18365)|**[link](https://github.com/StibiumT16/Robust-Fine-tuning)**|
|**2025-01-30**|**Leveraging LLM Agents for Automated Optimization Modeling for SASP Problems: A Graph-RAG based Approach**|Tianpeng Pan et.al.|[2501.18320](http://arxiv.org/abs/2501.18320)|null|
|**2025-01-29**|**GLLM: Self-Corrective G-Code Generation using Large Language Models with User Feedback**|Mohamed Abdelaal et.al.|[2501.17584](http://arxiv.org/abs/2501.17584)|null|
|**2025-01-29**|**AugmenTest: Enhancing Tests with LLM-Driven Oracles**|Shaker Mahmud Khandaker et.al.|[2501.17461](http://arxiv.org/abs/2501.17461)|null|
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

<p align=right>(<a href=#updated-on-20250224>back to top</a>)</p>

## text2sql

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-02-17**|**SQL-o1: A Self-Reward Heuristic Dynamic Search Method for Text-to-SQL**|Shuai Lyu et.al.|[2502.11741](http://arxiv.org/abs/2502.11741)|**[link](https://github.com/shuailyu0110/sql-o1)**|**文本到SQL（Text2SQL）任务旨在将自然语言查询转换为可执行的SQL查询。得益于大型语言模型（LLMs）的应用，该领域已经取得了显著进展。然而，诸如模型可扩展性、有限的生成空间以及SQL生成中的连贯性问题等挑战仍然存在。为了解决这些问题，我们提出了SQL-o1，这是一种基于自我奖励的启发式搜索方法，旨在增强LLMs在SQL查询生成中的推理能力。SQL-o1结合了蒙特卡洛树搜索（MCTS）进行启发式过程级搜索，并构建了一个Schema感知的数据集，以帮助模型更好地理解数据库模式。在Bird和Spider数据集上的广泛实验表明，与最新的基线方法相比，SQL-o1在复杂的Bird数据集上提高了10.8%的执行准确率，甚至超过了基于GPT-4的方法。此外，SQL-o1在少量学习场景中表现出色，并显示出强大的跨模型迁移能力。我们的代码公开发布于：https://github.com/ShuaiLyu0110/SQL-o1。**|
|**2025-01-30**|**Fundamental Challenges in Evaluating Text2SQL Solutions and Detecting Their Limitations**|Cedric Renggli et.al.|[2501.18197](http://arxiv.org/abs/2501.18197)|null|在这项工作中，我们深入探讨了评估Text2SQL解决方案的基本挑战，并指出了潜在的失败原因以及依赖现有基准中的聚合指标可能带来的风险。我们识别出当前开放基准中两个主要未解决的局限性：（1）评估数据中的数据质量问题，主要是由于未能捕捉自然语言描述转化为结构化查询过程中的概率性质（例如，自然语言的歧义），以及（2）使用不同的匹配函数作为SQL等价性的近似方法所引入的偏差。为了将这两种局限性置于具体情境中，我们提出了一种统一的分类法，涵盖了可能导致预测和评估错误的所有Text2SQL局限性。然后，我们通过使用最先进的Text2SQL解决方案和基准对这些局限性进行了调查来论证这一分类法。我们用实际例子描述了局限性的原因，并为分类法中的每个类别提出了潜在的缓解方案。最后，我们强调了在部署此类缓解策略或尝试自动应用该分类法时遇到的开放性挑战。|
|**2025-02-13**|**Is Long Context All You Need? Leveraging LLM's Extended Context for NL2SQL**|Yeounoh Chung et.al.|[2501.12372](http://arxiv.org/abs/2501.12372)|null|大型语言模型（LLMs）在一系列自然语言处理任务中展示了令人印象深刻的能力。特别是在推理能力和上下文窗口扩展方面的改进为利用这些强大的模型开辟了新的途径。NL2SQL是一个具有挑战性的领域，因为自然语言问题本质上是模糊的，而生成SQL查询则需要对复杂的数据模式和语义有精确的理解。解决这种语义模糊问题的一种方法是提供更多且充足的上下文信息。在这项工作中，我们探索了由谷歌最先进的LLM（gemini-1.5-pro）提供的扩展上下文窗口（也称为长上下文）在性能和延迟之间的权衡。我们研究了各种上下文信息的影响，包括列示例值、问题与SQL查询对、用户提供的提示、SQL文档和模式。据我们所知，这是首次研究扩展上下文窗口和额外上下文信息如何在准确性和延迟成本方面帮助NL2SQL生成的工作。我们表明，长上下文LLMs是健壮的，并不会迷失在扩展的上下文信息中。此外，基于谷歌gemini-pro-1.5的长上下文NL2SQL管道在多个基准数据集上实现了强大的表现，无需微调和昂贵的自一致性技术。|
|**2025-02-08**|**Semantic Captioning: Benchmark Dataset and Graph-Aware Few-Shot In-Context Learning for SQL2Text**|Ali Al-Lawati et.al.|[2501.03166](http://arxiv.org/abs/2501.03166)|**[link](https://github.com/aliwister/ast-icl)**|**大型语言模型（LLM）在各种自然语言处理任务中表现出色，包括将自然语言转换为形式化代码表示的语义解析。然而，将代码转换为自然语言的过程，即语义标注，受到的关注较少。随着LLM被集成到代码生成、安全分析和教育平台中，这项任务变得越来越重要。本文重点关注SQL查询的标注（SQL2Text），以应对理解并解释SQL查询的需求，尤其是在LLM生成的代码可能带来潜在安全风险的时代。我们通过引入使用GPT-4o生成多个额外表述的迭代ICL提示，重新利用Text2SQL数据集进行SQL2Text任务，从而增强了数据集在反向任务中的鲁棒性。我们基于不同的样本选择方法进行了基于上下文学习（ICL）的实验，重点放在更小、计算效率更高的LLM上。研究结果表明，利用SQL固有的图属性进行ICL样本选择，在BLEU评分上比随机选择高出多达39%，并且优于其他方法。数据集和代码已发布：https://github.com/aliwister/ast-icl。**|
|**2025-01-03**|**CarbonChat: Large Language Model-Based Corporate Carbon Emission Analysis and Climate Knowledge Q&A System**|Zhixuan Cao et.al.|[2501.02031](http://arxiv.org/abs/2501.02031)|null|随着全球气候变化的影响加剧，企业碳排放已成为全球关注的焦点。针对大型语言模型中气候变化知识更新滞后、传统增强生成架构在处理复杂问题时缺乏专业性和准确性以及可持续性报告分析成本高且耗时等问题，本文提出了CarbonChat：基于大型语言模型的企业碳排放分析与气候知识问答系统，旨在实现精准的碳排放分析和政策理解。首先，提出了一种多样化的指标模块构建方法，用于处理基于规则和长文本文档的分割以及结构化数据的提取，从而优化关键信息的解析。其次，设计了一种增强的自提示检索增强生成架构，集成了意图识别、结构化推理链、混合检索和Text2SQL，提高了语义理解和查询转换的效率。接下来，基于温室气体核算框架，建立了14个维度进行碳排放分析，能够实现报告总结、相关性评估和定制化响应。最后，通过多层次分块机制、时间戳和幻觉检测功能，确保了分析结果的准确性和可验证性，降低了幻觉率并提高了响应的精度。|
|**2024-12-22**|**A Plug-and-Play Natural Language Rewriter for Natural Language to SQL**|Peixian Ma et.al.|[2412.17068](http://arxiv.org/abs/2412.17068)|null|现有的自然语言到SQL（NL2SQL）解决方案已经取得了显著进展，但仍存在一些挑战，主要原因是用户对数据库模式的理解有限或对特定表或列值的记忆偏差。这些挑战经常导致NL2SQL翻译不正确。为了解决这些问题，我们提出了REWRITER，这是一个即插即用的模块，旨在通过自动重写模糊或有缺陷的自然语言查询来增强NL2SQL系统。通过结合数据库知识和内容（例如，列值和外键），REWRITER减少了由于有缺陷的自然语言输入导致的错误，并提高了SQL生成的准确性。我们的REWRITER将NL2SQL模型视为黑盒，确保与各种NL2SQL方法兼容，包括基于代理和基于规则的NL2SQL解决方案。REWRITER由三个关键组件组成：检查器、反射器和重写器。检查器通过评估生成的SQL的正确性来识别有缺陷的自然语言查询，从而减少不必要的重写和潜在的幻觉。反射器分析并积累经验以识别自然语言查询中的问题，而重写器则根据反射器的反馈修改查询。在Spider和BIRD基准上的广泛实验表明，REWRITER始终能够增强下游模型，在执行准确性方面分别平均提高了1.6%和2.0%。|
|**2024-12-17**|**SynthCypher: A Fully Synthetic Data Generation Framework for Text-to-Cypher Querying in Knowledge Graphs**|Aman Tiwari et.al.|[2412.12612](http://arxiv.org/abs/2412.12612)|null|
|**2024-12-13**|**ROUTE: Robust Multitask Tuning and Collaboration for Text-to-SQL**|Yang Qin et.al.|[2412.10138](http://arxiv.org/abs/2412.10138)|**[link](https://github.com/alibaba/route)**|**尽管大型语言模型（LLMs）在文本到SQL（Text2SQL）方面取得了显著进展，但最新的技术仍然局限于闭源LLM（如GPT-4）的上下文学习中，这限制了它们在开放场景中的应用。为了解决这一挑战，我们提出了一种新颖的鲁棒多任务调优和协作方法（ROUTE），以提高开源LLM在Text2SQL方面的综合能力，从而提供一种更为实用的解决方案。我们的方法首先使用多种与SQL生成相关的合成训练数据进行多任务监督微调（SFT）。与现有的基于SFT的Text2SQL方法不同，我们引入了几个额外的SFT任务，包括模式链接、噪声校正和连续写作。参与多种SQL生成任务增强了模型对SQL语法的理解，并提高了其生成高质量SQL查询的能力。此外，受LLM代理的协作模式启发，我们引入了一种多任务协作提示策略（MCP）。该策略通过跨多个SQL相关任务的协作来减少SQL生成过程中的幻觉，从而最大限度地发挥显式多任务能力在提升Text2SQL性能方面的潜力。我们在八个开源LLM和五个广泛使用的基准上进行了广泛的实验和深入分析。结果表明，我们的方法优于最新的Text2SQL方法，并取得了领先的性能。**|
|**2024-12-04**|**DataLab: A Unified Platform for LLM-Powered Business Intelligence**|Luoxuan Weng et.al.|[2412.02205](http://arxiv.org/abs/2412.02205)|null|商业智能（BI）将现代组织中的大量数据转化为可执行的见解，以支持明智的决策。最近，基于大型语言模型（LLM）的代理通过根据自然语言（NL）查询自动执行任务规划、推理和操作，简化了BI工作流程。然而，现有的方法主要集中在单个BI任务上，如NL2SQL和NL2VIS。由于BI的迭代性和协作性，任务在不同数据角色和工具之间的分散导致了效率低下和潜在错误。在本文中，我们介绍了DataLab，这是一个统一的BI平台，集成了一个一站式的基于LLM的代理框架和增强的计算笔记本界面。DataLab通过在一个环境中无缝结合LLM辅助与用户自定义，为不同的数据角色支持广泛的BI任务。为了实现这一整合，我们设计了一个针对企业特定BI任务的领域知识融合模块、一个跨BI工作流的信息共享机制以及一种单元格上下文管理策略，以提高BI笔记本中的上下文利用效率。大量的实验表明，DataLab在各种流行的基准测试中的多种BI任务上达到了最先进的性能。此外，DataLab在腾讯的真实世界数据集上保持了高效性和有效性，在企业特定的BI任务上实现了高达58.58%的准确率提升和61.65%的代币成本降低。|
|**2024-11-05**|**Grounding Natural Language to SQL Translation with Data-Based Self-Explanations**|Yuankai Fan et.al.|[2411.02948](http://arxiv.org/abs/2411.02948)|**[link](https://github.com/Kaimary/CycleSQL)**|**自然语言接口使非技术用户能够使用自然语言（NL）与数据进行交互。先进的方法通常利用神经序列到序列模型或最近更复杂的大型语言模型，以端到端的方式实现从自然语言到SQL（NL2SQL）的转换。然而，就像人类一样，这些端到端的翻译模型并不总能在第一次尝试时生成最佳的SQL输出。在本文中，我们提出了CycleSQL，这是一个迭代框架，旨在让端到端翻译模型通过自我评估自主生成最佳输出。CycleSQL的主要思想是引入基于数据的查询结果自然语言解释作为自我提供的反馈，并利用该反馈来迭代验证翻译的正确性，从而提高整体翻译准确性。为了研究CycleSQL，我们在五个广泛使用的基准测试上将其应用于七个现有的翻译模型，进行了包括定量和定性评估在内的广泛实验。结果显示：1）CycleSQL中引入的反馈循环可以一致地提高现有模型的性能，特别是将CycleSQL应用于REDSQL时，在Spider基准测试的验证集上获得了82.0%（+2.6%）的翻译准确率，在测试集上获得了81.6%（+3.2%）的翻译准确率；2）生成的自然语言解释还可以为用户提供有价值的见解，帮助理解翻译结果，从而增强NL2SQL翻译的可解释性。**|
|**2024-10-30**|**BIS: NL2SQL Service Evaluation Benchmark for Business Intelligence Scenarios**|Bora Caglayan et.al.|[2410.22925](http://arxiv.org/abs/2410.22925)|**[link](https://github.com/boracaglayan/bis-nl2sql)**|**近年来，自然语言到结构化查询语言（NL2SQL）的转换在商业智能（BI）应用中得到了广泛采用。然而，现有的NL2SQL基准并不适合生产环境中的BI场景，因为它们并不是为常见的商业智能问题设计的。为了解决这一差距，我们开发了一个专注于工业BI场景中典型自然语言问题的新基准。我们讨论了构建以BI为重点的基准所面临的挑战以及现有基准的不足之处。此外，我们在基准中引入了反映常见BI查询的问题类别。最后，我们提出了两种新的语义相似性评估指标，用于评估BI应用程序和服务中的NL2SQL能力。**|
|**2024-10-15**|**LR-SQL: A Supervised Fine-Tuning Method for Text2SQL Tasks under Low-Resource Scenarios**|Wen Wuzhenghong et.al.|[2410.11457](http://arxiv.org/abs/2410.11457)|**[link](https://github.com/hongwin/lr-sql)**|
|**2024-08-27**|**Text2SQL is Not Enough: Unifying AI and Databases with TAG**|Asim Biswal et.al.|[2408.14717](http://arxiv.org/abs/2408.14717)|**[link](https://github.com/tag-research/tag-bench)**|
|**2024-12-04**|**A Survey of NL2SQL with Large Language Models: Where are we, and where are we going?**|Xinyu Liu et.al.|[2408.05109](http://arxiv.org/abs/2408.05109)|**[link](https://github.com/hkustdial/nl2sql_handbook)**|
|**2024-07-21**|**Towards Automated Data Sciences with Natural Language and SageCopilot: Practices and Lessons Learned**|Yuan Liao et.al.|[2407.21040](http://arxiv.org/abs/2407.21040)|null|
|**2024-11-07**|**A Survey on Employing Large Language Models for Text-to-SQL Tasks**|Liang Shi et.al.|[2407.15186](http://arxiv.org/abs/2407.15186)|null|
|**2024-06-12**|**DeTriever: Decoder-representation-based Retriever for Improving NL2SQL In-Context Learning**|Yuxi Feng et.al.|[2406.07913](http://arxiv.org/abs/2406.07913)|null|
|**2024-07-27**|**The Dawn of Natural Language to SQL: Are We Fully Ready?**|Boyan Li et.al.|[2406.01265](http://arxiv.org/abs/2406.01265)|**[link](https://github.com/hkustdial/nl2sql360)**|
|**2024-05-01**|**ChatBI: Towards Natural Language to Complex Business Intelligence SQL**|Jinqing Lian et.al.|[2405.00527](http://arxiv.org/abs/2405.00527)|null|
|**2024-03-29**|**PURPLE: Making a Large Language Model a Better SQL Writer**|Tonghui Ren et.al.|[2403.20014](http://arxiv.org/abs/2403.20014)|null|

<p align=right>(<a href=#updated-on-20250224>back to top</a>)</p>

## PPC

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-02-20**|**Vision Foundation Models in Medical Image Analysis: Advances and Challenges**|Pengchen Liang et.al.|[2502.14584](http://arxiv.org/abs/2502.14584)|null|视觉基础模型（VFM），特别是视觉变换器（ViT）和Segment Anything Model（SAM）的快速发展，在医学图像分析领域引发了显著的进步。这些模型在捕捉长距离依赖关系和实现高泛化能力方面表现出色。然而，将这些大型模型应用于医学图像分析面临若干挑战，包括医学图像与自然图像之间的域差异、高效的模型适应策略的需求以及小规模医学数据集的限制。本文综述了VFMs在医学图像分割领域的最新研究进展，重点关注域适应、模型压缩和联邦学习方面的挑战。我们讨论了基于适配器改进、知识蒸馏技术和多尺度上下文特征建模的最新发展，并提出了克服这些瓶颈的未来方向。我们的分析强调了VFMs结合新兴方法如联邦学习和模型压缩在革新医学图像分析和增强临床应用方面的潜力。本工作的目标是提供当前方法的全面概述，并建议未来研究的关键领域，以推动医学图像分割领域的下一波创新。|
|**2025-02-20**|**FUIA: Model Inversion Attack against Federated Unlearning**|Lei Zhou et.al.|[2502.14558](http://arxiv.org/abs/2502.14558)|null|随着“被遗忘权”相关法规的出台，联邦学习（FL）面临着新的隐私合规挑战。为应对这些挑战，研究人员提出了联邦卸载学习（FU）。然而，现有的FU研究主要集中在提高卸载效率上，较少关注这些方法中潜在的隐私漏洞。为填补这一空白，我们从FL中的梯度反转攻击中汲取灵感，提出了联邦卸载学习反转攻击（FUIA）。FUIA专门针对三种类型的FU（样本卸载、客户端卸载和类别卸载），旨在全面分析与FU相关的隐私泄露风险。在FUIA中，服务器作为诚实但好奇的攻击者，记录并利用卸载前后模型的差异来暴露被遗忘数据的特征和标签。FUIA显著泄露了被遗忘数据的隐私，并可以针对所有类型的FU。这种攻击违背了FU消除特定数据影响的目标，反而利用其漏洞恢复被遗忘的数据并暴露其隐私缺陷。广泛的实验结果表明，FUIA能够有效揭示被遗忘数据的私人信息。为了减轻这种隐私泄露，我们还探讨了两种潜在的防御方法，尽管这些方法会以降低卸载效果和卸载后模型的可用性为代价。|
|**2025-02-20**|**PQBFL: A Post-Quantum Blockchain-based Protocol for Federated Learning**|Hadi GHaravi et.al.|[2502.14464](http://arxiv.org/abs/2502.14464)|null|联邦学习（FL）的一个目标是通过远程参与者的本地模型协作训练一个全局模型。然而，FL过程容易受到各种安全挑战的影响，包括模型的拦截和篡改、通过共享梯度导致的信息泄露以及在敏感领域（如医疗环境）中暴露参与者身份或数据的隐私泄露。此外，量子计算的出现通过Shor和Grover算法对现有的加密协议构成了严重威胁，导致FL系统通信中的安全问题。为了解决这些挑战，我们提出了一种基于后量子区块链的联邦学习协议（PQBFL），该协议利用后量子密码（PQC）算法和区块链来增强FL系统的模型安全性和参与者身份隐私。它采用了一种混合通信策略，结合了链下和链上通道，以优化成本效率、提高安全性和保护参与者隐私，同时确保FL系统中基于声誉的身份验证的问责制。PQBFL特别针对FL迭代性质的安全需求进行了设计，这是文献中较少提及的一点。因此，它利用棘轮机制在整个学习过程中提供前向保密和后妥协安全性。总之，PQBFL为联邦学习提供了一个安全且有弹性的解决方案，非常适合量子计算时代的需求。|
|**2025-02-20**|**VFL-RPS: Relevant Participant Selection in Vertical Federated Learning**|Afsana Khan et.al.|[2502.14375](http://arxiv.org/abs/2502.14375)|null|联邦学习（FL）允许不同参与者之间的协作，同时确保这些参与者之间的数据不被共享。然而，并非每次协作都有助于提高模型性能。因此，选择正确的协作参与者是一个重要的挑战。目前，文献中大多数关于参与者选择的努力都集中在横向联邦学习（HFL）上，假设所有参与者的所有特征都是相同的，而忽略了参与者之间可能存在不同特征的情况，这种情况在纵向联邦学习（VFL）中得到了体现。为了填补这一研究空白，我们提出了一种新的方法VFL-RPS，用于VFL中的参与者选择，作为预训练步骤。我们在多个数据集上进行了测试，执行了回归和分类任务，结果显示，通过仅选择少数参与者，我们的方法能够达到与使用全部数据相当的结果。此外，我们还展示了我们的方法在VFL的参与者选择方面优于现有方法。|
|**2025-02-20**|**A Note on Efficient Privacy-Preserving Similarity Search for Encrypted Vectors**|Dongfang Zhao et.al.|[2502.14291](http://arxiv.org/abs/2502.14291)|null|传统的向量相似性搜索方法在处理加密数据时依赖于全同态加密（FHE），以实现在不解密的情况下进行计算。然而，FHE的大量计算开销使其在大规模实时应用中不切实际。本文探讨了一种更高效的替代方案：使用加法同态加密（AHE）进行隐私保护相似性搜索。我们考虑了查询向量或数据库向量之一保持加密的情况，这种情况在诸如保密推荐系统和安全联邦学习等应用中经常出现。虽然AHE仅支持加法和标量乘法，但我们展示了它足以计算内积相似性——这是向量检索中最广泛使用的相似性度量之一。与基于FHE的解决方案相比，我们的方法通过避免密文-密文乘法和引导操作显著减少了计算开销，同时仍保持正确性和隐私性。我们提出了一种在AHE下进行加密相似性搜索的有效算法，并分析了其误差增长和安全性影响。我们的方法为现实世界中的机器学习应用提供了可扩展且实用的隐私保护向量搜索解决方案。|
|**2025-02-20**|**Accurate Forgetting for Heterogeneous Federated Continual Learning**|Abudukelimu Wuerkaixi et.al.|[2502.14205](http://arxiv.org/abs/2502.14205)|null|近年来，联邦学习（FL）引起了越来越多的关注。然而，在客户端参与顺序学习的场景下，相关研究仍较为有限。将联邦学习与持续学习（CL）结合，产生了一个具有挑战性的实际问题：联邦持续学习（FCL）。现有的FCL研究主要集中在减轻持续学习中的灾难性遗忘问题，同时与其他客户端协作。我们认为遗忘现象并不总是有害的。在本文中，我们考虑了一个更实用且更具挑战性的FCL设置，其中不同客户端的数据或任务可能是无关甚至对立的。在联邦学习场景中，客户端之间的统计异质性和数据噪声可能会导致虚假相关性，从而造成特征学习的偏差。尽管现有的持续学习策略侧重于充分利用先前的知识，我们在研究中发现忘记有偏差的信息是有益的。因此，我们提出了一个新的概念——准确遗忘（AF），并开发了一种新的生成重放方法~\method~，该方法在联邦网络中有选择地利用先前的知识。我们采用基于归一化流模型的概率框架来量化先前知识的可信度。综合实验表明，我们的方法优于基线方法。|
|**2025-02-20**|**Federated Fine-Tuning of Large Language Models: Kahneman-Tversky vs. Direct Preference Optimization**|Fernando Spadea et.al.|[2502.14187](http://arxiv.org/abs/2502.14187)|null|我们评估了Kahneman-Tversky优化（KTO）作为大型语言模型（LLM）在联邦学习（FL）设置中的微调方法，并将其与直接偏好优化（DPO）进行了比较。使用Alpaca-7B作为基础模型，我们在一个现实的数据集上用这两种方法进行微调，并使用MT-Bench-1、Vicuna和AdvBench基准来评估性能。此外，我们引入了一个重新分配的数据集设置，在这种设置下，由于KTO能够处理单响应反馈，而DPO依赖于成对响应，因此只有KTO适用。我们的结果表明，无论是原始配置（KTOO）还是重新分配配置（KTOR），KTO在所有基准测试中都持续优于DPO。在重新分配的设置中，KTO进一步验证了其灵活性和鲁棒性，在DPO无法应用的情况下仍保持优越性能。这些发现确立了KTO作为一种稳健且可扩展的微调方法在联邦学习中的地位，鼓励其在保护隐私、去中心化和异构环境中的采用。|
|**2025-02-20**|**Blockchain-based Framework for Scalable and Incentivized Federated Learning**|Bijun Wu et.al.|[2502.14170](http://arxiv.org/abs/2502.14170)|null|联邦学习（FL）能够在不共享原始数据的情况下实现协作模型训练，既保护了隐私又利用了分布式数据集。然而，传统的FL系统通常依赖于中心化的聚合机制，这带来了信任问题、单点故障以及对有意义的客户端贡献激励不足的问题。随着FL扩展到训练资源密集型模型（如大型语言模型LLM），这些挑战变得更加严重，需要可扩展的、去中心化的解决方案。本文提出了一种基于区块链的FL框架，通过集成智能合约和一种新颖的混合激励机制来解决这些问题。该框架自动化了FL的关键任务，包括客户端注册、更新验证、奖励分配以及维护透明的全局状态。混合激励机制结合了链上对齐奖励、链下公平性检查和一致性乘数，以确保公平性、透明性和持续参与。我们通过gas成本分析对该框架进行了评估，证明了其在不同规模的联邦学习场景中的可行性。|
|**2025-02-19**|**Homophily Heterogeneity Matters in Graph Federated Learning: A Spectrum Sharing and Complementing Perspective**|Wentao Yu et.al.|[2502.13732](http://arxiv.org/abs/2502.13732)|null|由于异质性是图联邦学习中的一个基本挑战，许多现有方法被提出用于处理节点特征异质性和结构异质性。然而，它们忽视了关键的同质性异质性，即不同客户端的图数据在同质性水平上存在显著差异。同质性水平表示连接属于同一类别的节点的边的比例。由于适应本地同质性，局部模型在不同客户端之间捕获不一致的谱特性，这大大降低了协作的有效性。具体来说，在高同质性图上训练的局部模型倾向于捕获低频信息，而在低同质性图上训练的局部模型倾向于捕获高频信息。为有效应对同质性异质性，我们引入了谱图神经网络（GNN），并提出了一种通过挖掘图谱特性的新型联邦学习方法（FedGSP）。一方面，我们提出的FedGSP使客户端能够共享通用的谱特性（即低频信息），从而使所有客户端通过协作受益。另一方面，受我们理论发现的启发，我们提出的FedGSP允许客户端通过获取他们缺乏的谱特性（即高频信息）来补充非通用的谱特性，从而获得额外的信息增益。在六个同质性和五个异质性图数据集上进行的广泛实验，涵盖非重叠和重叠设置，验证了我们的方法优于十一种最先进方法的优势。值得注意的是，在所有异质性数据集上，我们的FedGSP平均比第二好的方法高出3.28%。|
|**2025-02-19**|**Smoothed Normalization for Efficient Distributed Private Optimization**|Egor Shulgin et.al.|[2502.13482](http://arxiv.org/abs/2502.13482)|null|联邦学习能够在保护参与者隐私的同时训练机器学习模型。令人惊讶的是，目前还没有针对平滑非凸优化问题的差分隐私分布式方法。原因在于标准的隐私技术要求限制参与者的贡献，这通常是通过对更新进行“裁剪”来实现的。现有文献通常通过假设梯度范数有界或分析带裁剪的分布式算法但忽略差分隐私约束来忽略裁剪的影响。在这项工作中，我们研究了一种通过更新的“平滑归一化”替代方法，其在单节点设置中的表现良好。通过将平滑归一化与误差反馈机制相结合，我们设计了一种新的分布式算法α-NormEC。我们证明了我们的方法比先前的工作具有更好的收敛率。通过将α-NormEC扩展到差分隐私设置中，我们获得了第一个具有可证明收敛保证的差分隐私分布式优化算法。最后，从神经网络训练的实证结果表明，α-NormEC在不同的参数设置下表现出稳健的收敛性。|
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

<p align=right>(<a href=#updated-on-20250224>back to top</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[contributors-url]: https://github.com/Vincentqyw/cv-arxiv-daily/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[forks-url]: https://github.com/Vincentqyw/cv-arxiv-daily/network/members
[stars-shield]: https://img.shields.io/github/stars/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[stars-url]: https://github.com/Vincentqyw/cv-arxiv-daily/stargazers
[issues-shield]: https://img.shields.io/github/issues/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[issues-url]: https://github.com/Vincentqyw/cv-arxiv-daily/issues

