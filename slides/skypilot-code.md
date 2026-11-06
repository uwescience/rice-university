---
id: skypilot-code
title: "SkyPilot serving vLLM"
layout: code
layout_rationale: "The audience reads the short task file that launches the infrastructure-level demo."
objective: obj-3
status: draft
duration: 2
section: "4. Thinking like a cloud engineer"
---

# Key message
SkyPilot: describe the job, not the servers

## Talking points
- SkyPilot makes the infrastructure level feel almost like a platform
- One file names the GPU, the setup and the command; SkyPilot finds a cloud and region with capacity
- It works with the accounts CloudBank opens for the researcher
- Set autostop at launch, and never open the port without an API key (Part 5)

## Slot: code
```yaml
resources:
  accelerators: A10G:1
  ports: 8000
setup: pip install vllm
run: vllm serve $MODEL --port 8000
```

## Slot: caption
sky launch finds an A10G, installs vLLM and serves the model on port 8000.

## Source
SkyPilot documentation, docs.skypilot.co

## Notes
MODEL is passed at launch (sky launch --env MODEL=...). In the live run, add --api-key to the vllm serve command and an autostop setting; they are left off the slide for space.
VERIFY: check the YAML keys against the SkyPilot version used, that the chosen model fits on one A10G, and the docs URL.
