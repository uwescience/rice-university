---
id: abstraction-levels
title: "Levels of abstraction"
layout: custom
layout_rationale: "Who manages what is a stack that shifts layer by layer, so three side-by-side stacks show the hand-off at a glance where a table made the audience read every cell."
layout_intent: "Three columns (managed infrastructure, managed platform, managed service), each headed by its AI example, each a stack of the same five layers from your requests at the top to hardware and network at the bottom. Layers you manage are dark; layers the provider manages are light, so the dark part shrinks from left to right. A double arrow above runs from more control (left) to more convenience (right); a legend sits below."
locked: true
objective: obj-3
status: draft
duration: 3
section: "4. Thinking like a cloud engineer"
---

# Key message
Choose how much of the stack you manage

## Talking points
- Every cloud offers the same three levels under different product names
- Moving right, the provider takes over layer by layer: you trade control for convenience, and staff time for a higher unit price
- Researchers from HPC default to the left column because it looks like the cluster; often a column further right is the better fit
- CloudBank Classroom's JupyterHub is a platform you already met in Part 1

## Slot: stacks
Layers, top to bottom: Your requests · Code and model choice · Scaling and patching · OS and software · Hardware and network

| Level | AI example | You manage (top layers) |
|---|---|---|
| Managed infrastructure | vLLM on a GPU node | Top four; provider manages hardware and network |
| Managed platform | A managed model endpoint | Requests and code and model choice |
| Managed service | A chat API | Requests only |

## Notes
Product names to say aloud if helpful, per level: on AWS, EC2, then SageMaker, then Bedrock; on Google Cloud, Compute Engine, then Vertex AI, then the Gemini API.
VERIFY: the product-to-level mapping above is the planner's; confirm it with the Part 4 presenter, since some products span two levels.
HTML is hand-drafted (locked). Unlock and regenerate only if you want the generator to redraw it.
