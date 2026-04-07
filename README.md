# Regional Index Pools (RWA DeFi)

**Децентрализованный протокол для инвестирования в токенизированные региональные экономические индексы на Solana**

![CI](https://github.com/Marakaya/regional-index-pools/actions/workflows/ci.yml/badge.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Solana](https://img.shields.io/badge/Solana-Devnet-9945FF?style=for-the-badge&logo=solana)
![Hackathon](https://img.shields.io/badge/Hackathon-2026-FF0060?style=for-the-badge)

---

## 🎯 О проекте

**Regional Index Pools** — DeFi-протокол для токенизации реальных региональных экономик (RWA).

```
┌─────────────────────────────────────────────────────────────┐
│                      INVESTOR                               │
│  💰 $1000 USDC → LP-токены → 📈 8.5% APY                  │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                   REGIONAL POOL                             │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐       │
│  │ Real Estate │  │  Treasury   │  │  IP / Tech  │       │
│  │    40%      │  │    30%      │  │    30%      │       │
│  └─────────────┘  └─────────────┘  └─────────────┘       │
└─────────────────────────────────────────────────────────────┘
```

---

## 🧱 Архитектура

```
┌─────────────────────────────────────────────────────────────┐
│                        FRONTEND                             │
│   Next.js + Tailwind + Solana Wallet Adapter               │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                    ANCHOR PROGRAM                           │
│   Program: RWIPool                                         │
│   Devnet: RwaPooL111111111111111111111111111111111111      │
└─────────────────────────────────────────────────────────────┘
```

---

## 📜 Смарт-контракт

Program ID: `RwaPooL111111111111111111111111111111111111`

### Account структуры:

```
Pool:       [authority, mint, lp_mint, total_deposits, total_shares, apy, region]
Investor:   [wallet, pool, shares, total_deposited, kyc_verified, whitelisted]
```

### Функции:

| Функция | Описание |
|---------|----------|
| `initializePool` | Создание регионального пула |
| `initializeInvestor` | Регистрация инвестора с KYC |
| `deposit` | Депозит USDC, получение LP токенов |
| `withdraw` | Вывод: сжигание LP → USDC + доход |

---

## 🚀 Quick Start

### Prerequisites:
- Node.js 18+
- Rust
- Anchor CLI
- Solana CLI

```bash
# Clone
git clone https://github.com/Marakaya/regional-index-pools
cd regional-index-pools

# Install dependencies
npm install

# Build programs
anchor build

# Run tests
anchor test

# Start frontend
cd frontend && npm install && npm run dev
```

---

## 📊 Примеры пулов (MVP)

| Пул | APY | TVL | Инвесторов | Риск |
|-----|-----|-----|-----------|------|
| Asia-Pacific Real Estate | 8.5% | $1.24M | 342 | Low |
| European Infrastructure | 7.2% | $890K | 198 | Low |

---

## 🎨 UI/UX

- 🌙 Dark theme
- 💜 Violet accents
- 📊 Real-time графики
- 🔒 KYC verification
- 💰 Portfolio dashboard

---

## 👥 Команда

| Участник | Роль | Контакт |
|---------|------|---------|
| Marakaya | Lead Developer | [Telegram](https://t.me/marakaya) |

---

## 📄 Лицензия

MIT License — see [LICENSE](LICENSE)

---

## 🔗 Полезные ссылки

- [Solana Docs](https://docs.solana.com)
- [Anchor Framework](https://www.anchor-lang.com)
- [Solana Playground](https://beta.solpg.io)
- [Phantom Wallet](https://phantom.app)

---

**Hackathon MVP** | Solana | 2026
