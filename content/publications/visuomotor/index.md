---
title: 'Visuomotor Robotic Pruning in Planar Orchards Using Hybrid Reinforcement Learning'

authors:
  - me
  - 'Cindy Grimm'
  - 'Stefan Lee'

date: '2026-09-01T00:00:00Z'

publication_types: ['article-journal']

publication: '*IEEE Transactions on Field Robotics*, Special Issue on Precision Agriculture and Forestry'

abstract: 'Dormant tree pruning is labor-intensive yet essential for maintaining modern high-productivity fruit orchards. In this work, we focus on pruning of modern planar tree training systems—V-Trellis apples and UFO cherries—where trunks and primary branches are trained into approximately planar walls. We introduce an end-to-end pipeline to learn a closed-loop visuomotor controller for robotic pruning. This controller is trained entirely using simulation and synthetically generated data and deployed in real orchards in a zero-shot manner. The pipeline comprises synthetic generation of planar orchard tree meshes, construction of a physics-based orchard simulator, automated collection of successful pruning trajectories via motion planning, and policy learning with a novel hybrid reinforcement-learning algorithm (Hybrid-PPO) that combines offline demonstrations with online simulated rollouts. The controller uses optical-flow inputs from a wrist-mounted camera—avoiding the need for full 3D-reconstruction—and continuously guides the cutter through cluttered branch environments to a specified cutpoint with correct tool orientation. In exhaustive simulated task-space evaluations over 3,000 pruning points, the policy attains 49.9% success on V-Trellis apples and 46.0% on UFO cherries. We validate the learned controller across 38 physical trials—comprising 28 outdoor field trials in commercial and experimental orchards and 10 indoor laboratory tests—demonstrating zero-shot sim-to-real transfer. The learned policy also outperforms a classical RRT-Connect baseline on physical hardware in laboratory trials.'

featured: true

tags:
  - Precision Agriculture
  - Field Robots
  - Robot Vision Systems
  - Robot Learning
  - Deep Reinforcement Learning
  - Sim-to-Real Transfer

# Standard identifiers for auto-linking
hugoblox:
  ids:
    doi: '10.48550/arXiv.2609.24906'

links:
  - type: preprint
    name: arXiv
    url: 'https://arxiv.org/abs/2609.24906'
  - type: pdf
    url: 'https://arxiv.org/pdf/2609.24906'
  - type: video
    url: 'https://www.youtube.com/watch?v=AjlBe6A0xdo'

# Featured image
# Ensure your graphical abstract is named `featured.jpg` or `featured.png` in this folder
image:
  caption: 'A UR5e robotic arm with a custom pruning tool on a Farm-NG Amiga platform performing zero-shot sim-to-real pruning in a real V-Trellis apple orchard.'
  focal_point: 'Center'
  preview_only: false

---

## Watch the Demo

See the visuomotor policy achieving zero-shot sim-to-real transfer in real commercial and experimental orchards:

{{< youtube AjlBe6A0xdo >}}

## Abstract

Dormant tree pruning is labor-intensive yet essential for maintaining modern high-productivity fruit orchards. In this work, we focus on pruning of modern planar tree training systems—V-Trellis apples and UFO cherries—where trunks and primary branches are trained into approximately planar walls. We introduce an **end-to-end pipeline** to learn a closed-loop visuomotor controller for robotic pruning, trained entirely in simulation and deployed in real orchards **zero-shot**.

Key contributions:
- **Novel orchard simulator**: Physics-based PyBullet environment with synthetically generated planar orchard tree meshes (Tree-L-Py)
- **Automated demonstration generation**: Motion planning pipeline (RRT-Connect) to collect successful pruning trajectories as offline data
- **Hybrid-PPO**: A novel hybrid reinforcement-learning algorithm combining offline expert demonstrations with online PPO rollouts
- **Optical-flow perception**: Avoids 3D reconstruction; wrist-mounted camera optical flow enables strong sim-to-real generalization
- **Real-world validation**: 38 physical trials (28 outdoor field trials in commercial orchards + 10 indoor lab tests) with zero-shot sim-to-real transfer; outperforms RRT-Connect baseline on hardware

**Simulation results**: 49.9% success on V-Trellis apples and 46.0% on UFO cherries (3,000 cutpoints). **Real-world results**: 71% success on V-Trellis apples in outdoor commercial orchards.
