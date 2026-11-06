---
id: llm-hpc-vs-cloud
title: "LLMs: cluster or cloud"
layout: custom
layout_rationale: "Three LLM tasks compared across cluster, cloud and risks form a table, which no layout offers."
layout_intent: "A four-column table (LLM task, cluster, cloud, watch out for) with three rows, the task column bold."
objective: obj-2
status: draft
duration: 2
section: "2. Flowchart"
---

# Key message
Where LLM work runs best depends on the task

## Talking points
- When researchers talk about LLMs, they mean one of three jobs.
- Calling a hosted model needs no GPUs at all. It is a service billed per use, and CloudBank dollars can pay for model access
- Running an open model: batch jobs suit cluster GPUs, but a service that is always on suits the cloud
- Large training runs need GPUs that sync constantly over fast networks, which is big-cluster territory; Part 2 covers where researchers can get that capacity

## Slot: table
| LLM task | Cluster | Cloud | Watch out for |
|---|---|---|---|
| Call a hosted model | Not needed | API, billed per use | Data leaves campus |
| Run an open model | Good for batch jobs | Good for always-on services | GPU queues and quotas |
| Fine-tune or train | Best for large runs | Good for small fine-tunes | GPU hours add up fast |

## Notes
The data question is the advocacy point for IT: sending prompts to a hosted API sends data off campus, which matters for student records, health data and data-use agreements.
VERIFY: whether Rice has an institutional agreement with any model provider, and what data it allows.
VERIFY: "Best for large runs" assumes researchers can get large GPU capacity on campus or through a national program; adjust if not.