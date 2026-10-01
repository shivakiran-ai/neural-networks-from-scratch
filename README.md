<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D3B6E,50:1A56A0,100:2E75B6&height=220&section=header&text=Neural%20Networks%20from%20Scratch&fontSize=46&fontColor=ffffff&fontAlignY=40&desc=Every%20neuron,%20gradient%20and%20optimizer%20built%20from%20first%20principles%20in%20NumPy&descAlignY=60&descSize=16"/>

<br/>

![Author](https://img.shields.io/badge/Author-SHIVA%20KIRAN%20DADISHETTY-0D3B6E?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Only-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active%20Development-22C55E?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-F59E0B?style=for-the-badge)

![Topics Complete](https://img.shields.io/badge/Topics%20Complete-0%20%2F%2034-1A56A0?style=for-the-badge)
![Stage 1](https://img.shields.io/badge/Stage%201%20%7C%20Forward%20Pass-0%2F7-2E75B6?style=for-the-badge)
![Stage 2](https://img.shields.io/badge/Stage%202%20%7C%20Loss%20%26%20Calculus-0%2F4-6B7280?style=for-the-badge)
![Stage 3](https://img.shields.io/badge/Stage%203%20%7C%20Backpropagation-0%2F10-6B7280?style=for-the-badge)
![Stage 4](https://img.shields.io/badge/Stage%204%20%7C%20Optimizers-0%2F6-6B7280?style=for-the-badge)
![Stage 5](https://img.shields.io/badge/Stage%205%20%7C%20Regularization-0%2F4-6B7280?style=for-the-badge)
![Stage 6](https://img.shields.io/badge/Stage%206%20%7C%20Projects-0%2F3-6B7280?style=for-the-badge)

</div>

---

## About This Repository

This repository documents a complete, ground-up implementation of a neural network library, from a single neuron's weighted sum all the way to trained models on real-world datasets.

Every component is built from first principles in **pure Python and NumPy**. No PyTorch. No TensorFlow. No autograd. Every forward pass, every gradient, every optimizer update is derived by hand and coded explicitly.

This is the **foundation series** of a three-part research preparation path toward doctoral study in machine learning, with a focus on LLM pretraining and finetuning. The mechanics built here (dense layers, softmax, cross-entropy, backpropagation, Adam, dropout) are exactly the mechanics that reappear, at scale, inside every Transformer.

---

## The Learning Path

```
neural-networks-from-scratch    ← You are here
        │  Pure NumPy · manual backpropagation · optimizers · regularization
        ▼
llm-from-scratch
        │  PyTorch · tokenization → attention → GPT-2 124M → pretraining → finetuning
        ▼
deepseek-from-scratch           (coming soon)
           MLA · GQA · Mixture-of-Experts · Multi-Token Prediction · RoPE · quantization
```

---

## How to Use This Repository

Every topic folder contains exactly **three files**:

| File | Purpose |
|------|---------|
| `README.md` | Sharp summary: key concept, what was built, core insight, paper connection. **Start here.** |
| `TopicN_Title.docx` | Complete deep dive: every derivation, all mathematics, full code reference, every design decision explained. |
| `notebook.ipynb` | Fully annotated, runnable NumPy implementation, built from scratch and extensively commented. |

Read the `README.md` first. Run the `.ipynb` to see it in action. Open the `.docx` to go completely deep.

---

## Progress

```
Overall  ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░   0 / 34 topics complete

Stage 1  Neurons & Forward Pass    ░░░░░░░░░░░░░░░░░░░░   0 / 7   ← active
Stage 2  Loss & Calculus           ░░░░░░░░░░░░░░░░░░░░   0 / 4
Stage 3  Backpropagation           ░░░░░░░░░░░░░░░░░░░░   0 / 10
Stage 4  Optimizers                ░░░░░░░░░░░░░░░░░░░░   0 / 6
Stage 5  Generalization            ░░░░░░░░░░░░░░░░░░░░   0 / 4
Stage 6  Projects & Capstone       ░░░░░░░░░░░░░░░░░░░░   0 / 3
```

*Updated with every new topic. Star this repository ⭐ to follow the journey.*

---

## The Series Roadmap

### 🧱 Stage 1 — Neurons, Layers & the Forward Pass

> *How inputs flow through weights, biases and activations to produce an output*

| # | Topic | Status | Core Concept |
|---|-------|--------|--------------|
| 01 | [Coding Neurons and Layers](./01_neurons_and_layers/README.md) | 🔲 | Weighted sum + bias · one neuron → one layer · pure Python lists |
| 02 | [NumPy and the Dot Product](./02_numpy_dot_product/README.md) | 🔲 | np.dot · vector vs matrix products · replacing Python loops |
| 03 | [Stacking Multiple Layers](./03_multiple_layers/README.md) | 🔲 | Batches of inputs · matrix transpose · layer-to-layer chaining |
| 04 | [The Dense Layer Class](./04_dense_layer_class/README.md) | 🔲 | Layer_Dense · weight & bias initialization · forward() |
| 05 | [Broadcasting and Array Summation](./05_broadcasting/README.md) | 🔲 | Broadcasting rules · axis · keepdims · bias addition across a batch |
| 06 | [Activation Functions from Scratch](./06_activation_functions/README.md) | 🔲 | Step · Linear · Sigmoid · ReLU · Softmax · exp(x − max) stability trick |
| 07 | [The Full Forward Pass (No Loss)](./07_forward_pass/README.md) | 🔲 | Dense → ReLU → Dense → Softmax · end-to-end shape trace |

---

### 📉 Stage 2 — Loss, Optimization & Calculus Foundations

> *Measuring how wrong the network is, and the mathematics needed to fix it*

| # | Topic | Status | Core Concept |
|---|-------|--------|--------------|
| 08 | [Categorical Cross-Entropy Loss](./08_cross_entropy_loss/README.md) | 🔲 | −log(ŷ_correct) · sparse vs one-hot labels · clipping log(0) · accuracy |
| 09 | [Introduction to Optimization](./09_optimization_intro/README.md) | 🔲 | Why random weight search fails · the need for a gradient |
| 10 | [Partial Derivatives and Gradients](./10_partial_derivatives/README.md) | 🔲 | ∂f/∂x · gradient vector · numerical vs analytical derivatives |
| 11 | [The Chain Rule — Backbone of Neural Networks](./11_chain_rule/README.md) | 🔲 | Composite functions · derivative of nested operations |

---

### 🔁 Stage 3 — Backpropagation

> *Deriving and coding every gradient by hand, from a single neuron to the full network*

| # | Topic | Status | Core Concept |
|---|-------|--------|--------------|
| 12 | [Backpropagation on a Single Neuron](./12_backprop_single_neuron/README.md) | 🔲 | ReLU(w·x + b) · chain rule applied to one neuron |
| 13 | [Backpropagation Through a Layer of Neurons](./13_backprop_layer/README.md) | 🔲 | dvalues · gradients for every neuron in a layer |
| 14 | [The Role of Matrices in Backpropagation](./14_matrices_in_backprop/README.md) | 🔲 | dW = Xᵀ·dvalues · dX = dvalues·Wᵀ · db = Σ over batch |
| 15 | [Input Gradients — Why We Need dinputs](./15_input_gradients/README.md) | 🔲 | Passing gradients backward to the previous layer |
| 16 | [Backpropagation Building Blocks in Python](./16_backprop_building_blocks/README.md) | 🔲 | Layer_Dense.backward() · caching inputs during forward |
| 17 | [Backpropagation Through ReLU](./17_relu_backprop/README.md) | 🔲 | Gradient mask · zero where input ≤ 0 |
| 18 | [Backpropagation Through Cross-Entropy Loss](./18_cross_entropy_backprop/README.md) | 🔲 | ∂L/∂ŷ = −y/ŷ · normalizing by sample count |
| 19 | [Combined Softmax + Cross-Entropy Backward](./19_softmax_ce_backprop/README.md) | 🔲 | ∂L/∂z = ŷ − y · faster and numerically stable |
| 20 | [The Complete Backpropagation Pipeline](./20_backprop_pipeline/README.md) | 🔲 | Chained backward() calls through every layer · no frameworks |
| 21 | [Full Forward + Backward Pass](./21_full_forward_backward/README.md) | 🔲 | Forward → loss → backward · one complete training step |

---

### ⚙️ Stage 4 — Optimizers

> *From plain gradient descent to Adam, each optimizer derived from the weakness of the one before it*

| # | Topic | Status | Core Concept |
|---|-------|--------|--------------|
| 22 | [Gradient Descent Optimizer (SGD)](./22_gradient_descent/README.md) | 🔲 | w ← w − η·∂L/∂w · learning rate · training loop |
| 23 | [Learning Rate Decay](./23_lr_decay/README.md) | 🔲 | η_t = η₀ / (1 + decay·t) · large steps early, fine steps late |
| 24 | [Momentum](./24_momentum/README.md) | 🔲 | Velocity term · escaping local minima · smoother updates |
| 25 | [AdaGrad](./25_adagrad/README.md) | 🔲 | Per-parameter learning rate · cache += g² |
| 26 | [RMSProp](./26_rmsprop/README.md) | 🔲 | Moving average of g² · fixes AdaGrad's shrinking step |
| 27 | [Adam](./27_adam/README.md) | 🔲 | Momentum + RMSProp · bias correction (1 − βᵗ) |

---

### 🛡️ Stage 5 — Generalization & Regularization

> *Making a network that works on data it has never seen*

| # | Topic | Status | Core Concept |
|---|-------|--------|--------------|
| 28 | [Testing, Generalization & Overfitting](./28_generalization_overfitting/README.md) | 🔲 | Train / validation / test split · diagnosing overfitting |
| 29 | [K-Fold Cross-Validation](./29_kfold_cv/README.md) | 🔲 | Rotating validation folds · averaged performance estimate |
| 30 | [L1 / L2 Regularization](./30_l1_l2_regularization/README.md) | 🔲 | λ·Σ\|w\| · λ·Σw² · gradient terms λ·sign(w) and 2λw |
| 31 | [Dropout Layers](./31_dropout/README.md) | 🔲 | Bernoulli mask · inverted scaling 1/(1 − p) · off at inference |

---

### 🚀 Stage 6 — Real-World Projects & Capstone

> *The from-scratch library, applied end to end on real datasets*

| # | Topic | Status | Core Concept |
|---|-------|--------|--------------|
| 32 | [Project — Fashion-MNIST Classification](./32_fashion_mnist_project/README.md) | 🔲 | 28×28 images · 10 classes · full training & evaluation pipeline |
| 33 | [Project — California Housing Regression](./33_california_housing_project/README.md) | 🔲 | Linear output · MSE loss · feature scaling · regression metrics |
| 34 | [Summary — Building, Training & Testing Neural Networks](./34_summary/README.md) | 🔲 | End-to-end recap · the complete library · lessons learned |

---

## Bridge to the LLM Series

Every component built here reappears inside the Transformer in [`llm-from-scratch`](https://github.com/shivakiran-ai/llm-from-scratch). This table maps the foundation to where it is used at scale.

| Built Here (NumPy) | Topics | Reappears in the LLM Series As |
|--------------------|--------|--------------------------------|
| Dense layer | 04 | W_Q, W_K, W_V projections and the 768 → 3072 → 768 FeedForward |
| Softmax | 06, 19 | Attention weights and next-token probabilities |
| Cross-entropy loss | 08, 18, 19 | LLM training loss and perplexity |
| Manual backpropagation | 12 – 21 | What `loss.backward()` computes automatically |
| Adam + L2 regularization | 27, 30 | AdamW — decoupled weight decay in pretraining |
| Learning rate decay | 23 | Learning rate schedules in pretraining |
| Dropout | 31 | Attention dropout and residual dropout |
| Train / validation split | 28 | Train / validation loss tracking during pretraining |

---

## Design Philosophy

Three principles guide every implementation in this series:

**1. No magic.** No autograd, no framework layers. Every derivative is worked out on paper first, then coded, then checked.

**2. The why before the what.** Each component begins with the problem it solves. Momentum exists because SGD oscillates; Adam exists because no single learning rate fits every parameter.

**3. Everything connects to the literature.** Each major component maps to the paper that introduced it.

| Paper | Relevance | Topics |
|-------|-----------|--------|
| McCulloch & Pitts (1943) — *A Logical Calculus of the Ideas Immanent in Nervous Activity* | The artificial neuron | 01 |
| Rosenblatt (1958) — *The Perceptron* | Learnable weights | 01 – 04 |
| Rumelhart, Hinton & Williams (1986) — *Learning Representations by Back-Propagating Errors* | Backpropagation | 10 – 21 |
| Nair & Hinton (2010) — *Rectified Linear Units Improve Restricted Boltzmann Machines* | ReLU | 06, 17 |
| Polyak (1964) — *Some Methods of Speeding Up the Convergence of Iteration Methods* | Momentum | 24 |
| Duchi, Hazan & Singer (2011) — *Adaptive Subgradient Methods* | AdaGrad | 25 |
| Tieleman & Hinton (2012) — *Lecture 6.5, Neural Networks for Machine Learning* | RMSProp | 26 |
| Kingma & Ba (2015) — *Adam: A Method for Stochastic Optimization* | Adam | 27 |
| Krogh & Hertz (1992) — *A Simple Weight Decay Can Improve Generalization* | L2 regularization | 30 |
| Srivastava et al. (2014) — *Dropout: A Simple Way to Prevent Neural Networks from Overfitting* | Dropout | 31 |
| Loshchilov & Hutter (2019) — *Decoupled Weight Decay Regularization* | AdamW (bridge to LLMs) | 27, 30 |
| Xiao, Rasul & Vollgraf (2017) — *Fashion-MNIST* | Project dataset | 32 |
| Pace & Barry (1997) — *Sparse Spatial Autoregressions* | California Housing dataset | 33 |

---

## Repository Structure

```
neural-networks-from-scratch/
│
├── README.md                          ← You are here
├── LICENSE
├── .gitignore
│
│   ── Stage 1 · Neurons & Forward Pass ──
├── 01_neurons_and_layers/             🔲 Next
│   ├── README.md
│   ├── Topic01_Neurons_and_Layers.docx
│   └── notebook.ipynb
├── 02_numpy_dot_product/              🔲
├── 03_multiple_layers/                🔲
├── 04_dense_layer_class/              🔲
├── 05_broadcasting/                   🔲
├── 06_activation_functions/           🔲
├── 07_forward_pass/                   🔲
│
│   ── Stage 2 · Loss & Calculus ──
├── 08_cross_entropy_loss/             🔲
├── 09_optimization_intro/             🔲
├── 10_partial_derivatives/            🔲
├── 11_chain_rule/                     🔲
│
│   ── Stage 3 · Backpropagation ──
├── 12_backprop_single_neuron/         🔲
├── 13_backprop_layer/                 🔲
├── 14_matrices_in_backprop/           🔲
├── 15_input_gradients/                🔲
├── 16_backprop_building_blocks/       🔲
├── 17_relu_backprop/                  🔲
├── 18_cross_entropy_backprop/         🔲
├── 19_softmax_ce_backprop/            🔲
├── 20_backprop_pipeline/              🔲
├── 21_full_forward_backward/          🔲
│
│   ── Stage 4 · Optimizers ──
├── 22_gradient_descent/               🔲
├── 23_lr_decay/                       🔲
├── 24_momentum/                       🔲
├── 25_adagrad/                        🔲
├── 26_rmsprop/                        🔲
├── 27_adam/                           🔲
│
│   ── Stage 5 · Generalization & Regularization ──
├── 28_generalization_overfitting/     🔲
├── 29_kfold_cv/                       🔲
├── 30_l1_l2_regularization/           🔲
├── 31_dropout/                        🔲
│
│   ── Stage 6 · Projects & Capstone ──
├── 32_fashion_mnist_project/          🔲
├── 33_california_housing_project/     🔲
├── 34_summary/                        🔲
│
│   (every topic folder follows the same 3-file structure)
│
└── data/
    └── README.md                      ← dataset download instructions
```

---

## Getting Started

```bash
# Clone the repository
git clone https://github.com/shivakiran-ai/neural-networks-from-scratch.git
cd neural-networks-from-scratch

# Install dependencies
pip install numpy matplotlib jupyter scikit-learn

# Open Topic 01
cd 01_neurons_and_layers
jupyter notebook notebook.ipynb
```

> **No GPU required** for any topic. `scikit-learn` is used only to load datasets and create splits in the projects; every model component is pure NumPy.

---

## Prerequisites

| Requirement | Level |
|-------------|-------|
| Python | Comfortable — functions, classes, list comprehensions |
| NumPy | Basic — arrays and indexing (introduced gradually from Topic 02) |
| Calculus | Helpful — derivatives; partial derivatives and the chain rule are taught in Stage 2 |
| Linear Algebra | Helpful — matrix multiplication, transpose |

> No prior deep learning knowledge is assumed. This is the starting point of the series.

---

## Related Repositories

| Repository | Description |
|------------|-------------|
| [`llm-from-scratch`](https://github.com/shivakiran-ai/llm-from-scratch) | The continuation — a GPT-2 (124M) Large Language Model built from first principles in PyTorch: tokenization, attention, architecture, pretraining and finetuning, plus an LLM systems companion series. |
| `deepseek-from-scratch` *(coming soon)* | Modern LLM architecture innovations — Multi-Head Latent Attention, Mixture-of-Experts, Multi-Token Prediction, RoPE and quantization. |

---

## About

This series is part of my preparation for PhD research in machine learning, with a focus on large language model pretraining and finetuning.

Before attention, before Transformers, before scale, there is a neuron, a loss and a gradient. Researchers who change how models are trained understand these mechanics deeply enough to question them. This series is where that understanding begins.

Every topic is documented with:

- Handwritten notes capturing the thinking process
- A complete NumPy implementation
- Connections to the original research papers
- Personal observations and insights from building each component

---

## License

This project is licensed under the MIT License — see the [LICENSE](./LICENSE) file for details.

---

<div align="center">

<br/>

*If this repository helped you understand neural networks more deeply, consider giving it a ⭐*

<br/>

**SHIVA KIRAN DADISHETTY**

*Building one component at a time. No shortcuts.*

<br/>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:2E75B6,50:1A56A0,100:0D3B6E&height=120&section=footer"/>

</div>
