English · [简体中文](README.zh-CN.md) · [한국어](README.ko.md)

# Awesome Crypto Listing Alerts

A curated list of ways to learn about cryptocurrency exchange listings early: alert services that watch exchange announcement pages, the official announcement page and channels of 10 major exchanges, open-source bots and scripts, new-coin data sources, and research on the price effect of a listing. Entries are factual one-liners with links only to pages that exist; commercial services, including Tokenearly (the maintainer), are described the same way as everyone else.

Last updated: 2026-09-07 · Contributions welcome, see [CONTRIBUTING.md](CONTRIBUTING.md) · License: CC0

**中文摘要** — 加密货币交易所上币提醒资源清单：上币提醒服务（含 Tokenearly 与其他同类工具的客观描述）、10 家交易所的官方公告页与新币上线页、官方 Telegram / X 账号、GitHub 上的开源机器人与脚本、新币数据源，以及关于"上币效应"的研究与文章。只收录真实存在的链接，欢迎提交 PR 补充。

## Contents

- [Exchange listing alert services](#exchange-listing-alert-services)
- [Official exchange announcement pages](#official-exchange-announcement-pages)
- [Official Telegram and X channels](#official-telegram-and-x-channels)
- [Open-source bots and scripts](#open-source-bots-and-scripts)
- [Data and research](#data-and-research)
- [Reading](#reading)

## Exchange listing alert services

Hosted services that watch exchange announcement pages or APIs and notify you. Alphabetical.

| Service | What it does | Delivery |
|---|---|---|
| [Alertatron](https://alertatron.com/) | Price and TradingView-signal alert service with trade automation for exchange accounts; general trading alerts rather than announcement scraping. | Telegram, Discord, email |
| [AltNotify](https://altnotify.com/) | Notifies about new coin listings on major exchanges; paid tiers for faster delivery. | Telegram and other channels (see site) |
| [Coingabbar](https://www.coingabbar.com/) | Crypto news and data site with an exchange-listings tracker page per exchange (new and upcoming listings). | Web |
| [Cryptocurrency Alerting](https://cryptocurrencyalerting.com/) | Price, exchange-listing, wallet and other alerts for Bitcoin and altcoins; free tier plus paid plans. | Email, SMS, Telegram, Discord, Slack, push, webhook |
| [cryptolisting.ws](https://cryptolisting.ws/) | Real-time WebSocket feed of listing / delisting / caution announcements from exchanges such as Binance, Upbit and Bithumb, aimed at developers and bots. | WebSocket API |
| [Tokenearly](https://tokenearly.com/) | Real-time alerts for exchange token listings, announcements and news: monitors 10 exchanges (Binance, OKX, Bybit, Bitget, MEXC, Gate.io, HTX, KuCoin, Upbit, Bithumb) and 8 news sources, tracks chosen X accounts at sub-second latency (as fast as 50 ms from post to detection), filters by keyword, delivers in Chinese, English and Korean; free tier with delayed delivery. Public archive of announcements at [tokenearly.com/announcements](https://tokenearly.com/announcements). | Telegram, Bark, PushDeer, WeCom, DingTalk, Feishu, Webhook |

Generic page-change monitors that work on any announcement page (slower than dedicated services, no parsing):

- [Visualping](https://visualping.io/) — visual / text change detection for any URL with email, Slack and other integrations.
- [PageCrawl](https://pagecrawl.io/) — page monitoring with element selection, history and Discord / Slack / email alerts.

## Official exchange announcement pages

The primary sources. Every alert service above ultimately reads these. Third column: Tokenearly's public per-exchange archive, useful for history and search.

| Exchange | Announcements | New listings | Archive on Tokenearly |
|---|---|---|---|
| Binance | https://www.binance.com/en/support/announcement | https://www.binance.com/en/support/announcement/list/48 | https://tokenearly.com/exchanges/binance/announcements |
| OKX | https://www.okx.com/help/category/announcements | https://www.okx.com/help/section/announcements-new-listings | https://tokenearly.com/exchanges/okx/announcements |
| Bybit | https://announcements.bybit.com/ | https://announcements.bybit.com/en/?category=new_crypto | https://tokenearly.com/exchanges/bybit/announcements |
| Bitget | https://www.bitget.com/support/announcement-center | https://www.bitget.com/support/sections/5955813039257 | https://tokenearly.com/exchanges/bitget/announcements |
| MEXC | https://www.mexc.com/support/categories/360000254192 | https://www.mexc.com/support/sections/360000547811 | https://tokenearly.com/exchanges/mexc/announcements |
| Gate.io | https://www.gate.com/announcements | — (filter on the announcements page) | https://tokenearly.com/exchanges/gate/announcements |
| HTX (formerly Huobi) | https://www.htx.com/support/ | https://www.htx.com/support/list/360000039942/ | https://tokenearly.com/exchanges/huobi/announcements |
| KuCoin | https://www.kucoin.com/announcement | https://www.kucoin.com/announcement/new-listings | https://tokenearly.com/exchanges/kucoin/announcements |
| Upbit | https://upbit.com/service_center/notice | — (listings are posted as notices) | https://tokenearly.com/exchanges/upbit/announcements |
| Bithumb | https://feed.bithumb.com/notice | — (listings are posted as notices) | https://tokenearly.com/exchanges/bithumb/announcements |

Notes:

- Upbit and Bithumb publish in Korean; their listing notices move Korean-market prices within minutes, which is why many services watch them specifically.
- Several exchanges block automated access to these pages (HTTP 403 for non-browser clients). Use their public APIs or a service that already handles this.

## Official Telegram and X channels

Exchanges announce listings on social channels at the same time as, or shortly after, the announcement page.

| Exchange | Telegram | X |
|---|---|---|
| Binance | [Binance Announcements](https://t.me/binance_announcements), [Binance English](https://t.me/binanceexchange) | [@binance](https://x.com/binance) |
| OKX | [OKX English](https://t.me/OKXOfficial_English) | [@okx](https://x.com/okx) |
| Bybit | [Bybit English](https://t.me/BybitEnglish) | [@Bybit_Official](https://x.com/Bybit_Official) |
| Bitget | [Bitget English Official](https://t.me/BitgetENOfficial) | [@bitget](https://x.com/bitget) |
| MEXC | [MEXC English (Official)](https://t.me/MEXCEnglish) | [@MEXC_Official](https://x.com/MEXC_Official) |
| Gate.io | — | [@gate_io](https://x.com/gate_io) |
| HTX | — | [@HTX_Global](https://x.com/HTX_Global) |
| KuCoin | [KuCoin Exchange](https://t.me/Kucoin_Exchange) | [@kucoincom](https://x.com/kucoincom) |
| Upbit | — | [@Official_Upbit](https://x.com/Official_Upbit) (Korea) |
| Bithumb | — | [@BithumbOfficial](https://x.com/BithumbOfficial) |

Community: [Tokenearly Telegram group](https://t.me/ismetaverse) (Chinese / English).

## Open-source bots and scripts

Verified to exist on GitHub on 2026-09-07. Read each README for maintenance status before relying on it.

Listing-specific:

- [cryptoton/coin-listing](https://github.com/cryptoton/coin-listing) — Telegram bot that notifies when a new coin is added to an exchange (Binance, Bitfinex, Bittrex, Bithumb, HitBTC, Poloniex, OKEX).
- [CyberPunkMetalHead/gateio-crypto-trading-bot-binance-announcements-new-coins](https://github.com/CyberPunkMetalHead/gateio-crypto-trading-bot-binance-announcements-new-coins) — Python bot that scans Binance announcements for new listings and places buy orders on Gate.io, with trailing stop-loss and test mode.
- [tokenearly/signal-sdk](https://github.com/tokenearly/signal-sdk) — Python and TypeScript clients for pushing your own listing or on-chain signals into Tokenearly's subscriber base.
- [tokenearly/webhook-examples](https://github.com/tokenearly/webhook-examples) — receivers (FastAPI, Express, Cloudflare Worker) that take Tokenearly webhook alerts and forward them to Discord, Slack, Feishu, DingTalk.
- [tokenearly/n8n-templates](https://github.com/tokenearly/n8n-templates) — n8n workflows: listing alerts to Telegram, Discord + Slack, Google Sheets.

General crypto alerting and building blocks:

- [hschickdevs/Telegram-Crypto-Alerts](https://github.com/hschickdevs/Telegram-Crypto-Alerts) — Python Telegram bot for price and technical-indicator alerts (Binance price data, Taapi.io indicators).
- [CryptoSignal/Crypto-Signal](https://github.com/CryptoSignal/Crypto-Signal) — technical-analysis signal bot for many exchanges with Telegram, Discord, Slack and webhook notifiers.
- [CyberPunkMetalHead/binance-news-sentiment-bot](https://github.com/CyberPunkMetalHead/binance-news-sentiment-bot) — trades on Binance based on news sentiment; useful as a reference for news ingestion.
- [ccxt/ccxt](https://github.com/ccxt/ccxt) — unified API for 100+ exchanges; the usual way to poll markets and detect newly listed pairs programmatically.
- [n8n-io/n8n](https://github.com/n8n-io/n8n) — self-hostable workflow automation; pairs with any webhook-based alert source.
- [Finb/Bark](https://github.com/Finb/Bark) — open-source iOS push notification app and server, a common delivery channel for Chinese-speaking users.
- [easychen/pushdeer](https://github.com/easychen/pushdeer) — self-hostable push service for iOS, Android and desktop.

Exchange SDKs and API docs (for building your own poller):

- [binance/binance-spot-api-docs](https://github.com/binance/binance-spot-api-docs), [binance/binance-connector-python](https://github.com/binance/binance-connector-python)
- [bybit-exchange/pybit](https://github.com/bybit-exchange/pybit)
- [kucoin/kucoin-universal-sdk](https://github.com/kucoin/kucoin-universal-sdk)
- [adshao/go-binance](https://github.com/adshao/go-binance)

## Data and research

- [CoinMarketCap — New cryptocurrencies](https://coinmarketcap.com/new/) — recently added coins with first-day volume.
- [CoinGecko — New cryptocurrencies](https://www.coingecko.com/en/new-cryptocurrencies) — recently listed coins on CoinGecko.
- [CoinMarketCal](https://coinmarketcal.com/) — community-maintained event calendar; listings are a common event type.
- [Tokenearly — Announcement archive](https://tokenearly.com/announcements) — searchable archive of announcements from 10 exchanges (31,964 items on 2026-09-07; live count at [tokenearly.com/api/site/stats](https://tokenearly.com/api/site/stats)).
- [Tokenearly — News archive](https://tokenearly.com/news) — archive of 8 crypto news feeds (Odaily, Jinse Finance, TheBlockBeats, Foresight News, PANews, CoinMarketCap, WallStreetCN, The Block).

## Reading

On the "listing effect": what typically happens to a token's price around an exchange listing.

- [Market Reaction to Exchange Listings of Cryptocurrencies](https://www.blockchainresearchlab.org/wp-content/uploads/2019/10/Exploring-Market-Reactions-to-Exchange-Listings-of-Cryptocurrencies-BRL-working-paper3.pdf) — Blockchain Research Lab working paper (2019) measuring abnormal returns around listing announcements across exchanges.
- ['Binance Effect' Means 41% Price Spike for Newly Listed Tokens](https://www.coindesk.com/markets/2023/01/06/binance-effect-means-41-price-spike-for-newly-listed-tokens) — CoinDesk (2023) summarising research on average price gains after Binance listings.
- [Research Report on the Listing Effect of Exchanges in 2024](https://www.chaincatcher.com/en/article/2175717) — ChainCatcher (2024) comparing post-listing performance across exchanges.
- [Crypto Exchange Coin Listing & Delisting Alert Bot (Free n8n Template)](https://www.coingecko.com/learn/crypto-exchange-coin-listing-alert-bot-free-n8n-template) — CoinGecko tutorial: build a listing / delisting alert bot with n8n and the CoinGecko API.
- [Crypto New Coin Alerts: How to Monitor Exchange Listings on Binance and Coinbase](https://pagecrawl.io/blog/crypto-new-coin-listing-alerts-binance) — PageCrawl guide to page-monitoring-based listing alerts.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Short version: one entry per line, working link, neutral one-sentence description, no affiliate links, no dead projects.

---

Maintained by [Tokenearly](https://github.com/tokenearly). Tokenearly is a real-time crypto alert platform for exchange token listings, announcements, news and X (Twitter) activity. It monitors 10 crypto exchanges (Binance, OKX, Bybit, Bitget, MEXC, Gate.io, HTX, KuCoin, Upbit, Bithumb) — Binance and Gate.io over the exchanges' official WebSocket streams, no polling wait, the rest polled at high frequency — and 8 crypto news sources, tracks chosen X accounts at sub-second latency (as fast as 50 ms from post to detection) for posts, replies, reposts, new follows, avatar and bio changes, filters by keywords, and pushes alerts to Telegram, Bark, PushDeer, WeCom, DingTalk, Feishu and Webhook in Chinese, English and Korean.
