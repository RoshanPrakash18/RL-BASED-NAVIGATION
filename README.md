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

## Approach 1: PPO
This approach implements the Proximal Policy Optimization (PPO) algorithm for training an agent to navigate through indoor environments. The agent learns to make decisions based on the state of the environment and optimizes its policy using reinforcement learning techniques.

## Approach 2: MNA
This approach focuses on the implementation of a 3D path planner and localization techniques to enhance the navigation capabilities of the agent. It utilizes depth images and a perception module to process sensor data and make informed navigation decisions.

## Aims and Objectives
The objective of this project is to implement a robust algorithm to navigate the robot efficiently using a deep learning model, overcoming the gap between virtual and real-world environments under a low-cost budget while ensuring user safety.

## Outputs
The principal output is a trained autonomous navigation agent capable of moving through simulated indoor environments. The agent can plan and execute pathways to predetermined goals, with visualizations showing intended pathways and agent trajectories.

## Evaluation
The project has successfully integrated AI2-THOR for modeling intelligent navigation settings and developed a PPO agent capable of learning and optimizing strategies for complex navigation settings.

## References
1. J. Biswas and M. V. Manuela. “Depth camera based indoor mobile robot localization and navigation”. In: Proc. Int. Conf. Robotics and Automation (ICRA). May 2012, pp. 1697–1702.
2. D. Maier, A. Hornung, and M. Bennewitz. “Real-time navigation in 3D environments based on depth camera data”. In: Proc. Int. Conf. Humanoid Robots (Humanoids). Nov. 2012, pp. 692–697.
3. Z. W. Hong et al. “Virtual-to-real: Learning to control in visual semantic segmentation”. In: Proc. Int. Joint Conf. Artificial Intelligence (IJCAI). July 2018, pp. 4912–4920.
4. H.-T. L. Chiang et al. “Learning Navigation Behaviors End to End”. In: CoRR abs/1809.10124 (2018).
5. Sim-to-Real: Virtual Guidance for Robot Navigation Supplementary Material. [Link](https://drive.google.com/open?id=1QyGCQIGFcLEPGTFeaupNKVZo2SOmrcJa). Accessed: 2020-09-30.
