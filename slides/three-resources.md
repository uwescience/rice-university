---
id: three-resources
title: "Three resources"
layout: custom
layout_rationale: "Storage, compute and network are sized together, not in sequence, so an architecture sketch replaces the step chain; network is drawn as the arrow because it is the connection, not a box."
layout_intent: "A dashed box labelled 'One cloud region' holds two dark cards, Storage and Compute, joined by a two-way arrow marked 'free in-region'. A heavier accent arrow labelled Network leaves the compute card, crosses the region line and points to a light card, 'Your laptop, collaborators, the web'. Each resource shows its question and a pill naming how it is billed. On 4:3 the sketch stacks vertically."
locked: true
objective: obj-3
status: draft
duration: 2
section: "4. Thinking like a cloud engineer"
---

# Key message
Every cloud design starts with three resources

## Talking points
- You already think this way on the cluster: scratch versus project storage, node types, the interconnect
- In the cloud each of the three is metered separately, so each answer has a price
- Network is the one researchers forget: moving data within a region is usually free, moving it out of the cloud is billed
- Thinking like an engineer means answering these before choosing a service

## Slot: diagram
- Region: One cloud region
- Storage: How much, and how often read? (Billed per GB-month)
- Compute: What shape, and for how long? (Billed per hour)
- Storage ⇄ Compute: free in-region
- Network: What moves, and how far? (Billed per GB out)
- Outside: Your laptop, collaborators, the web

## Slot: caption
Answer these before choosing a service; the cost follows from the answers.

## Notes
Point at the arrow leaving the region: that is the line researchers forget. Out-of-cloud transfer is about 9 cents per GB on AWS; the costs slide comes back to it.
HTML is hand-drafted (locked). Unlock and regenerate only if you want the generator to redraw it.
