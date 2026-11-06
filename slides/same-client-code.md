---
id: same-client-code
title: "Same client code"
layout: code
layout_rationale: "The audience reads the few lines that stay the same at every level."
objective: obj-3
status: draft
duration: 2
section: "4. Thinking like a cloud engineer"
---

# Key message
Switching levels can be a one-line change

## Talking points
- vLLM serves models through the same request format many hosted chat APIs use
- So the researcher's code does not care which level it talks to
- That is the "minimal changes to the Python you already write" promise, applied to AI
- The choice of level becomes a cost and governance decision, not a rewrite

## Slot: code
```python
from openai import OpenAI
client = OpenAI(base_url=URL, api_key=KEY)
reply = client.chat.completions.create(
    model=MODEL,
    messages=[{"role": "user", "content": q}])
```

## Slot: caption
Point URL at a hosted API or at your own vLLM server; the rest stays.

## Source
vLLM documentation, docs.vllm.ai

## Notes
URL, KEY, MODEL and q stand in for the endpoint, its key, the model name and the question.
VERIFY: not every hosted API accepts this request format natively; confirm the services used in the demo do before promising a one-line change.
