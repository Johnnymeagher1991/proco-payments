# procohq

Financial infrastructure for AI agents.

Agent wallets. Programmable spending. x402-native. Built for developers.

→ [procohq.com](https://procohq.com)

---

## Overview

Proco is the financial infrastructure layer for AI agents — giving every agent its own wallet, spend policy, and audit trail.

```bash
npm install @proco/sdk
```

```javascript
import Proco from '@proco/sdk';

const proco = new Proco({ apiKey: process.env.PROCO_KEY });

const tx = await proco.payments.create({
  amount: 100,
  currency: 'USDC',
  to: agent.walletAddress,
  trigger: { event: 'task.completed' }
});
// → settled in 8.2s · no approval needed
```

## What's in this repo

- `/sdk` — Proco SDK (coming soon)
- - `/examples` — LangChain integration, x402 demo, AI hedge fund agent demo (coming soon)
 
  - ## Links
 
  - - [procohq.com](https://procohq.com) — main site
    - - [procohq.com/protocol](https://procohq.com/protocol) — protocol docs
      - - [Start building free](https://procohq.com/sign-in) — free sandbox, no credit card
