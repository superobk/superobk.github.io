---
title: Research Notes
nav_label: News
slug: news
order: 40
status: current
show_in_nav: true
image: ""
image_alt: ""
---

### November 2026 · From checkpoint to motion

My recent MicroDuck work brings training recipes, checkpoints and simulation playback into one console. Standing and sit-to-stand tasks give me a simple way to inspect what a policy does at the start of a rollout and how its posture evolves.

I keep the export checks and the robot checks separate. Matching actions between the training model and ONNX checks the conversion. Replaying a policy tests its behaviour in simulation. Sensor calibration and joint checks on the robot establish the starting conditions for a later hardware trial.
