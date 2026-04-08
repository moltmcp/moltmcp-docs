# moltmcp-docs

> Official documentation for MoltMCP — autonomous AI agent payments on the Machine Payments Protocol.

[![Docs](https://img.shields.io/badge/docs-moltmcp.dev-8b5cf6)](https://docs.moltmcp.dev)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

---

## Documentation Structure

```
docs/
├── concepts/
│   ├── mpp-protocol.md          # What is MPP and HTTP 402
│   ├── base-settlement.md       # How on-chain escrow works on Base
│   └── agent-integration.md     # Autonomous payment workflows
├── guides/
│   ├── typescript-sdk.md        # Full TypeScript SDK guide
│   ├── openclaw-setup.md        # Configure OpenClaw agents
│   ├── merchant-integration.md  # Accept MPP payments
│   └── security.md              # Wallet security and policies
└── api/
    ├── sdk-reference.md         # SDK API reference
    └── contracts.md             # Smart contract ABIs
```

---

## Quick Links

- [What is MPP?](docs/concepts/mpp-protocol.md)
- [Base Settlement](docs/concepts/base-settlement.md)
- [TypeScript SDK Guide](docs/guides/typescript-sdk.md)
- [OpenClaw Setup](docs/guides/openclaw-setup.md)
- [Merchant Integration](docs/guides/merchant-integration.md)

---

## Core Concepts

### Machine Payments Protocol (MPP)

MPP is a standard by Stripe that enables AI agents to discover and pay for services autonomously via HTTP 402 responses. When an agent hits a 402, MoltMCP automatically negotiates and executes the payment.

### Base Settlement

All payments are settled on-chain via Base — an EVM-compatible L2 with sub-400ms finality and <$0.001 fees. Funds are held in escrow and released only after cryptographic proof of delivery.

### Agent Integration

MoltMCP acts as the payment layer between AI agent frameworks (OpenClaw, LangChain, etc.) and MPP-enabled services. Agents describe what they need in natural language; MoltMCP handles the rest.

---

## Contributing to Docs

Found a mistake or want to improve the docs? PRs are welcome!

```bash
git clone https://github.com/jackyixuan/moltmcp-docs.git
cd moltmcp-docs
# Edit markdown files and submit a PR
```

---

## License

[MIT](LICENSE) © 2025 MoltMCP
