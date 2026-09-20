<div align="center">

# Sarvagya Singh

**Full-Stack &amp; Backend Engineer**

I build production web applications end to end — event-driven backends,
real-time systems, and the interfaces that sit on top of them.

**Delhi NCR, India** &nbsp;·&nbsp; Open to remote, worldwide

<a href="https://sarvagyasingh.space"><img src="https://img.shields.io/badge/Portfolio-111111?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" /></a>
<a href="https://www.linkedin.com/in/sarvagya-singh-1015722a4"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:sarvagya3555cc@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://leetcode.com/u/Sarvagyasingh_2004/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>

</div>

---

## What I build

**Backend and distributed systems.** REST APIs, services that talk to each other
over RabbitMQ instead of blocking on each other, WebSocket real-time layers,
payment integration with Razorpay and Stripe, and schema and query design across
PostgreSQL, MySQL and MongoDB.

**Frontend and product.** React and Next.js applications, Redux state
architecture, data-heavy dashboards and internal admin tools, and animation work
with GSAP and Three.js when the interface has to sell something.

**Getting it live.** Dockerised services behind nginx with TLS on cloud VMs, and
Next.js on Vercel. Every project below has a URL you can open right now.

Currently open to **full-time roles**, remote or in Delhi NCR, and to **selective
freelance work** — most often an API, a real-time feature, or a dashboard that
has outgrown whatever it started as.

---

## Featured projects

