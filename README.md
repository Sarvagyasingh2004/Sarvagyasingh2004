<img src="assets/banner.png" width="100%" alt="Sarvagya Singh — Full-Stack &amp; Backend Engineer" />

<div align="center">

I build production web applications end to end — **event-driven backends, real-time systems,**
**and the interfaces that sit on top of them.**

<a href="https://sarvagyasingh.space"><img src="https://img.shields.io/badge/Portfolio-8B5CF6?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" /></a>
<a href="https://www.linkedin.com/in/sarvagya-singh-1015722a4"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:sarvagya3555cc@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://leetcode.com/u/Sarvagyasingh_2004/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>

</div>

<br/>

## 🛠 &nbsp;What I build

**Backend and distributed systems** &nbsp;—&nbsp; REST APIs, services that talk over RabbitMQ instead of
blocking on each other, WebSocket real-time layers, payments with Razorpay and Stripe, and schema
and query design across PostgreSQL, MySQL and MongoDB.

**Frontend and product** &nbsp;—&nbsp; React and Next.js applications, Redux state architecture,
data-heavy dashboards and internal admin tools, and animation work with GSAP and Three.js when the
interface has to sell something.

**Getting it live** &nbsp;—&nbsp; Dockerised services behind nginx with TLS on cloud VMs, and Next.js
on Vercel. Every project below has a URL you can open right now.

<br/>

<div align="center">

<img src="https://skillicons.dev/icons?i=ts,js,python,java,react,nextjs,redux,tailwind,threejs,nodejs&perline=10" alt="languages and frontend" />
<img src="https://skillicons.dev/icons?i=express,mongodb,postgres,mysql,redis,rabbitmq,docker,nginx,aws,git&perline=10" alt="backend and infrastructure" />

</div>

<br/>

## 🚀 &nbsp;Featured projects

