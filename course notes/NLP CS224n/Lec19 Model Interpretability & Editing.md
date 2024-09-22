---
id: Lec19
created_date: 2024-09-13
updated_date: 2024-09-13
type: course
---

# 📚 Lec19 Model Interpretability & Editing
- **🏷️Tags** :   #09-2024 #course #pending #lecture 
## 📝 Notes


### 1. Introduction: Chasing Dreams of Communication with Machines
- This section outlines Been Kim's desire to leverage LLMs and generative models for the benefit of humanity, focusing on the dream of learning something new through communication with machines.
### 2. The Gap: What Machines Know vs. What We Think They Know
- This section highlights the discrepancy between our perception of machine knowledge and their actual capabilities.
- It introduces the challenge of imperfect tools for understanding machine learning models and their limitations in revealing true model behavior.

### 3. Challenging Assumptions: Unveiling Flaws in Interpretation Tools**

- This section dives into the shortcomings of existing tools used to interpret machine learning models, specifically focusing on:
- **3.1 Wrong Assumptions:** Tools often operate under flawed assumptions about model behavior, leading to inaccurate interpretations.
- **3.2 Unmet Expectations:** Tools may not function as intended, failing to capture the true decision-making processes of the models.
- **3.3 Beyond Human Comprehension:** The complexity of some models might surpass human understanding, rendering current tools insufficient.

### 4. Case Study: Gestalt Phenomenon and Misleading Explanations**

- This section delves into a specific case study demonstrating the limitations of interpretation tools:
- **4.1 The Gestalt Phenomenon:** Kim discusses how neural networks exhibit behavior analogous to the Gestalt principles, where the whole is greater than the sum of its parts. This challenges the assumption that understanding individual components translates to understanding the system's overall behavior.
- **4.2 Debugging Tests for Explanations:** Kim presents her work on testing and identifying potential failures in model explanations.
- **4.3 Limitations of Post-Hoc Explanations:** This section explores how post-hoc explanations might not effectively detect unknown spurious correlations in model behavior.

### 5. Theoretical and Empirical Evidence of Misalignment**

- **5.1 Zero Attribution Fallacy:** Kim demonstrates that just because an attribution method assigns zero importance to a feature, it doesn't mean the model isn't using that feature, challenging the validity of common interpretation techniques.
- **5.2 Theoretical Performance Guarantees:** This section examines the theoretical limitations of popular feature attribution methods, showing how they often fail to meet our expectations in practice.
- **5.3 Empirical Validation and Sample Complexity:** Kim presents empirical evidence supporting her theoretical claims, suggesting that increasing sample size might be a simpler solution than developing more complex interpretation methods.

### 6. Model Editing: Challenging Localization Assumptions**

- **6.1 Localization and Editing Success:** This section explores the relationship between localizing factual information in LLMs and the success of model editing techniques. Kim argues that contrary to common assumptions, localization might not be crucial for successful editing.
- **6.2 ROME and MEMIT Analysis:** Kim analyzes the causal tracing algorithms of ROME and MEMIT, popular model editing techniques, to demonstrate the disconnect between localization and editing outcomes.
- **6.3 The Importance of Layer Selection:** Instead of focusing on precise localization, Kim's findings suggest that selecting the appropriate layer for editing plays a more significant role in achieving desired changes in model behavior.

### 7. Bridging the Gap: New Approaches to Understanding Machine Behavior**

- Kim advocates for shifting our perspective towards studying machines as a new species, requiring observational and controlled studies to bridge the gap between our understanding and their actual capabilities.
- She emphasizes the importance of adapting our expectations of interpretation tools based on the specific tasks and goals we aim to achieve with machine learning models.

### 8. Observational Studies: Discovering Emergent Multi-Agent Behaviors**

- Kim introduces observational studies as a valuable approach to understanding machines, particularly in the context of multi-agent systems.
- She presents MOHBA (Multiagent Offline Hierarchical Behavior Analyzer), a method for automatically detecting and visualizing emergent multi-agent behaviors from observational data.
- Kim demonstrates MOHBA's ability to identify complex behaviors in multi-agent environments, highlighting its potential for understanding emergent phenomena.

