---
id: key-safety
title: "Access key safety"
layout: two-column
layout_rationale: "A set of practices with one aside on what to do after a leak."
objective: obj-4
status: draft
duration: 3
section: "5. Common pitfalls"
---

# Key message
Keep access keys out of code

## Talking points
- A key pushed to a public repository can be found and abused within hours
- The cheapest fix is never to create long-lived keys at all
- IT can make the safe path the default when helping set up a project
- Have an incident plan before you need one

## Slot: main
- Automated scanners search public repositories for keys
- Prefer SSO and short-lived credentials
- Require MFA on every human login
- Delete keys nobody is using

## Slot: side
### If one leaks
Deactivate the key, look for unexpected resources, check the bill, and tell CloudBank support right away.

## Notes
VERIFY: "found and abused within hours" is general knowledge, not from the provided sources. Confirm CloudBank's procedure for a compromised key and whether help@cloudbank.org is the right first contact.
