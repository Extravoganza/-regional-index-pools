# Regional Index Pools (RWA DeFi)

**Децентрализованный протокол для инвестирования в токенизированные региональные экономические индексы на Solana**

![Solana](https://img.shields.io/badge/Solana-000000?style=for-the-badge&logo=solana)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

---

## 🎯 О проекте

**Regional Index Pools** — это DeFi-протокол, который переносит модель liquidity pools в мир реальных активов (RWA).

Вместо традиционных крипто-активов, пользователи инвестируют в пулы, привязанные к региональным экономикам:

- 🌏 **Азиатско-Тихоокеанский регион** — коммерческая и жилая недвижимость
- 🌍 **Европа** — инфраструктурные проекты

---

## 💡 Ключевая идея

Мы создаём новый класс активов — **токенизированные региональные индексы**, которые объединяют реальные бизнесы и распределяют доход инвесторам через смарт-контракты.

---

## ⚙️ Как это работает

### Для инвестора:

1. **Подключи кошелёк** (Phantom, Solflare)
2. **Пройди верификацию** (KYC mock для MVP)
3. **Выбери региональный пул**
4. **Внеси USDC** → получи LP-токены
5. **Получай доход** автоматически

### Механика:

| Шаг | Действие | Результат |
|-----|----------|-----------|
| 1 | Депозит 1000 USDC | Получаешь 1000 LP токенов |
| 2 | Пулы растут | Доход начисляется автоматически |
| 3 | Через год | LP токены стоят $1085 (8.5% APY) |
| 4 | Вывод | Сжигаешь LP → получаешь USDC + доход |

---

## 📊 Финансовые метрики

### Примеры пулов:

| Пул | APY | TVL | Инвесторов | Риск |
|-----|-----|-----|-----------|------|
| Asia-Pacific Real Estate | 8.5% | $1.24M | 342 | Low |
| European Infrastructure | 7.2% | $890K | 198 | Low |

---

## 🧱 Архитектура
### Account структуры:
Pool: [authority, mint, lp_mint, total_deposits, total_shares, apy, region] Investor: [wallet, pool, shares, total_deposited, kyc_verified, whitelisted]


---

## 🚀 Запуск

### Фронтенд:

```bash
cd frontend
npm install
npm run dev
Открой: http://localhost:3000

Смарт-контракт:
Деплой в Solana Playground:

Скопируй programs/rwipool/src/lib.rs
Вставь в https://beta.solpg.io
Program ID: RwaPooL111111111111111111111111111111111111
Build → Deploy
🎨 UI/UX
Интерфейс в стиле modern fintech (Stripe / Linear):

🌙 Dark theme
💜 Violet accents
📊 Real-time графики
🔒 KYC verification flow
💰 Portfolio dashboard
👥 Команда
Участник	Роль
Marakaya	Lead Developer
📄 Лицензия
MIT License

🔗 Полезные ссылки
Solana Docs
Anchor Framework
Solana Playground
Phantom Wallet
