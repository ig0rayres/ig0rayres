Hi, I'm Igor Ayres 👋
Technical Founder · Staff-Level Engineer · AI Systems Builder
I'm a technical founder with 15+ years of experience building SaaS platforms, automation systems, and AI-driven products. My recent work focuses on the intersection of AI, multi-tenant architecture, messaging, and complex billing workflow.

Most of the systems I build are designed to operate in production from day one, often replacing multiple disconnected tools with a single cohesive platform. I solve messy real-world operational problems: customer support scaling, HR automation, community engagement, and internal admin governance.

I usually work across the full product cycle: understanding the business problem, designing the architecture, modeling the database, and shipping the initial production version to real users.

📍 Brazil · 🌎 Open to US remote work · 📧 igor@hashia.com.br

What I Build
I build complete platforms, not isolated features. I care about the infrastructure that makes a product resilient and scalable.

Most of my projects include:

Agentic AI: Tool-calling loops, RAG workflows, prompt routing, and vision models (OpenAI, Gemini, Whisper).
Multi-tenant Architecture: Pure database-level isolation (RLS), RBAC, white-label support, and secure admin impersonation.
Messaging-First Products: Omnichannel inboxes, routing engines, automation flows, and headless WhatsApp APIs.
SaaS Billing: Complex lifecycle handling with Stripe/Asaas — webhooks, modular add-ons, trials, and pro-rata upgrades.
Modern Stack: Next.js, Laravel, Supabase, PostgreSQL, Vercel, Docker, and Filament.
Selected Projects
Some repositories are private as they are commercial products. I can share architecture walkthroughs or demos upon request.

Hello Paco — AI Omnichannel SaaS for Customer Service
Status: Private repository · Architecture walkthrough available

Hello Paco is a multi-tenant platform built to centralize WhatsApp, Instagram, email, and web chat. It combines omnichannel support with AI-assisted ticket routing and RAG-based knowledge retrieval.

I pushed data isolation down to PostgreSQL Row-Level Security and kept tenant-specific RAG inside pgvector, ensuring that customer data, tickets, and AI knowledge bases remain strictly scoped at the database layer. I also designed a "Buffet" billing model that allows B2B partners to provision headless WhatsApp instances while enforcing usage limits through a unified billing layer.

Engineering: Managed 120+ TS files, 40+ PostgreSQL tables, and messaging adapters for Evolution/WAHA.
AI: Integrated Google Gemini with pgvector for tenant-isolated RAG, ticket classification, and priority detection.
Infrastructure: Used Supabase Realtime and Zustand to synchronize agents with sub-200ms message delivery.
Stack: Next.js · React · TypeScript · Supabase · PostgreSQL (RLS/pgvector) · Gemini · Zustand · Asaas

Elyon — AI Workforce Management Platform
Status: Production deployment · Private repository

Elyon is an AI-powered ERP for HR, recruitment, and time tracking. It features a 47-tool agentic AI that operates with full parity across both the web admin panel and WhatsApp.

The AI isn't just a chatbot; it executes operations like opening job requisitions, checking department budgets, and extracting CV data. For legally sensitive contract generation, I deliberately bypassed the LLM in favor of a deterministic state machine to ensure 100% predictable outcomes for digital signatures.

Scale: Solo founder-engineer project with 53K+ lines of PHP, 163 classes, and 23 Eloquent models.
Optimization: Reduced AI token usage by ~70% using modular context loading that detects active business domains.
Governance: Implemented a contract lifecycle system with digital signatures (SHA-256), Brazilian legal text parsing, and audit trails.
Stack: Laravel · Filament · PostgreSQL · Supabase · GPT-4o · WhatsApp APIs · Docker · EasyPanel

Legendários — Gamified Community SaaS
Status: Active Production · Private repository

A multi-tenant platform for a global organization with 79+ chapters across 12 countries. It was built to solve a specific problem: keeping members engaged through validated real-world interaction.

The platform uses OpenAI Vision to validate photo proof of offline meetups before awarding XP. I architected the full gamification engine, internal marketplace, and commission workflows to run on a serverless edge architecture with database-level tenant isolation.

AI & Logic: Built AI anti-fraud validation and a gamification engine with 6 rank tiers and automated leaderboards.
Infrastructure: Designed chapter-level administration with PostgreSQL RLS to prevent data leakage across 12 countries.
Billing: Implemented Stripe subscription flows with pro-rata billing and referral payout workflows.
Stack: Next.js · TypeScript · Supabase · PostgreSQL (RLS) · Stripe · OpenAI Vision · Vercel

Ligare — Institutional Governance SaaS
Status: Private repository · Case study available

Ligare is a B2B2C operational hub for institutions managing member relationship and governed WhatsApp communications. It replaces fragmented personal chats with a managed institutional platform.

I rebuilt the admin impersonation engine from a risky DB-mutation approach into a stateless, cookie-based flow that preserves tenant context securely. I also automated WhatsApp provisioning through the Hello Paco API, triggering instance creation immediately upon payment confirmation.

Architecture: Implemented white-label subdomain routing via Next.js Edge Middleware.
Innovation: Shifted from raw messaging to governed, button-driven workflows for privacy and auditability.
Development: Built 28 routed pages and 20+ RLS-protected tables solo.
Stack: Next.js · TypeScript · Supabase · PostgreSQL · Asaas · WAHA · Hello Paco API

Technical Strengths
text
Copy
Product Architecture   Multi-tenant SaaS · White-label · RBAC · Impersonation engines
AI / LLM Systems       Agentic loops · RAG · Prompt routing · Vision · GPT-4o · Gemini
Messaging              WhatsApp (WAHA/Evolution) · Instagram · Email · Omnichannel
Backend                Laravel · Next.js Server Actions · Supabase · Queues · Cron
Database               PostgreSQL · RLS · pgvector · JSONB · Triggers · Indexing
Billing                Stripe · Asaas · Webhooks · Pro-rata logic · Add-on models
How I Work
I care deeply about the bridge between product strategy and engineering execution. I don't just build features; I build systems.

A lot of my work starts with architectural constraints:

Where should tenant isolation live to ensure zero data leakage?
Which workflow needs to be deterministic (Wizard), and which one can safely use AI (Agent)?
How will the system behave when we scale from 10 to 1,000 tenants?
I use AI heavily to speed up implementation and refactoring, but never as a replacement for architecture. The important work is deciding what should exist, where the boundaries are, and which trade-offs are safe for the product's long-term health.

Background
Before focusing on AI/SaaS, I spent years building businesses in technology, IoT, and operations. This includes Dot House, an IoT company that scaled across 4 cities in Brazil. This experience shaped me into an engineer who understands business models, unit economics, and operational workflows.

Let's Connect
