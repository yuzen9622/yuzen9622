# Hi, I'm Yuzen 👋

> Student developer 

Information Management student at **National Taichung University of Science and Technology (NTCUST)**, with a focus on building practical full-stack systems end-to-end — from authentication flows to real-time data pipelines to browser extensions.

I build the part of the system you only notice when it's gone.

---

## 🔭 Currently Focused On

- **Real-time systems** — event-driven architecture, pub/sub patterns, latency optimization
- **Authentication & security** — JWT, session management, middleware design
- **Frontend performance** — rendering strategy, bundle optimization, perceived performance
- **LLM integration** — bringing AI into browser-based workflows with BYOK (bring-your-own-key) models

---

## 🛠️ Tech Stack

**Proficient**
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white&style=flat-square)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=next.js&logoColor=white&style=flat-square)
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black&style=flat-square)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white&style=flat-square)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white&style=flat-square)

**Familiar**
![Express](https://img.shields.io/badge/Express-000000?logo=express&logoColor=white&style=flat-square)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white&style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white&style=flat-square)
![C++](https://img.shields.io/badge/C++-00599C?logo=c%2B%2B&logoColor=white&style=flat-square)

---

## 🚀 Featured Projects

### 💬 [chat.to](https://github.com/yuzen9622/chat.to) — Real-time chat, built the way modern chat should be

A full-featured real-time chat application with group rooms, typing indicators, and media uploads.

**Stack:** Next.js (API Routes) · TypeScript · Supabase · Ably · NextAuth · Cloudinary

**What I built & why it's interesting:**
- **Real-time via Ably pub/sub** instead of rolling my own WebSocket server — lets the app scale horizontally on Vercel's serverless runtime without long-lived connections on the origin
- **Session-based auth with NextAuth**, integrated into API routes and Ably channel authorization so users can only subscribe to rooms they belong to
- **Media uploads offloaded to Cloudinary** via signed uploads, keeping large payloads out of the API layer entirely
- **Typing indicators** implemented as ephemeral Ably presence events (not persisted), which was a deliberate trade-off between UX fidelity and DB write pressure

🔗 **Live demo:** https://chat-to-sage.vercel.app/introduce

---

### 🔤 [TermExpander-ai](https://github.com/yuzen9622/TermExpander-ai) — A Chrome extension for normalizing academic terminology

Highlight any term on a webpage, click the floating button, and get a normalized academic version — expanded acronyms, standardized translations, and formal replacements for informal phrasing. Built for students and researchers working across languages and citation styles.

**Stack:** TypeScript · Chrome Extension (Manifest V3) · OpenAI & Gemini APIs

**What I built & why it's interesting:**
- **Multi-provider LLM support** (GPT + Gemini) behind a small adapter layer, so adding a new provider is a single file
- **BYOK (bring-your-own-key) architecture** — API keys are stored locally in the user's browser, never touching my servers. No backend, no billing, no data retention
- **Floating-button UX** that appears on text selection, built to stay out of the way on dense academic pages
- **Designed for real research workflows**: acronym expansion (e.g. *RAG → Retrieval-Augmented Generation*), cross-language term standardization, and informal-to-formal rewriting

Not yet published to the Chrome Web Store — currently a developer-install build.

---

## 📊 GitHub Stats

[![Yuzen's GitHub stats](https://github-readme-stats.vercel.app/api?username=yuzen9622&show_icons=true&hide_border=true&theme=default&count_private=true)](https://github.com/yuzen9622)

[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=yuzen9622&layout=compact&hide_border=true&theme=default)](https://github.com/yuzen9622)

---

## 📬 Get in Touch

- 🌐 Website — [yuzen.dev](https://www.yuzen.dev)
- 💬 Discord — [@yuzen](https://discord.com/users/994875175885611018)
- 📸 Instagram — [@zn._.622](https://www.instagram.com/zn._.622/)

Always open to collaborating on interesting projects, discussing system design, or exploring internship opportunities.

Thanks for stopping by ☕
