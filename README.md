# Hi, I'm Sanjarbek Ashurboyev

**Backend Developer (Python / Django)** · Tashkent, Uzbekistan

I build backend systems with Python and Django: REST APIs, background jobs, Telegram bots,
real-time features and payments, and I deploy and run them on Linux servers with Docker,
nginx and HTTPS.

Currently a **backend intern at Yurideks** (an async Telegram transcription bot and a legal
workspace for lawyers) and a **freelance developer** of two live platforms.

**Open to backend roles**, remote or in Tashkent.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-sanjarbek--ashurboyev-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sanjarbek-ashurboyev/)
[![Email](https://img.shields.io/badge/Email-ashurboyevsanjarbek%40gmail.com-EA4335?logo=gmail&logoColor=white)](mailto:ashurboyevsanjarbek@gmail.com)

---

## Tech stack

| Area | Tools |
|---|---|
| **Language** | Python, SQL, TypeScript |
| **Backend** | Django, Django REST Framework, Django Channels (WebSockets), Celery, GraphQL (Graphene), aiogram, SQLAlchemy |
| **Data** | PostgreSQL (locking, row-level security, window functions), asyncpg, Redis, MinIO / S3 |
| **Auth & APIs** | JWT (SimpleJWT), role-based access control, OpenAPI / Swagger (drf-spectacular), Stripe |
| **Frontend** | React, TypeScript, Vite, TanStack Query |
| **DevOps** | Docker, Docker Compose, nginx, Caddy, Gunicorn, Linux servers, GitHub Actions CI |

---

## Production work

The code for these is private (client work); happy to walk through it in an interview.

### Hanyuban · [hanyuban.online](https://hanyuban.online)
Online Chinese school: public site, student area, admin panel and a Telegram bot for
homework and grading. Django REST API, React + TypeScript client, Celery and Redis.
Access grants are race-safe (row locks, version checks, idempotency keys); video is served
through signed Bunny Stream URLs. 1,700+ backend tests in CI; scripted deploys with a
database backup and rollback.
`Django REST Framework` `PostgreSQL` `Redis` `Celery` `aiogram` `React` `TypeScript` `Docker`

### AI Rivora · [@ai_rlvorabot](https://t.me/ai_rlvorabot)
Telegram bot that sells timed access to a private channel for Telegram Stars, with a React
admin panel. Idempotent payments, exactly-once broadcasts through a rate-limited Celery
queue, automatic expiry and removal, churn and conversion analytics. 890 tests in CI.
`aiogram` `Django REST Framework` `PostgreSQL` `Celery` `React`

### Yurideks (internship)
Async Telegram bot that transcribes lawyers' consultations: question answering over
transcripts with every quote checked against its source, a transcription API shared by the
bot and the website, and Google Calendar sync in the team's legal workspace.
`aiogram` `asyncpg` `PostgreSQL` `TypeScript` `LLM APIs`

---

## Featured projects

### [CineVault](https://github.com/sanjarbek-ashurboyev/Cinevault)
Movie reservation service. Browse movies and showtimes, pick seats, pay with Stripe.
Only verified users can book and each user sees only their own reservations; email
verification through Redis, async email delivery with Celery.
Deployed with Docker behind nginx and Caddy with automatic HTTPS. Covered by 114 tests.
[Design notes](https://github.com/sanjarbek-ashurboyev/Cinevault/blob/main/DESIGN.md): how double
booking is prevented and how the payment webhook and the seat-hold expiry avoid overwriting
each other.
`Django REST Framework` `PostgreSQL` `Redis` `Celery` `Stripe` `Docker`

### [ShopInventory](https://github.com/sanjarbek-ashurboyev/ShopInventory)
Inventory and point-of-sale system for a shoe shop. Scan barcodes with a phone camera,
track stock by size, sell for cash or card, print labels, and export daily reports to
Excel and PDF. Django REST API with a React + TypeScript frontend, covered by 72 tests.
`Django REST Framework` `React` `TypeScript` `PostgreSQL` `Docker`

### [Nova](https://github.com/sanjarbek-ashurboyev/Nova)
Multi-role e-commerce platform for the Uzbek social-commerce market. Sellers promote
products through referral links, operators work a shared order queue, and drivers handle
deliveries, each in their own workspace. Order status changes follow enforced rules, and
cancelled or returned orders put their stock back. Covered by 59 tests.
`Django` `Bootstrap`

### [OnlineChat](https://github.com/sanjarbek-ashurboyev/OnlineChat)
Real-time chat over WebSockets with online presence, JWT authentication and a REST API
for chat history. Covered by 48 tests, including WebSocket tests that run through the
full ASGI stack.
`Django Channels` `Redis` `PostgreSQL` `DRF`

---

## Starter templates

Reusable project skeletons I use to start new services quickly:
[Telegram bot](https://github.com/sanjarbek-ashurboyev/TgBotTemplate) (aiogram, SQLAlchemy, Alembic) ·
[Django + Docker](https://github.com/sanjarbek-ashurboyev/DjangoTemplate) ·
[Django + MinIO](https://github.com/sanjarbek-ashurboyev/DjangoMinIOTemplate)

---

**Languages:** Uzbek (native) · English (IELTS 7.5)
