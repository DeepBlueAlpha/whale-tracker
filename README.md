# 🐳 Deep Blue Alpha — Ethereum Whale Intelligence Platform

**Live at:** [deepbluealpha.io](https://deepbluealpha.io)

> Track 11,000+ Ethereum whale wallets in real-time. Surface accumulation signals, token clustering, and on-chain alpha before it becomes news.

![Platform](https://img.shields.io/badge/Platform-Ethereum-blue?style=flat-square&logo=ethereum)
![Accuracy](https://img.shields.io/badge/30--Day%20Accuracy-71%25-brightgreen?style=flat-square)
![Wallets](https://img.shields.io/badge/Wallets%20Tracked-11%2C000%2B-cyan?style=flat-square)
![Status](https://img.shields.io/badge/Status-Live-success?style=flat-square)

---

## 📊 30-Day Live Scoreboard

| Metric | Value |
|--------|-------|
| **Hit Rate** | 71% |
| **Confirmed Wins** | 84 |
| **Big Wins (>20% return)** | 20 |
| **Pending** | 84 |

### 🔥 Recent Notable Picks

| Token | Signal Date | Outcome | Return |
|-------|-------------|---------|--------|
| $SCFG | Apr 2026 | ✅ Win | +35.8% |
| $BASER | Apr 2026 | ✅ Win | +15.6% |
| $COMP | Apr 2026 | ✅ Win | +12.6% |
| $ZRO | Apr 2026 | ⏳ Loading | — |
| $SMORPH | Apr 2026 | ⏳ Loading | — |

*Not financial advice. Data intelligence tool only.*

---

## 🔑 Features

- **Real-time whale feed** — Live Ethereum on-chain transaction monitoring
- **Wallet clustering & attribution** — Identify related whale wallets and hidden position sizes
- **Token accumulation alerts** — Get notified when large wallets start loading a token
- **30-day historical scoreboard** — Full transparency on signal accuracy
- **Market sentiment overlay** — Fear & Greed context alongside whale data
- **API access** — Programmatic access for developers and researchers (paid tiers)

---

## 💰 Pricing Tiers

| Tier | Price | Features |
|------|-------|---------|
| **Free** | $0 | Live dashboard, 24h whale feed, basic stats — no email required |
| **Alpha** | $19/mo | Real-time alerts, full wallet tracking, 7-day history, email notifications |
| **Whale** | $49/mo | Everything in Alpha + API access (rate-limited), 30-day history, custom alerts |
| **Leviathan** | $99/mo | Unlimited API, full historical data, webhook integrations, priority support |

---

## 🏗 Architecture

```
Ethereum Node (Alchemy/Infura)
        │
        ▼
Whale Tracker Core (Python/Flask)
  ├── Wallet clustering engine
  ├── Accumulation scoring
  └── Token signal generator
        │
        ▼
Redis (real-time queue)
        │
        ▼
SQLite / whale_tracker.db
        │
        ▼
Flask-SocketIO → WebSocket → Browser Dashboard
```

**Stack:** Python · Flask · Flask-SocketIO · SQLite · Redis · Cloudflare · Nginx

---

## 🚀 Getting Started (API)

```python
import requests

# Free tier — no auth required for public feed
response = requests.get("https://deepbluealpha.io/api/feed")
whales = response.json()

for move in whales["data"]:
    print(f"{move['wallet']} | {move['token']} | {move['action']} | {move['value_usd']}")
```

See the [whale-feed-sample](https://github.com/DeepBlueAlpha/whale-feed-sample) repo for full API docs and example responses.

---

## 📡 Tracked Signals

1. **Batch accumulation** — Same wallet buying a token across multiple transactions over 3–14 days
2. **Wallet clustering** — Multiple addresses controlled by the same entity accumulating in parallel
3. **Supply concentration** — Token supply moving from exchange wallets to private whale wallets
4. **Pre-pump positioning** — Anomalous wallet activity 7–21 days before price moves
5. **Smart money divergence** — Whale behavior diverging from retail sentiment index

---

## 📈 Why Whale Tracking Works

When the Fear & Greed Index is at **extreme fear** levels, sophisticated capital often accumulates quietly:

- Retail sees headlines → sells
- Whales see discounted supply → buys
- Price follows smart money (with a lag)

Our platform surfaces this divergence in real-time, not after the fact.

---

## 🛡 Disclaimer

Deep Blue Alpha is a data intelligence platform. Nothing on this platform constitutes financial advice. Whale wallet activity is observable on-chain but past signal accuracy does not guarantee future results. Always do your own research.

---

## 🔗 Links

- 🌊 **Platform:** [deepbluealpha.io](https://deepbluealpha.io)
- 🐦 **X / Twitter:** [@DeepBlueAlpha](https://x.com/DeepBlueAlpha)
- 📰 **Substack:** [The Deep Blue Brief](https://deepbluealpha.substack.com)
- 🔗 **LinkedIn:** [Deep Blue Alpha](https://linkedin.com/in/deep-blue-alpha)
- 🚀 **Product Hunt:** [@deepbluealpha](https://producthunt.com/@deepbluealpha)

---

*Built with 🐳 by the Deep Blue Alpha team — tracking the smart money so you don't have to.*
