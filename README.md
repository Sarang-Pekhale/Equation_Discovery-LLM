# LLM-DDE: Large Language Model for Data-Driven Equation Discovery
Equation discovery—the automatic extraction of governing equations directly from data—has emerged as a crucial challenge in understanding complex nonlinear dynamics. Traditional methods often struggle with generalization, require manually crafted priors, or face optimization hurdles.

We introduce a new framework that utilizes the reasoning capabilities of Large Language Models (LLMs) combined with data-driven self-improvement and evolutionary search to automatically discover interpretable equations.

## 🚀 Key Contributions

### Natural Language Prompting with Data:
Subsampled system data (operands and operators) are embedded into the prompts given to the LLM, grounding the generation of plausible, physically interpretable candidate equations.

### Exploration-Exploitation Strategy:

#### Self-Improvement (Exploitation): Iteratively refines candidate equations using black-box optimization principles.

#### Genetic Algorithm Reasoning (Exploration): Encourages global search by mimicking mutation, crossover, and selection behaviors through LLM prompting.

### Automated Evaluation Loop:
Candidate equations are evaluated numerically on the system data, scored, and iteratively refined until convergence to the best solution.

## 🛠️ Framework Overview
![Flowchart_AI_EQ drawio (1)](https://github.com/user-attachments/assets/b861ad9c-1371-4b29-854c-c2b26da6ec14)

## 📊 Experimental Systems

We evaluate our method across a set of well-known partial differential equations (PDEs):

- **Burgers' Equation**  
  *Modeling nonlinear convection and diffusion phenomena in fluid dynamics.*

- **Chafee–Infante Equation**  
  *Captures bistable reaction-diffusion processes in pattern formation.*

- **Kuramoto–Sivashinsky (KS) Equation**  
  *Describes chaotic behavior in laminar flame fronts and unstable media.*

- **PDE-Divide Dataset**  
  *A collection of diverse PDE systems designed for equation discovery evaluation.*

- **Fisher–KPP Equation**  
  *Models population growth and spread phenomena in biological systems.*

- **Korteweg–de Vries (KdV) Equation**  
  *Describes nonlinear wave propagation and soliton dynamics.*

## 📈 Results
Our method demonstrates competitive or superior performance compared to state-of-the-art models such as LLM4ED (Mengge Du et al.), especially in discovering interpretable and accurate equations from sparse or noisy data.
![Comparison](https://github.com/user-attachments/assets/5053f614-0ce1-44f0-9f44-36c4cd8e09de)

## 📚 Citation

@misc{roy_pekhale_2025,
  author = {Roy, Amartya and Pekhale, Sarang},
  title = {Large Language Models for Automatic Equation Discovery of Nonlinear Dynamics},
  year = {2025},
  note = {Unpublished work}
}

