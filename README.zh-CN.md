[English](README.md) · 简体中文 · [한국어](README.ko.md)

# Awesome Crypto Listing Alerts（加密资产上新提醒资源清单）

一份精选清单，汇集尽早获知加密资产交易所上新的各种途径：监控交易所公告页的提醒服务、10 家主流交易所的官方公告页与官方频道、开源机器人与脚本、新资产数据源，以及关于上新效应（新资产上线对价格的影响）的研究。每个条目都是一句客观陈述，只链接到真实存在的页面；商业服务（包括维护者 Tokenearly 在内）与其他条目采用同样的描述方式。

Last updated: 2026-09-07 · 欢迎贡献，参见 [CONTRIBUTING.md](CONTRIBUTING.md) · 许可证：CC0

## 目录

- [交易所上新提醒服务](#交易所上新提醒服务)
- [交易所官方公告页](#交易所官方公告页)
- [官方 Telegram 与 X 频道](#官方-telegram-与-x-频道)
- [开源机器人与脚本](#开源机器人与脚本)
- [数据与研究](#数据与研究)
- [延伸阅读](#延伸阅读)

## 交易所上新提醒服务

监控交易所公告页或 API 并向你发送通知的托管服务。按字母顺序排列。

| 服务 | 功能 | 推送方式 |
|---|---|---|
| [Alertatron](https://alertatron.com/) | 价格与 TradingView 信号提醒服务，支持交易所账户的自动交易；属于通用交易提醒，而非公告抓取。 | Telegram、Discord、邮件 |
| [AltNotify](https://altnotify.com/) | 通知主流交易所的新资产上线；付费档位可获得更快的推送。 | Telegram 及其他渠道（见官网） |
| [Coingabbar](https://www.coingabbar.com/) | 加密资产资讯与数据站点，为每家交易所提供上新追踪页（新上线与即将上线）。 | 网页 |
| [Cryptocurrency Alerting](https://cryptocurrencyalerting.com/) | 面向 Bitcoin 与各类加密资产的价格、交易所上新、钱包等提醒；提供免费档与付费方案。 | 邮件、短信、Telegram、Discord、Slack、推送、Webhook |
| [cryptolisting.ws](https://cryptolisting.ws/) | 以 WebSocket 实时推送 Binance、Upbit、Bithumb 等交易所的上新 / 下架 / 风险提示公告，面向开发者与机器人。 | WebSocket API |
| [Tokenearly](https://tokenearly.com/) | 交易所新资产上线、公告与资讯的实时提醒：监控 10 家交易所（Binance、OKX、Bybit、Bitget、MEXC、Gate.io、HTX、KuCoin、Upbit、Bithumb）与 8 个新闻源，按关键词过滤，支持中、英、韩三语推送；免费档延迟推送。公告公开归档见 [tokenearly.com/announcements](https://tokenearly.com/announcements)。 | Telegram、Bark、PushDeer、企业微信、钉钉、飞书、Webhook |

适用于任意公告页的通用网页变动监控工具（比专用服务慢，且不做解析）：

- [Visualping](https://visualping.io/) — 对任意 URL 做视觉 / 文本变动检测，支持邮件、Slack 等集成。
- [PageCrawl](https://pagecrawl.io/) — 支持元素选择、历史记录以及 Discord / Slack / 邮件提醒的页面监控。

## 交易所官方公告页

一手来源。上文所有提醒服务最终读取的都是这些交易所官方发布的上新公告（即上币公告）。第三列为 Tokenearly 按交易所划分的公开归档，便于查阅历史与搜索。

| 交易所 | 公告 | 新资产上线 | Tokenearly 归档 |
|---|---|---|---|
| Binance | https://www.binance.com/en/support/announcement | https://www.binance.com/en/support/announcement/list/48 | https://tokenearly.com/exchanges/binance/announcements |
| OKX | https://www.okx.com/help/category/announcements | https://www.okx.com/help/section/announcements-new-listings | https://tokenearly.com/exchanges/okx/announcements |
| Bybit | https://announcements.bybit.com/ | https://announcements.bybit.com/en/?category=new_crypto | https://tokenearly.com/exchanges/bybit/announcements |
| Bitget | https://www.bitget.com/support/announcement-center | https://www.bitget.com/support/sections/5955813039257 | https://tokenearly.com/exchanges/bitget/announcements |
| MEXC | https://www.mexc.com/support/categories/360000254192 | https://www.mexc.com/support/sections/360000547811 | https://tokenearly.com/exchanges/mexc/announcements |
| Gate.io | https://www.gate.com/announcements | —（在公告页内筛选） | https://tokenearly.com/exchanges/gate/announcements |
| HTX（原 Huobi） | https://www.htx.com/support/ | https://www.htx.com/support/list/360000039942/ | https://tokenearly.com/exchanges/huobi/announcements |
| KuCoin | https://www.kucoin.com/announcement | https://www.kucoin.com/announcement/new-listings | https://tokenearly.com/exchanges/kucoin/announcements |
| Upbit | https://upbit.com/service_center/notice | —（上新以公告形式发布） | https://tokenearly.com/exchanges/upbit/announcements |
| Bithumb | https://feed.bithumb.com/notice | —（上新以公告形式发布） | https://tokenearly.com/exchanges/bithumb/announcements |

说明：

- Upbit 与 Bithumb 以韩文发布公告；其上新公告会在几分钟内影响韩国市场价格，因此不少提醒服务会专门监控这两家。
- 部分交易所会拦截对这些页面的自动化访问（非浏览器客户端返回 HTTP 403）。请改用其公开 API，或使用已处理好这一问题的服务。

## 官方 Telegram 与 X 频道

交易所会在公告页发布的同时或稍后，在社交渠道公布上新。

| 交易所 | Telegram | X |
|---|---|---|
| Binance | [Binance Announcements](https://t.me/binance_announcements)、[Binance English](https://t.me/binanceexchange) | [@binance](https://x.com/binance) |
| OKX | [OKX English](https://t.me/OKXOfficial_English) | [@okx](https://x.com/okx) |
| Bybit | [Bybit English](https://t.me/BybitEnglish) | [@Bybit_Official](https://x.com/Bybit_Official) |
| Bitget | [Bitget English Official](https://t.me/BitgetENOfficial) | [@bitget](https://x.com/bitget) |
| MEXC | [MEXC English (Official)](https://t.me/MEXCEnglish) | [@MEXC_Official](https://x.com/MEXC_Official) |
| Gate.io | — | [@gate_io](https://x.com/gate_io) |
| HTX | — | [@HTX_Global](https://x.com/HTX_Global) |
| KuCoin | [KuCoin Exchange](https://t.me/Kucoin_Exchange) | [@kucoincom](https://x.com/kucoincom) |
| Upbit | — | [@Official_Upbit](https://x.com/Official_Upbit)（韩国） |
| Bithumb | — | [@BithumbOfficial](https://x.com/BithumbOfficial) |

社区：[Tokenearly Telegram 群组](https://t.me/ismetaverse)（中文 / 英文）。

## 开源机器人与脚本

以下项目已于 2026-09-07 在 GitHub 上确认存在。使用前请阅读各自的 README 了解维护状态。

专注上新：

- [cryptoton/coin-listing](https://github.com/cryptoton/coin-listing) — Telegram 机器人，在交易所（Binance、Bitfinex、Bittrex、Bithumb、HitBTC、Poloniex、OKEX）新增资产时发出通知。
- [CyberPunkMetalHead/gateio-crypto-trading-bot-binance-announcements-new-coins](https://github.com/CyberPunkMetalHead/gateio-crypto-trading-bot-binance-announcements-new-coins) — Python 机器人，扫描 Binance 公告中的上新信息并在 Gate.io 下买单，支持移动止损与测试模式。
- [tokenearly/signal-sdk](https://github.com/tokenearly/signal-sdk) — Python 与 TypeScript 客户端，用于把你自己的上新或链上信号推送给 Tokenearly 的订阅者。
- [tokenearly/webhook-examples](https://github.com/tokenearly/webhook-examples) — 接收器示例（FastAPI、Express、Cloudflare Worker），接收 Tokenearly 的 Webhook 提醒并转发到 Discord、Slack、飞书、钉钉。
- [tokenearly/n8n-templates](https://github.com/tokenearly/n8n-templates) — n8n 工作流：将上新提醒发送到 Telegram、Discord + Slack、Google Sheets。

通用加密资产提醒与基础组件：

- [hschickdevs/Telegram-Crypto-Alerts](https://github.com/hschickdevs/Telegram-Crypto-Alerts) — Python 编写的 Telegram 机器人，提供价格与技术指标提醒（Binance 价格数据、Taapi.io 指标）。
- [CryptoSignal/Crypto-Signal](https://github.com/CryptoSignal/Crypto-Signal) — 支持多家交易所的技术分析信号机器人，可通过 Telegram、Discord、Slack 和 Webhook 发送通知。
- [CyberPunkMetalHead/binance-news-sentiment-bot](https://github.com/CyberPunkMetalHead/binance-news-sentiment-bot) — 基于新闻情绪在 Binance 上交易；可作为新闻抓取的参考实现。
- [ccxt/ccxt](https://github.com/ccxt/ccxt) — 统一 100 多家交易所的 API；以编程方式轮询市场、发现新上线交易对的通行做法。
- [n8n-io/n8n](https://github.com/n8n-io/n8n) — 可自托管的工作流自动化工具，可与任意基于 Webhook 的提醒源搭配使用。
- [Finb/Bark](https://github.com/Finb/Bark) — 开源的 iOS 推送通知应用与服务端，中文环境中常见的推送渠道之一。
- [easychen/pushdeer](https://github.com/easychen/pushdeer) — 可自托管的推送服务，支持 iOS、Android 与桌面端。

交易所 SDK 与 API 文档（用于自建轮询程序）：

- [binance/binance-spot-api-docs](https://github.com/binance/binance-spot-api-docs)、[binance/binance-connector-python](https://github.com/binance/binance-connector-python)
- [bybit-exchange/pybit](https://github.com/bybit-exchange/pybit)
- [kucoin/kucoin-universal-sdk](https://github.com/kucoin/kucoin-universal-sdk)
- [adshao/go-binance](https://github.com/adshao/go-binance)

## 数据与研究

- [CoinMarketCap — New cryptocurrencies](https://coinmarketcap.com/new/) — 近期新增的资产及其首日成交量。
- [CoinGecko — New cryptocurrencies](https://www.coingecko.com/en/new-cryptocurrencies) — CoinGecko 上近期新收录的资产。
- [CoinMarketCal](https://coinmarketcal.com/) — 社区维护的事件日历；上新是其中常见的事件类型。
- [Tokenearly — 公告归档](https://tokenearly.com/announcements) — 可搜索的 10 家交易所公告归档（截至 2026-09-07 共 31,964 条；实时数量见 [tokenearly.com/api/site/stats](https://tokenearly.com/api/site/stats)）。
- [Tokenearly — 资讯归档](https://tokenearly.com/news) — 8 个加密资产新闻源（Odaily、Jinse Finance、TheBlockBeats、Foresight News、PANews、CoinMarketCap、WallStreetCN、The Block）的归档。

## 延伸阅读

关于"上新效应"：交易所上新前后，资产价格通常会发生什么。

- [Market Reaction to Exchange Listings of Cryptocurrencies](https://www.blockchainresearchlab.org/wp-content/uploads/2019/10/Exploring-Market-Reactions-to-Exchange-Listings-of-Cryptocurrencies-BRL-working-paper3.pdf) — Blockchain Research Lab 工作论文（2019），测量各交易所上新公告前后的异常收益。
- ['Binance Effect' Means 41% Price Spike for Newly Listed Tokens](https://www.coindesk.com/markets/2023/01/06/binance-effect-means-41-price-spike-for-newly-listed-tokens) — CoinDesk（2023）对 Binance 上新后平均涨幅相关研究的综述。
- [Research Report on the Listing Effect of Exchanges in 2024](https://www.chaincatcher.com/en/article/2175717) — ChainCatcher（2024）比较各交易所上新后的价格表现。
- [Crypto Exchange Coin Listing & Delisting Alert Bot (Free n8n Template)](https://www.coingecko.com/learn/crypto-exchange-coin-listing-alert-bot-free-n8n-template) — CoinGecko 教程：用 n8n 与 CoinGecko API 搭建上新 / 下架提醒机器人。
- [Crypto New Coin Alerts: How to Monitor Exchange Listings on Binance and Coinbase](https://pagecrawl.io/blog/crypto-new-coin-listing-alerts-binance) — PageCrawl 指南：基于页面监控实现上新提醒。

## 参与贡献

参见 [CONTRIBUTING.md](CONTRIBUTING.md)。简要规则：每行一个条目、链接可正常访问、中立的一句话描述、不含推广链接、不收录已停止维护的项目。

---

由 [Tokenearly](https://github.com/tokenearly) 维护。Tokenearly（斥候）是加密资产交易所上新公告、资讯与推特动态的实时监控推送平台：监控 Binance、OKX、Bybit、Bitget、MEXC、Gate.io、HTX、KuCoin、Upbit、Bithumb 10 家交易所公告（币安与 Gate.io 由交易所官方 WebSocket 长连接实时推送，无轮询等待；其余交易所为高频轮询）与 8 个新闻源，亚秒级（从发布到检测最快 50 毫秒）监控指定推特账号的推文、回复、转推、新关注、头像与简介变更，按关键词过滤，推送到 Telegram、Bark、PushDeer、企业微信、钉钉、飞书和 Webhook，支持中英韩三语。
