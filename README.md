---
name: portal-agent-payments
description: >
  Charge 0.1 SOL for portal access. Verify payments and trigger 40% buyback.
metadata:
  author: One Dev
  version: "1.0"
---

## Configuration
- Agent Mint: 5J5xLoDeC9Rk6boeoYhnYDA52zMk2cfbygLsxkLUpump
- Currency: SOL (Smallest unit: 100000000)
- Buyback: 40% to burn address

## Logic
1. Build payment instruction for 0.1 SOL.
2. Use @pump-fun/agent-payments-sdk to validate.
3. Upon success, deliver portal RNG and trigger buyback.
