# Project Title

## Description
The project is a daring endeavor at the intersection of robotics and artificial intelligence. Its goal is to equip machines, such as service robots, to autonomously navigate through complex indoor environments, just as humans do. The project scope leaps forward in the field of advanced machine learning for applications ranging from smart homes to industrial automation.

The project leverages reinforcement learning (RL), inspired by biological psychology, where an agent maximizes the sum of reward signals by making actions in an environment. This is achieved through the simulation of sensor measurements, enabling intelligent navigational decisions similar to human spatial awareness.

The key contribution of this project is the comprehensive navigation system that merges RL and localization techniques to autonomously navigate indoor spaces. The Proximal Policy Optimization (PPO) algorithm implemented using the PyTorch framework optimizes policies to make informed movements based on the environment’s feedback.

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
