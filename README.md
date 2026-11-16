# Ignacio Bastos

**Tech Lead & Full-Stack Developer · AI & Automation**

I've spent ten years building web platforms, e-commerce, custom business software and system integrations. I take products from architecture to production, then keep them running. I care about the parts users never see, like data models, infrastructure and failure modes, and about the interface they do see.

🌐 [ignaciobastos.com](https://ignaciobastos.com) · ✉️ ignacio@softuo.com

---

### What I've built recently

**Multi-tenant booking & ordering SaaS** *(Softuo, private repo)*
Three products on one platform: table reservations for restaurants, appointment scheduling, and a QR digital menu with a visual editor. I designed and built it solo.
- Serverless backend: Python 3.12 on AWS Lambda behind an HTTP API, with DynamoDB, Cognito auth (roles and up to 5 users per business), S3 media, and SES email. All infrastructure is defined in CloudFormation.
- An availability engine handles split opening hours, closures per business or per staff member, buffers between services, lead times and capacity per time slot. It is unit-tested, and its JS twin powers the public demos.
- Scheduled reminders run on EventBridge, alongside per-tenant quotas and abuse limits.
- Self-service onboarding: sign-up, contract e-signature with an email verification code, Stripe payment and automatic activation.
- Each tenant gets a privacy policy generated from its own data, plus share previews (Open Graph images) for every public page.

**Cognitive stimulation platform** *(in pilot, private repo)*
A web app for therapists and older adults: 14 games with three difficulty levels, guided sessions, results and reports, and home access.
- Next.js 15, TypeScript, Prisma and PostgreSQL 17, with Caddy, all in Docker Compose on AWS Lightsail.
- It installs as a PWA and keeps working offline (up to 8 h) on tablets, then syncs when the connection returns.
- Playwright end-to-end tests cover accounts, accessibility and each game. Nightly database dumps run alongside instance snapshots.
- Every game has its own written spec and an independent audit.

**Marketing site & content pipeline** *(Softuo, private repo)*
A static site generator in Python with built-in SEO checks: canonical URLs, structured data, a sitemap, a news sitemap and an RSS feed. The build fails on any warning. Deploys go to AWS Amplify.

### Open source

**[FreeSoon](https://github.com/ignaciobastos/freesoon)**. A free WordPress plugin for "coming soon" and maintenance pages. It offers live visual editing, image or video backgrounds, countdowns and optional contact forms. No paid tier, ads or telemetry. GPL-2.0.

### Toolbox

- **Languages:** TypeScript, JavaScript, Python, PHP, SQL
- **Frontend:** React, Next.js, Tailwind CSS, Vite
- **Backend:** Node.js, FastAPI, Laravel, REST, OAuth 2.0, webhooks
- **Data:** PostgreSQL, MySQL, DynamoDB, Prisma, Supabase
- **Cloud & DevOps:** AWS (Lambda, API Gateway, DynamoDB, Cognito, S3, SES, EventBridge, CloudFormation, Amplify, Lightsail), Docker, Cloudflare, GitHub Actions
- **Testing:** Playwright, unit testing
- **CMS & e-commerce:** WordPress, WooCommerce, Shopify
- **AI & automation:** Claude API, OpenAI API, Gemini API, n8n
- **Design:** Figma, Photoshop, Blender
