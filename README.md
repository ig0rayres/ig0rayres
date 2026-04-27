# Hi, I'm Igor Ayres 👋

### Technical Founder · Staff-Level Engineer · AI Systems Builder

I'm a technical founder with 15+ years of experience building SaaS platforms, automation systems, and AI-driven products. My recent work focuses on the intersection of **AI, multi-tenant architecture, messaging, and complex billing workflows**.

Most of the systems I build are designed to operate in production from day one, often replacing multiple disconnected tools with a single cohesive platform. I solve messy real-world operational problems: customer support scaling, HR automation, community engagement, and internal admin governance.

I usually work across the full product cycle: understanding the business problem, designing the architecture, modeling the database, and shipping the initial production version to real users.

📍 Brazil · 🌎 Open to US remote work · 📧 [igor@hashia.com.br](mailto:igor@hashia.com.br)

---

## 🚀 What I Build

I build complete platforms, not isolated features. I care about the infrastructure that makes a product resilient and scalable.

Most of my projects include:

*   **Agentic AI:** Tool-calling loops, RAG workflows, prompt routing, and vision models (OpenAI, Gemini, Whisper).
*   **Multi-tenant Architecture:** Pure database-level isolation (RLS), RBAC, white-label support, and secure admin impersonation.
*   **Messaging-First Products:** Omnichannel inboxes, routing engines, automation flows, and headless WhatsApp APIs.
*   **SaaS Billing:** Complex lifecycle handling with Stripe/Asaas — webhooks, modular add-ons, trials, and pro-rata upgrades.
*   **Modern Stack:** Next.js, Laravel, Supabase, PostgreSQL, Vercel, Docker, and Filament.

---

## 🏗️ Selected Projects

*Some repositories are private as they are commercial products. I can share architecture walkthroughs or demos upon request.*

### [Hello Paco](https://github.com/ig0rayres/hello_paco) — AI Omnichannel SaaS
**Status:** Private repository · Architecture walkthrough available

Hello Paco is a multi-tenant platform built to centralize WhatsApp, Instagram, email, and web chat. It combines omnichannel support with AI-assisted ticket routing and RAG-based knowledge retrieval. I pushed data isolation down to **PostgreSQL Row-Level Security** and kept tenant-specific RAG inside **pgvector**.

*   **Engineering:** Managed 120+ TS files, 40+ PostgreSQL tables, and messaging adapters for Evolution/WAHA.
*   **AI:** Integrated Google Gemini with pgvector for tenant-isolated RAG and priority detection.
*   **Infrastructure:** Used Supabase Realtime and Zustand for sub-200ms message delivery.

**Stack:** Next.js · React · TypeScript · Supabase · PostgreSQL · Gemini · Zustand · Asaas

---

### [Elyon](https://elyon.hashia.com.br) — AI Workforce Management Platform
**Status:** Production deployment · Private repository

Elyon is an AI-powered ERP for HR, recruitment, and time tracking. It features a **47-tool agentic AI** that operates with full parity across both the web admin panel and WhatsApp.

*   **Scale:** Solo founder-engineer project with 53K+ lines of PHP, 163 classes, and 23 Eloquent models.
*   **Optimization:** Reduced AI token usage by ~70% using modular context loading.
*   **Governance:** Contract lifecycle system with digital signatures (SHA-256) and audit trails.

**Stack:** Laravel · Filament · PostgreSQL · Supabase · GPT-4o · WhatsApp APIs · Docker

---

### [Legendários](https://github.com/ig0rayres/profissional_legendario) — Gamified Community SaaS
**Status:** Active Production · Private repository

A multi-tenant platform for a global organization with 79+ chapters across 12 countries. Uses **OpenAI Vision** to validate photo proof of offline meetups before awarding XP.

*   **AI & Logic:** AI anti-fraud validation and a gamification engine with 6 rank tiers.
*   **Infrastructure:** Chapter-level administration with PostgreSQL RLS to prevent data leakage.
*   **Billing:** Stripe subscription flows with pro-rata billing and referral payout workflows.

**Stack:** Next.js · TypeScript · Supabase · PostgreSQL · Stripe · OpenAI Vision · Vercel

---

### [Ligare](https://github.com/ig0rayres/ligare) — Institutional Governance SaaS
**Status:** Private repository · Case study available

Ligare is a B2B2C operational hub for institutions. I rebuilt the admin impersonation engine from a risky DB-mutation approach into a stateless, cookie-based flow that preserves tenant context securely.

*   **Architecture:** White-label subdomain routing via Next.js Edge Middleware.
*   **Innovation:** Automated WhatsApp provisioning triggered immediately upon payment confirmation.

**Stack:** Next.js · TypeScript · Supabase · PostgreSQL · Asaas · WAHA

---

## 🧠 Technical Strengths

```text
Product Architecture   Multi-tenant SaaS · White-label · RBAC · Impersonation engines
AI / LLM Systems       Agentic loops · RAG · Prompt routing · Vision · GPT-4o · Gemini
Messaging              WhatsApp (WAHA/Evolution) · Instagram · Email · Omnichannel
Backend                Laravel · Next.js Server Actions · Supabase · Queues · Cron
Database               PostgreSQL · RLS · pgvector · JSONB · Triggers · Indexing
Billing                Stripe · Asaas · Webhooks · Pro-rata logic · Add-on models
