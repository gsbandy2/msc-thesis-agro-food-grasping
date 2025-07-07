# Learning Pushing and Grasping for Agro-Food Clutter Clearance

This project, developed as part of Gregory Bandy’s MSc Thesis in Biosystems Engineering, explores how deep reinforcement learning can be applied to robotic manipulation tasks in agro-food processing environments. The work builds upon and extends the open-source Visual Pushing for Grasping (VPG) framework from [andyzeng/visual-pushing-grasping](https://github.com/andyzeng/visual-pushing-grasping) with feature engineering modifications and a systematic investigation of pushing rewards, training regimens, and object generalization.

---

## Project Overview

### Thesis Title
**Learning Pushing and Grasping for Agro-Food Clutter Clearance: An Exploration of Deep Reinforcement Learning for Food Manipulation**

### Key Goals
- Develop and evaluate a deep reinforcement learning system capable of pushing and grasping agro-food objects in cluttered environments.
- Investigate the effect of pushing rewards and training object diversity on performance.
- Adapt and extend the original VPG method to focus on agro-food bin picking.
- Explore trade-offs between specialization and generalization in training object sets.

---

## Key Contributions
- **Reward System Tweaks:** Explored the impact of removing pushing rewards and modifying success thresholds.
- **Training Object Variations:** Investigated how training on agro-food-like objects (crop shapes) affects agent performance.
- **Agro-Food Variant (AFV) Agent:** Developed a tuned variant that significantly improved completion rates in agro-food clutter scenarios.
- **Benchmark Comparisons:** Tested performance on block adversarial cases, crop adversarial cases, and real-world clutter simulations.

---

## Repository Structure

- `MScThesis_GregoryBandy.pdf` – Full MSc thesis report, including methodology, results, and discussion.
- `Final_Seminar_GregoryBandy.pdf`
- `README.md` – Project documentation.
- Codebase:
  - Reference to the forked repository: [andyzeng/visual-pushing-grasping](https://github.com/andyzeng/visual-pushing-grasping)
  - Modifications to feature engineering, reward functions, and training regimens are described in the thesis.

---

## Method Summary
- **Base Framework:** Visual Pushing for Grasping (VPG) by Zeng et al.
- **Simulated Environment:** CoppeliaSim with a UR5 robot and RG2 gripper.
- **Learning Approach:** Deep Q-Learning using fully convolutional networks (FCNs).
- **Motion Primitives:** Combined top-down grasping and planar pushing.

---

## Limitations
- Full hardware integration was not possible due to firmware incompatibilities with modern UR5 cobots.
- Experiments were limited to simulation using CoppeliaSim.

---

## Future Work
- Port the system to updated robot firmware.
- Develop modular code for easier integration of 6-DoF grasping and multi-modal rewards.
- Extend to real-world agro-food objects with deformable properties.
- Investigate adding masking functions or additional motion primitives as described in recent literature.

---

## How to Use
1. Fork the original [Visual Pushing for Grasping repository](https://github.com/andyzeng/visual-pushing-grasping).
2. Apply the reward system changes and training object configurations as described in the thesis.
3. Run the training and evaluation pipelines using CoppeliaSim as the simulation backend.
4. Refer to the provided thesis for detailed experiment setups and hyperparameters.

---

## Acknowledgments
This work was completed under the supervision of Dr. Rekha Raja PhD, Dr. Ali Leylavi Shoushatari, and Dr. Gert Kootstra at Wageningen University & Research, Farm Technology Group.

---

If you would like to contribute or further develop this project for real-world agro-food manipulation, please feel free to fork and build upon this repository.
