---
id: genai-prompt
title: "Prompt for deployment"
layout: code
layout_rationale: "The audience reads the exact prompt that will be used in the demo."
objective: obj-3
status: draft
duration: 2
section: "3. Live demo: AI-assisted deployment"
---

# Key message
Ask for the guardrails up front

## Talking points
- Name the account route, the cloud, the region and the size
- Ask for tags and an automatic stop in the first prompt, not after the bill
- Paste errors back verbatim; do not paraphrase them

## Slot: code
```text
I have an AWS account through CloudBank.
Give me AWS CLI steps to run a Python API
on a small spot instance in us-east-1.
Tag everything project=rice-demo and stop
the instance automatically after 4 hours.
```

## Slot: caption
Assistants often skip tags and auto-stop unless you ask for them.

## Notes
VERIFY: adjust the cloud, region and instance type to match the live demo.
