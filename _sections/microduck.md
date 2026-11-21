---
title: MicroDuck & Reinforcement Learning
nav_label: MicroDuck
slug: microduck
order: 25
status: current
show_in_nav: true
image: /assets/notebook/robot.webp
image_alt: Pencil concept study of a small two-legged robot
---

How does a biped learn to stand up, and how can we tell whether an exported policy still behaves like the one we trained?

I work on tools for training and evaluating MicroDuck locomotion policies. I replay checkpoints in MuJoCo to inspect the motion, then compare the training model with its ONNX export on the same inputs and in a short simulation rollout.

[MicroDuck: from checkpoint to motion](/projects/microduck/) · [Reinforcement learning](/projects/microduck/#training)
