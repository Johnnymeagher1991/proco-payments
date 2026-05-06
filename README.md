# procohq

**The future of finance is on-chain.**

Programmable money for builders, traders, treasuries, and the autonomous agents that come next. Wallets, payments, settlement, and treasury — open, programmable, multi-chain.

→ [procohq.com](https://procohq.com)

---

## What Proco is

Proco is the on-chain programmable money platform. Non-custodial wallets, programmable conditions (`pay_when`, `pay_if`, `sweep_when`), instant settlement on Base / Solana / Hyperliquid, and a marketplace for on-chain services.

- **Wallets** — non-custodial, multi-chain, owned by their principal (human, business, bot, or agent)
- **Programmable conditions** — `pay_when`, `pay_if`, `sweep_when` at the API level
- **Payments and settlement** — on-chain by default, transparent fees, instant USDC settlement
- **Treasury automation** — auto-rebalancing, yield routing, drawdown caps, threshold triggers
- **Catalog** — a marketplace for on-chain services any wallet can pay for
- **x402 compatible** — native support for the machine-to-machine payment protocol backed by Coinbase, Google, Anthropic, Visa, and AWS

## For developers

```bash
npm install @proco/sdk
```

```javascript
import Proco from '@proco/sdk';

const proco = new Proco({ apiKey: process.env.PROCO_KEY });

const tx = await proco.payments.create({
  amount: 100,
  currency: 'USDC',
  to: wallet.address,
  trigger: { event: 'invoice.due' }
});
// → settled in 8.2s · on-chain · transparent fees
```

## Links

- [procohq.com](https://procohq.com) — main site
- [procohq.com/protocol](https://procohq.com/protocol) — protocol docs
- [Open-source SDK](https://github.com/procohq/proco-sdk) — TypeScript client
- [Start building free](https://procohq.com/sign-in) — free sandbox, no credit card

---

The future of finance is on-chain. Proco is building the layer.
