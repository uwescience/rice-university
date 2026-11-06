---
id: pytorch-multinode
title: "PyTorch multi-node"
layout: diagram
layout_rationale: "The training job is a four-stage pipeline across nodes."
objective: obj-3
status: draft
duration: 3
section: "4. Scaling with Ray and SkyPilot"
---

# Key message
A PyTorch training job across cloud nodes

## Talking points
- Data and code go to object storage first, not to the nodes
- SkyPilot starts the GPU nodes and runs the same script on each
- PyTorch DistributedDataParallel keeps the model copies in sync
- Checkpoints let a preempted spot node rejoin instead of starting over

## Slot: nodes
- Stage: Data and code in a bucket
- Launch: SkyPilot starts two GPU nodes
- Train: DDP synchronizes gradients across nodes
- Wrap up: Checkpoint to storage, then autostop

## Slot: caption
Spot nodes cost about half; checkpoints let training resume after a preemption.

## Notes
Likely a short live run or a recorded one. The "about half" spot figure comes from the catalog cost slide.
