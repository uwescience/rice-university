---
id: abstraction-levels
title: "Levels of abstraction"
layout: custom
layout_rationale: "Three levels compared on who manages what form a table, which no layout offers."
layout_intent: "A table with three rows (managed infrastructure, managed platform, managed service) and four columns (level, you manage, provider manages, AI example), with a side arrow running from more control at the top to more convenience at the bottom."
objective: obj-3
status: draft
duration: 3
section: "4. Thinking like a cloud engineer"
---

# Key message
Choose how much of the stack you manage

## Talking points
- Every cloud offers the same three levels under different product names
- Going down the table, you trade control for convenience, and staff time for a higher unit price
- Researchers from HPC default to the top row because it looks like the cluster; often a lower row is the better fit
- CloudBank Classroom's JupyterHub is a platform you already met in Part 1

## Slot: table
| Level | You manage | Provider manages | AI example |
|---|---|---|---|
| Managed infrastructure | OS, software, scaling | Hardware and network | vLLM on a GPU node |
| Managed platform | Your code and model choice | Servers, scaling, patching | A managed model endpoint |
| Managed service | Your requests | Everything else | A chat API |

## Notes
Product names to say aloud if helpful, per level: on AWS, EC2, then SageMaker, then Bedrock; on Google Cloud, Compute Engine, then Vertex AI, then the Gemini API.
VERIFY: the product-to-level mapping above is the planner's; confirm it with the Part 4 presenter, since some products span two levels.
