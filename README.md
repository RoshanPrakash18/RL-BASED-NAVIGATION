# 🧭 Autonomous Navigation Agents
> *Smart Indoor Navigation using Reinforcement Learning and Modular Robotics*

This repository presents an advanced indoor navigation system leveraging **deep reinforcement learning (DRL)** and **modular classical robotics**, trained in high-fidelity 3D simulations. The agent is capable of navigating complex indoor environments — a critical milestone for **embodied AI**, **robotics**, and **autonomous systems**.

> Developed using the [AI2-THOR](https://ai2thor.allenai.org/) framework, this research contributes to **sim-to-real transfer learning**, **sensor fusion**, and **intelligent planning**, pushing the frontier of robot navigation for real-world deployment.

---

## 🚀 Key Features

- 🧠 **Proximal Policy Optimization (PPO)** for continuous visuomotor control.
- 🗺️ **3D Path Planning** using A* search and NetworkX-based graph modeling.
- 🧭 **Particle Filter Localization** for robust pose tracking.
- 👁️‍🗨️ **Depth-Based Perception Module** with obstacle segmentation.
- 🏠 Realistic indoor simulation via **AI2-THOR**.
- 🔁 Modular design enabling flexible sim-to-real integration.

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/Autonomous-Navigation-Agents.git
cd Autonomous-Navigation-Agents
pip install --upgrade ai2thor ai2thor-colab prior networkx pyvirtualdisplay
```

## 🧠 Learning Approaches

### 1. 📘 PPO-Based Visuomotor Control
- End-to-end training using RGB-D inputs.  
- Trained in randomized start/goal environments.  
- Learns raw visual input to action mappings.  
- Goal-oriented, reward-optimized behavior.

### 2. 🧩 Modular Navigation Architecture
A high-level hybrid system integrating:
- **Perception** → Processes raw depth into spatial features.  
- **Localization** → Estimates pose using motion updates.  
- **Planning** → Graph-based A* pathfinder.  
- **Policy** → High-level PPO agent using structured state input.

---

## 🎯 Project Objectives
- Design efficient navigation agents using DRL.  
- Benchmark end-to-end RL vs hybrid modular systems.  
- Enable real-world deployment through robust sim-based training.  
- Contribute to generalizable models for indoor robotics.

---

## 🖼️ Visual Results

| PPO Learning Curve        | Modular Architecture Trajectory |
|---------------------------|----------------------------------|
| ![ppo_curve](images/ppo_curve.png) | ![modular_path](images/modular_path.png) |

---

## 📊 Evaluation

| Metric               | PPO Only | Modular Architecture |
|----------------------|----------|-----------------------|
| Convergence Speed    | Moderate | 🔼 Fast               |
| Goal Proximity       | 0.2 m    | 🔼 0.05 m             |
| Scene Generalization | Medium   | 🔼 High               |
| Robustness to Noise  | Low      | 🔼 High               |

> 🏆 **Modular design achieved 25% better goal accuracy and faster convergence across all test scenes.**

---

## 🧪 Experiments

- ✅ Trained agents in 50+ AI2-THOR house layouts.  
- ✅ Robust visualizations: PPO trajectories, planned paths, depth maps.  
- ✅ Simulated environmental noise, occlusions, and sensor drift.  
- ✅ Conducted ablation studies to validate modular contributions.

---

## 🛠 Real-World Applications

- 🤖 Assistive robots for elderly care and home automation.  
- 🏥 Hospital navigation in complex, crowded indoor spaces.  
- 📦 Autonomous inventory robots in warehouse logistics.  
- 📬 Last-mile delivery agents for office and retail spaces.

---

## 🧬 Research Impact

This work contributes to:
- Scalable **embodied navigation** via DRL in realistic simulations.  
- Fusion of **SLAM-inspired localization** with deep policies.  
- Advancing **low-cost sim-to-real pipelines** for robotics.  
- Reinforcement of **sample efficiency** through structured representations.

---

## 📚 References

1. J. Biswas, M. M. Veloso. *“Depth Camera Based Indoor Mobile Robot Navigation”*. ICRA, 2012.  
2. D. Maier et al. *“Real-Time Navigation in 3D Environments”*. Humanoids, 2012.  
3. Z. Hong et al. *“Virtual-to-Real Learning for Visual Control”*. IJCAI, 2018.  
4. H.-T. L. Chiang et al. *“Learning Navigation Behaviors End-to-End”*. CoRR abs/1809.10124.  
5. [Sim-to-Real: Google Drive Supplement](https://drive.google.com/open?id=1QyGCQIGFcLEPGTFeaupNKVZo2SOmrcJa)

---

## 🔗 Connect

📧 codetoroshan@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/roshanprakash)
