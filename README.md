# PULSAR Mail Sender 🚀

> Self-hosted Windows bulk email sender — AI deliverability, SMTP rotation, embedded tracking. No per-email fees ever.

[![Version](https://img.shields.io/badge/version-1.0.0-cyan?style=flat-square)](https://github.com/multidigitaltools/pulsar-mail-sender/releases)
[![Platform](https://img.shields.io/badge/platform-Windows-blue?style=flat-square)](https://github.com/multidigitaltools/pulsar-mail-sender/releases)
[![License](https://img.shields.io/badge/license-Proprietary-orange?style=flat-square)](LICENSE)
[![Trial](https://img.shields.io/badge/trial-14--day%20free-green?style=flat-square)](https://multidigitaltools.com/products/pulsar-mail-sender)

PULSAR is a professional bulk email platform that runs entirely on your Windows machine — no monthly SaaS fees, no per-email charges, no data leaving your control. Built on .NET 10 with a MailKit SMTP engine, it combines enterprise-grade deliverability tools (DKIM, IP warm-up, SMTP rotation, SOCKS5 proxies) with an AI spam-scoring assistant powered by Claude API. Buy it once, own it forever.

---

## ✨ Features

- **Multi-SMTP Rotation** — add unlimited SMTP servers, set per-server rate limits, and let PULSAR balance load automatically
- **Automated IP Warm-Up** — structured warm-up scheduler ramps sending volume day-by-day to build sender reputation safely
- **Per-Domain DKIM Signing** — manage DKIM private keys inside the app; signatures applied automatically at send time
- **SOCKS5 Proxy Support** — route outbound connections through proxies for additional IP diversity
- **Embedded Tracking Server** — built-in ASP.NET Core server captures opens, clicks, and unsubscribes locally — zero third-party dependencies
- **Drip Sequences** — build multi-step automation campaigns triggered by time delays or subscriber behaviour
- **A/B Split Testing** — test subject lines and full content variants; PULSAR picks the winner automatically
- **AI Spam & Content Scoring** — Claude API integration checks every campaign before send; falls back to local Ollama when offline
- **Local Contact Database** — SQLite via EF Core; import from CSV or XLSX, segment with tags and custom fields
- **Encrypted Settings Store** — all credentials stored in LiteDB encrypted with Windows DPAPI — nothing in plain text
- **Live Analytics Dashboard** — real-time open/click/bounce charts powered by LiveCharts2
- **Auto-Updates** — Velopack-based silent updater; new versions install in seconds without reinstalling

---

## 🎯 Why PULSAR?

| Feature | PULSAR | Atomic Mail Sender | MailWizz | Gammadyne Mailer |
|---|---|---|---|---|
| **Price** | **$89 one-time** | $129/year | $59/month (server) | $149 one-time |
| **AI spam scoring** | ✅ Claude + Ollama | ❌ | ❌ | ❌ |
| **Embedded tracking server** | ✅ local, no SaaS | ❌ (3rd party) | ✅ server-side | ❌ |
| **SMTP rotation** | ✅ unlimited servers | ✅ limited | ✅ | ✅ |
| **IP warm-up scheduler** | ✅ automated | ❌ manual | partial | ❌ |
| **DKIM signing in-app** | ✅ per-domain keys | ❌ | ✅ | ✅ |
| **SOCKS5 proxy support** | ✅ | ❌ | ❌ | ✅ |
| **Drip sequences** | ✅ | ❌ | ✅ | ❌ |
| **A/B split testing** | ✅ subject + content | subject only | ✅ | ❌ |
| **Local data (no cloud)** | ✅ 100% local | ✅ | ❌ (server app) | ✅ |
| **Auto-updates** | ✅ Velopack | ❌ manual | n/a | ❌ manual |

---

## 🆓 14-Day Free Trial

The full-featured trial includes **everything** in the paid version — no feature gating, no send limits, no credit card required.

**What's included in the trial:**
- All SMTP server slots (unlimited)
- Full campaign wizard with A/B testing and drip sequences
- Embedded tracking server — opens, clicks, unsubscribes
- AI spam scoring (requires your own Claude API key or local Ollama)
- CSV/XLSX contact import
- Live analytics dashboard
- Complete documentation access

**How to start:**
1. Download the installer from the link below
2. Run `PULSAR-Setup.exe` — no account registration needed
3. Launch PULSAR; the 14-day trial activates automatically on first run
4. When the trial expires, enter your license key to continue

---

## 💾 Download

| Release | Platform | Size | Link |
|---|---|---|---|
| PULSAR Mail Sender v1.0.0 | Windows 10/11 x64 | ~95 MB | [[DOWNLOAD_LINK]](DOWNLOAD_LINK) |

> SHA-256 checksums are published alongside each release on the [Releases page](https://github.com/multidigitaltools/pulsar-mail-sender/releases).

---

## 🚀 Quick Start

1. **Install** — run `PULSAR-Setup.exe` and follow the wizard (installs .NET 10 runtime automatically if not present)
2. **Add an SMTP server** — go to **Settings → SMTP Servers → Add**, enter host/port/credentials, set your hourly rate limit, and click **Test Connection**
3. **Import contacts** — open **Contacts → Import**, choose a CSV or XLSX file, map columns (Email, FirstName, LastName, custom fields), and click **Import**
4. **Create a template** — go to **Templates → New**, write your HTML or plain-text email, use `{{FirstName}}` merge tags, and click **Save**
5. **Run AI check** — in the Campaign Wizard on step 4, click **AI Score** — PULSAR will flag spam trigger words, missing unsubscribe links, and image-to-text ratio issues
6. **Launch campaign** — review the send summary (recipient count, estimated duration, SMTP assignment) and click **Send Campaign**

---

## 💰 Pricing

| | PULSAR | Typical Competitor |
|---|---|---|
| **Price** | **$89 one-time** | $299 one-time |
| **Savings** | — | **You save $210 (70%)** |
| **Updates** | Lifetime (Velopack auto-update) | 1 year included |
| **Seats** | 1 machine per license | 1 machine per license |
| **Subscription** | None — ever | None |

**$89 one-time · compare $299 · 70% cheaper**

[Buy Now →](https://multidigitaltools.com/products/pulsar-mail-sender)

---

## 📋 System Requirements

| Component | Minimum | Recommended |
|---|---|---|
| **OS** | Windows 10 x64 (21H2+) | Windows 11 x64 |
| **RAM** | 4 GB | 8 GB |
| **Disk** | 500 MB free | 2 GB free (for logs/DB) |
| **Runtime** | .NET 10 (auto-installed) | .NET 10 |
| **Network** | SMTP outbound access | Dedicated IP or SMTP relay |
| **Optional** | Claude API key or Ollama | Claude API key (better AI scoring) |

---

## 📚 Documentation

Full user guide, SMTP setup tutorials, DKIM configuration walkthrough, deliverability best practices, and API key setup:

**[https://multidigitaltools.com/docs/pulsar-mail-sender/](https://multidigitaltools.com/docs/pulsar-mail-sender/)**

---

## 🛒 Buy

One-time payment. Lifetime license. Instant delivery.

**[Get PULSAR Mail Sender — $89 →](https://multidigitaltools.com/products/pulsar-mail-sender)**

---

## 🤝 Support

| Channel | Details |
|---|---|
| **Email** | support@multidigitaltools.com |
| **Docs** | [https://multidigitaltools.com/docs/pulsar-mail-sender/](https://multidigitaltools.com/docs/pulsar-mail-sender/) |
| **GitHub Issues** | Bug reports and feature requests: [open an issue](https://github.com/multidigitaltools/pulsar-mail-sender/issues) |
| **Response time** | Within 24 hours on business days |

---

*PULSAR Mail Sender is proprietary software © 2026 MultiDigitalTools. All rights reserved.*