### Legwork — AI interview prep kit
**[Live demo](https://legwork-the-ai-interview-prep-kit-w.vercel.app)** &nbsp;·&nbsp; **[Code](https://github.com/Sarvagyasingh2004/Legwork-The-AI-Interview-Prep-Kit)**

Turns a job posting and a company URL into a researched prep kit: a company
brief, a role breakdown, a categorised question bank, flashcards and a
day-by-day study schedule.

What makes it more than a prompt wrapper is that it refuses to invent things.
The model has to quote the span of the posting every requirement came from, and
code verifies that span really appears there — anything it cannot prove is
discarded. Question coverage is then checked in code rather than by a model, and
gaps go back for a targeted second pass.

`Next.js 16` `Express 5` `MongoDB` `TypeScript` `Gemini 2.5 Flash` `Vitest` `Supertest`

### Eatlify — food ordering platform
**[Live demo](https://eatlify-food-ordering-microservices.vercel.app)** &nbsp;·&nbsp; **[Code](https://github.com/Sarvagyasingh2004/eatlify-food-ordering-microservices)**

A Swiggy-style ordering platform: six services — auth, restaurant, rider,
realtime, admin and utils — coordinating one order, built so any of them can
fail without taking the order with it. Retries, a dead-letter queue and health
checks; Redis caching cut DB reads ~60%.

Services talk over RabbitMQ rather than calling each other directly, so a slow
payment callback never blocks an order being placed. Live order and rider
tracking runs over Socket.IO, payments go through Razorpay and Stripe, and the
whole stack comes up with Docker Compose behind nginx with TLS.

`Node` `TypeScript` `RabbitMQ` `Socket.IO` `Redis` `Docker` `nginx`

### Skein — real-time chat
**[Live demo](https://skein-frontend-kappa.vercel.app)** &nbsp;·&nbsp; **[Frontend](https://github.com/Sarvagyasingh2004/Skein-frontend)** &nbsp;·&nbsp; **[Backend](https://github.com/Sarvagyasingh2004/Skein-backend)**

Passwordless chat — you sign in with an emailed OTP, then get live messages,
typing indicators and read receipts.

Three services behind it. Email is decoupled over RabbitMQ so a slow SMTP
handshake never holds up a login, and failed sends land in a dead-letter queue
with a `peek` / `replay` / `purge` tool rather than disappearing. Socket.IO is
scaled through the Redis adapter, so presence survives more than one instance.

`Next.js 16` `TypeScript` `Node.js` `MongoDB` `Redis` `RabbitMQ` `Socket.IO`

### SaaSify-AI — AI content platform
**[Live demo](https://saasify-ai.vercel.app)** &nbsp;·&nbsp; **[Code](https://github.com/Sarvagyasingh2004/SaaSify-AI)**

A PERN-stack AI SaaS with article and image generation and a résumé scorer that
reads an uploaded PDF and reports back against a role.

`React` `Node.js` `Express` `PostgreSQL` `Gemini` `Clerk` `Cloudinary`

### Portfolio — sarvagyasingh.space
**[Live demo](https://sarvagyasingh.space)** &nbsp;·&nbsp; **[Code](https://github.com/Sarvagyasingh2004/sarvagya-singh-portfolio)**

Next.js and React Three Fiber: a scroll-driven WebGL sequence, a theme that
follows your local clock, and a Gemini-backed assistant that answers questions
about my work from a curated corpus instead of improvising.

`Next.js` `TypeScript` `React Three Fiber` `GSAP` `MongoDB Atlas` `Gemini`

### Velvet Pour — animated marketing site
**[Live demo](https://gsap-velvet-pour.vercel.app)** &nbsp;·&nbsp; **[Code](https://github.com/Sarvagyasingh2004/gsap_velvet_pour)**

A cocktail bar landing page built to practise scroll-driven animation — pinned
sections, timeline-sequenced reveals and a responsive layout that reworks the
choreography rather than just reflowing it.

`React` `GSAP` `Tailwind CSS` `Vite`

---

## Experience

### Kraftshala &nbsp;·&nbsp; Software Developer, Full-stack &nbsp;·&nbsp; Mar – Sep 2026 &nbsp;·&nbsp; Delhi

Six months owning features end to end on the internal operations platform a real
team used every day — **331 commits** across a Node/TypeScript/MySQL backend and a
React/Redux frontend.

The piece I'd most want to walk you through is a **self-service alerting
platform**. Teams define a SQL rule and a threshold through an API, a per-minute
cron evaluates them and posts to Google Chat. Because the SQL is user-supplied it
needed a validation layer that permits only `SELECT` and `WITH` and blocks DDL and
DML. A few months later another engineer shipped two of their own alert features
on top of it without needing me. That's the part I'm proud of — not the feature,
the fact that it became something someone else could build on.

Elsewhere on that platform: a **bulk Excel upload engine** that validates, parses
and deduplicates 1,000+ records per upload and cut the manual work by ~80%;
**Google OAuth 2.0 SSO** plus HTTP 409 conflict detection that stopped
double-bookings across the Zoom, CRM and payment integrations; and a **Placements
Opportunity Tracker** with transactional owner reassignment, a reusable audit log,
and a listing query rewritten from six subqueries down to one join.

I also broke production once: an SSO restriction I added locked some admins out of
password sign-in. I caught it and rolled it back inside 48 hours. I'd rather say
that up front than have you find it.

### BWS &nbsp;·&nbsp; Full-Stack Developer &nbsp;·&nbsp; Jul – Dec 2025 &nbsp;·&nbsp; Remote

My first fully remote role, maintaining a production website across frontend and
backend. I built and deployed an **AI chatbot** on the company site with the MERN
stack that handles 100+ visitor queries without a human, a **"Request a Callback"**
flow that syncs leads straight into Zoho CRM over REST (200 of them so far), and a
WhatsApp community integration. I also took the site from **~8s to ~2s** through
performance and on-page SEO work.

### Coding Blocks &nbsp;·&nbsp; Teaching Assistant &nbsp;·&nbsp; May – Aug 2024 &nbsp;·&nbsp; Noida

Mentored 100+ students through Java, data structures and algorithms in doubt
sessions and one-on-one code reviews. Reading other people's code that closely,
that often, is where I learned what actually makes code easy to follow.

<table>
<tr><td><b>~40s → ~400ms</b></td><td>Dashboard queries rebuilt around a deferred join, and the inflated pagination counts fixed with them &nbsp;<sub>Kraftshala</sub></td></tr>
<tr><td><b>~2k → ~400k/day</b></td><td>Calendar-invite throughput, after decoupling event creation from delivery via AWS SES behind default-off feature flags &nbsp;<sub>Kraftshala</sub></td></tr>
<tr><td><b>1,000+ rows</b></td><td>Per bulk Excel upload, validated before any write, processed through a Bull queue &nbsp;<sub>Kraftshala</sub></td></tr>
<tr><td><b>~8s → ~2s</b></td><td>Page load on a production site, through performance and on-page SEO work &nbsp;<sub>BWS</sub></td></tr>
</table>

---

## Stack

**Languages** &nbsp; TypeScript · JavaScript · Python · Java · SQL

**Frontend** &nbsp; React · Next.js · Redux · Tailwind CSS · Material-UI · GSAP · Three.js

**Backend** &nbsp; Node.js · Express · REST APIs · Socket.IO · RabbitMQ · JWT · OAuth 2.0

**Data** &nbsp; PostgreSQL · MySQL · MongoDB · Redis · query optimisation and indexing

**Infrastructure** &nbsp; Docker · nginx · AWS EC2 · Oracle Cloud · Vercel · Git

---

<div align="center">

Currently deepening **data structures, algorithms and system design**, and
writing the systems above up as proper case studies.

**[sarvagya3555cc@gmail.com](mailto:sarvagya3555cc@gmail.com)** &nbsp;·&nbsp; **[LinkedIn](https://www.linkedin.com/in/sarvagya-singh-1015722a4)** &nbsp;·&nbsp; **[sarvagyasingh.space](https://sarvagyasingh.space)**

</div>
