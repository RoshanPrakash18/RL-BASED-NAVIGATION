<h1 align="center">🧭 Autonomous Navigation Agents</h1>
<h3 align="center">Smart Indoor Navigation using Reinforcement Learning & Modular Robotics</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Embodied_AI-Robotic_Navigation-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Reinforcement_Learning-PPO-ff69b4?style=for-the-badge" />
  <img src="https://img.shields.io/badge/AI2--THOR-3D_Simulation-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Planner-A*_Search-lightgrey?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Localization-Particle_Filter-brightgreen?style=for-the-badge" />
</p>

---

## 🚀 Overview

This repository implements an **autonomous indoor navigation system** combining **deep reinforcement learning (DRL)** and **classical modular robotics**, trained entirely within the high-fidelity [AI2-THOR](https://ai2thor.allenai.org/) simulator.

> ⚙️ From perception to planning to control, the agent integrates **depth sensing**, **pose tracking**, and **goal-directed pathfinding** in cluttered indoor environments.

<p align="center">
  <img src="images/system_architecture.png" width="800px" alt="Architecture Overview"/>
</p>

---

## 🧠 Learning Approaches

### 📘 PPO-Based Visuomotor Control
- End-to-end agent trained via **Proximal Policy Optimization**.
- Learns visuomotor mappings directly from **RGB-D inputs**.
- Goal-driven behaviors optimized using **reward shaping**.

### 🧩 Modular Navigation Architecture

| Module         | Role                               | Technology                 |
|----------------|------------------------------------|----------------------------|
| `perception.py`| Depth map → obstacle segmentation  | OpenCV + NumPy             |
| `localization.py`| Pose estimation via motion model | Particle Filter + Noisy Odometry |
| `planner.py`   | Path planning in navigable graph   | A* + NetworkX              |
| `policy_network/`| Action selection + DRL agent     | PyTorch PPO                |

<p align="center">
  <img src="images/modular_pipeline.png" width="750px" alt="Modular Pipeline"/>
</p>

---

## ⚡ Key Features

- 🔁 **Hybrid architecture** combining DRL with classical robotics.
- 🗺️ **A\* Graph-Based Planning** using a topological layout of navigable nodes.
- 🧠 **Policy Network** using PPO with LSTM-based memory.
- 👁️‍🗨️ **Obstacle Detection** from depth inputs using CV + morphology.
- 🧭 **Robust Localization** via particle filters with motion and perception updates.
- 🧪 **Benchmarking framework** for reproducible experiments and ablations.

---

## 📊 Evaluation Results

| Metric               | PPO Only | Modular Hybrid |
|----------------------|----------|----------------|
| 🚀 Convergence Speed | Medium   | **Fast**       |
| 🎯 Goal Accuracy     | 78%      | **95%**        |
| 🧩 Scene Generalization | Medium   | **High**       |
| 🔊 Robustness to Noise | Low      | **High**       |

> ✅ Modular design improves **goal proximity by 25%** and convergence speed across 50+ test scenes.

<p align="center">
  <img src="images/ppo_curve.png" width="45%" />
  <img src="images/modular_path.png" width="45%" />
</p>

---

## 🧪 Experiments

- ✅ Trained agents in **50+ houses** across AI2-THOR scenes.
- ✅ Injected **sensor noise**, **depth occlusions**, and **pose drift**.
- ✅ Conducted **ablation studies** on perception, localization, and planner modules.
- ✅ Visualized rollouts and **trajectory overlays** for DRL vs Modular agents.

---

## 🔧 Installation

```bash
git clone https://github.com/yourusername/Autonomous-Navigation-Agents.git
cd Autonomous-Navigation-Agents
pip install --upgrade ai2thor ai2thor-colab prior networkx pyvirtualdisplay
```

---

## 🛠️ Real-World Applications

<table>
<tr>
  <td>🤖</td>
  <td><strong>Elder Care Robots</strong><br>Assistive navigation for aging-in-place and home automation.</td>
</tr>
<tr>
  <td>🏥</td>
  <td><strong>Hospital Delivery Agents</strong><br>Navigate dynamic, cluttered hospital corridors for contactless transport.</td>
</tr>
<tr>
  <td>📦</td>
  <td><strong>Warehouse Bots</strong><br>Efficient inventory movement with optimized paths and real-time re-planning.</td>
</tr>
<tr>
  <td>📬</td>
  <td><strong>Indoor Delivery</strong><br>Smart navigation for offices, hotels, malls, and indoor logistics.</td>
</tr>
</table>

---

## 🔬 Research Contributions

> **This project accelerates research at the intersection of AI, robotics, and sim-to-real learning.**

| 🧠 Focus Area               | 🎯 Contribution                                                                 |
|----------------------------|---------------------------------------------------------------------------------|
| 🚶‍♂️ Embodied AI            | Visual + proprioceptive agents trained in 3D environments                        |
| 🧭 Sim-to-Real Transfer     | Modular pipeline fusing DRL with classical robotics                             |
| 📉 Sample Efficiency        | Structured state representation → faster convergence, fewer episodes            |
| 🛠️ Hybrid Architectures     | DRL policy enhanced with SLAM-inspired localization and classical planning       |

---

## 📚 References
J. Biswas, M. M. Veloso. “Depth Camera Based Indoor Mobile Robot Navigation”. ICRA, 2012.

D. Maier et al. “Real-Time Navigation in 3D Environments”. Humanoids, 2012.

Z. Hong et al. “Virtual-to-Real Learning for Visual Control”. IJCAI, 2018.

H.-T. L. Chiang et al. “Learning Navigation Behaviors End-to-End”. CoRR abs/1809.10124.

📎 Sim-to-Real Supplement (Google Drive)

📬 Contact & Collaboration
<p align="center"> <a href="mailto:codetoroshan@gmail.com"> <img src="https://img.shields.io/badge/Email-codetoroshan@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" /> </a> <a href="https://www.linkedin.com/in/roshanprakash/"> <img src="https://img.shields.io/badge/LinkedIn-Roshan%20Prakash-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /> </a> <a href="https://roshanprakash.vercel.app/"> <img src="https://img.shields.io/badge/Portfolio-roshanprakash.vercel.app-121212?style=for-the-badge&logo=vercel&logoColor=white" /> </a> </p>



