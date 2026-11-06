---
id: wrong-service
title: "Cluster vs cloud habits"
layout: comparison
layout_rationale: "Old habit versus cloud habit is a two-sided contrast."
objective: obj-4
status: draft
duration: 2
section: "5. Common pitfalls"
---

# Key message
Bring cloud habits, not cluster habits

## Talking points
- The commonest mistake is treating the cloud as a rented cluster node
- Object storage is cheap; moving data out of the cloud is not
- Managed services often replace a VM someone has to patch
- The cloud rewards launching, finishing and shutting down

## Slot: left
### Cluster habit
- One big machine for everything
- Shared filesystem holds all data
- Copy results back home
- Queue jobs and wait

## Slot: right
### Cloud habit
- Right-size, or use managed services
- Object storage with lifecycle rules
- Analyze in the same region
- Launch, finish, shut down
