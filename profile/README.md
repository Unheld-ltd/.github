# Unheld

**Unheld is a non-custodial crypto payment gateway that lets merchants accept BTC, ETH, USDC, USDT, POL, and BNB across supported networks — paid directly to wallets only the merchant controls, with flat subscription pricing and no percentage fees — through a no-code dashboard, shareable payment links, and a REST API.**

[unheld.io](https://unheld.io) · [Pricing](https://unheld.io/pricing/) · [Developers](https://unheld.io/developers/) · [Security](https://unheld.io/security/)

---

## What "non-custodial" means here

The merchant generates their own wallet in their own browser. **The recovery phrase is never sent to us and we have never stored one.** Payments are detected on-chain and settle to addresses derived from that wallet, so there is no platform balance, no withdrawal step, and no payout schedule.

The practical consequence, stated plainly: if this company disappeared tomorrow, every merchant would still control every payment ever made to them. The worst case is that they stop being able to create new invoices.

## What it does

- **Invoices with real states** — detected and confirmed are separate events, because they are separate facts. Underpayment and overpayment are accounted for rather than rounded away.
- **A fresh address per invoice**, so a payment identifies itself instead of arriving in a shared wallet that has to be reconciled by amount.
- **Per-customer deposit addresses** for platforms that need to attribute funds to an end user.
- **Signed webhooks** with retries — `invoice.created`, `invoice.receiving`, `invoice.confirming`, `invoice.paid`, `invoice.underpaid`, `invoice.overpaid`, `invoice.expired`.
- **Recurring billing** without a card on file.
- **Flat subscription pricing.** We take **0%** of any payment. Network fees are paid on-chain by the payer and are not ours.

## Live networks

| Network | Assets |
|---|---|
| Bitcoin Mainnet | BTC |
| Ethereum Mainnet | ETH, USDC, USDT |
| Base | ETH, USDC |
| Polygon PoS | POL, USDC |
| BNB Chain | BNB, USDT |
| Lisk | ETH |
| Tron | TRX, USDT |
| Solana | SOL, USDC, USDT |
| XRP Ledger | XRP |

Testnets: Ethereum Sepolia (ETH, USDC), Base Sepolia (ETH, USDC), Polygon Amoy (POL, USDC), BNB Chain Testnet (BNB), Bitcoin Signet (BTC), and Bitcoin Testnet (BTC).

See the maintained public catalogue at [unheld.io/supported-networks](https://unheld.io/supported-networks/) and [unheld.io/supported-currencies](https://unheld.io/supported-currencies/).

## Status

[Try Unheld for free](https://app.unheld.io/register). This organization hosts focused public artefacts including the OpenAPI description, webhook signature-verification examples, and integration samples. The application itself is not open source.

## Contact

- General and support — **support@unheld.io**
- Security and abuse — **abuse@unheld.io** ([security.txt](https://unheld.io/.well-known/security.txt))

Availability depends on applicable law and our [terms](https://unheld.io/terms/).
