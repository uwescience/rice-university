---
id: ai-three-ways
title: "AI at three levels"
layout: diagram
layout_rationale: "The same AI task run at three levels is a sequence of increasing control."
objective: obj-3
status: draft
duration: 3
section: "4. Thinking like a cloud engineer"
---

# Key message
One AI task at three levels

## Talking points
- Same task each time, for example answering questions about a set of papers
- Service: billed per request, nothing to run, but the data leaves campus
- Platform: you choose an open model and the provider runs it
- Infrastructure: vLLM serves the model on your own GPU node, and a coding agent such as OpenCode can use it, so even the assistant runs on hardware you control

## Slot: nodes
- Service: Call a hosted chat API
- Platform: Deploy to a managed endpoint
- Infrastructure: vLLM on your GPU node

## Slot: caption
Same task each time: more control and more responsibility at every step.

## Notes
Live demo: run the task once at each level, and say out loud what changed each time (cost model, who patches, where the data goes).
VERIFY: confirm the demo model, the managed platform used, and that OpenCode can be pointed at the vLLM endpoint in the version you demo.
