---
id: three-resources
title: "Three resources"
layout: diagram
layout_rationale: "A design passes through storage, compute and network in order, one question each."
objective: obj-3
status: draft
duration: 2
section: "4. Thinking like a cloud engineer"
---

# Key message
Every cloud design starts with three resources

## Talking points
- You already think this way on the cluster: scratch versus project storage, node types, the interconnect
- In the cloud each of the three is metered separately, so each answer has a price
- Network is the one researchers forget: moving data out of the cloud is billed
- Thinking like an engineer means answering these before choosing a service

## Slot: nodes
- Storage: How much, and how often read?
- Compute: What shape, and for how long?
- Network: What moves, and how far?

## Slot: caption
Answer these before choosing a service; the cost follows from the answers.
