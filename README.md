[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## Updated on 2025.03.10
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
|**2025-03-06**|**ToolFuzz -- Automated Agent Tool Testing**|Ivan Milev et.al.|[2503.04479](http://arxiv.org/abs/2503.04479)|null|大型语言模型（LLM）代理利用LLM在实际应用中的高级推理能力。为了与环境交互，这些代理通常依赖于工具，如网络搜索或数据库API。当代理将工具文档连同用户查询一起提供给LLM时，该文档的完整性和正确性至关重要。然而，工具文档往往存在过度指定、指定不足或错误指定的问题，这阻碍了代理的准确性。标准的软件测试方法难以识别这些以自然语言表达的错误。因此，尽管其重要性，目前还没有自动化的方法来测试工具文档。为了解决这个问题，我们提出了ToolFuzz，这是首个用于自动测试工具文档的方法。ToolFuzz旨在发现两种类型的错误：(1) 导致工具运行时错误的用户查询；(2) 导致代理响应不正确的用户查询。ToolFuzz能够生成大量多样化的自然输入，有效地以低误报率找到工具描述中的错误。此外，我们还介绍了两种简单的提示工程方法。我们在32个常见的LangChain工具和35个新创建的自定义工具以及2个新的基准上评估了这三种工具测试方法，以进一步加强评估。我们发现许多公开可用的工具存在指定不足的问题。具体来说，我们展示了ToolFuzz相比提示工程方法能识别出20倍以上的错误输入，使其成为构建可靠AI代理的关键组件。|
|**2025-03-06**|**Measuring temporal effects of agent knowledge by date-controlled tool use**|R. Patrick Xian et.al.|[2503.04188](http://arxiv.org/abs/2503.04188)|null|时间进展是知识积累和更新的重要组成部分。网络搜索常被用作代理知识的基础，但其不恰当的配置会影响代理响应的质量。在这里，我们构建了一个基于工具的样本外测试框架，以衡量来自不同日期控制工具（DCTs）的大语言模型（LLM）代理的知识变异性。我们展示了作为写作助手的LLM代理在使用网络搜索帮助完成科学出版物摘要时的时间效应。我们表明，搜索引擎的时间效应会转化为工具依赖性的代理性能，但可以通过选择基础模型和明确的推理指令（如思维链提示）来缓解。我们的结果表明，代理评估应采取动态视角，并考虑到工具的时间影响以及外部资源的更新。|
|**2025-03-06**|**InterChat: Enhancing Generative Visual Analytics using Multimodal Interactions**|Juntong Chen et.al.|[2503.04110](http://arxiv.org/abs/2503.04110)|null|大型语言模型（LLM）和生成式可视化分析系统的兴起已经改变了数据驱动的洞察方式，但在准确解释用户的分析意图和交互意图方面仍然存在重大挑战。虽然语言输入提供了灵活性，但它们往往缺乏精确性，使得复杂意图的表达变得低效、容易出错且耗时。为了解决这些局限性，我们通过文献综述和初步头脑风暴会议探讨了生成式可视化分析中多模态交互的设计空间。基于这些见解，我们引入了一个高度可扩展的工作流程，该流程集成了多个LLM代理以进行意图推断和可视化生成。我们开发了InterChat，这是一个生成式可视化分析系统，结合了视觉元素的直接操作和自然语言输入。这种集成使意图沟通更加精确，并支持渐进式的、以视觉为导向的探索性数据分析。通过有效的提示工程、上下文交互链接以及直观的可视化和交互设计，InterChat在用户交互和LLM驱动的可视化之间架起了桥梁，提高了可解释性和可用性。广泛的评估，包括两个使用场景、一项用户研究和专家反馈，展示了InterChat的有效性。结果表明，在处理复杂的可视化分析任务时，准确性和效率都有显著提高，突显了多模态交互在重新定义用户参与度和分析深度方面的潜力。|
|**2025-03-07**|**A Practical Memory Injection Attack against LLM Agents**|Shen Dong et.al.|[2503.03704](http://arxiv.org/abs/2503.03704)|null|基于大型语言模型（LLMs）的代理已经在广泛的复杂现实世界应用中展示了强大的能力。然而，当记忆库中的过往记录被恶意篡改时，这些代理很容易产生有害输出。在本文中，我们提出了一种新颖的记忆注入攻击方法——MINJA，该方法仅通过与代理进行查询和观察输出交互，就能将恶意记录注入到记忆库中。这些恶意记录旨在引发一系列导致不良代理行为的恶意推理步骤。具体来说，我们引入了一系列桥接步骤，将受害者查询与恶意推理步骤联系起来。在注入恶意记录的过程中，我们提出了一个指示提示来引导代理自主生成我们设计的桥接步骤。我们还提出了一种逐步缩短策略，逐渐移除指示提示，使得在后续处理受害者查询时更容易检索到恶意记录。我们在不同代理上的广泛实验表明，MINJA 在破坏代理记忆方面非常有效。由于执行要求极低，MINJA 使任何用户都能影响代理记忆，这突显了 LLM 代理的实际风险。|
|**2025-03-05**|**Benchmarking LLMs and LLM-based Agents in Practical Vulnerability Detection for Code Repositories**|Alperen Yildiz et.al.|[2503.03586](http://arxiv.org/abs/2503.03586)|null|大型语言模型（LLM）在软件漏洞检测方面显示出了潜力，尤其是在函数级别的基准测试如Devign和BigVul中。然而，现实世界的检测需要进行过程间分析，因为漏洞往往通过多跳函数调用而非孤立的函数出现。尽管仓库级别的基准测试如ReposVul和VulEval引入了过程间上下文，但它们仍然计算成本高昂，缺乏对漏洞修复的成对评估，并且探索的上下文检索有限，限制了其实用性。我们引入了JitVul，这是一个即时漏洞检测基准，将每个函数与其引入漏洞和修复漏洞的提交关联起来。JitVul基于879个CVE构建，涵盖了91种漏洞类型，能够全面评估检测能力。我们的结果显示，利用思考-行动-观察和过程间上下文的ReAct代理在区分易受攻击代码和良性代码方面优于LLM。虽然像思维链这样的提示策略有助于LLM，但ReAct代理仍需进一步改进。两种方法都显示出不一致性，要么错误地识别漏洞，要么过度分析安全防护措施，表明还有很大的改进空间。|
|**2025-03-04**|**MPO: Boosting LLM Agents with Meta Plan Optimization**|Weimin Xiong et.al.|[2503.02682](http://arxiv.org/abs/2503.02682)|null|最近，大型语言模型（LLM）的发展使得基于LLM的代理能够成功应对交互式规划任务。然而，尽管取得了这些成就，现有的方法经常遭受规划幻觉的影响，并且需要为每个新代理重新训练。为了解决这些挑战，我们提出了元计划优化（MPO）框架，该框架通过直接纳入明确指导来增强代理的规划能力。与依赖复杂知识、要么需要大量人力投入要么缺乏质量保证的先前方法不同，MPO利用高层次的一般性指导通过元计划来辅助代理规划，并根据代理执行任务时的反馈持续优化这些元计划。我们在两个代表性任务上进行的实验表明，MPO显著优于现有的基线方法。此外，我们的分析指出，MPO提供了一种即插即用的解决方案，不仅提高了任务完成效率，还增强了在以前未见过的情景中的泛化能力。|
|**2025-03-04**|**Generator-Assistant Stepwise Rollback Framework for Large Language Model Agent**|Xingzuo Li et.al.|[2503.02519](http://arxiv.org/abs/2503.02519)|null|大型语言模型（LLM）代理通常采用一种逐步推理框架，在这种框架中，它们交替进行思考和行动以完成给定任务。然而，这种范式面临一个根深蒂固的一次性问题，即无论每个生成的中间思维是否正确，都会被插入到轨迹中，这可能导致不可逆的错误传播。为了解决这个问题，本文提出了一种新的框架，称为生成器-助手逐步回滚（GA-Rollback），以诱导LLM代理做出更好的决策。特别地，GA-Rollback利用一个生成器与环境交互，并使用一个助手检查生成器产生的每一个动作，当助手检测到不正确的动作时触发回滚操作。此外，我们引入了两种额外的策略，针对回滚场景进一步提高其有效性。大量实验表明，GA-Rollback在三个广泛使用的基准测试上显著优于几个强大的基线。我们的分析进一步揭示，GA-Rollback可以作为一个稳健的即插即用模块，与其他方法无缝集成。|
|**2025-03-04**|**AppAgentX: Evolving GUI Agents as Proficient Smartphone Users**|Wenjia Jiang et.al.|[2503.02268](http://arxiv.org/abs/2503.02268)|null|近期大型语言模型（LLM）的发展催生了能够与图形用户界面（GUI）交互的智能LLM代理。这些代理表现出强大的推理能力和适应性，使它们能够执行传统上需要预定义规则的复杂任务。然而，基于LLM的代理依赖于逐步推理，在处理常规任务时往往效率低下。相比之下，传统的基于规则的系统虽然在效率上表现出色，但缺乏应对新场景所需的智能和灵活性。为了解决这一挑战，我们提出了一种新颖的进化框架，旨在提高GUI代理的操作效率，同时保持其智能性和灵活性。我们的方法引入了一种记忆机制，用于记录代理的任务执行历史。通过分析该历史记录，代理能够识别重复的动作序列，并发展出高级动作作为快捷方式，替代这些低级操作，从而提升效率。这使得代理能够专注于需要更复杂推理的任务，同时简化常规操作。实验结果表明，在多个基准任务上，我们的方法在效率和准确性方面显著优于现有方法。代码将开源以支持进一步的研究。|
|**2025-03-04**|**Haste Makes Waste: Evaluating Planning Abilities of LLMs for Efficient and Feasible Multitasking with Time Constraints Between Actions**|Zirui Wu et.al.|[2503.02238](http://arxiv.org/abs/2503.02238)|null|虽然基于大型语言模型的代理在任务完成方面已经取得了显著进展，但现有的评估基准往往过于强调单一任务的表现，而对现实场景中至关重要的多任务规划和执行效率关注不足。为了解决这一问题，我们提出了Recipe2Plan，这是一个基于真实烹饪场景的新型基准框架。与传统的基准不同，Recipe2Plan要求代理通过并行任务执行来优化烹饪时间，同时遵守时间约束，即特定操作需要在前序步骤之后的特定时间间隔内完成。过度激进的局部并行化可能会破坏这种约束，从而可能危及整个烹饪过程。这些严格的时间约束给代理带来了独特的挑战，需要在最大化并发操作和遵守关键时间限制之间找到平衡。通过对最先进模型的广泛实验表明，在保持效率和可行性之间的平衡方面存在挑战。结果突显了大型语言模型需要改进时间意识和全局多任务处理能力。我们在https://github.com/WilliamZR/Recipe2Plan开源了我们的基准和代码。|
|**2025-03-04**|**ATLaS: Agent Tuning via Learning Critical Steps**|Zhixun Chen et.al.|[2503.02197](http://arxiv.org/abs/2503.02197)|null|大型语言模型（LLM）代理在多领域任务中展现了显著的泛化能力。现有的代理调优方法通常采用对整个专家轨迹进行监督微调的方式。然而，对完整轨迹的行为克隆可能会引入专家偏差，并削弱对专家数据未覆盖状态的泛化能力。此外，规划、复杂推理以完成中间子任务以及策略性决策等关键步骤对于代理任务的成功至关重要，因此学习这些步骤是提高LLM代理的关键。为了实现更有效和高效的代理调优，我们提出了ATLaS方法，该方法能够识别专家轨迹中的关键步骤，并仅针对这些步骤对LLM进行微调，从而降低了成本。通过将训练的重点转向少数几个关键步骤，我们的方法减少了对整个轨迹过度拟合的风险，并促进了在不同环境和任务中的泛化能力。在广泛的实验中，仅在ATLaS选择的30%关键步骤上进行微调的LLM，其表现优于在整个步骤上进行微调的LLM及最近的开源LLM代理。ATLaS保持并提高了基础LLM作为与多样化环境交互的通用代理的能力。|
|**2025-03-03**|**Persuasion at Play: Understanding Misinformation Dynamics in Demographic-Aware Human-LLM Interactions**|Angana Borah et.al.|[2503.02038](http://arxiv.org/abs/2503.02038)|null|
|**2025-03-03**|**MultiAgentBench: Evaluating the Collaboration and Competition of LLM agents**|Kunlun Zhu et.al.|[2503.01935](http://arxiv.org/abs/2503.01935)|null|
|**2025-03-03**|**Can (A)I Change Your Mind?**|Miriam Havin et.al.|[2503.01844](http://arxiv.org/abs/2503.01844)|null|
|**2025-03-03**|**Student engagement in collaborative learning with AI agents in an LLM-empowered learning environment: A cluster analysis**|Zhanxin Hao et.al.|[2503.01694](http://arxiv.org/abs/2503.01694)|null|
|**2025-03-02**|**Evaluating Personalized Tool-Augmented LLMs from the Perspectives of Personalization and Proactivity**|Yupu Hao et.al.|[2503.00771](http://arxiv.org/abs/2503.00771)|**[link](https://github.com/hypasd-art/etapp)**|
|**2025-02-28**|**ARIES: Autonomous Reasoning with LLMs on Interactive Thought Graph Environments**|Pedro Gimenes et.al.|[2502.21208](http://arxiv.org/abs/2502.21208)|null|
|**2025-02-28**|**PASemiQA: Plan-Assisted Agent for Question Answering on Semi-Structured Data with Text and Relational Information**|Hansi Yang et.al.|[2502.21087](http://arxiv.org/abs/2502.21087)|null|
|**2025-02-28**|**The Power of Personality: A Human Simulation Perspective to Investigate Large Language Model Agents**|Yifan Duan et.al.|[2502.20859](http://arxiv.org/abs/2502.20859)|null|
|**2025-02-28**|**Digital Player: Evaluating Large Language Models based Human-like Agent in Games**|Jiawei Wang et.al.|[2502.20807](http://arxiv.org/abs/2502.20807)|null|
|**2025-02-27**|**Collab-Overcooked: Benchmarking and Evaluating Large Language Models as Collaborative Agents**|Haochen Sun et.al.|[2502.20073](http://arxiv.org/abs/2502.20073)|**[link](https://github.com/yusaemeow/collab-overcooked)**|
|**2025-02-27**|**MIND: Towards Immersive Psychological Healing with Multi-agent Inner Dialogue**|Yujia Chen et.al.|[2502.19860](http://arxiv.org/abs/2502.19860)|null|
|**2025-02-26**|**Language-Driven Opinion Dynamics in Agent-Based Simulations with LLMs**|Erica Cau et.al.|[2502.19098](http://arxiv.org/abs/2502.19098)|null|
|**2025-02-26**|**Letters from Future Self: Augmenting the Letter-Exchange Exercise with LLM-based Agents to Enhance Young Adults' Career Exploration**|Hayeon Jeon et.al.|[2502.18881](http://arxiv.org/abs/2502.18881)|null|
|**2025-02-26**|**AgentSociety Challenge: Designing LLM Agents for User Modeling and Recommendation on Web Platforms**|Yuwei Yan et.al.|[2502.18754](http://arxiv.org/abs/2502.18754)|null|
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
|**2025-02-20**|**Is Safety Standard Same for Everyone? User-Specific Safety Evaluation of Large Language Models**|Yeonjun In et.al.|[2502.15086](http://arxiv.org/abs/2502.15086)|null|
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
|**2025-02-19**|**An LLM-based Agent for Reliable Docker Environment Configuration**|Ruida Hu et.al.|[2502.13681](http://arxiv.org/abs/2502.13681)|null|
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
|**2025-01-17**|**A Survey on LLM Test-Time Compute via Search: Tasks, LLM Profiling, Search Algorithms, and Relevant Frameworks**|Xinzhe Li et.al.|[2501.10069](http://arxiv.org/abs/2501.10069)|null|
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

<p align=right>(<a href=#updated-on-20250310>back to top</a>)</p>

## llm

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-03-07**|**Shifting Long-Context LLMs Research from Input to Output**|Yuhao Wu et.al.|[2503.04723](http://arxiv.org/abs/2503.04723)|null|近期长上下文大型语言模型（LLM）的进步主要集中在处理扩展的输入上下文上，这在长上下文理解方面取得了显著进展。然而，同样关键的长文本生成方面却相对较少受到关注。本文呼吁自然语言处理研究转向解决长文本生成的挑战。诸如小说写作、长期规划和复杂推理等任务要求模型不仅要理解广泛的上下文，还要生成连贯、内容丰富且逻辑一致的扩展文本。这些需求凸显了当前LLM能力中的一个重要空白。我们强调这一未充分探索领域的关键重要性，并呼吁集中努力开发基础LLM，以生成高质量的长文本输出，这在实际应用中具有巨大潜力。|
|**2025-03-06**|**Enough Coin Flips Can Make LLMs Act Bayesian**|Ritwik Gupta et.al.|[2503.04722](http://arxiv.org/abs/2503.04722)|null|大型语言模型（LLMs）在输入提示中给出少量示例时能够展现出泛化能力，这种新兴的能力被称为上下文学习（ICL）。我们研究了LLMs是否利用ICL以符合贝叶斯框架的方式进行结构化推理，还是依赖于模式匹配。通过控制偏差硬币投掷的实验设置，我们发现：(1) LLMs经常具有偏差先验，在零样本设置下导致初始分歧；(2) 上下文证据超过了明确的偏差指令的影响；(3) LLMs大体上遵循贝叶斯后验更新，偏离主要由于先验估计不准确而不是更新过程有缺陷；(4) 注意力大小对贝叶斯推断几乎没有影响。通过足够的偏差硬币投掷演示，LLMs能够以贝叶斯方式更新其先验。|
|**2025-03-06**|**Predictable Scale: Part I -- Optimal Hyperparameter Scaling Law in Large Language Model Pretraining**|Houyi Li et.al.|[2503.04715](http://arxiv.org/abs/2503.04715)|null|大型语言模型（LLMs）在各种任务上的卓越能力现已得到广泛认可，但其有效部署需要仔细的超参数优化。通过在不同配置下进行广泛的网格搜索实验，我们发现了这些超参数的通用缩放定律：最优学习率与模型参数和数据规模之间存在幂律关系，而最优批量大小主要随数据规模变化。我们的分析揭示了在固定模型和数据规模条件下，超参数优化景观是凸的。这种凸性意味着存在一个最优超参数平台区。我们为社区贡献了一个通用的即插即用最优超参数工具。它在测试集上的估计值仅比通过穷举搜索找到的全局最优LLM性能低0.07%。这些定律在模型稀疏性、训练数据分布和模型结构的变化下表现出显著的鲁棒性。据我们所知，这是首次统一不同模型形状和结构（如专家混合模型和密集型变换器），并建立跨多种数据分布的最优超参数缩放定律的工作。这一详尽的优化过程需要大量的计算资源，利用近一百万NVIDIA H800 GPU小时从头开始训练3,700个不同规模和超参数的LLM，并消耗了大约100万亿个令牌。为了促进可重复性和进一步研究，我们将逐步通过指定的存储库https://step-law.github.io/发布所有损失测量结果和模型检查点。|
|**2025-03-06**|**Universality of Layer-Level Entropy-Weighted Quantization Beyond Model Architecture and Size**|Alireza Behtash et.al.|[2503.04704](http://arxiv.org/abs/2503.04704)|null|我们提出了一种新颖的选择性模型量化方法，即熵加权量化（EWQ），该方法超越了特定架构和大小依赖的压缩方法对大型语言模型（LLMs）的限制。通过分析变压器块之间的熵分布，EWQ能够确定哪些块可以在不引起显著性能下降的情况下安全地进行量化，且与模型架构或大小无关。我们的方法优于均匀量化方法，在保持大规模多任务语言理解（MMLU）准确率分数与未量化模型相差不超过0.5%的同时，减少了高达18%的内存使用量。我们在多个架构中展示了EWQ的有效性，从16亿到700亿参数，无论模型规模或架构设计如何，均表现出一致的质量-压缩折衷改进。令人惊讶的是，EWQ还能降低相比未量化模型的困惑度，表明通过选择性精度降低存在有益的正则化效果。这种改进在不同模型家族中都成立，表明层级熵与最佳精度需求之间存在基本关系。此外，我们引入了FastEWQ，这是一种快速的熵分布分析方法，无需加载模型权重。该技术利用了跨各种架构和规模普遍存在的熵分布特性，能够在几乎瞬间做出量化决策，同时保持80%的分类准确性与完整的熵分析。我们的结果表明，可以独立于具体的架构选择或模型大小来开发有效的量化策略，为高效部署大型语言模型开辟了新的可能性。|
|**2025-03-06**|**UIPE: Enhancing LLM Unlearning by Removing Knowledge Related to Forgetting Targets**|Wenyu Wang et.al.|[2503.04693](http://arxiv.org/abs/2503.04693)|null|大型语言模型（LLM）在大规模数据集上训练时不可避免地会获取有害信息。LLM遗忘旨在消除这些有害信息的影响，同时保持模型的整体性能。现有的遗忘方法，以基于梯度上升的方法为代表，主要关注于忘记目标数据，而忽略了逻辑相关知识对遗忘效果的重要影响。在这篇论文中，我们通过理论和实验分析首次证明了遗忘效果不佳的一个关键原因是模型可以通过与逻辑相关知识进行推理来重建目标内容。为了解决这个问题，我们提出了一种通过参数外推来改进遗忘的方法（UIPE），该方法能够移除与遗忘目标高度相关的知识。实验结果表明，UIPE显著提高了各种主流LLM遗忘方法在TOFU基准测试中的表现。|
|**2025-03-06**|**LLM-guided Plan and Retrieval: A Strategic Alignment for Interpretable User Satisfaction Estimation in Dialogue**|Sangyeop Kim et.al.|[2503.04675](http://arxiv.org/abs/2503.04675)|null|理解用户对对话系统的满意度，即用户满意度估计（USE），对于评估对话质量和提升用户体验至关重要。然而，现有的USE方法面临着由于对用户不满的根本原因理解有限以及标注用户意图成本高昂的挑战。为了解决这些挑战，我们提出了PRAISE（Plan and Retrieval Alignment for Interpretable Satisfaction Estimation），这是一种可解释的有效用户满意度预测框架。PRAISE通过三个关键模块运作。策略规划器开发了策略，这些策略是用于分类用户满意度的自然语言标准。特征检索器随后整合来自大型语言模型（LLM）的用户满意度知识，并从话语中检索相关特征。最后，评分分析器评估策略预测并分类用户满意度。实验结果表明，PRAISE在三个USE任务基准上达到了最先进的性能。除了其卓越的性能外，PRAISE还提供了额外的好处。它通过有效对齐话语和策略提供实例级解释来增强可解释性。此外，PRAISE在推理阶段不需要使用大型语言模型，因此比现有方法运行更高效。|
|**2025-03-06**|**Implicit Cross-Lingual Rewarding for Efficient Multilingual Preference Alignment**|Wen Yang et.al.|[2503.04647](http://arxiv.org/abs/2503.04647)|null|直接偏好优化（DPO）已成为使大型语言模型（LLMs）与人类偏好对齐的重要方法。虽然DPO在对齐英语LLMs方面取得了显著进展，但多语言偏好对齐受到数据稀缺性的限制。为了解决这一问题，我们提出了一种新颖的方法，通过隐式奖励来捕获从良好对齐的英语模型中学到的偏好，并通过迭代训练将其转移到其他语言中。具体来说，我们从一个经过DPO对齐的英语模型及其相应的参考模型的logits中推导出一个隐式奖励模型。然后利用该奖励模型，使用英语指令评估多语言响应，从而标注跨语言指令跟随对中的偏好关系。随后，这些标注的数据被用于多语言DPO微调，促进了偏好知识从英语向其他语言的转移。经过两轮Llama3的微调，在X-AlpacaEval排行榜上所有训练语言的平均胜率提高了12.72%，长度控制胜率提高了5.97%。我们的研究结果表明，利用现有的英语对齐模型可以实现高效且有效的多语言偏好对齐，大大减少了对大量多语言偏好数据的需求。代码可在https://github.com/ZNLP/Implicit-Cross-Lingual-Rewarding获取。|
|**2025-03-06**|**Mark Your LLM: Detecting the Misuse of Open-Source Large Language Models via Watermarking**|Yijie Xu et.al.|[2503.04636](http://arxiv.org/abs/2503.04636)|null|随着像Llama3这样的开源大型语言模型（LLM）变得越来越强大，开发用于检测其潜在滥用的水印技术变得至关重要。现有的水印方法要么在LLM推理过程中添加水印，这不适合开源LLM，要么主要针对分类LLM而不是最近的生成型LLM。将这些水印适应于开源LLM以检测其滥用仍然是一个开放性的挑战。本研究定义了开源LLM的两种滥用场景：知识产权（IP）侵犯和LLM使用违规。然后，我们探讨了在这两个情境下应用推理时水印蒸馏和后门水印技术的可能性。我们提出了全面的评估方法来衡量各种实际进一步微调场景对水印的影响以及这些水印对LLM性能的影响。实验结果显示，后门水印能够有效地检测IP侵犯，而推理时水印蒸馏虽然适用于两种场景，但对进一步微调的鲁棒性较差，并且对LLM性能的影响比后门水印更大。探索更先进的开源LLM水印技术以检测其滥用应该是未来的重要方向。|
|**2025-03-06**|**Better Process Supervision with Bi-directional Rewarding Signals**|Wenxiang Chen et.al.|[2503.04618](http://arxiv.org/abs/2503.04618)|null|过程监督，即评估每一步骤，对于复杂的大型语言模型（LLM）推理和测试时搜索具有重要的作用，尤其是在增加推理计算的情况下。现有的方法，如过程奖励模型（PRMs），主要侧重于到当前步骤为止的奖励信号，表现出单向性，并且缺乏一种机制来建模到达最终目标的距离。为了解决这个问题，我们从A*算法中汲取灵感，该算法指出有效的监督信号应同时考虑已产生的成本和达到目标的估计成本。基于这一关键见解，我们引入了BiRM，这是一种新颖的过程监督模型，它不仅评估先前步骤的正确性，还建模未来成功的概率。我们在数学推理任务上进行了广泛的实验，结果表明BiRM能够更准确地评估LLM推理步骤，在Gaokao2023数据集上使用最佳N采样方法时相比PRM提高了3.1%。此外，在基于搜索的策略中，BiRM提供了更全面的指导，在MATH-500数据集上分别比ORM和PRM高出5.0%和3.8%。|
|**2025-03-06**|**Towards Data-Efficient Language Models: A Child-Inspired Approach to Language Learning**|Mohammad Amin Ghanizadeh et.al.|[2503.04611](http://arxiv.org/abs/2503.04611)|null|在这项工作中，我们解释了在BabyLM挑战中采用的方法，该方法使用多种训练语言模型（LMs）的技术，与传统的大型语言模型（LLMs）相比，这些技术使用的数据显著减少，并且受到儿童学习方式的启发。尽管人类儿童接触到的语言输入远远少于大型语言模型，但他们仍然能够达到令人惊叹的语言理解和生成能力。为此，我们开发了一个基于精心策划的数据集进行训练的模型，该数据集包含1000万词汇，主要来源于面向儿童的转录文本。2024年BabyLM挑战赛初始的1000万词汇数据集被筛选至850万词汇，随后补充了从电视对话数据集中随机选取的150万词汇子集。后者确保了模型也能像儿童一样通过媒体接触语言。此外，我们将词汇量减少到32,000个标记，使其与儿童早期语言习得阶段的有限词汇相匹配。我们采用了课程学习法，并能够在某些基准测试上与基线持平，在其他一些基准测试上超越基线。此外，加入常见的大型语言模型训练数据集，如MADLAD-400，反而会降低性能。这些发现强调了数据集选择、词汇规模调整以及课程学习在创建更高效利用数据的语言模型方面的重要性，这些模型更好地模仿了人类的学习过程。|
|**2025-03-05**|**The MASK Benchmark: Disentangling Honesty From Accuracy in AI Systems**|Richard Ren et.al.|[2503.03750](http://arxiv.org/abs/2503.03750)|null|
|**2025-03-05**|**Towards Understanding Distilled Reasoning Models: A Representational Approach**|David D. Baek et.al.|[2503.03730](http://arxiv.org/abs/2503.03730)|null|
|**2025-03-05**|**Improving LLM Safety Alignment with Dual-Objective Optimization**|Xuandong Zhao et.al.|[2503.03710](http://arxiv.org/abs/2503.03710)|null|
|**2025-03-05**|**Effective LLM Knowledge Learning via Model Generalization**|Mingkang Zhu et.al.|[2503.03705](http://arxiv.org/abs/2503.03705)|null|
|**2025-03-05**|**A Practical Memory Injection Attack against LLM Agents**|Shen Dong et.al.|[2503.03704](http://arxiv.org/abs/2503.03704)|null|
|**2025-03-05**|**Developing and Utilizing a Large-Scale Cantonese Dataset for Multi-Tasking in Large Language Models**|Jiyue Jiang et.al.|[2503.03702](http://arxiv.org/abs/2503.03702)|null|
|**2025-03-05**|**Addressing Overprescribing Challenges: Fine-Tuning Large Language Models for Medication Recommendation Tasks**|Zihao Zhao et.al.|[2503.03687](http://arxiv.org/abs/2503.03687)|null|
|**2025-03-05**|**Analogical Reasoning Inside Large Language Models: Concept Vectors and the Limits of Abstraction**|Gustaw Opiełka et.al.|[2503.03666](http://arxiv.org/abs/2503.03666)|null|
|**2025-03-05**|**Improving Neutral Point of View Text Generation through Parameter-Efficient Reinforcement Learning and a Small-Scale High-Quality Dataset**|Jessica Hoffmann et.al.|[2503.03654](http://arxiv.org/abs/2503.03654)|null|
|**2025-03-05**|**Psy-Copilot: Visual Chain of Thought for Counseling**|Keqi Chen et.al.|[2503.03645](http://arxiv.org/abs/2503.03645)|null|
|**2025-03-04**|**Wikipedia in the Era of LLMs: Evolution and Risks**|Siming Huang et.al.|[2503.02879](http://arxiv.org/abs/2503.02879)|null|
|**2025-03-04**|**The First Few Tokens Are All You Need: An Efficient and Effective Unsupervised Prefix Fine-Tuning Method for Reasoning Models**|Ke Ji et.al.|[2503.02875](http://arxiv.org/abs/2503.02875)|null|
|**2025-03-04**|**FairSense-AI: Responsible AI Meets Sustainability**|Shaina Raza et.al.|[2503.02865](http://arxiv.org/abs/2503.02865)|null|
|**2025-03-04**|**Calibrating LLM Confidence with Semantic Steering: A Multi-Prompt Aggregation Framework**|Ziang Zhou et.al.|[2503.02863](http://arxiv.org/abs/2503.02863)|null|
|**2025-03-04**|**Shakespearean Sparks: The Dance of Hallucination and Creativity in LLMs' Decoding Layers**|Zicong He et.al.|[2503.02851](http://arxiv.org/abs/2503.02851)|null|
|**2025-03-04**|**Mask-DPO: Generalizable Fine-grained Factuality Alignment of LLMs**|Yuzhe Gu et.al.|[2503.02846](http://arxiv.org/abs/2503.02846)|null|
|**2025-03-04**|**AlignDistil: Token-Level Language Model Alignment as Adaptive Policy Distillation**|Songming Zhang et.al.|[2503.02832](http://arxiv.org/abs/2503.02832)|null|
|**2025-03-04**|**RAAD-LLM: Adaptive Anomaly Detection Using LLMs and RAG Integration**|Alicia Russell-Gilbert et.al.|[2503.02800](http://arxiv.org/abs/2503.02800)|null|
|**2025-03-04**|**Implicit Bias in LLMs: A Survey**|Xinru Lin et.al.|[2503.02776](http://arxiv.org/abs/2503.02776)|null|
|**2025-03-04**|**BatchGEMBA: Token-Efficient Machine Translation Evaluation with Batched Prompting and Prompt Compression**|Daniil Larionov et.al.|[2503.02756](http://arxiv.org/abs/2503.02756)|null|
|**2025-02-28**|**LLM Post-Training: A Deep Dive into Reasoning Large Language Models**|Komal Kumar et.al.|[2502.21321](http://arxiv.org/abs/2502.21321)|null|
|**2025-02-28**|**FANformer: Improving Large Language Models Through Effective Periodicity Modeling**|Yihong Dong et.al.|[2502.21309](http://arxiv.org/abs/2502.21309)|null|
|**2025-02-28**|**Contextualizing biological perturbation experiments through language**|Menghua Wu et.al.|[2502.21290](http://arxiv.org/abs/2502.21290)|**[link](https://github.com/genentech/perturbqa)**|
|**2025-02-28**|**Adaptive Keyframe Sampling for Long Video Understanding**|Xi Tang et.al.|[2502.21271](http://arxiv.org/abs/2502.21271)|null|
|**2025-02-28**|**Semantic Volume: Quantifying and Detecting both External and Internal Uncertainty in LLMs**|Xiaomin Li et.al.|[2502.21239](http://arxiv.org/abs/2502.21239)|null|
|**2025-02-28**|**ByteScale: Efficient Scaling of LLM Training with a 2048K Context Length on More Than 12,000 GPUs**|Hao Ge et.al.|[2502.21231](http://arxiv.org/abs/2502.21231)|null|
|**2025-03-03**|**ECLeKTic: a Novel Challenge Set for Evaluation of Cross-Lingual Knowledge Transfer**|Omer Goldman et.al.|[2502.21228](http://arxiv.org/abs/2502.21228)|null|
|**2025-02-28**|**Transformers Learn to Implement Multi-step Gradient Descent with Chain of Thought**|Jianhao Huang et.al.|[2502.21212](http://arxiv.org/abs/2502.21212)|null|
|**2025-02-28**|**Optimizing Large Language Models for ESG Activity Detection in Financial Texts**|Mattia Birti et.al.|[2502.21112](http://arxiv.org/abs/2502.21112)|null|
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
|**2025-02-20**|**GATE: Graph-based Adaptive Tool Evolution Across Diverse Tasks**|Jianwen Luo et.al.|[2502.14848](http://arxiv.org/abs/2502.14848)|null|
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

<p align=right>(<a href=#updated-on-20250310>back to top</a>)</p>

## moe

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-03-07**|**Question-Aware Gaussian Experts for Audio-Visual Question Answering**|Hongyeob Kim et.al.|[2503.04459](http://arxiv.org/abs/2503.04459)|**[link](https://github.com/AIM-SKKU/QA-TIGER)**|**音频-视觉问答（AVQA）不仅需要基于问题的多模态推理，还需要精确的时间定位来捕捉细微动态以进行准确预测。然而，现有的方法主要隐式地使用问题信息，限制了对问题特定细节的关注。此外，大多数研究依赖于均匀帧采样，这可能会错过关键的问题相关帧。尽管最近的Top-K帧选择方法试图解决这一问题，但其离散性质仍然忽略了细粒度的时间细节。本文提出了一种新颖的框架QA-TIGER，该框架显式地结合了问题信息并建模连续时间动态。我们的核心思想是使用基于高斯的建模方法，根据问题自适应地关注连续和非连续的帧，同时显式注入问题信息并应用逐步细化。我们利用专家混合模型（MoE）灵活实现多个高斯模型，激活专门针对问题的时间专家。在多个AVQA基准上的广泛实验表明，QA-TIGER始终达到最先进的性能。代码可在https://aim-skku.github.io/QA-TIGER/获取。**|
|**2025-03-06**|**DM-Adapter: Domain-Aware Mixture-of-Adapters for Text-Based Person Retrieval**|Yating Liu et.al.|[2503.04144](http://arxiv.org/abs/2503.04144)|null|基于文本的人体检索（TPR）作为一个精细且具有挑战性的任务，因其与实际应用的紧密关联而受到了广泛关注。由于视觉-语言预训练中丰富的知识，将CLIP调整到人体领域已成为一个新兴的研究课题，但在微调过程中仍存在一些挑战：(i) 之前在TPR中的全模型微调计算成本高且容易过拟合；(ii) 现有的针对TPR的参数高效迁移学习(PETL)缺乏细粒度特征提取。为了解决这些问题，我们提出了域感知混合适配器（DM-Adapter），它统一了专家混合(MOE)和PETL，以增强细粒度特征表示同时保持效率。具体来说，在视觉和语言分支的MLP层并行设计了稀疏混合适配器，其中不同的专家专门处理人体知识的不同方面，以更精细地处理特征。为了促进路由器有效地利用领域信息并缓解路由不平衡问题，我们通过构建一种新的门控函数并注入可学习的领域感知提示来开发了域感知路由器。广泛的实验表明，我们的DM-Adapter达到了最先进的性能，显著优于以前的方法。|
|**2025-03-05**|**Convergence Rates for Softmax Gating Mixture of Experts**|Huy Nguyen et.al.|[2503.03213](http://arxiv.org/abs/2503.03213)|null|专家混合（MoE）作为一种有效的框架，通过将复杂任务软性地分配给多个称为专家的专门子模型来提高机器学习模型的效率和可扩展性。MoE成功的核心在于自适应softmax门控机制，该机制负责确定每个专家对给定输入的相关性，并动态地为各专家分配权重。尽管在实践中被广泛使用，但关于softmax门控对MoE影响的全面研究在文献中仍然缺乏。为了填补这一空白，本文对采用标准softmax门控或其变体（包括密集到稀疏门控和层次softmax门控）的MoE进行了参数估计与专家估计的收敛性分析。此外，我们的理论还为设计样本高效型专家结构提供了有价值的见解。特别地，我们证明了要估计满足我们提出的“强可识别性”条件的专家，即常用的两层前馈网络，需要多项式数量的数据点。相比之下，由于内在参数相互作用（用偏微分方程的语言表达），估计违反强可识别性条件的线性专家则需要指数数量的数据点。所有理论结果都得到了严格的保证。|
|**2025-03-04**|**MX-Font++: Mixture of Heterogeneous Aggregation Experts for Few-shot Font Generation**|Weihang Wang et.al.|[2503.02799](http://arxiv.org/abs/2503.02799)|null|少样本字体生成（FFG）旨在使用有限的参考字形创建新的字体库，具有关键的应用价值，特别是在数字可访问性和低资源语言的公平性方面，尤其是在多语言人工智能系统中。尽管现有方法已经显示出有希望的表现，但在低资源语言中过渡到未见过的字符仍然是一个重大挑战，尤其是当字体字形在训练集之间差异很大时。MX-Font 从局部组件的角度考虑字符的内容，采用专家混合（MoE）方法自适应地提取组件以实现更好的过渡。然而，缺乏强大的特征提取器使它们无法充分解耦内容和风格，导致生成结果不理想。为了解决这些问题，我们提出了异构聚合专家（HAE），这是一种强大的特征提取专家，能够从通道和空间维度聚合信息，从而帮助下游解耦内容和风格。此外，我们提出了一种新颖的内容-风格同质性损失来增强这种解耦。在多个数据集上的广泛实验表明，我们的 MX-Font++ 在 FFG 中产生了更优的视觉效果，并有效超越了最先进的方法。代码和数据可在 https://github.com/stephensun11/MXFontpp 获取。|
|**2025-03-04**|**FinArena: A Human-Agent Collaboration Framework for Financial Market Analysis and Forecasting**|Congluo Xu et.al.|[2503.02692](http://arxiv.org/abs/2503.02692)|null|为了提高股票趋势预测的准确性并支持个性化的投资决策，本文提出了一种新颖的人机协作框架FinArena。受专家混合（MoE）方法的启发，FinArena结合了多模态金融数据分析与用户交互。人类模块提供了一个互动界面，能够捕捉个人的风险偏好，从而允许制定个性化的投资策略。机器模块利用基于大型语言模型（LLM）的多代理系统整合了多种数据源，如股票价格、新闻文章和财务报表。为了解决LLM中的幻觉问题，FinArena采用自适应检索增强生成（RAG）方法来处理非结构化的新闻数据。最终，一个通用的专家代理根据从多模态数据中提取的特征以及投资者的个人风险偏好做出投资决策。广泛的实验表明，FinArena在股票趋势预测方面超过了传统和最先进的基准，并在不同风险概况下的交易模拟中取得了有希望的结果。这些发现突显了FinArena通过将战略见解与个性化风险考量相结合以提升投资结果的潜力。|
|**2025-03-04**|**Union of Experts: Adapting Hierarchical Routing to Equivalently Decomposed Transformer**|Yujiao Yang et.al.|[2503.02495](http://arxiv.org/abs/2503.02495)|null|
|**2025-03-03**|**ECG-EmotionNet: Nested Mixture of Expert (NMoE) Adaptation of ECG-Foundation Model for Driver Emotion Recognition**|Nastaran Mansourian et.al.|[2503.01750](http://arxiv.org/abs/2503.01750)|null|驾驶员情绪识别在驾驶员监控系统中起着关键作用，能够增强人机交互以及自动驾驶（AD）的可信度。为此目的已经探索了多种生理和行为模式，心电图（ECG）因其在动态和不可预测的驾驶条件下进行实时情绪监测的能力而脱颖而出。然而，现有的方法通常依赖于在静态条件下记录的多通道ECG信号，这限制了它们在实际动态驾驶场景中的应用。为了解决这一局限性，本文介绍了一种名为ECG-EmotionNet的新架构，专门用于动态驾驶环境下的情绪识别。ECG-EmotionNet通过调整最近引入的心电图基础模型（FM）构建，并且独特地使用单通道ECG信号，确保了强大的泛化能力和计算效率。与传统的适应方法如全微调、线性探测或低秩适应不同，我们提出了一种直观令人满意的替代方案，称为嵌套专家混合（MoE）适应。具体来说，将基础模型中的每个变压器层视为一个独立的专家，并通过门控机制中的可训练权重融合从这些专家提取的嵌入。这种方法增强了全局和局部ECG特征的表示能力，使得准确率提高了6%，F1分数提高了7%，同时保持了计算效率。提出的ECG-EmotionNet架构的有效性通过一个新近引入的具有挑战性的驾驶员情绪监控数据集进行了评估。|
|**2025-03-03**|**DeRS: Towards Extremely Efficient Upcycled Mixture-of-Experts Models**|Yongqi Huang et.al.|[2503.01359](http://arxiv.org/abs/2503.01359)|null|升级再利用的专家混合（MoE）模型通过将预训练密集模型中的原始前馈网络（FFN）层转换为MoE层，在各种任务中展现了巨大潜力。然而，由于引入了多个专家，这些模型仍然存在显著的参数效率低下问题。在本工作中，我们提出了一种新颖的DeRS（分解、替换和合成）范式来克服这一缺点，该方法受到我们对升级再利用MoE专家独特的冗余机制观察的启发。具体而言，DeRS将专家分解为一个共享的基础权重和多个特定于专家的增量权重，并随后以轻量级形式表示这些增量权重。我们提出的DeRS范式可以应用于两个不同场景以提高参数效率：1）用于推理阶段的DeRS压缩，通过对原生升级再利用MoE模型进行稀疏化或量化来进行压缩；2）用于训练阶段的DeRS升级再利用，采用轻量级稀疏或低秩矩阵高效地将密集模型升级再利用为MoE模型。在三个不同任务上的广泛实验表明，所提出的方法能够在保持性能的同时实现极高的参数效率，适用于升级再利用MoE模型的训练与压缩。|
|**2025-03-03**|**PROPER: A Progressive Learning Framework for Personalized Large Language Models with Group-Level Adaptation**|Linhai Zhang et.al.|[2503.01303](http://arxiv.org/abs/2503.01303)|null|个性化大型语言模型（LLM）旨在使其输出符合用户偏好。最近，参数高效微调（PEFT）方法的进步突显了通过使用用户历史数据对用户特定参数进行微调来将群体级别的LLM调整为个性化LLM的有效性。然而，用户数据通常是稀疏的，这使得将LLM适应特定用户模式变得具有挑战性。为了解决这一挑战，我们提出了PROgressive PERsonalization（PROPER），这是一种受社会科学中中观层面理论启发的新颖渐进式学习框架。PROPER通过根据偏好对用户进行分组并在不同阶段逐步调整LLM，从而在群体级别和用户级别模型之间架起桥梁。它结合了专家混合（MoE）结构与低秩适应（LoRA），并使用用户感知路由器自动将用户分配到合适的组别。此外，还提出了一种LoRA感知路由器，以促进个体用户LoRA与组级别LoRA之间的集成。实验结果表明，PROPER在多个任务上显著优于当前最先进的模型，证明了我们方法的有效性。|
|**2025-03-02**|**Explainable Classifier for Malignant Lymphoma Subtyping via Cell Graph and Image Fusion**|Daiki Nishiyama et.al.|[2503.00925](http://arxiv.org/abs/2503.00925)|null|恶性淋巴瘤亚型分类直接影响治疗策略和患者预后，需要同时具备高准确性和足够可解释性的分类模型。本研究提出了一种新颖的可解释多实例学习（MIL）框架，该框架能够从全切片图像（WSIs）中识别特定于亚型的兴趣区域（ROIs），同时整合细胞分布特征和图像信息。我们的框架同时解决了三个目标：(1) 为每个亚型指示合适的兴趣区域，(2) 解释特征细胞类型的频率和空间分布，(3) 通过利用图像和细胞分布模态实现高精度的亚型分类。所提出的方法使用专家混合（MoE）方法融合从WSI中的每个斑块提取的细胞图和图像特征，并在MIL框架内进行亚型分类。在包含1,233张WSIs的数据集上的实验表明，我们的方法在十种比较方法中达到了最先进的准确性，并提供了与病理学家观点一致的区域级和细胞级解释。|
|**2025-03-01**|**Efficiently Editing Mixture-of-Experts Models with Compressed Experts**|Yifei He et.al.|[2503.00634](http://arxiv.org/abs/2503.00634)|null|混合专家（MoE）模型已成为通过仅在训练和推理期间激活一部分专家来高效扩展大型语言模型的关键方法。通常，激活的专家数量存在一个权衡：较少的专家可以减少计算成本，而较多的专家则可以提高性能。最近的研究表明，并非所有激活的专家对模型性能的贡献都是均等的，有些专家在对预训练的MoE模型进行特定下游任务微调时提供的效用极小。重要参数与冗余参数在专家中的共存为我们提供了一个机会，可以在保持模型性能的同时减少激活的专家数量。在这项工作中，我们提出了压缩专家的概念，这是一种作为完整专家紧凑表示的轻量级模块。我们的方法保留了最重要的专家，同时将其他辅助激活的专家替换为压缩专家。活动参数的减少显著降低了推理成本，同时实现了可比较的性能。在包括Phi-MoE和OLMoE在内的模型上的大量实验表明，压缩专家在各种任务上恢复了超过90%的完整专家性能，同时减少了30%以上的活动参数，并节省了20%的推理成本。这种方法使得MoE模型能够在资源受限的情况下高效部署，并有助于以可控的开销扩展到更大的模型。我们的代码可在https://github.com/yifei-he/Compressed-Experts获取。|
|**2025-02-28**|**CoSMoEs: Compact Sparse Mixture of Experts**|Patrick Huber et.al.|[2503.00245](http://arxiv.org/abs/2503.00245)|null|
|**2025-03-01**|**R2-T2: Re-Routing in Test-Time for Multimodal Mixture-of-Experts**|Zhongyang Li et.al.|[2502.20395](http://arxiv.org/abs/2502.20395)|**[link](https://github.com/tianyi-lab/R2-T2)**|
|**2025-02-27**|**Mixture of Experts for Recognizing Depression from Interview and Reading Tasks**|Loukas Ilias et.al.|[2502.20213](http://arxiv.org/abs/2502.20213)|null|
|**2025-02-27**|**Mixture of Experts-augmented Deep Unfolding for Activity Detection in IRS-aided Systems**|Zeyi Ren et.al.|[2502.20183](http://arxiv.org/abs/2502.20183)|null|
|**2025-03-01**|**Comet: Fine-grained Computation-communication Overlapping for Mixture-of-Experts**|Shulai Zhang et.al.|[2502.19811](http://arxiv.org/abs/2502.19811)|null|
|**2025-02-26**|**Drop-Upcycling: Training Sparse Mixture of Experts with Partial Re-initialization**|Taishi Nakamura et.al.|[2502.19261](http://arxiv.org/abs/2502.19261)|null|
|**2025-02-26**|**OneRec: Unifying Retrieve and Rank with Generative Recommender and Iterative Preference Alignment**|Jiaxin Deng et.al.|[2502.18965](http://arxiv.org/abs/2502.18965)|null|
|**2025-02-25**|**Generative AI-enabled Wireless Communications for Robust Low-Altitude Economy Networking**|Changyuan Zhao et.al.|[2502.18118](http://arxiv.org/abs/2502.18118)|null|
|**2025-02-24**|**The Empirical Impact of Reducing Symmetries on the Performance of Deep Ensembles and MoE**|Andrei Chernov et.al.|[2502.17391](http://arxiv.org/abs/2502.17391)|null|
|**2025-02-24**|**Delta Decompression for MoE-based LLMs Compression**|Hao Gu et.al.|[2502.17298](http://arxiv.org/abs/2502.17298)|**[link](https://github.com/lliai/d2moe)**|
|**2025-02-24**|**Evaluating Expert Contributions in a MoE LLM for Quiz-Based Tasks**|Andrei Chernov et.al.|[2502.17187](http://arxiv.org/abs/2502.17187)|null|
|**2025-02-24**|**Muon is Scalable for LLM Training**|Jingyuan Liu et.al.|[2502.16982](http://arxiv.org/abs/2502.16982)|null|
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

<p align=right>(<a href=#updated-on-20250310>back to top</a>)</p>

## SSMs

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-03-06**|**An Extended State Space Model of Aggregated Electric Vehicles for Flexibility Estimation and Power Control**|Yiping Liu et.al.|[2503.04714](http://arxiv.org/abs/2503.04714)|null|电动汽车（EV）的普及可以为电网提供大量电力，支持电网的稳定性。状态空间模型（SSM）已被提出作为预测和集中控制聚合电动汽车的有效建模方法，具有较低的通信需求和计算复杂度。然而，SSM可能忽略某些特定情况，导致显著的预测和控制不准确性。本文提出了一种扩展的状态空间模型（eSSM）用于聚合电动汽车，并开发了相应的控制策略。通过考虑满充和满放状态下电动汽车有限的灵活性，eSSM更准确地捕捉了不同荷电状态（SOC）下电动汽车的状态转换动态。综合仿真表明，与传统SSM方法相比，eSSM能够更准确地预测聚合电动汽车的灵活性和功率轨迹，并更有效地跟踪实时功率参考。|
|**2025-03-05**|**State-offset Tuning: State-based Parameter-Efficient Fine-Tuning for State Space Models**|Wonjun Kang et.al.|[2503.03499](http://arxiv.org/abs/2503.03499)|null|状态空间模型（SSM）作为高效的替代方案出现，缓解了Transformer的二次计算成本问题。然而，将参数高效微调（PEFT）方法应用于SSM的研究还相对较少。特别是像提示调优和前缀调优这样的基于提示的方法，在Transformer中广泛应用，但在SSM上表现不佳。为了解决这个问题，我们提出了一种基于状态的方法，作为优于基于提示方法的替代方案。这类新方法自然源于SSM的架构特性，通过直接调整与状态相关的特征而不是依赖外部提示来实现。此外，我们引入了一种新颖的基于状态的PEFT方法：状态偏移调优。在每个时间步，我们的方法直接影响当前步骤的状态，从而实现更有效的适应。通过在多个数据集上的广泛实验，我们证明了该方法的有效性。代码可从https://github.com/furiosa-ai/ssm-state-tuning获取。|
|**2025-03-04**|**S4D-Bio Audio Monitoring of Bone Cement Disintegration in Pulsating Fluid Jet Surgery under Laboratory Conditions**|Melanie Schaller et.al.|[2503.02714](http://arxiv.org/abs/2503.02714)|null|本研究探讨了一种脉冲流体喷射作为一种新颖的精确、微创且冷技术用于骨水泥移除。我们利用脉冲流体喷射装置从模拟临床条件的样本中去除骨水泥。测试了长喷嘴的有效性，以实现微创手术。通过音频信号监测，并辅以状态空间模型（SSM）S4D-Bio，动态优化流体喷射参数，解决了飞溅导致视线受阻等挑战。在实验过程中，我们生成了一个全面的数据集，将各种工艺参数及其对应的音频信号与材料侵蚀相关联。使用SSM可以对预测侵蚀过程进行精确控制，达到98.93%的准确率。研究表明，一方面，结合先进的音频监测技术的脉冲流体喷射装置是精确去除骨水泥的高度有效工具；另一方面，本研究首次将SSM应用于生物医学手术技术，标志着该领域的重大进展。这项研究通过将机器学习与脉冲流体喷射技术相结合，在生物医学工程领域取得了显著进展，为骨科应用提供了一种新颖的、微创的、冷的和自适应的骨水泥移除方法。|
|**2025-03-04**|**SSNet: Saliency Prior and State Space Model-based Network for Salient Object Detection in RGB-D Images**|Gargi Panda et.al.|[2503.02270](http://arxiv.org/abs/2503.02270)|null|RGB-D图像中的显著物体检测（SOD）是计算机视觉中的一个重要任务，能够应用于场景理解、机器人技术和增强现实。然而，现有的方法难以捕捉跨模态的全局依赖关系，缺乏来自RGB和深度数据的全面显著性先验，并且在处理低质量深度图时效果不佳。为了解决这些挑战，我们提出了SSNet，一种基于显著性先验和状态空间模型（SSM）的网络，用于RGB-D SOD任务。与现有的基于卷积或变换器的方法不同，SSNet引入了一种基于SSM的多模态多尺度解码器模块，能够以线性复杂度高效地捕捉模态内和模态间的全局依赖关系。具体来说，我们提出了一种跨模态选择性扫描SSM（CM-S6）机制，可以有效地捕捉不同模态之间的全局依赖关系。此外，我们引入了一种显著性增强模块（SEM），将三种显著性先验与深层特征结合，以细化特征表示并提高显著物体的定位。为了进一步解决低质量深度图的问题，我们提出了一种自适应对比度增强技术，能够动态优化深度图，使其更适合于RGB-D SOD任务。在七个基准数据集上的广泛定量和定性实验表明，SSNet优于现有最先进方法。|
|**2025-03-03**|**DCAMamba: Mamba-based Rapid Response DC Arc Fault Detection**|Lukun Wang et.al.|[2503.01264](http://arxiv.org/abs/2503.01264)|null|在电气设备中，即使是轻微的接触问题也可能导致电弧故障。传统方法往往难以同时满足高精度和快速响应的要求，以实现有效的电弧故障检测。为了解决这一挑战，我们引入了DCAMamba，这是一种新的电弧故障检测框架。具体来说，DCAMamba基于状态空间模型（SSM），并利用了一种硬件感知的并行算法，该算法采用循环模式设计，并使用了Mamba架构。为了满足电弧故障检测中对高精度和快速响应的双重需求，我们改进了原始的Mamba模型，并结合了特征放大策略（FAS），这是一种简单但有效的方法，能够增强模型解释电弧故障数据的能力。实验结果表明，带有FAS的DCAMamba相比原始Mamba模型，在准确率上提高了12%，同时保持了仅1.87毫秒的推理时间。这些结果突显了DCAMamba作为未来信号处理骨干技术的巨大潜力。我们的代码将在同行评审后开源。|
|**2025-02-28**|**Visual Attention Exploration in Vision-Based Mamba Models**|Junpeng Wang et.al.|[2502.20764](http://arxiv.org/abs/2502.20764)|null|状态空间模型（SSM）作为一种高效的替代方案，相较于基于Transformer的模型提供了更好的线性复杂度。最新的SSM进展之一——Mamba，引入了一种选择性扫描机制，为输入标记分配可训练权重，有效模仿了注意力机制。Mamba还通过将2D图像分解成较小的块并将其排列为1D序列，成功扩展到了视觉领域。然而，这些块如何根据其原始2D空间位置相互作用（或关注）仍不清楚。此外，用于将块排列成序列的顺序也对其注意力分布有显著影响。为了更好地理解块之间的注意力并探索注意力模式，我们引入了一种专门针对基于视觉的Mamba模型设计的可视化分析工具。该工具使我们能够更深入地了解注意力在不同Mamba块中的分布情况以及在整个Mamba模型中的演变过程。利用该工具，我们还研究了不同的块排序策略对学习到的注意力的影响，进一步揭示了模型的行为。|
|**2025-02-27**|**Accelerating Model-Based Reinforcement Learning with State-Space World Models**|Maria Krinner et.al.|[2502.20168](http://arxiv.org/abs/2502.20168)|null|强化学习（RL）是机器人学习的一种强大方法。然而，无模型强化学习（MFRL）需要大量的环境交互来学习成功的控制策略。这是由于RL训练更新的噪声以及机器人系统的复杂性，这些系统通常涉及高度非线性的动态特性和嘈杂的传感器信号。相比之下，基于模型的强化学习（MBRL）不仅训练策略，还同时学习一个捕捉环境动态和奖励的世界模型。世界模型可以用于规划、数据收集或为训练提供一阶策略梯度。利用世界模型显著提高了样本效率，相比于无模型强化学习。但是，与策略一起训练世界模型增加了计算复杂性，导致较长的训练时间，在复杂的现实场景中通常是难以处理的。在这项工作中，我们提出了一种使用状态空间世界模型加速基于模型的强化学习的新方法。我们的方法利用状态空间模型（SSM）并行化动力学模型的训练，这通常是主要的计算瓶颈。此外，我们提出了一种在训练过程中向世界模型提供特权信息的架构，这对于部分可观测环境尤其相关。我们在多个现实世界的敏捷四旋翼飞行任务中评估了我们的方法，这些任务涉及复杂的动态特性，既包括完全可观测也包括部分可观测环境。我们展示了显著的速度提升，将世界模型训练时间减少了高达10倍，并且整体MBRL训练时间减少了高达4倍。这种好处并没有牺牲性能，因为我们的方法达到了与最先进的MBRL方法相似的样本效率和任务奖励。|
|**2025-02-26**|**On Pruning State-Space LLMs**|Tamer Ghattas et.al.|[2502.18886](http://arxiv.org/abs/2502.18886)|null|最近的工作提出状态空间模型（SSM）作为基于变压器的大规模语言模型的有效替代方案。这些模型能否通过剪枝进一步降低计算成本？我们将几种剪枝方法适应到SSM结构中，并应用于四个基于SSM的大规模语言模型的多个任务。我们发现，这些模型对某些剪枝方法（如WANDA）具有很强的鲁棒性，而使用其他方法则会导致性能迅速下降。|
|**2025-02-25**|**Revisiting Convolution Architecture in the Realm of DNA Foundation Models**|Yu Bo et.al.|[2502.18538](http://arxiv.org/abs/2502.18538)|null|近年来，基于Transformer和状态空间模型（SSM）架构的各种方法被提出，推进了基础DNA语言模型的发展。然而，在这些新方法与经典卷积网络（CNNs）架构在基础模型基准上的对比研究还比较缺乏。这引发了一个问题：基于Transformer和SSM架构的新方法是否真的超越了CNNs？在本文中，我们开发了一种简单但设计精良的基于CNN的方法，称为ConvNova。ConvNova识别并提出了三种有效设计：1）扩张卷积，2）门控卷积，3）用于门控机制的双分支框架。通过广泛的实验证明，ConvNova在多个基础模型基准上超过一半的任务中显著优于最近的方法。例如，在组蛋白相关任务中，ConvNova平均比第二好的方法高出5.8%，同时通常使用更少的参数，并实现更快的计算。此外，实验观察到了可能与生物特性相关的发现。这表明，与Transformer和SSM相比，CNN仍然是一个强有力的竞争对手。我们期望这项工作能够重新激发对基于CNN方法在DNA基础模型中的兴趣。|
|**2025-02-24**|**PICASO: Permutation-Invariant Context Composition with State Space Models**|Tian Yu Liu et.al.|[2502.17605](http://arxiv.org/abs/2502.17605)|null|在推理时为大型语言模型提供相关的上下文知识已被证明可以显著提高其生成的质量。这通常是通过将从外部知识库检索到的信息性文本段落或“上下文”前置到输入中来实现的。然而，在线处理额外的上下文会带来与它们长度成比例的显著计算成本。状态空间模型（SSM）通过允许将上下文数据库映射到固定维度的状态上以开始生成，提供了一个有前景的解决方案。当试图利用多个上下文中存在的信息时，会出现一个关键挑战，因为在现有的SSM中没有直接的方法可以在多个独立状态下进行生成条件化。为了解决这个问题，我们利用从SSM动态导出的一个简单数学关系，将多个状态组合成一个能够有效近似文本上下文串联效果的状态。由于上下文的时间顺序往往不具备信息性，我们通过对所有可能的上下文顺序获得的状态进行高效平均来强制实现排列不变性。我们在WikiText和MSMARCO数据集上对我们的方法进行了评估，包括零样本和微调设置，并表明我们可以匹配表现最强的基线方法，同时平均享受5.4倍的速度提升。|
|**2025-02-24**|**MambaFlow: A Novel and Flow-guided State Space Model for Scene Flow Estimation**|Jiehao Luo et.al.|[2502.16907](http://arxiv.org/abs/2502.16907)|**[link](https://github.com/scnu-rislab/mambaflow)**|
|**2025-02-22**|**Linear Attention for Efficient Bidirectional Sequence Modeling**|Arshia Afzal et.al.|[2502.16249](http://arxiv.org/abs/2502.16249)|**[link](https://github.com/lions-epfl/lion)**|
|**2025-02-22**|**Improving Speech Enhancement by Cross- and Sub-band Processing with State Space Model**|Jizhen Li et.al.|[2502.16207](http://arxiv.org/abs/2502.16207)|null|
|**2025-02-24**|**LaTIM: Measuring Latent Token-to-Token Interactions in Mamba Models**|Hugo Pitorro et.al.|[2502.15612](http://arxiv.org/abs/2502.15612)|null|
|**2025-02-21**|**LightMamba: Efficient Mamba Acceleration on FPGA with Quantization and Hardware Co-design**|Renjie Wei et.al.|[2502.15260](http://arxiv.org/abs/2502.15260)|null|
|**2025-02-20**|**Inferring System and Optimal Control Parameters of Closed-Loop Systems from Partial Observations**|Victor Geadah et.al.|[2502.15014](http://arxiv.org/abs/2502.15014)|null|
|**2025-02-18**|**DAMamba: Vision State Space Model with Dynamic Adaptive Scan**|Tanzhe Li et.al.|[2502.12627](http://arxiv.org/abs/2502.12627)|null|
|**2025-02-12**|**From Layers to States: A State Space Model Perspective to Deep Neural Network Layer Dynamics**|Qinshuo Liu et.al.|[2502.10463](http://arxiv.org/abs/2502.10463)|null|
|**2025-02-12**|**SS4Rec: Continuous-Time Sequential Recommendation with State Space Models**|Wei Xiao et.al.|[2502.08132](http://arxiv.org/abs/2502.08132)|null|
|**2025-02-14**|**Implicit Language Models are RNNs: Balancing Parallelization and Expressivity**|Mark Schöne et.al.|[2502.07827](http://arxiv.org/abs/2502.07827)|null|
|**2025-02-11**|**A Survey on Mamba Architecture for Vision Applications**|Fady Ibrahim et.al.|[2502.07161](http://arxiv.org/abs/2502.07161)|null|
|**2025-02-18**|**XAMBA: Enabling Efficient State Space Models on Resource-Constrained Neural Processing Units**|Arghadip Das et.al.|[2502.06924](http://arxiv.org/abs/2502.06924)|**[link](https://github.com/arghadippurdue/xamba)**|
|**2025-02-08**|**TrackDiffuser: Nearly Model-Free Bayesian Filtering with Diffusion Model**|Yangguang He et.al.|[2502.05629](http://arxiv.org/abs/2502.05629)|null|
|**2025-02-07**|**CMamba: Learned Image Compression with State Space Models**|Zhuojie Wu et.al.|[2502.04988](http://arxiv.org/abs/2502.04988)|null|
|**2025-02-07**|**SSMLoRA: Enhancing Low-Rank Adaptation with State Space Model**|Jiayang Yu et.al.|[2502.04958](http://arxiv.org/abs/2502.04958)|**[link](https://github.com/yuhkalhic/ssmlora)**|
|**2025-02-07**|**A Foundational Brain Dynamics Model via Stochastic Optimal Control**|Joonhyeong Park et.al.|[2502.04892](http://arxiv.org/abs/2502.04892)|null|
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

<p align=right>(<a href=#updated-on-20250310>back to top</a>)</p>

## Communication Intelligence

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2024-09-21**|**LLM Agents as 6G Orchestrator: A Paradigm for Task-Oriented Physical-Layer Automation**|Zhuoran Xiao et.al.|[2410.03688](http://arxiv.org/abs/2410.03688)|null|生成式预训练模型的快速发展正在推动技术进步从基础应用如聊天机器人向更复杂的基于代理的系统转变。将6G系统与大型语言模型（LLM）代理和数字孪生（DT）相结合，对于管理具有新兴特性（如原生AI服务和感知功能）的高度复杂通信系统具有巨大的潜力和必要性。通过6G导向的代理，基站能够理解各种动态上层任务的传输需求，并自动编排最优系统工作流程。通过不断从6G DT获取反馈进行强化，这些代理最终可以相应地提高实际系统的性能。与现有的为通用应用设计的LLM代理不同，6G导向的代理旨在利用大量额外的专业知识来进行高度严谨和精确的规划，这不可避免地需要从模型训练到实施的特定系统设计。本文提出了一种构建面向任务的6G LLM代理的新颖综合方法。我们首先提出了一种两阶段持续预训练和微调方案，以构建领域基础模型和满足各种应用场景需求的各种专业专家模型。此外，还提出了一种基于语义检索的新颖推理框架，以利用现有的通信相关功能。物理层任务分解等示例任务的实验结果表明了所提范式的可行性和有效性。|

<p align=right>(<a href=#updated-on-20250310>back to top</a>)</p>

## RAG

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-03-06**|**More Documents, Same Length: Isolating the Challenge of Multiple Documents in RAG**|Shahar Levy et.al.|[2503.04388](http://arxiv.org/abs/2503.04388)|null|检索增强生成（RAG）为大型语言模型提供相关文档。尽管先前的研究指出，检索大量文档可能会降低性能，但这些研究并未在控制上下文长度的情况下，单独分析文档数量对性能的影响。我们在自定义数据集上评估了多种语言模型，这些数据集来源于一个多跳问答任务。我们保持上下文长度和相关信息位置不变，同时改变文档数量，并发现增加RAG设置中的文档数量对大型语言模型构成了显著挑战。此外，我们的结果表明，处理多个文档与处理长上下文是两个不同的挑战。我们还公开了数据集和代码：https://github.com/shaharl6000/MoreDocsSameLen。|
|**2025-03-06**|**In-depth Analysis of Graph-based RAG in a Unified Framework**|Yingli Zhou et.al.|[2503.04338](http://arxiv.org/abs/2503.04338)|null|基于图的检索增强生成（RAG）已被证明在将外部知识整合到大型语言模型（LLMs）中非常有效，提高了它们的事实准确性、适应性、可解释性和可信度。文献中已经提出了许多基于图的RAG方法。然而，这些方法尚未在同一实验设置下进行系统和全面的比较。在这篇论文中，我们首先从高层次的角度总结了一个统一的框架来整合所有基于图的RAG方法。然后，我们在一系列问答（QA）数据集上广泛比较了代表性的基于图的RAG方法——从具体问题到抽象问题，并检查了所有方法的有效性，提供了对基于图的RAG方法的全面分析。作为实验分析的副产品，我们还能够通过结合现有技术，在特定QA任务和抽象QA任务上识别出新的基于图的RAG方法变体，这些变体超越了当前最先进的方法。最后，基于这些发现，我们提出了有前景的研究机会。我们认为，更深入地理解现有方法的行为可以为未来研究提供新的有价值的见解。|
|**2025-03-04**|**Optimizing open-domain question answering with graph-based retrieval augmented generation**|Joyce Cahoon et.al.|[2503.02922](http://arxiv.org/abs/2503.02922)|null|在这项工作中，我们对各种基于图的检索增强生成（RAG）系统进行了基准测试，涵盖了从OLTP风格（基于事实）到OLAP风格（主题性）的各种查询类型，以应对开放领域问答（QA）中的复杂需求。传统的RAG方法在处理细微的多文档合成任务时往往表现不佳。通过将知识结构化为图，我们可以促进捕捉更深层次语义背景的上下文检索，从而增强语言模型的操作。我们探讨了基于图的RAG方法，并引入了TREX，这是一种新颖且成本效益高的替代方案，结合了基于图和基于向量的检索技术。我们在四个不同数据集上的基准测试突出了不同RAG方法的优势，展示了TREX处理多种开放领域QA类型的能力，并揭示了当前评估方法的局限性。在一个真实的技术支持案例研究中，我们展示了TREX解决方案如何在高效合成来自异构源的数据方面超越传统的基于向量的RAG。我们的研究结果强调了通过先进的检索和编排能力来增强大型语言模型的潜力，推进了可扩展的、基于图的人工智能解决方案的发展。|
|**2025-03-04**|**Wikipedia in the Era of LLMs: Evolution and Risks**|Siming Huang et.al.|[2503.02879](http://arxiv.org/abs/2503.02879)|null|在本文中，我们对大型语言模型（LLMs）对维基百科的影响进行了全面分析，通过现有数据研究了维基百科的演变，并利用模拟探索潜在风险。我们首先通过分析页面浏览量和文章内容来研究维基百科近期的变化，并评估LLMs的影响。随后，我们评估了LLMs如何影响与维基百科相关的各种自然语言处理（NLP）任务，包括机器翻译和检索增强生成（RAG）。我们的发现和模拟结果表明，维基百科的文章受到了LLMs的影响，在某些类别中的影响约为1%-2%。如果基于维基百科的机器翻译基准受到LLMs的影响，模型的得分可能会被抬高，而模型之间的比较结果也可能发生变化。此外，如果知识库被LLMs生成的内容污染，RAG的有效性可能会降低。虽然LLMs尚未完全改变维基百科的语言和知识结构，但我们认为，我们的实证发现表明需要谨慎考虑未来的潜在风险。|
|**2025-03-06**|**RAAD-LLM: Adaptive Anomaly Detection Using LLMs and RAG Integration**|Alicia Russell-Gilbert et.al.|[2503.02800](http://arxiv.org/abs/2503.02800)|null|在复杂工业环境中进行异常检测面临着独特的挑战，特别是在数据稀疏和操作条件不断变化的背景下。这样的设置下的预测性维护（PdM）要求方法具有适应性、可迁移性，并能够整合特定领域的知识。本文提出了RAAD-LLM，这是一种新颖的自适应异常检测框架，它利用了大型语言模型（LLMs）与检索增强生成（RAG）相结合的方法。这种方法解决了上述PdM中的挑战。通过有效利用领域特定的知识，RAAD-LLM能够在无需对特定数据集进行微调的情况下提高时间序列数据中异常检测的准确性。该框架的适应性机制使其能够动态调整对正常操作条件的理解，从而提高了检测精度。我们通过一个塑料制造工厂的真实应用案例以及Skoltech异常基准（SKAB）验证了这一方法的有效性。结果显示，在实际数据集上的准确率从70.7%提升到了89.1%。通过允许输入系列数据与语义信息的丰富结合，RAAD-LLM具备了多模态能力，这有助于模型与工厂操作员之间更加协作的决策制定。总体而言，我们的研究结果支持RAAD-LLM有能力革新PdM中的异常检测方法论，可能引领不同行业中异常检测实施方式的范式转变。|
|**2025-03-04**|**ImpedanceGPT: VLM-driven Impedance Control of Swarm of Mini-drones for Intelligent Navigation in Dynamic Environment**|Faryal Batool et.al.|[2503.02723](http://arxiv.org/abs/2503.02723)|null|群机器人技术在动态和不可预测环境中实现自主操作方面发挥着关键作用。然而，一个主要挑战是确保在充满动态生物（例如，人类）和动态无生命物体障碍物的环境中安全高效地导航。在本文中，我们提出了ImpedanceGPT，这是一种新颖的系统，它结合了视觉-语言模型（VLM）和检索增强生成（RAG），以实现实时推理，使微型无人机群能够在复杂环境中进行自适应导航。ImpedanceGPT的关键创新在于VLM与RAG的集成，这为无人机提供了对其周围环境的增强语义理解。这使得系统能够根据障碍物类型和环境条件动态调整阻抗控制参数。我们的方法不仅确保了安全和精确的导航，还提高了无人机群之间的协调性。实验评估证明了该系统的有效性。VLM-RAG框架在最佳光照条件下实现了80%的障碍物检测和检索准确率。在静态环境中，无人机以1.4米/秒的速度导航动态无生命障碍物，但在接近人类时速度降至0.7米/秒，并增加了间距。在动态环境中，无人机在靠近硬障碍物时速度调整为1.0米/秒，而在需要更大偏移量以安全避开移动的人类时速度降低至0.6米/秒。|
|**2025-03-04**|**FinArena: A Human-Agent Collaboration Framework for Financial Market Analysis and Forecasting**|Congluo Xu et.al.|[2503.02692](http://arxiv.org/abs/2503.02692)|null|为了改进股票趋势预测并支持个性化的投资决策，本文提出了一种新颖的人机协作框架FinArena。受专家混合（MoE）方法的启发，FinArena结合了多模态金融数据分析与用户交互。人类模块提供了一个互动界面，可以捕捉个人的风险偏好，从而允许制定个性化的投资策略。机器模块利用基于大型语言模型（LLM）的多智能体系统来整合多种数据源，如股票价格、新闻文章和财务报表。为了解决LLM中的幻觉问题，FinArena采用自适应检索增强生成（RAG）方法处理非结构化的新闻数据。最后，一个通用的专家智能体根据从多模态数据中提取的特征以及投资者的个人风险偏好做出投资决策。广泛的实验表明，FinArena在股票趋势预测方面超越了传统及最先进的基准，并在不同风险偏好的交易模拟中取得了令人鼓舞的结果。这些发现突显了FinArena通过将战略见解与个性化风险考量相结合来提高投资结果的潜力。|
|**2025-03-05**|**OkraLong: A Flexible Retrieval-Augmented Framework for Long-Text Query Processing**|Yulong Hui et.al.|[2503.02603](http://arxiv.org/abs/2503.02603)|null|大型语言模型（LLM）在高效处理长文本查询时遇到挑战，这在企业文档分析和财务报告理解等应用中尤为明显。虽然传统的解决方案采用长上下文处理或检索增强生成（RAG），但这些方法存在输入成本过高或信息不完整的问题。最近的进展采用了上下文压缩和动态检索循环，但仍会牺牲关键细节或产生迭代成本。为了解决这些限制，我们提出了OkraLong，这是一种新颖的框架，可以灵活优化整个处理工作流。与之前的静态或粗粒度自适应策略不同，OkraLong通过三个协同组件实现细粒度编排：分析器、组织者和执行器。分析器表征任务状态，指导组织者动态调度工作流。执行器执行任务并生成最终答案。实验结果表明，OkraLong不仅提高了答案准确性，还在各种数据集上实现了成本效益。|
|**2025-03-04**|**PennyLang: Pioneering LLM-Based Quantum Code Generation with a Novel PennyLane-Centric Dataset**|Haider Asif et.al.|[2503.02497](http://arxiv.org/abs/2503.02497)|null|大型语言模型（LLM）在代码生成、自然语言处理和领域特定推理方面展现出卓越的能力。然而，它们在辅助量子软件开发方面的潜力，尤其是在PennyLane框架——一个领先的混合量子-经典计算平台上的应用仍待进一步探索。为解决这一问题，我们引入了一个新颖的高质量数据集，包含3,347个PennyLane特定的量子电路代码样本及其上下文描述，专门用于训练/微调基于LLM的量子代码辅助系统。我们的主要贡献有三点：(1) 利用量子计算教科书、官方文档和开源仓库自动生成并开源发布了一个全面的PennyLane数据集；(2) 开发了一套系统的数据精炼、注释和格式化方法，以优化LLM训练效率；(3) 基于检索增强生成（RAG）框架进行了全面评估，展示了我们的数据集在简化PennyLane代码生成和改进量子开发工作流程方面的有效性。与现有主要关注Qiskit的努力相比，我们的数据集显著扩展了AI驱动代码辅助所覆盖的量子框架范围。通过填补这一空白并提供可复现的数据集创建方法，我们旨在推进AI辅助量子编程领域的发展，使量子计算对新手和经验丰富的开发者都更加易于接近。|
|**2025-03-03**|**Cracking Vector Search Indexes**|Vasilis Mageirakos et.al.|[2503.01823](http://arxiv.org/abs/2503.01823)|null|检索增强生成（RAG）利用向量数据库来扩展大型语言模型的专业知识，而无需重新训练。这一理念可以应用于数据湖，从而产生了嵌入式数据湖的概念，即一组准备供RAG使用的向量数据库。这些系统中的关键组件是支持近似最近邻搜索（ANNS）的索引。然而，在数据湖中，我们不能现实地期望为每个可能的数据集构建索引。在本文中，我们提出了一种自适应、基于分区的索引方法CrackIVF，其性能优于预先构建索引的方法。CrackIVF通过近乎暴力搜索的方式开始回答查询，并仅在看到足够多的查询后才进行扩展。它通过逐步适应查询工作负载来实现这一点。这样，可以在不先构建完整索引的情况下立即回答查询。在处理了足够多的查询后，CrackIVF将产生一个与使用传统技术构建的最佳索引相媲美的索引。实验评估表明，CrackIVF通常可以在其他方法甚至还没有完成索引构建之前就回答超过100万个查询，并且能够立即开始回答查询，实现比其他方法快10到1000倍的初始化时间。这使得它非常适合处理冷数据或不常用的数据，或是作为访问未见过的数据集的一种启动方式。|
|**2025-03-03**|**SAGE: A Framework of Precise Retrieval for RAG**|Jintao Zhang et.al.|[2503.01713](http://arxiv.org/abs/2503.01713)|null|
|**2025-03-03**|**Generate, Discriminate, Evolve: Enhancing Context Faithfulness via Fine-Grained Sentence-Level Self-Evolution**|Kun Li et.al.|[2503.01695](http://arxiv.org/abs/2503.01695)|null|
|**2025-03-04**|**SePer: Measure Retrieval Utility Through The Lens Of Semantic Perplexity Reduction**|Lu Dai et.al.|[2503.01478](http://arxiv.org/abs/2503.01478)|**[link](https://github.com/sepermetric/seper)**|
|**2025-02-28**|**RuCCoD: Towards Automated ICD Coding in Russian**|Aleksandr Nesterov et.al.|[2502.21263](http://arxiv.org/abs/2502.21263)|null|
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
|**2025-02-26**|**OntologyRAG: Better and Faster Biomedical Code Mapping with Retrieval-Augmented Generation (RAG) Leveraging Ontology Knowledge Graphs and Large Language Models**|Hui Feng et.al.|[2502.18992](http://arxiv.org/abs/2502.18992)|null|
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
|**2025-02-20**|**Benchmarking Multimodal RAG through a Chart-based Document Question-Answering Generation Framework**|Yuming Yang et.al.|[2502.14864](http://arxiv.org/abs/2502.14864)|null|
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
|**2025-02-05**|**Rankify: A Comprehensive Python Toolkit for Retrieval, Re-Ranking, and Retrieval-Augmented Generation**|Abdelrahman Abdallah et.al.|[2502.02464](http://arxiv.org/abs/2502.02464)|null|
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

<p align=right>(<a href=#updated-on-20250310>back to top</a>)</p>

## text2sql

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-03-04**|**NLI4DB: A Systematic Review of Natural Language Interfaces for Databases**|Mengyi Liu et.al.|[2503.02435](http://arxiv.org/abs/2503.02435)|null|随着在生活各个领域中对数据库查询需求的不断增加，研究人员对自然语言接口数据库（NLIDB）给予了极大的关注。本文全面综述了最近提出的自然语言接口数据库。我们首先简要介绍了自然语言处理技术、可执行数据库语言以及自然语言与可执行语言之间的中间表示，然后概述了从自然语言到可执行数据库语言的转换过程。该转换过程分为三个阶段：(i) 自然语言预处理，(ii) 自然语言理解，和 (iii) 自然语言翻译。在预处理阶段使用了传统方法和数据驱动方法。传统方法依赖于预定义的规则和语法，并涉及正则表达式、依存句法分析和命名实体识别等技术。数据驱动的方法则依赖大规模数据和机器学习模型，使用包括词嵌入和模式链接在内的技术。自然语言理解方法被分为三类：(i) 基于规则的方法，(ii) 基于机器学习的方法，以及 (iii) 混合方法。接着，我们描述了关系型数据库和时空数据库上可执行语言的一般构建过程。随后，介绍了将自然语言转化为可执行语言时常用的基准测试和评估指标，并探讨了生成新基准测试的方法。最后，我们总结了自然语言接口数据库系统的分类、发展和改进，并讨论了与自然语言接口数据库相关的深度语言理解和数据库交互技术，包括 (i) 使用大语言模型进行 Text2SQL 任务，(ii) 从 SQL 生成自然语言解释，以及 (iii) 将语音查询转换为 SQL。|
|**2025-02-23**|**SQLong: Enhanced NL2SQL for Longer Contexts with LLMs**|Dai Quoc Nguyen et.al.|[2502.16747](http://arxiv.org/abs/2502.16747)|null|开放权重的大规模语言模型（LLMs）在自然语言到SQL（NL2SQL）任务中显著提升了性能。然而，当处理大型数据库模式时，由于上下文长度增加，它们的有效性会减弱。为了解决这一限制，我们提出了SQLong，这是一种新颖且高效的数据增强框架，旨在提高LLM在长上下文场景下执行NL2SQL任务的性能。SQLong通过使用来自训练数据中多样模式的额外合成CREATE TABLE命令及其对应的数据行扩展现有数据库模式来生成增强的数据集。这种方法在微调和评估过程中有效模拟了长上下文场景。通过对Spider和BIRD数据集的实验，我们证明了使用SQLong增强数据进行微调的LLMs比那些仅在标准数据集上训练的模型表现更优。这表明了SQLong的实际应用及其对提升真实世界复杂数据库模式下NL2SQL能力的影响。|
|**2025-01-28**|**Balancing Content Size in RAG-Text2SQL System**|Prakhar Gurawa et.al.|[2502.15723](http://arxiv.org/abs/2502.15723)|null|大型语言模型（LLMs）已成为将自然语言查询转换为SQL命令的有效解决方案，使得数据库交互变得无缝。然而，这些文本到SQL（Text2SQL）系统面临着固有的局限性，包括幻觉、过时的知识和不可追溯的推理。为了解决这些挑战，将检索增强生成（RAG）与Text2SQL模型结合的方法越来越受到关注。RAG作为一种检索机制，可以提供重要的上下文信息，如表结构和元数据，以增强查询生成过程。尽管具有潜力，但RAG + Text2SQL系统对检索文档的质量和大小非常敏感。虽然更丰富的文档内容可以提高模式相关性和检索准确性，但它也引入了噪声，随着Text2SQL模型提示大小的增加，增加了产生幻觉的风险并降低了查询的保真度。本研究探讨了文档大小和质量之间的微妙权衡，旨在找到一个优化系统性能的平衡点。我们确定了性能下降的关键阈值，并提出了缓解这些挑战的可行策略。此外，我们还探讨了Text2SQL模型中的幻觉现象，强调精心策划的文档呈现对于减少错误至关重要。我们的研究结果为提高RAG + Text2SQL系统的鲁棒性提供了路线图，为实际应用提供了实用见解。|
|**2025-02-17**|**SQL-o1: A Self-Reward Heuristic Dynamic Search Method for Text-to-SQL**|Shuai Lyu et.al.|[2502.11741](http://arxiv.org/abs/2502.11741)|**[link](https://github.com/shuailyu0110/sql-o1)**|**文本到SQL（Text2SQL）任务旨在将自然语言查询转换为可执行的SQL查询。得益于大规模语言模型（LLMs）的应用，这一领域已经取得了显著进展。然而，仍然存在一些挑战，如模型的可扩展性、有限的生成空间以及SQL生成中的连贯性问题。为了解决这些问题，我们提出了SQL-o1，这是一种基于自奖励的启发式搜索方法，旨在增强LLMs在SQL查询生成中的推理能力。SQL-o1结合了蒙特卡洛树搜索（MCTS）进行启发式过程级搜索，并构建了一个模式感知数据集以帮助模型更好地理解数据库模式。在Bird和Spider数据集上的广泛实验表明，与最新的基线方法相比，SQL-o1在复杂的Bird数据集上提高了10.8%的执行准确率，甚至超过了基于GPT-4的方法。此外，SQL-o1在少样本学习场景中表现出色，并显示出强大的跨模型迁移能力。我们的代码公开发布在：https://github.com/ShuaiLyu0110/SQL-o1。**|
|**2025-01-30**|**Fundamental Challenges in Evaluating Text2SQL Solutions and Detecting Their Limitations**|Cedric Renggli et.al.|[2501.18197](http://arxiv.org/abs/2501.18197)|null|在这项工作中，我们深入探讨了评估Text2SQL解决方案的基本挑战，并指出了潜在的失败原因以及依赖现有基准测试中聚合指标的潜在风险。我们发现了当前开放基准测试中的两个主要未解决的限制：(1) 评估数据中的数据质量问题，主要是由于未能捕捉自然语言描述转化为结构化查询的概率性质（例如，自然语言的模糊性），以及(2) 使用不同的匹配函数作为SQL等价性的近似值时引入的偏差。为了将这两个限制放在具体情境中，我们提出了一种统一的分类法，涵盖所有可能导致预测和评估错误的Text2SQL限制。然后，我们通过使用最先进的Text2SQL解决方案和基准测试对这些限制进行了调查来说明该分类法。我们用实际例子描述了限制的原因，并为分类法中的每一类提出了潜在的缓解方案。最后，我们强调了在部署此类缓解策略或尝试自动应用该分类法时遇到的开放性挑战。|
|**2025-02-13**|**Is Long Context All You Need? Leveraging LLM's Extended Context for NL2SQL**|Yeounoh Chung et.al.|[2501.12372](http://arxiv.org/abs/2501.12372)|null|大型语言模型（LLMs）在一系列自然语言处理任务中展示了令人印象深刻的能力。特别是在推理能力和上下文窗口扩展方面的改进为利用这些强大模型开辟了新的途径。NL2SQL具有挑战性，因为自然语言问题本身具有模糊性，而生成SQL则需要对复杂的数据模式和语义有精确的理解。解决这种语义模糊问题的一种方法是提供更多的充分的上下文信息。在这项工作中，我们探讨了谷歌最先进的LLM（\textit{gemini-1.5-pro}）提供的扩展上下文窗口（也称为长上下文）在性能和延迟之间的权衡。我们研究了各种上下文信息的影响，包括列示例值、问题与SQL查询对、用户提供的提示、SQL文档和模式。据我们所知，这是首次研究扩展上下文窗口和额外上下文信息如何帮助NL2SQL生成，在准确性和延迟成本方面都有所考虑。我们表明，长上下文LLMs是稳健的，不会在扩展的上下文信息中迷失方向。此外，基于谷歌的\textit{gemini-pro-1.5}构建的长上下文NL2SQL流水线在多个基准数据集上实现了强大的性能，无需微调和昂贵的一致性技术。|
|**2025-02-08**|**Semantic Captioning: Benchmark Dataset and Graph-Aware Few-Shot In-Context Learning for SQL2Text**|Ali Al-Lawati et.al.|[2501.03166](http://arxiv.org/abs/2501.03166)|**[link](https://github.com/aliwister/ast-icl)**|**大型语言模型（LLM）在各种自然语言处理任务中表现出色，包括将自然语言翻译成形式化的代码表示的语义解析。然而，反向过程，即将代码翻译成自然语言，称为语义标注，受到的关注较少。随着LLM被集成到代码生成、安全分析和教育用途的平台中，这一任务变得越来越重要。本文专注于SQL查询的标注（SQL2Text），以应对理解并解释SQL查询的需求，尤其是在LLM生成的代码可能带来潜在安全风险的时代。我们通过引入使用GPT-4o生成多个额外表达的迭代ICL提示，重新利用了Text2SQL数据集来进行SQL2Text任务，从而增强了数据集对于反向任务的鲁棒性。我们基于不同的样本选择方法进行了基于上下文学习（ICL）的实验，重点放在更小、计算效率更高的LLM上。我们的研究结果表明，利用SQL固有的图属性进行ICL样本选择，在BLEU评分上比随机选择高出多达39%，并且提供了比其他方法更好的结果。数据集和代码已发布：https://github.com/aliwister/ast-icl。**|
|**2025-01-03**|**CarbonChat: Large Language Model-Based Corporate Carbon Emission Analysis and Climate Knowledge Q&A System**|Zhixuan Cao et.al.|[2501.02031](http://arxiv.org/abs/2501.02031)|null|随着全球气候变化影响的加剧，企业碳排放已成为全球关注的焦点。针对大型语言模型中气候知识更新滞后、传统增强生成架构在处理复杂问题时缺乏专业性和准确性以及可持续性报告分析成本高和耗时长等问题，本文提出了CarbonChat：基于大型语言模型的企业碳排放分析和气候知识问答系统，旨在实现精准的碳排放分析和政策理解。首先，提出了一种多样化的指数模块构建方法，用于处理基于规则和长文本文档的分割及结构化数据提取，从而优化关键信息解析。其次，设计了一种增强的自提示检索增强生成架构，集成了意图识别、结构化推理链、混合检索和Text2SQL，提高了语义理解和查询转换的效率。接着，基于温室气体核算框架，建立了14个维度的碳排放分析体系，能够进行报告摘要、相关性评估和定制化响应。最后，通过多层次分块机制、时间戳和幻觉检测功能，确保了分析结果的准确性和可验证性，降低了幻觉率，提升了响应的精度。|
|**2024-12-22**|**A Plug-and-Play Natural Language Rewriter for Natural Language to SQL**|Peixian Ma et.al.|[2412.17068](http://arxiv.org/abs/2412.17068)|null|现有的自然语言到SQL（NL2SQL）解决方案已经取得了显著进展，但由于用户对数据库模式理解有限或对特定表或列值存在记忆偏差，导致在解释和翻译自然语言查询时仍然面临挑战。这些挑战常常导致不正确的NL2SQL转换。为了解决这些问题，我们提出了REWRITER，这是一个即插即用的模块，旨在通过自动重写模糊或有缺陷的自然语言查询来增强NL2SQL系统。通过整合数据库知识和内容（例如，列值和外键），REWRITER减少了由有缺陷的自然语言输入引起的错误，并提高了SQL生成的准确性。我们的REWRITER将NL2SQL模型视为黑盒，确保与各种NL2SQL方法兼容，包括基于代理和基于规则的NL2SQL解决方案。REWRITER包含三个关键组件：Checker、Reflector和Rewriter。Checker通过评估生成的SQL的正确性来识别有缺陷的自然语言查询，从而最小化不必要的重写和潜在的幻觉。Reflector分析并积累经验以识别自然语言查询中的问题，而Rewriter则根据Reflector的反馈修改查询。在Spider和BIRD基准测试上的广泛实验表明，REWRITER能够持续改进下游模型，在执行准确性方面分别平均提升了1.6%和2.0%。|
|**2024-12-17**|**SynthCypher: A Fully Synthetic Data Generation Framework for Text-to-Cypher Querying in Knowledge Graphs**|Aman Tiwari et.al.|[2412.12612](http://arxiv.org/abs/2412.12612)|null|
|**2024-12-13**|**ROUTE: Robust Multitask Tuning and Collaboration for Text-to-SQL**|Yang Qin et.al.|[2412.10138](http://arxiv.org/abs/2412.10138)|**[link](https://github.com/alibaba/route)**|**尽管大型语言模型（LLMs）在文本到SQL（Text2SQL）方面取得了显著进展，但最新的技术仍然局限于闭源LLM（如GPT-4）的上下文学习中，这限制了它们在开放场景中的应用。为了解决这一挑战，我们提出了一种新颖的鲁棒多任务调优和协作方法（ROUTE），以提高开源LLM在Text2SQL方面的综合能力，从而提供一个更实用的解决方案。我们的方法首先使用多种与SQL生成相关的合成训练数据进行多任务监督微调（SFT）。与现有的基于SFT的Text2SQL方法不同，我们引入了几个额外的SFT任务，包括模式链接、噪声校正和续写。参与多种SQL生成任务增强了模型对SQL语法的理解，并提高了其生成高质量SQL查询的能力。此外，受LLM代理协作模式的启发，我们引入了一种多任务协作提示策略（MCP）。该策略利用多个SQL相关任务之间的协作来减少SQL生成过程中的幻觉，从而通过显式的多任务能力最大限度地提升Text2SQL性能。我们在八个开源LLM和五个广泛使用的基准上进行了广泛的实验和深入分析。结果表明，我们的方法优于最新的Text2SQL方法，并取得了领先的性能。**|
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

<p align=right>(<a href=#updated-on-20250310>back to top</a>)</p>

## PPC

|Publish Date|Title|Authors|PDF|Code|Abstract|
|---|---|---|---|---|---|
|**2025-03-07**|**Fundamental Limits of Hierarchical Secure Aggregation with Cyclic User Association**|Xiang Zhang et.al.|[2503.04564](http://arxiv.org/abs/2503.04564)|null|安全聚合在联邦学习（FL）中被提出，其中云服务器旨在计算众多客户端本地训练模型的平均模型（即深度神经网络的权重），同时遵守数据安全要求。分层安全聚合（HSA）将这一概念扩展到三层网络，其中集群用户通过中间继电器层与服务器通信。在HSA中，除了传统的服务器安全性外，还强制执行继电器安全性，以确保继电器对用户的输入保持不知情（这是FL中本地模型的一种抽象）。现有的HSA研究假设每个用户仅与一个继电器关联，这限制了跨集群用户之间进行编码以实现高效通信和密钥生成的机会。在本文中，我们考虑了一种循环关联模式的HSA，其中每个用户以环绕方式连接到B个连续的继电器。我们提出了一种高效的聚合方案，该方案包括受梯度编码启发的输入消息设计——这是一种在分布式计算中用于高效通信的知名技术——以及一种高度非平凡的安全密钥设计。我们还利用信息论论证推导了关于最小可实现通信和密钥速率的新颖反向界。|
|**2025-03-06**|**Federated Dynamic Modeling and Learning for Spatiotemporal Data Forecasting**|Thien Pham et.al.|[2503.04528](http://arxiv.org/abs/2503.04528)|null|本文提出了一种先进的联邦学习（FL）框架，用于预测复杂的时空数据，改进了最近的最先进模型。在所提出的方案中，首先将先前动态时空图卷积循环网络（DSTGCRN）建模中的门控循环单元（GRU）模块替换为长短期记忆（LSTM）网络，使生成的模型能够更有效地捕捉时间序列数据中的长期依赖关系。这种架构显著提高了模型处理各种预测应用中复杂时间模式的能力。此外，所提出的FL框架集成了一个新颖的客户端验证（CSV）机制，在客户端层面引入了一个关键的验证步骤，以确保在将中央服务器的聚合参数纳入本地模型之前，仅采用最有效的更新。这不仅提高了预测模型在各客户端上的鲁棒性和准确性，还通过广泛的实验在实际应用中展示了其效率，包括多模式交通需求预测的公共数据集和城市区域内的起终点（OD）矩阵预测的私有数据集。结果表明，该方法相比传统方法有了显著改进，突显了该框架在捕获复杂时空依赖关系的同时保护数据隐私的能力。这项工作不仅为实时、区域特定的预测和管理提供了一个可扩展且保护隐私的解决方案，还强调了在联邦学习背景下利用分布式数据源的潜力。我们已在GitHub上开源了我们的算法。|
|**2025-03-06**|**Runtime Backdoor Detection for Federated Learning via Representational Dissimilarity Analysis**|Xiyue Zhang et.al.|[2503.04473](http://arxiv.org/abs/2503.04473)|null|联邦学习（FL）作为一种强大的学习范式，通过聚合来自分布式客户端的模型更新来训练共享模型。然而，模型学习与本地数据的解耦使得FL极易受到后门攻击的影响，其中单个被攻破的客户端就可能污染共享模型。尽管在后门检测方面已经取得了一些进展，但现有方法在检测准确性和运行时效率方面仍面临挑战，尤其是在处理复杂的模型架构时。在这项工作中，我们提出了一种新的方法，能够在准确、稳定和高效的方式下检测恶意客户端。我们的方法利用基于采样的网络表示方法来量化客户端之间的差异性，从而识别由后门注入引起的模型偏差。我们还提出了一种迭代算法，根据这些差异性度量逐步检测并排除恶意客户端作为异常值。在一系列基准任务上的评估表明，我们的方法在检测准确性和防御效果方面优于最先进的方法。当部署用于运行时保护时，我们的方法能够以微小的开销有效消除后门注入。|
|**2025-03-06**|**Privacy Preserving and Robust Aggregation for Cross-Silo Federated Learning in Non-IID Settings**|Marco Arazzi et.al.|[2503.04451](http://arxiv.org/abs/2503.04451)|null|联邦平均仍然是联邦学习中最广泛使用的聚合策略，因为它简单且可扩展。然而，在非独立同分布（非-IID）数据设置中，其性能显著下降，特别是在客户端分布高度不平衡或倾斜的情况下。此外，它依赖于客户端传输元数据，特别是训练样本的数量，这引入了隐私风险，并可能与欧洲的GDPR等监管框架相冲突。在本文中，我们提出了一种新的聚合策略，通过引入类感知梯度掩蔽来解决这些挑战。与传统方法不同，我们的方法仅依赖于梯度更新，消除了对任何额外客户端元数据的需求，从而增强了隐私保护。此外，我们的方法根据类特定的重要性验证并动态加权客户端贡献，确保在非-IID分布、防止收敛和后门攻击方面具有鲁棒性。在基准数据集上的大量实验表明，我们的方法不仅在非-IID设置中优于FedAvg和其他广泛接受的聚合策略，而且在对抗场景中也保持了模型的完整性。我们的结果确立了梯度掩蔽作为联邦学习中实用且安全的解决方案的有效性。|
|**2025-03-06**|**InFL-UX: A Toolkit for Web-Based Interactive Federated Learning**|Tim Maurer et.al.|[2503.04318](http://arxiv.org/abs/2503.04318)|null|本文介绍了InFL-UX，这是一个交互式的概念验证浏览器联邦学习（FL）工具包，旨在将用户贡献无缝集成到机器学习（ML）工作流程中。InFL-UX使多设备上的用户能够上传数据集、定义类别，并使用现代网络技术直接在浏览器中协作训练分类模型。与通常专注于后端模拟的传统FL工具包不同，InFL-UX为研究人员提供了一个简单的用户界面，以便探索用户如何在现实世界中的交互环境中与FL系统互动并做出贡献。通过优先考虑可用性和去中心化的模型训练，InFL-UX弥合了FL和交互式机器学习（IML）之间的差距，使非技术用户也能积极参与到ML分类任务中。|
|**2025-03-06**|**One-Shot Clustering for Federated Learning**|Maciej Krzysztof Zuziak et.al.|[2503.04231](http://arxiv.org/abs/2503.04231)|null|联邦学习（FL）是一种广泛采用的去中心化学习范式，它允许从多个来源训练一个模型，而无需在参与的客户端之间直接传输数据。自2015年提出以来，它已经细分为众多子领域，以处理特定应用问题，无论是数据异质性还是资源分配。其中一个子领域，集群联邦学习（CFL），致力于将客户端群体划分为不同的队列，以提供个性化模型。尽管在这个领域已经发表了一些杰出的工作，但该问题仍然很大程度上未被探索，因为其基本假设和设置与标准FL略有不同。在这项工作中，我们提出了一种与聚类无关的算法——单次集群联邦学习（OCFL），它可以自动检测进行聚类的最早合适时机。我们的算法基于计算客户端梯度之间的余弦相似度以及一个温度测量值来检测联邦模型何时开始收敛。我们通过在三个基准数据集上的三十多个不同任务中测试各种单次聚类算法来实证评估我们的方法。实验结果展示了我们的方法在自动化执行CFL时的良好性能，无需调整超参数。|
|**2025-03-06**|**LiteChain: A Lightweight Blockchain for Verifiable and Scalable Federated Learning in Massive Edge Networks**|Handi Chen et.al.|[2503.04140](http://arxiv.org/abs/2503.04140)|null|利用区块链在联邦学习（FL）中作为一种新的范式，为大规模边缘网络（MENs）中的安全协作学习提供了可能。随着MENs规模的扩大，在边缘设备之间实现和管理区块链变得更加困难，这主要是由于复杂的通信拓扑、异构的计算能力和有限的存储容量。此外，缺乏一个标准的区块链安全度量指标成为一个重要的问题。为了解决这些挑战，我们提出了一种轻量级的区块链，名为LiteChain，旨在为MENs提供高效且安全的服务。具体来说，我们开发了一种分布式聚类算法，将MENs重组为两层结构，以提高在安全要求下的通信和计算效率。此外，我们引入了一种综合拜占庭容错（CBFT）共识机制和一种安全更新机制，通过LiteChain确保模型交易的安全性。基于Hyperledger Fabric的实验表明，与另外两个基准相比，LiteChain在不同网络规模下表现出最低的端到端延迟和链上存储开销。此外，LiteChain对重放攻击和数据投毒攻击表现出了高水平的鲁棒性。|
|**2025-03-06**|**FLAME: A Federated Learning Approach for Multi-Modal RF Fingerprinting**|Kiarash Kianfar et.al.|[2503.04136](http://arxiv.org/abs/2503.04136)|null|授权系统越来越多地依赖于在接收器上处理射频（RF）波形来指纹识别（即确定身份）相应的发射器。联邦学习（FL）已成为在具有多个接入点（APs）的网络中执行RF指纹识别的一种流行范式，因为它们允许有效的基于深度学习的设备识别，而无需将本地收集并存储在多个AP上的RF信号集中化。然而，仅在同相和正交（IQ）时间样本上操作的FL算法会带来较高的收敛率，导致过多的训练轮次和低效的训练时间。在这项工作中，我们提出了FLAME：一种用于多模态RF指纹识别的FL方法。我们的框架包括同时以多种互补模态表示接收到的RF波形，除了IQ样本外，旨在减少训练时间。我们从理论上证明了该方法的可行性和效率，并推导出一个收敛界，在相同的训练轮次下，该界能带来更低的损失和更高的准确性，与单模态FL-based RF指纹识别相比。广泛的实证评估验证了我们的理论结果，并展示了FLAME相对于多个基线方法的优越性，改进幅度最高可达30%。|
|**2025-03-06**|**Generalization in Federated Learning: A Conditional Mutual Information Framework**|Ziqiao Wang et.al.|[2503.04091](http://arxiv.org/abs/2503.04091)|null|联邦学习（FL）是一种广泛采用的隐私保护分布式学习框架，但其泛化性能相比集中式学习而言探索较少。在FL中，泛化误差由两个部分组成：样本外差距，它衡量参与客户端的经验风险与真实风险之间的差距；以及参与差距，它量化了参与和非参与客户端之间的风险差异。在这项工作中，我们通过条件互信息（CMI）框架的信息论分析来研究FL的两层泛化。除了传统的基于超样本的CMI框架之外，我们引入了一种超级客户端构造以适应FL中的两层泛化设置。我们推导了多个基于CMI的界，包括基于假设的CMI界，说明了FL中的隐私约束如何暗示泛化保证。此外，我们提出了快速评估的CMI界，在小经验风险状态下恢复了两层FL泛化的最佳已知收敛率。对于特定的FL模型聚合策略和结构化损失函数，我们细化了我们的界，以实现关于参与客户端数量的改进收敛率。实证评估证实，我们的评估CMI界是非空洞的，并且能够准确捕捉FL算法的泛化行为。|
|**2025-03-06**|**Brain Tumor Detection in MRI Based on Federated Learning with YOLOv11**|Sheikh Moonwara Anjum Monisha et.al.|[2503.04087](http://arxiv.org/abs/2503.04087)|null|在医学诊断中，使用磁共振成像（MRI）准确高效地检测脑肿瘤是一个主要挑战。但目前的机器学习（ML）方法存在两个主要限制：数据隐私和高延迟。为了解决这个问题，本研究提出了一种联邦学习架构，结合YOLOv11算法以实现更准确的脑肿瘤检测。与之前的集中式学习方法不同，我们的联邦学习方法在支持多个机构间合作进行深度学习模型训练的同时保护了底层医疗数据。我们调整YOLOv11模型以处理MRI数据，使其能够定位和识别肿瘤区域。为了确保鲁棒性和泛化能力，该模型在从多个匿名医疗机构收集的广泛MRI数据上进行了训练和测试。结果表明，我们的方法显著保持了比传统方法更高的准确性。|
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
|**2025-03-04**|**Federated nnU-Net for Privacy-Preserving Medical Image Segmentation**|Grzegorz Skorupko et.al.|[2503.02549](http://arxiv.org/abs/2503.02549)|null|
|**2025-03-04**|**AugFL: Augmenting Federated Learning with Pretrained Models**|Sheng Yue et.al.|[2503.02154](http://arxiv.org/abs/2503.02154)|null|
|**2025-03-03**|**A Lightweight and Secure Deep Learning Model for Privacy-Preserving Federated Learning in Intelligent Enterprises**|Reza Fotohi et.al.|[2503.02017](http://arxiv.org/abs/2503.02017)|null|
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
|**2025-02-27**|**Can Textual Gradient Work in Federated Learning?**|Minghui Chen et.al.|[2502.19980](http://arxiv.org/abs/2502.19980)|null|
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

<p align=right>(<a href=#updated-on-20250310>back to top</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[contributors-url]: https://github.com/Vincentqyw/cv-arxiv-daily/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[forks-url]: https://github.com/Vincentqyw/cv-arxiv-daily/network/members
[stars-shield]: https://img.shields.io/github/stars/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[stars-url]: https://github.com/Vincentqyw/cv-arxiv-daily/stargazers
[issues-shield]: https://img.shields.io/github/issues/Vincentqyw/cv-arxiv-daily.svg?style=for-the-badge
[issues-url]: https://github.com/Vincentqyw/cv-arxiv-daily/issues

