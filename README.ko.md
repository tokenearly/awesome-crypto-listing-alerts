[English](README.md) · [简体中文](README.zh-CN.md) · 한국어

# Awesome Crypto Listing Alerts(암호화폐 상장 알림 자료 모음)

암호화폐 거래소의 토큰 상장 소식을 남보다 먼저 접할 수 있는 방법을 정리한 목록입니다. 거래소 공지 페이지를 감시하는 알림 서비스, 10개 주요 거래소의 공식 공지 페이지와 공식 채널, 오픈소스 봇과 스크립트, 신규 코인 데이터 소스, 그리고 상장이 가격에 미치는 영향에 관한 연구를 담았습니다. 각 항목은 사실에 근거한 한 줄 설명이며 실제 존재하는 페이지만 링크합니다. 상용 서비스는 관리자인 Tokenearly(토큰얼리)를 포함해 모두 동일한 방식으로 기술합니다.

Last updated: 2026-09-07 · 기여를 환영합니다. [CONTRIBUTING.md](CONTRIBUTING.md)를 참고하세요 · 라이선스: CC0

## 목차

- [거래소 상장 알림 서비스](#거래소-상장-알림-서비스)
- [거래소 공식 공지 페이지](#거래소-공식-공지-페이지)
- [공식 Telegram 및 X 채널](#공식-telegram-및-x-채널)
- [오픈소스 봇과 스크립트](#오픈소스-봇과-스크립트)
- [데이터와 연구](#데이터와-연구)
- [읽을거리](#읽을거리)

## 거래소 상장 알림 서비스

거래소 공지 페이지나 API를 감시하고 알림을 보내 주는 호스팅 서비스입니다. 알파벳순으로 정렬했습니다.

| 서비스 | 기능 | 전달 채널 |
|---|---|---|
| [Alertatron](https://alertatron.com/) | 가격 및 TradingView 시그널 알림 서비스로, 거래소 계정 자동 매매를 지원합니다. 공지 수집이 아닌 일반 트레이딩 알림에 해당합니다. | Telegram, Discord, 이메일 |
| [AltNotify](https://altnotify.com/) | 주요 거래소의 신규 코인 상장을 알려 줍니다. 유료 요금제에서 더 빠른 알림을 제공합니다. | Telegram 및 기타 채널(사이트 참고) |
| [Coingabbar](https://www.coingabbar.com/) | 암호화폐 뉴스·데이터 사이트로, 거래소별 상장 추적 페이지(신규 및 예정 상장)를 제공합니다. | 웹 |
| [Cryptocurrency Alerting](https://cryptocurrencyalerting.com/) | Bitcoin과 알트코인의 가격, 거래소 상장, 지갑 등 다양한 알림을 제공합니다. 무료 요금제와 유료 플랜이 있습니다. | 이메일, SMS, Telegram, Discord, Slack, 푸시, Webhook |
| [cryptolisting.ws](https://cryptolisting.ws/) | Binance, Upbit, Bithumb 등 거래소의 상장 / 상장폐지 / 유의 종목 공지를 WebSocket으로 실시간 제공하며, 개발자와 봇을 대상으로 합니다. | WebSocket API |
| [Tokenearly](https://tokenearly.com/) | 거래소 토큰 상장, 공지, 뉴스 실시간 알림 서비스입니다. 10개 거래소(Binance, OKX, Bybit, Bitget, MEXC, Gate.io, HTX, KuCoin, Upbit, Bithumb)와 8개 뉴스 소스를 모니터링하고, 키워드로 필터링해 한국어·영어·중국어로 알림을 보냅니다. 무료 요금제는 지연 전송이 있습니다. 공개 공지 아카이브: [tokenearly.com/announcements](https://tokenearly.com/announcements). | Telegram, Bark, PushDeer, WeCom, DingTalk, Feishu, Webhook |

어떤 공지 페이지에도 적용할 수 있는 범용 페이지 변경 감시 도구입니다(전용 서비스보다 느리고, 파싱은 하지 않습니다).

- [Visualping](https://visualping.io/) — 임의의 URL에 대한 시각적 / 텍스트 변경 감지 서비스로, 이메일, Slack 등과 연동됩니다.
- [PageCrawl](https://pagecrawl.io/) — 요소 선택, 변경 이력, Discord / Slack / 이메일 알림을 지원하는 페이지 모니터링 서비스입니다.

## 거래소 공식 공지 페이지

1차 정보원입니다. 위의 모든 알림 서비스는 결국 이 페이지들을 읽습니다. 세 번째 열은 Tokenearly의 거래소별 공개 아카이브로, 과거 기록 조회와 검색에 유용합니다.

| 거래소 | 공지 | 신규 상장 | Tokenearly 아카이브 |
|---|---|---|---|
| Binance | https://www.binance.com/en/support/announcement | https://www.binance.com/en/support/announcement/list/48 | https://tokenearly.com/exchanges/binance/announcements |
| OKX | https://www.okx.com/help/category/announcements | https://www.okx.com/help/section/announcements-new-listings | https://tokenearly.com/exchanges/okx/announcements |
| Bybit | https://announcements.bybit.com/ | https://announcements.bybit.com/en/?category=new_crypto | https://tokenearly.com/exchanges/bybit/announcements |
| Bitget | https://www.bitget.com/support/announcement-center | https://www.bitget.com/support/sections/5955813039257 | https://tokenearly.com/exchanges/bitget/announcements |
| MEXC | https://www.mexc.com/support/categories/360000254192 | https://www.mexc.com/support/sections/360000547811 | https://tokenearly.com/exchanges/mexc/announcements |
| Gate.io | https://www.gate.com/announcements | —(공지 페이지에서 필터링) | https://tokenearly.com/exchanges/gate/announcements |
| HTX(구 Huobi) | https://www.htx.com/support/ | https://www.htx.com/support/list/360000039942/ | https://tokenearly.com/exchanges/huobi/announcements |
| KuCoin | https://www.kucoin.com/announcement | https://www.kucoin.com/announcement/new-listings | https://tokenearly.com/exchanges/kucoin/announcements |
| Upbit | https://upbit.com/service_center/notice | —(상장 소식은 공지사항으로 게시) | https://tokenearly.com/exchanges/upbit/announcements |
| Bithumb | https://feed.bithumb.com/notice | —(상장 소식은 공지사항으로 게시) | https://tokenearly.com/exchanges/bithumb/announcements |

참고:

- Upbit과 Bithumb은 한국어로 공지를 게시합니다. 두 거래소의 상장 공지는 몇 분 안에 한국 시장 가격을 움직이기 때문에 많은 알림 서비스가 이 두 곳을 따로 감시합니다.
- 일부 거래소는 이 페이지들에 대한 자동화 접근을 차단합니다(브라우저가 아닌 클라이언트에는 HTTP 403 응답). 공개 API를 사용하거나 이 문제를 이미 처리한 서비스를 이용하세요.

## 공식 Telegram 및 X 채널

거래소는 공지 페이지 게시와 동시에, 또는 직후에 소셜 채널에서도 상장 소식을 알립니다.

| 거래소 | Telegram | X |
|---|---|---|
| Binance | [Binance Announcements](https://t.me/binance_announcements), [Binance English](https://t.me/binanceexchange) | [@binance](https://x.com/binance) |
| OKX | [OKX English](https://t.me/OKXOfficial_English) | [@okx](https://x.com/okx) |
| Bybit | [Bybit English](https://t.me/BybitEnglish) | [@Bybit_Official](https://x.com/Bybit_Official) |
| Bitget | [Bitget English Official](https://t.me/BitgetENOfficial) | [@bitget](https://x.com/bitget) |
| MEXC | [MEXC English (Official)](https://t.me/MEXCEnglish) | [@MEXC_Official](https://x.com/MEXC_Official) |
| Gate.io | — | [@gate_io](https://x.com/gate_io) |
| HTX | — | [@HTX_Global](https://x.com/HTX_Global) |
| KuCoin | [KuCoin Exchange](https://t.me/Kucoin_Exchange) | [@kucoincom](https://x.com/kucoincom) |
| Upbit | — | [@Official_Upbit](https://x.com/Official_Upbit)(한국) |
| Bithumb | — | [@BithumbOfficial](https://x.com/BithumbOfficial) |

커뮤니티: [Tokenearly Telegram 그룹](https://t.me/ismetaverse)(중국어 / 영어).

## 오픈소스 봇과 스크립트

2026-09-07 기준으로 GitHub에 존재함을 확인했습니다. 사용하기 전에 각 README에서 유지보수 상태를 확인하세요.

상장 특화:

- [cryptoton/coin-listing](https://github.com/cryptoton/coin-listing) — 거래소(Binance, Bitfinex, Bittrex, Bithumb, HitBTC, Poloniex, OKEX)에 새 코인이 추가되면 알려 주는 Telegram 봇입니다.
- [CyberPunkMetalHead/gateio-crypto-trading-bot-binance-announcements-new-coins](https://github.com/CyberPunkMetalHead/gateio-crypto-trading-bot-binance-announcements-new-coins) — Binance 공지에서 신규 상장을 스캔해 Gate.io에 매수 주문을 넣는 Python 봇으로, 트레일링 스톱로스와 테스트 모드를 지원합니다.
- [tokenearly/signal-sdk](https://github.com/tokenearly/signal-sdk) — 자체 상장 또는 온체인 시그널을 Tokenearly 구독자에게 전송하기 위한 Python 및 TypeScript 클라이언트입니다.
- [tokenearly/webhook-examples](https://github.com/tokenearly/webhook-examples) — Tokenearly Webhook 알림을 받아 Discord, Slack, Feishu, DingTalk으로 전달하는 수신기 예제(FastAPI, Express, Cloudflare Worker)입니다.
- [tokenearly/n8n-templates](https://github.com/tokenearly/n8n-templates) — n8n 워크플로: 상장 알림을 Telegram, Discord + Slack, Google Sheets로 전송합니다.

일반 암호화폐 알림 및 구성 요소:

- [hschickdevs/Telegram-Crypto-Alerts](https://github.com/hschickdevs/Telegram-Crypto-Alerts) — 가격 및 기술 지표 알림용 Python Telegram 봇입니다(Binance 가격 데이터, Taapi.io 지표).
- [CryptoSignal/Crypto-Signal](https://github.com/CryptoSignal/Crypto-Signal) — 여러 거래소를 지원하는 기술적 분석 시그널 봇으로, Telegram, Discord, Slack, Webhook 알림을 제공합니다.
- [CyberPunkMetalHead/binance-news-sentiment-bot](https://github.com/CyberPunkMetalHead/binance-news-sentiment-bot) — 뉴스 감성 분석을 바탕으로 Binance에서 거래하는 봇으로, 뉴스 수집 구현의 참고 자료로 유용합니다.
- [ccxt/ccxt](https://github.com/ccxt/ccxt) — 100개 이상의 거래소를 아우르는 통합 API로, 프로그램으로 마켓을 폴링해 신규 상장 페어를 감지하는 일반적인 방법입니다.
- [n8n-io/n8n](https://github.com/n8n-io/n8n) — 자체 호스팅 가능한 워크플로 자동화 도구로, Webhook 기반 알림 소스와 함께 사용할 수 있습니다.
- [Finb/Bark](https://github.com/Finb/Bark) — 오픈소스 iOS 푸시 알림 앱 및 서버로, 중국어권에서 흔히 쓰이는 전달 채널입니다.
- [easychen/pushdeer](https://github.com/easychen/pushdeer) — iOS, Android, 데스크톱을 지원하는 자체 호스팅 가능한 푸시 서비스입니다.

거래소 SDK 및 API 문서(직접 폴러를 만들 때):

- [binance/binance-spot-api-docs](https://github.com/binance/binance-spot-api-docs), [binance/binance-connector-python](https://github.com/binance/binance-connector-python)
- [bybit-exchange/pybit](https://github.com/bybit-exchange/pybit)
- [kucoin/kucoin-universal-sdk](https://github.com/kucoin/kucoin-universal-sdk)
- [adshao/go-binance](https://github.com/adshao/go-binance)

## 데이터와 연구

- [CoinMarketCap — New cryptocurrencies](https://coinmarketcap.com/new/) — 최근 추가된 코인과 첫날 거래량을 보여 줍니다.
- [CoinGecko — New cryptocurrencies](https://www.coingecko.com/en/new-cryptocurrencies) — CoinGecko에 최근 등록된 코인 목록입니다.
- [CoinMarketCal](https://coinmarketcal.com/) — 커뮤니티가 관리하는 이벤트 캘린더로, 상장은 흔한 이벤트 유형 중 하나입니다.
- [Tokenearly — 공지 아카이브](https://tokenearly.com/announcements) — 10개 거래소 공지를 검색할 수 있는 아카이브입니다(2026-09-07 기준 31,964건, 실시간 집계는 [tokenearly.com/api/site/stats](https://tokenearly.com/api/site/stats) 참고).
- [Tokenearly — 뉴스 아카이브](https://tokenearly.com/news) — 8개 암호화폐 뉴스 피드(Odaily, Jinse Finance, TheBlockBeats, Foresight News, PANews, CoinMarketCap, WallStreetCN, The Block) 아카이브입니다.

## 읽을거리

'상장 효과'에 관한 자료입니다. 거래소 상장 전후로 토큰 가격에 일반적으로 어떤 일이 일어나는지 다룹니다.

- [Market Reaction to Exchange Listings of Cryptocurrencies](https://www.blockchainresearchlab.org/wp-content/uploads/2019/10/Exploring-Market-Reactions-to-Exchange-Listings-of-Cryptocurrencies-BRL-working-paper3.pdf) — Blockchain Research Lab 워킹 페이퍼(2019)로, 여러 거래소의 상장 공지 전후 비정상 수익률을 측정했습니다.
- ['Binance Effect' Means 41% Price Spike for Newly Listed Tokens](https://www.coindesk.com/markets/2023/01/06/binance-effect-means-41-price-spike-for-newly-listed-tokens) — CoinDesk(2023)가 Binance 상장 후 평균 가격 상승에 관한 연구를 요약한 기사입니다.
- [Research Report on the Listing Effect of Exchanges in 2024](https://www.chaincatcher.com/en/article/2175717) — ChainCatcher(2024)가 거래소별 상장 후 성과를 비교한 보고서입니다.
- [Crypto Exchange Coin Listing & Delisting Alert Bot (Free n8n Template)](https://www.coingecko.com/learn/crypto-exchange-coin-listing-alert-bot-free-n8n-template) — CoinGecko 튜토리얼: n8n과 CoinGecko API로 상장 / 상장폐지 알림 봇을 만드는 방법입니다.
- [Crypto New Coin Alerts: How to Monitor Exchange Listings on Binance and Coinbase](https://pagecrawl.io/blog/crypto-new-coin-listing-alerts-binance) — 페이지 모니터링 기반 상장 알림에 관한 PageCrawl 가이드입니다.

## 기여하기

[CONTRIBUTING.md](CONTRIBUTING.md)를 참고하세요. 요약: 한 줄에 한 항목, 정상 동작하는 링크, 중립적인 한 문장 설명, 제휴 링크 금지, 중단된 프로젝트 금지.

---

[Tokenearly](https://github.com/tokenearly)가 관리합니다. Tokenearly(토큰얼리)는 암호화폐 거래소의 토큰 상장 공지, 뉴스, X(트위터) 활동을 실시간으로 모니터링하고 알림을 보내는 플랫폼입니다. Binance, OKX, Bybit, Bitget, MEXC, Gate.io, HTX, KuCoin, Upbit, Bithumb 10개 거래소 공지(바이낸스와 Gate.io는 거래소 공식 WebSocket 상시 연결로 실시간 수신해 폴링 대기가 없고, 나머지 거래소는 고빈도 폴링)와 8개 뉴스 소스를 모니터링하고, 지정한 X 계정의 게시물·답글·리포스트·새 팔로우·프로필 사진과 소개 변경을 서브초(게시부터 감지까지 최단 50ms)로 추적해 키워드로 필터링한 뒤 Telegram, Bark, PushDeer, WeCom, DingTalk, Feishu, Webhook으로 한국어·영어·중국어 알림을 제공합니다.