<table cellpadding="16">
<tr>
<td width="50%" valign="top">
<div align="center">
<br/>
<a href="https://legwork-the-ai-interview-prep-kit-w.vercel.app"><img src="assets/legwork.png" width="94%" alt="Legwork" /></a>
<h3>Legwork</h3>
<p><em>AI interview prep kit</em></p>
<p>Turns a job posting and a company URL into a researched prep kit. The model must quote the span every requirement came from, and code verifies it really exists — anything unproven is discarded. Coverage is checked in code, not by a model.</p>
<img src="https://skillicons.dev/icons?i=nextjs,express,mongodb,ts,tailwind,vercel" height="34" alt="stack" />
<br/><br/>
<a href="https://legwork-the-ai-interview-prep-kit-w.vercel.app"><img src="https://img.shields.io/badge/Live_Demo-8B5CF6?style=for-the-badge&logo=vercel&logoColor=white" alt="Live demo" /></a> <a href="https://github.com/Sarvagyasingh2004/Legwork-The-AI-Interview-Prep-Kit"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" alt="Source code" /></a>
<br/>
</div>
</td>
<td width="50%" valign="top">
<div align="center">
<br/>
<a href="https://eatlify-food-ordering-microservices.vercel.app"><img src="assets/eatlify-login.png" width="94%" alt="Eatlify" /></a>
<h3>Eatlify</h3>
<p><em>Food ordering platform</em></p>
<p>Six services coordinating one order, built so any of them can fail without taking the order with it. Retries, a dead-letter queue and health checks; Redis caching cut DB reads ~60%. Live rider tracking over Socket.IO, payments via Razorpay and Stripe.</p>
<img src="https://skillicons.dev/icons?i=nodejs,ts,rabbitmq,redis,mongodb,docker,nginx" height="34" alt="stack" />
<br/><br/>
<a href="https://eatlify-food-ordering-microservices.vercel.app"><img src="https://img.shields.io/badge/Live_Demo-8B5CF6?style=for-the-badge&logo=vercel&logoColor=white" alt="Live demo" /></a> <a href="https://github.com/Sarvagyasingh2004/eatlify-food-ordering-microservices"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" alt="Source code" /></a>
<br/>
</div>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<div align="center">
<br/>
<a href="https://skein-frontend-kappa.vercel.app"><img src="assets/skein.png" width="94%" alt="Skein" /></a>
<h3>Skein</h3>
<p><em>Real-time chat</em></p>
<p>Passwordless chat — sign in with an emailed OTP, then live messages, typing indicators and read receipts. Email is decoupled over RabbitMQ, failed sends land in a dead-letter queue with peek/replay/purge tooling, and Socket.IO scales through the Redis adapter.</p>
<img src="https://skillicons.dev/icons?i=nextjs,ts,nodejs,mongodb,redis,rabbitmq" height="34" alt="stack" />
<br/><br/>
<a href="https://skein-frontend-kappa.vercel.app"><img src="https://img.shields.io/badge/Live_Demo-8B5CF6?style=for-the-badge&logo=vercel&logoColor=white" alt="Live demo" /></a><br/><br/><a href="https://github.com/Sarvagyasingh2004/Skein-frontend"><img src="https://img.shields.io/badge/Frontend-181717?style=for-the-badge&logo=github&logoColor=white" alt="Frontend" /></a> <a href="https://github.com/Sarvagyasingh2004/Skein-backend"><img src="https://img.shields.io/badge/Backend-181717?style=for-the-badge&logo=github&logoColor=white" alt="Backend" /></a>
<br/>
</div>
</td>
<td width="50%" valign="top">
<div align="center">
<br/>
<a href="https://saasify-ai.vercel.app"><img src="assets/saasify.png" width="94%" alt="SaaSify&#8209;AI" /></a>
<h3>SaaSify&#8209;AI</h3>
<p><em>AI content platform</em></p>
<p>A PERN-stack AI SaaS with article and image generation, plus a r&eacute;sum&eacute; scorer that reads an uploaded PDF and reports back against a role.</p>
<img src="https://skillicons.dev/icons?i=react,nodejs,express,postgres,vercel" height="34" alt="stack" />
<br/><br/>
<a href="https://saasify-ai.vercel.app"><img src="https://img.shields.io/badge/Live_Demo-8B5CF6?style=for-the-badge&logo=vercel&logoColor=white" alt="Live demo" /></a> <a href="https://github.com/Sarvagyasingh2004/SaaSify-AI"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" alt="Source code" /></a>
<br/>
</div>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<div align="center">
<br/>
<a href="https://sarvagyasingh.space"><img src="assets/portfolio.png" width="94%" alt="Portfolio" /></a>
<h3>Portfolio</h3>
<p><em>sarvagyasingh.space</em></p>
<p>Next.js and React Three Fiber — a scroll-driven WebGL sequence, a theme that follows your local clock, and a Gemini-backed assistant that answers from a curated corpus instead of improvising.</p>
<img src="https://skillicons.dev/icons?i=nextjs,ts,threejs,tailwind,mongodb,vercel" height="34" alt="stack" />
<br/><br/>
<a href="https://sarvagyasingh.space"><img src="https://img.shields.io/badge/Live_Demo-8B5CF6?style=for-the-badge&logo=vercel&logoColor=white" alt="Live demo" /></a> <a href="https://github.com/Sarvagyasingh2004/sarvagya-singh-portfolio"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" alt="Source code" /></a>
<br/>
</div>
</td>
<td width="50%" valign="top">
<div align="center">
<br/>
<a href="https://gsap-velvet-pour.vercel.app"><img src="assets/velvet.png" width="94%" alt="Velvet Pour" /></a>
<h3>Velvet Pour</h3>
<p><em>Animated marketing site</em></p>
<p>A cocktail bar landing page built to practise scroll-driven animation — pinned sections, timeline-sequenced reveals, and a responsive layout that reworks the choreography rather than just reflowing it.</p>
<img src="https://skillicons.dev/icons?i=react,tailwind,vite,js" height="34" alt="stack" />
<br/><br/>
<a href="https://gsap-velvet-pour.vercel.app"><img src="https://img.shields.io/badge/Live_Demo-8B5CF6?style=for-the-badge&logo=vercel&logoColor=white" alt="Live demo" /></a> <a href="https://github.com/Sarvagyasingh2004/gsap_velvet_pour"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" alt="Source code" /></a>
<br/>
</div>
</td>
</tr>
</table>

<br/>

## 💼 &nbsp;Experience

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

<br/>

<div align="center">

Currently deepening **data structures, algorithms and system design**, and writing the systems above
up as proper case studies.

### Get in touch

<a href="mailto:sarvagya3555cc@gmail.com"><img src="https://img.shields.io/badge/sarvagya3555cc@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://www.linkedin.com/in/sarvagya-singh-1015722a4"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>

</div>

<img src="assets/footer.png" width="100%" alt="Get in touch" />
