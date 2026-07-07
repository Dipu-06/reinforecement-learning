# 🧠 Cliff Walking using SARSA

A Reinforcement Learning project that implements the **SARSA (State–Action–Reward–State–Action)** algorithm using the **Gymnasium CliffWalking-v1** environment.

---

## 📌 Overview

This project demonstrates how an intelligent agent learns to navigate from the **Start** state to the **Goal** while avoiding dangerous cliff cells.

The agent learns through interaction with the environment by receiving rewards and penalties. Training is performed using the **SARSA** algorithm, an **on-policy** reinforcement learning method that updates action values based on the action actually taken.

---

## 🎯 Objectives

* Understand Reinforcement Learning concepts.
* Implement the SARSA algorithm.
* Train an agent using an ε-greedy policy.
* Learn a safe path while avoiding the cliff.
* Evaluate the learned policy after training.

---

## 🛠️ Technologies Used

* Python
* NumPy
* Gymnasium (CliffWalking-v1)

---

## 📂 Project Structure

```text
SARSA.ipynb
README.md
```

---

## 📖 SARSA Update Rule

[
Q(s,a) = Q(s,a) + \alpha \left[r + \gamma Q(s',a') - Q(s,a)\right]
]

Where:

* **Q(s,a)** = Current action-value
* **α** = Learning rate
* **γ** = Discount factor
* **r** = Reward received
* **s'** = Next state
* **a'** = Next action selected using the current policy

---

## ⚙️ Hyperparameters

| Parameter            | Value |
| -------------------- | ----: |
| Learning Rate (α)    |   0.5 |
| Discount Factor (γ)  |  0.99 |
| Exploration Rate (ε) |   0.1 |
| Training Episodes    |   500 |

---

## 🚀 Features

* SARSA implementation from scratch
* ε-greedy action selection
* Q-table based learning
* Gymnasium CliffWalking-v1 environment
* Agent training over multiple episodes
* Demonstration of the learned policy

---

## ▶️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/cliff-walking-sarsa.git
```

Navigate to the project directory:

```bash
cd cliff-walking-sarsa
```

Install the required packages:

```bash
pip install gymnasium "gymnasium[toy-text]" numpy
```

Run the notebook:

```bash
jupyter notebook SARSA.ipynb
```

---

## 📊 Results

After training:

* The agent successfully learns to avoid the cliff.
* The Q-table converges toward an effective policy.
* The learned policy guides the agent safely to the goal.
* Training demonstrates the effectiveness of the SARSA on-policy algorithm.

---

## 📚 Concepts Covered

* Reinforcement Learning
* SARSA
* On-policy Learning
* Markov Decision Process (MDP)
* Q-Table
* ε-Greedy Policy
* Exploration vs. Exploitation

---

## 🔮 Future Improvements

* Compare SARSA with Q-Learning.
* Add reward graphs for training visualization.
* Tune hyperparameters for faster convergence.
* Implement Expected SARSA.
* Extend the project to custom grid-world environments.

---


If you found this project helpful, consider giving it a ⭐ on GitHub!