### 9. Controlled Studies: Intervening and Discovering Emergent Behaviors**

- This section focuses on controlled studies, where researchers intervene in multi-agent systems to understand the causal relationships between interventions and emergent behaviors.
- Kim introduces a novel approach for building controllable multi-agent systems that maintain performance comparable to baseline methods while allowing for targeted interventions.
- She presents two case studies showcasing the effectiveness of this approach:
- **9.1 Emerging Coordination in Cooking Games:** This study investigates the factors influencing coordination between agents in a simulated cooking environment.
- **9.2 Inter-Agent Social Dynamics in Clean Up Tasks:** This study explores the complex social interactions and dependencies between agents in a simulated cleanup scenario.

### 10. Looking Ahead: Future Directions and Hopes for Human-Machine Collaboration**

- Kim concludes by highlighting promising future directions for research, including:
- Studying superhuman AI systems like AlphaZero to discover new strategies and knowledge beyond human capabilities.
- Improving existing interpretation tools to address their limitations and better align them with our expectations.
- Continuing to develop novel approaches for studying and understanding machine behavior, particularly in complex multi-agent settings.
- The lecture emphasizes the ongoing journey of bridging the gap between machines and humans, driven by the ultimate dream of learning something new and beneficial through this collaborative exploration.

## ❓ Questions
- 

## 👋 New terms
- **LLM (Large Language Model):** A type of artificial intelligence model trained on vast amounts of text data, capable of understanding and generating human-like text.
- **Generative Model:** A class of AI models that learn data distributions and generate new data samples that resemble the training data.
- **Saliency Map:** A visualization technique used to highlight the importance of different input features in a model's prediction.
- **Gestalt Phenomenon:** The principle that the human mind tends to perceive the whole rather than the sum of its parts. In the context of AI, it refers to models potentially learning representations that go beyond individual features.
- **Spurious Correlation:** A statistical relationship between two variables that appears to be causal but is not, often due to a hidden, confounding variable.
- **Post-hoc Explanation:** Interpretations of a model's decision-making process that are generated _after_ the model has been trained, aiming to explain how the model arrived at a particular output.
- **Attribution Method:** Techniques that assign importance scores to input features, indicating their contribution to a model's prediction. Examples include SHAP (SHapley Additive exPlanations) and Integrated Gradients.
- **Completeness and Additive Properties (in Attribution Methods):** Desirable properties of attribution methods ensuring that they fully account for the model's prediction and that the contributions of individual features add up to the overall output.
- **Recourse:** In the context of AI fairness, it refers to the possibility of an individual changing their features to achieve a desired outcome from a model.
- **Model Editing:** Techniques that modify a trained model by changing its internal parameters or representations to adjust its behavior or correct errors.
- **ROME (Rank One Model Editing):** A specific model editing technique that identifies and modifies a rank-one subspace within a model's representation to alter its behavior on a target fact.
- **MEMIT (Multi-Layer Editing for Mitigation of Interference in Transformers):** An extension of ROME that considers multiple layers for model editing.
- **Causal Tracing:** A method for analyzing the flow of information within a model to identify the causal pathways leading to a particular prediction.
- **Multi-Agent System:** A system composed of multiple interacting intelligent agents, each acting autonomously to achieve individual or shared goals.
- **Emergent Behavior:** Complex patterns or behaviors that arise from the interaction of simpler components within a system. In multi-agent systems, emergent behavior refers to collective outcomes that are not explicitly programmed but result from the agents' interactions.
- **MOHBA (Multiagent Offline Hierarchical Behavior Analyzer):** A technique for automatically discovering and visualizing emergent behaviors in multi-agent systems from observational data.
- **PPO (Proximal Policy Optimization):** A reinforcement learning algorithm that learns a policy by iteratively improving it while constraining the changes to ensure stability.

| Term | Definition |
| ---- | ---------- |
|      |            |

## 🔗 Related links
