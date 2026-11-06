---
id: scaling-ladder
title: "Scaling ladder"
layout: diagram
layout_rationale: "The path from laptop to multi-node training is a four-step sequence."
objective: obj-3
status: draft
duration: 2
section: "4. Scaling with Ray and SkyPilot"
---

# Key message
The same Python code at every scale

## Talking points
- Researchers resist the cloud when it means rewriting working code
- Ray parallelizes Python functions; SkyPilot provisions the machines
- Each rung changes configuration, not the science
- This maps onto what HPC users already do with job arrays and MPI

## Slot: nodes
- Laptop: Prototype on a data sample
- Ray: Parallelize functions with a decorator
- SkyPilot: Provision nodes on any cloud
- Multi-node: Distributed PyTorch training runs

## Slot: caption
Each step changes configuration, not the science code.
