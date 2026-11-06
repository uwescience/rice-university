---
id: hpc-vs-cloud
title: "HPC and cloud"
layout: comparison
layout_rationale: "Maps what the audience already knows (the cluster) to the cloud, as two equal columns."
objective: obj-1
status: draft
duration: 2
section: "1. Cloud and CloudBank"
---

# Key message
Your cluster and the cloud work together

## Talking points
- You already know the hard part: scheduling, storage tiers, software environments
- The cloud trades a shared queue for a bill. That changes who has to watch costs.
- Tightly coupled MPI work usually still belongs on the cluster
- The cloud wins on elasticity, special hardware and services you cannot run on campus

## Slot: left
### HPC cluster
- Shared queue, fixed hardware
- Free at point of use
- Tuned for tightly coupled MPI
- Admins manage the software

## Slot: right
### Commercial cloud
- On demand, any hardware
- Pay per hour used
- Managed services and APIs
- Researcher controls the stack

## Notes
VERIFY: "Free at point of use" assumes Rice's research computing clusters do not charge researchers per core-hour; confirm with Rice's Center for Research Computing.
