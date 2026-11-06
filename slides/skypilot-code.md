---
id: skypilot-code
title: "SkyPilot code"
layout: code
layout_rationale: "The audience reads the short task file that provisions cloud nodes."
objective: obj-3
status: draft
duration: 2
section: "4. Scaling with Ray and SkyPilot"
---

# Key message
SkyPilot: describe the job, not the servers

## Talking points
- One YAML file names the hardware, the setup and the command
- SkyPilot finds a cloud and region with capacity and launches the nodes
- Spot instances and autostop are settings, not extra scripts
- It works with the accounts CloudBank opens for the researcher

## Slot: code
```yaml
resources:
  accelerators: A10G:1
  use_spot: true
num_nodes: 2
setup: pip install -r requirements.txt
run: python train.py
```

## Slot: caption
sky launch picks a cloud and region with capacity; autostop stops idle clusters.

## Source
SkyPilot documentation, docs.skypilot.co

## Notes
For the real multi-node run, the run line becomes a torchrun command that reads SkyPilot's node-rank and node-IP environment variables; show it in the demo, not on the slide.
VERIFY: check the YAML keys, the docs URL and that SkyPilot works with CloudBank-provisioned accounts as described.
