# 🛡️ SaboLabs Soroban Security Portal

> Fork & Security Enhancement of the [Stellar Security Portal](https://stellarsecurityportal.com) — **SaboLabs Security** focus on bug bounty writeups and real-world vulnerability analysis.

[![Soroban](https://img.shields.io/badge/Soroban-%239987E6.svg?logo=stellar&logoColor=white)](https://soroban.stellar.org)
[![Security: Audit Ready](https://img.shields.io/badge/Security-Audit%20Ready-green.svg)](https://github.com/naninu123/soroban-security-portal/security)
[![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

---

## 🎯 What's This?

This is **SaboLabs' fork** of the original [Inferara/Soroban Security Portal](https://github.com/Inferara/soroban-security-portal), with enhanced focus on:

- 🐛 **Real-world bug bounty writeups** — sanitized PoC + findings from Immunefi/H1
- 📊 **Vulnerability classification** — AST-based detection, common vulnerability patterns
- 🔍 **Audit methodology** — step-by-step Soroban smart contract security review guide
- 🛠️ **Tooling integration** — Foundry + Soroban CLI + custom audit scripts

---

## 📚 Sections

| Section | Description | Status |
|---------|-------------|--------|
| [Vulnerability Database](./docs/vulnerabilities/) | Catalog of known Soroban vulnerabilities | ✅ Active |
| [Bug Bounty Writeups](./writeups/) | Sanitized PoC from authorized audits | ✅ Active |
| [Audit Checklist](./docs/audit-checklist/) | Step-by-step security review guide | 🔄 In Progress |
| [Tooling](./scripts/) | CLI utilities for automated audit tasks | 🚧 WIP |

---

## 🚀 Quick Start

```bash
# Clone the repo
git clone https://github.com/naninu123/soroban-security-portal.git
cd soroban-security-portal

# View vulnerability catalog
open ./docs/vulnerabilities/

# Run audit helper scripts
python scripts/audit_helper.py --help
```

---

## 🔍 Supported Vulnerability Types

| Category | Pattern | Severity |
|----------|---------|----------|
| Storage | Incomplete cleanup on `store_set` | Critical |
|Math | Integer overflow/underflow | High |
| Access | Missing `auth.required()` guards | Critical |
| Events | Unbounded event emission | Medium |
| Time | Ledger time manipulation | High |
| Token | Asset authorization bypass | Critical |

---

## 🛠️ Tech Stack

- **Frontend:** React, Next.js, Tailwind CSS
- **Backend:** Rust (Stellar Soroban SDK)
- **Audit Scripts:** Python, Foundry
- **Hosting:** Tansu, Cloudflare Pages

---

## 🤝 Acknowledgments

This project builds on top of the [Stellar Security Portal](https://github.com/Inferara/soroban-security-portal) — funded by the [Stellar Community Fund](https://communityfund.stellar.org/).

**SaboLabs Security** adds:
- Real-world bug bounty analysis
- Automated vulnerability scanner integrations
- Expanded vulnerability database with PoC

---

## 📄 License

Apache License 2.0 — see [LICENSE](LICENSE) for details.

---

*⚡ SaboLabs Security · Soroban Security Enhancement · 2026 ⚡*
