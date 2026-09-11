<div align="center">

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=25&pause=1400&color=8B5CF6&center=true&vCenter=true&width=680&height=45&lines=Full-stack+engineer%2C+backend-leaning;I+build+the+boring+infrastructure;that+other+people+build+on." alt="Full-stack engineer — I build the boring infrastructure that other people build on" />

<br />

**Delhi NCR, India** &nbsp;·&nbsp; B.Tech CSE @ MAIT (GGSIPU), 2026 &nbsp;·&nbsp; 9.2 CGPA

<!-- sarvagyasingh.space is still a Hostinger parking page. The moment Vercel +
     DNS are done, swap the href below for https://sarvagyasingh.space and change
     the label back to sarvagyasingh.space. -->
<a href="https://github.com/Sarvagyasingh2004/sarvagya-singh-portfolio"><img src="https://img.shields.io/badge/Portfolio-source-8B5CF6?style=for-the-badge&logo=github&logoColor=white" alt="Portfolio source" /></a>
<a href="https://www.linkedin.com/in/sarvagya-singh-1015722a4"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://leetcode.com/u/Sarvagyasingh_2004/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
<a href="mailto:sarvagya3555cc@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email sarvagya3555cc@gmail.com" /></a>

</div>

---

## What I actually do

Two full-stack roles and a teaching assistantship since 2024, alongside a B.Tech
in CSE at MAIT that I finish in 2026 (9.2 CGPA, top 25 in GGSIPU). Backend-leaning
— but I've usually shipped the frontend for whatever I built on the backend.

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

## Things I've built

| Project | What makes it interesting | Built with |
|---|---|---|
| **[Eatlify](https://github.com/Sarvagyasingh2004/eatlify-food-ordering-microservices)** — food delivery microservices | Six services coordinating one order, built so any of them can fail without taking the order with it. Retries, a dead-letter queue and health checks; Redis caching cut DB reads ~60%. | `Node` `TypeScript` `RabbitMQ` `Socket.IO` `Redis` `Docker` |
| **Skein** — real-time chat &nbsp;·&nbsp; [frontend](https://github.com/Sarvagyasingh2004/Skein-frontend) &nbsp;·&nbsp; [backend](https://github.com/Sarvagyasingh2004/Skein-backend) | RabbitMQ sits *behind* the WebSocket layer instead of the socket writing straight to the database — which is what makes acknowledgements and offline delivery actually work. | `Next.js` `TypeScript` `MongoDB` `Redis` `RabbitMQ` |
| **[SaaSify-AI](https://github.com/Sarvagyasingh2004/SaaSify-AI)** | Two LLM providers behind one adapter, so swapping or adding a model is a config change rather than a rewrite. | `React` `Node` `PostgreSQL` `OpenAI` `Claude` |
| **[My portfolio](https://github.com/Sarvagyasingh2004/sarvagya-singh-portfolio)** | Next.js 16 + React Three Fiber. A scroll-driven WebGL constellation, a Gemini-backed assistant, and a theme that follows your local clock. | `Next.js` `R3F` `GSAP` `Gemini` |

---

## Stack

<div align="center">

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white)

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white)

</div>

---

## The numbers

<div align="center">

<!-- github-readme-stats' shared instance answers 503, and the trophy and
     activity-graph apps answer 402 (their Vercel quota is spent). These cards
     are the ones that actually respond. -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Sarvagyasingh2004&theme=github_dark" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Sarvagyasingh2004&theme=default" alt="profile details" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Sarvagyasingh2004&theme=github_dark" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Sarvagyasingh2004&theme=default" alt="repos per language" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Sarvagyasingh2004&theme=github_dark" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Sarvagyasingh2004&theme=default" alt="most commit language" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Sarvagyasingh2004&theme=github_dark" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Sarvagyasingh2004&theme=default" alt="stats" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=Sarvagyasingh2004&theme=github_dark" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=Sarvagyasingh2004&theme=default" alt="productive time" />
</picture>

<br />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=Sarvagyasingh2004&hide_border=true&theme=tokyonight&background=00000000&ring=8B5CF6&fire=8B5CF6&currStreakLabel=8B5CF6" />
  <img src="https://streak-stats.demolab.com?user=Sarvagyasingh2004&hide_border=true&background=00000000&ring=7C3AED&fire=7C3AED&currStreakLabel=7C3AED" height="165" alt="Contribution streak" />
</picture>

<br /><br />

<!-- Generated hourly by .github/workflows/snake.yml -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Sarvagyasingh2004/Sarvagyasingh2004/output/snake-dark.svg" />
  <img src="https://raw.githubusercontent.com/Sarvagyasingh2004/Sarvagyasingh2004/output/snake.svg" alt="A snake eating my contribution graph" />
</picture>

</div>

---

<div align="center">

**Open to full-time backend or full-stack roles** — Delhi NCR, hybrid, or fully remote.

Currently deepening DSA and system design, and writing the systems above up as case studies.

<a href="https://www.linkedin.com/in/sarvagya-singh-1015722a4"><img src="https://img.shields.io/badge/Get%20in%20touch-8B5CF6?style=for-the-badge&logo=linkedin&logoColor=white" alt="Get in touch" /></a>

</div>
