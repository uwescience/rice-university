---
id: ray-code
title: "Ray code"
layout: code
layout_rationale: "The audience reads the few lines that turn a loop into parallel tasks."
objective: obj-3
status: draft
duration: 2
section: "4. Scaling with Ray and SkyPilot"
---

# Key message
Ray: parallelize with one decorator

## Talking points
- The function body is unchanged; the decorator makes it a remote task
- On a laptop, tasks spread over local cores
- Pointed at a Ray cluster, the same script spreads over many nodes
- HPC analogy: a job array without writing a submission script

## Slot: code
```python
import ray
ray.init()  # laptop today, cluster later
@ray.remote
def simulate(p): return run_model(p)
futures = [simulate.remote(p) for p in grid]
results = ray.get(futures)
```

## Slot: caption
On a cluster, ray.init() connects to it and the same tasks spread across nodes.

## Source
Ray documentation, docs.ray.io

## Notes
run_model and grid stand in for the researcher's own function and parameter list.
