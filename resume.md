# Xiaozhe Bai

**Full-stack Software Engineer focused on cross-border e-commerce systems.**

Full-stack · Cross-border commerce · Chongqing, China

[jeff2025white@gmail.com](mailto:jeff2025white@gmail.com) · [Upwork](https://www.upwork.com/freelancers/~01b3f98c7ba6c47674) · [Intro video](https://youtube.com/shorts/cTRGQABL8Tg) · [Website](https://webpans.com/) · [PDF](https://webpans.com/Xiaozhe-Bai-Resume.pdf)

---

## 01 About

Full-stack engineer with 7 years at Alibaba, building distributed systems for AliExpress’s global cross-border business. Day-to-day work centers on order and transaction systems, merchant open APIs, high-concurrency optimization, and multi-region deployment — with personal projects spanning web consoles, Laravel marketplaces, and Android clients end to end.

## 02 Skills

`Java` `Go` `Python` `PHP` `Kotlin` `Microservices` `MySQL` `PostgreSQL` `Redis` `Kafka` `RocketMQ` `API gateway` `Distributed locks` `DB sharding` `FastAPI` `Django` `Laravel` `Blade` `Phaser` `Android` `Payment` `LLM integration` `OCR / computer vision`

## 03 Experience

### Full-stack engineer

*Alibaba · AliExpress · 7 years*

Owned services for order, settlement, and merchant open APIs on a global cross-border marketplace, from high-concurrency tuning to multi-region deployment. See [order & settlement](#cross-border-order--settlement-backend) and [open API gateway](#merchant-open-api-gateway) below.

## 04 Education & languages

### Shanghai Jiao Tong University

*Bachelor of Applied Science (BASc), Computer Science · 2015 – 2019*

### Languages

- Chinese — native or bilingual
- English — fluent (written)

## 05 Projects

### Employer work

> Selected work from a previous employer. Descriptions stay high-level and do not disclose confidential business data, internal metrics, or proprietary code.

### Cross-border Order & Settlement Backend

*Full-stack Software Engineer · AliExpress / Alibaba*

- Owned the order/settlement pipeline for a global cross-border marketplace: state machine, settlement split, idempotent writes, and merchant async notifications.
- Prevented oversell and duplicate orders under flash-sale traffic with MQ decoupling, sharding, distributed locks, and rate limits; stabilized peaks via hot-cache and slow-SQL tuning across multi-region deploy.

**Stack:** Java · Microservices · MySQL · Redis · Apache Kafka

![Architecture diagram for order core, settlement, Redis, MySQL sharding, and async messaging](https://webpans.com/images/project2/order-settlement.png)
*Architecture overview*

### Merchant Open API Gateway

*Full-stack Software Engineer · AliExpress / Alibaba*

- Built merchant open APIs for third-party ISVs to batch-query orders, products, and funds behind auth, permission, quota, and tracing.
- Isolated open-API traffic from core commerce with throttling and graceful degradation so partner integrations stayed reliable without hurting checkout.

**Stack:** Go · API gateway · Microservices · Redis · Performance optimization

![Architecture diagram for open API gateway, auth, quota, circuit breaker, and Redis cache](https://webpans.com/images/project2/open-api-gateway.png)
*Gateway architecture*

### Personal projects

> Personal projects. They do not use or disclose any former employer’s confidential business information. Private repositories: access can be granted on request. Public repositories are linked below.

### NPC2

*Motive-driven generative agents · personal project*

[github.com/jeff2025white/npc2](https://github.com/jeff2025white/npc2) · [Demo video](https://youtu.be/Dw7ou_apSb4) · Private

- Built a sandbox where agents act from competing motives and skills, not fixed scripts; routine pathfinding stays local, while dialogue, conflict, and decisions call an LLM router.
- Shipped a web console to edit motives, relations, and skills and assign different models per character; demo video available, private repo on request.

**Stack:** Python · Django · Phaser · LLM routing

![NPC2 sandbox with three characters and live motive labels](https://webpans.com/images/npc2/%E6%88%AA%E5%B1%8F2026-11-04%2011.40.00.png)
*Live sandbox*

![NPC2 motive editor with sensitivity tiers and social relations](https://webpans.com/images/npc2/%E6%88%AA%E5%B1%8F2026-11-04%2011.45.41.png)
*Motive editor*

### Gather + Flash

*In-store capture and quick-commerce retail insight · personal project*

[github.com/jeff2025white/gather](https://github.com/jeff2025white/gather) · [github.com/jeff2025white/flash](https://github.com/jeff2025white/flash) · Private

- Built an edge capture system that drives a mirrored phone (frames in, HID touch out) to scrape in-store shelf cards for quick-commerce pricing and sales intel.
- Control center batches capture and OCR into price, sales, brand, and spec; Flash turns that catalog into district assortment, price, and sales boards.
- One batch parsed 5,207 screenshots in 2 h 19 min, about 370 frames every 10 minutes.

**Stack:** Python · FastAPI · PostgreSQL · SQLite · PaddleOCR · MQTT · RP2040 · Kotlin

![Gather live cast console with phone stream and HID touch controls](https://webpans.com/images/gather/%E6%88%AA%E5%B1%8F2026-11-04%2011.21.33.png)
*Gather · live cast*

![Gather capture task panel with batch history](https://webpans.com/images/gather/%E6%88%AA%E5%B1%8F2026-11-04%2011.22.12.png)
*Gather · capture tasks*

![Gather item table of parsed product cards](https://webpans.com/images/gather/%E6%88%AA%E5%B1%8F2026-11-04%2011.22.39.png)
*Gather · parsed cards*

![Flash district board with assortment gaps and price suggestions](https://webpans.com/images/flash/%E6%88%AA%E5%B1%8F2026-11-01%2013.57.15.png)
*Flash · district board*

![Flash competitor sales comparison](https://webpans.com/images/flash/%E6%88%AA%E5%B1%8F2026-11-01%2013.56.50.png)
*Flash · competitor sales*

### Online Auction Platform

*Production-oriented timed bidding marketplace · personal project*

- Built a timed auction marketplace (catalog, bidding, Buy It Now, history) with auth-gated bids.
- Made concurrent bidding safe with transactions and optimistic locking plus bid-increment rules; a scheduler closes lots and picks winners.
- Hardened for production with CSRF/policies, rate-limited bid APIs, Redis cache/queues, and role-based admin.

**Stack:** Laravel · PHP · MySQL · Redis · Queues · Scheduler · Blade

![Lotboard auction catalog with categories, filters, and timed lots](https://webpans.com/images/auction/lotboard-catalog.png)
*Auction catalog*

### Live Streaming Android Client

*Multi-module live / short-video / social app · personal project*

[github.com/jeff2025white/live-prj-h5-android-p](https://github.com/jeff2025white/live-prj-h5-android-p) · Public

- Shipped a multi-module Android live/social client with login, live rooms, short video, feed, messaging, and wallet against a REST backend.
- Live rooms combine RTC and IM for gifts, danmaku, and DMs; open/close live and room state stay in sync with backend APIs and tokens.
- Modularized with ARouter and product flavors; integrated pay, push, maps, and short-video upload for a releasable APK.

**Stack:** Android · Java · REST API · OkHttp / OkGo · ARouter · Agora RTC · Tencent IM

![Live hall feed with category tabs and live room grid](https://webpans.com/images/live/1.jpg)
*Live · hall*

![Live room with streamer video, chat, gifts, and viewer overlays](https://webpans.com/images/live/2.jpg)
*Live · room*

![Profile page with wallet, VIP, and certification center](https://webpans.com/images/live/3.jpg)
*Live · profile*

---

Open to full-stack and cross-border commerce work · [jeff2025white@gmail.com](mailto:jeff2025white@gmail.com)
