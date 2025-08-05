# 🧭 Autonomous Navigation Agents
Smart Indoor Navigation with Deep Reinforcement Learning and Modular Robotics

## Description
This project showcases a hybrid approach combining Proximal Policy Optimization (PPO) and classical robotic localization and planning techniques to train agents that autonomously navigate cluttered indoor environments. Built using the AI2-THOR simulation framework, this system lays the foundation for real-world robotic applications in homes, hospitals, warehouses, and smart environments.

🎯 Key Features
🧠 Deep Reinforcement Learning using PPO

🗺️ 3D Path Planning with A* and graph-based navigation

🧭 Particle Filter-based Localization

👁️‍🗨️ Depth-based Perception module with sensor preprocessing

🏡 Simulated environments via AI2-THOR

🛠️ Modular and extensible architecture for sim-to-real transfer

## Installation Instructions
1. Clone the repository.
2. Install the required libraries:
   ```bash
   pip install --upgrade ai2thor ai2thor-colab prior networkx pyvirtualdisplay
   ```

## 🧠 Approaches

# 1. 📘 Proximal Policy Optimization (PPO)

Train an agent end-to-end using visual observations (RGB-D) to navigate to target positions.

Trains in AI2-THOR using OpenAI Gym interface

Neural network maps image inputs to actions

Learns locomotion policies with no prior maps

# 2. 🧩 Modular Navigation Architecture (MNA)

Enhances navigation by combining classic robotics with learning:

Perception: Preprocesses depth maps (denoising, filtering)

Localization: Tracks pose via action-based updates

Planning: Graph-based A* search in 3D for waypoint generation

Policy: Learns high-level control using PPO on modular inputs

## 🎯 Objectives

Develop efficient autonomous agents for real-time indoor navigation.

Benchmark end-to-end RL vs. modular hybrid systems.

Bridge the sim-to-real gap using low-cost simulation and robust sensor models.

## Aims and Objectives
The objective of this project is to implement a robust algorithm to navigate the robot efficiently using a deep learning model, overcoming the gap between virtual and real-world environments under a low-cost budget while ensuring user safety.

## Outputs
The principal output is a trained autonomous navigation agent capable of moving through simulated indoor environments. The agent can plan and execute pathways to predetermined goals, with visualizations showing intended pathways and agent trajectories.

## 🧪 Experiments

✅ Trained agents in 50+ AI2-THOR environments

✅ Visualized planned and actual trajectories

✅ Simulated sensor noise, occlusion, pose drift

✅ Ran ablation studies to test each module’s contribution

## 🔍 Real-World Applications

🤖 Home assistant robots

🏥 Autonomous navigation in hospitals

📦 Indoor logistics and warehouse automation

🎯 Last-mile robotic delivery agents

## References
1. J. Biswas and M. V. Manuela. “Depth camera based indoor mobile robot localization and navigation”. In: Proc. Int. Conf. Robotics and Automation (ICRA). May 2012, pp. 1697–1702.
2. D. Maier, A. Hornung, and M. Bennewitz. “Real-time navigation in 3D environments based on depth camera data”. In: Proc. Int. Conf. Humanoid Robots (Humanoids). Nov. 2012, pp. 692–697.
3. Z. W. Hong et al. “Virtual-to-real: Learning to control in visual semantic segmentation”. In: Proc. Int. Joint Conf. Artificial Intelligence (IJCAI). July 2018, pp. 4912–4920.
4. H.-T. L. Chiang et al. “Learning Navigation Behaviors End to End”. In: CoRR abs/1809.10124 (2018).
5. Sim-to-Real: Virtual Guidance for Robot Navigation Supplementary Material. [Link](https://drive.google.com/open?id=1QyGCQIGFcLEPGTFeaupNKVZo2SOmrcJa). Accessed: 2020-09-30.
