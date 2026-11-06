---
id: scaling-ladder
title: "Scaling beyond one node"
layout: diagram
layout_rationale: "Scaling from a laptop to many nodes is a four-step sequence."
objective: obj-3
status: draft
duration: 2
section: "4. Thinking like a cloud engineer"
---

# Key message
When one node is not enough

## Talking points
- Most projects stop at one node, and that is fine
- Ray spreads Python functions across many nodes with a decorator: the HPC equivalent of a job array without a submission script
- SkyPilot's num_nodes setting starts several machines for distributed PyTorch training
- Both are covered step by step in the take-home tutorials and the Cloud Clinic recordings

## Slot: nodes
- Laptop: Prototype on a data sample
- One node: The levels you just saw
- Ray: Spread tasks across many nodes
- Multi-node: Distributed PyTorch training

## Slot: caption
Go deeper with the take-home tutorials and the Cloud Clinic recordings.
