# Hi, I'm Yuzen 👋

> Student developer · Taiwan

Information Management student at **National Taichung University of Science and Technology (NTCUST)**, building full-stack systems end-to-end — from authentication flows and real-time pipelines to RAG-powered AI applications and browser extensions.

I build the part of the system you only notice when it's gone.

---

## 🔭 Currently Focused On

- **Agentic AI & RAG** — retrieval-augmented generation, tool-calling agents, multi-modal pipelines
- **Real-time systems** — event-driven architecture, pub/sub patterns, latency optimization
- **Authentication & security** — JWT, session management, middleware design
- **Frontend performance** — rendering strategy, bundle optimization, perceived performance
- **Accessible technology** — building inclusive systems with map/navigation interfaces

---

## 🛠️ Tech Stack

**Proficient**
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white&style=flat-square)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=next.js&logoColor=white&style=flat-square)
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black&style=flat-square)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white&style=flat-square)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white&style=flat-square)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white&style=flat-square)

**Familiar**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white&style=flat-square)
![Express](https://img.shields.io/badge/Express-000000?logo=express&logoColor=white&style=flat-square)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white&style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white&style=flat-square)
![C++](https://img.shields.io/badge/C++-00599C?logo=c%2B%2B&logoColor=white&style=flat-square)

---

## 🚀 Featured Projects

### 💬 [chat.to](https://github.com/yuzen9622/chat.to) — Real-time chat, built the way modern chat should be

A full-featured real-time chat application with group rooms, typing indicators, and media uploads.

**Stack:** Next.js · TypeScript · Supabase · Ably · NextAuth · Cloudinary

**What I built & why it's interesting:**
- **Real-time via Ably pub/sub** instead of rolling my own WebSocket server — lets the app scale horizontally on Vercel's serverless runtime without long-lived connections on the origin
- **Session-based auth with NextAuth**, integrated into API routes and Ably channel authorization so users can only subscribe to rooms they belong to
- **Media uploads offloaded to Cloudinary** via signed uploads, keeping large payloads out of the API layer entirely
- **Typing indicators** implemented as ephemeral Ably presence events (not persisted) — a deliberate trade-off between UX fidelity and DB write pressure


---

### 🗺️ [taipei-accessible-map](https://github.com/yuzen9622/taipei-accessible-map) — 無障礙智慧導航系統

An accessible smart navigation system for Taipei that surfaces barrier-free routes and facilities for users with mobility needs.

**Stack:** Next.js · TypeScript · Google Maps JavaScript API · shadcn/ui · Express · Node.js

**What I built & why it's interesting:**
- **Barrier-free routing layer** on top of Google Maps, filtering and surfacing accessibility data that the default API doesn't expose
- **Separated frontend and backend** ([frontend](https://github.com/yuzen9622/taipei-accessible-map) + [REST API](https://github.com/yuzen9622/taipei-accessible-backend)) with a clean RESTful contract — easier to swap map providers or add mobile clients later
- **Designed around real constraints**: wheelchair ramps, elevator availability, accessible entrances — not just "avoid stairs" but modeling the actual decision tree a mobility-impaired user runs through

---

### 🤖 [MakeNTU2026](https://github.com/yuzen9622/MakeNTU2026) — Agentic RAG with voice input (hackathon)

A hackathon project combining agentic RAG, voice transcription, and a React frontend into a single AI-powered assistant.

**Stack:** TypeScript · React · FastAPI · Whisper · Agentic RAG

**What I built & why it's interesting:**
- **Whisper-powered voice input** transcribed server-side and fed directly into the RAG pipeline — no intermediate state between speech and retrieval
- **Agentic RAG loop** where the model can decide to re-query the retrieval layer before generating a final answer, reducing hallucination on domain-specific questions
- **FastAPI backend** handling transcription, embedding, and generation in a single request path to keep latency manageable under demo conditions

---

### 🔤 [TermExpander-ai](https://github.com/yuzen9622/TermExpander-ai) — Chrome extension for normalizing academic terminology

Highlight any term on a webpage, click the floating button, and get a normalized academic version — expanded acronyms, standardized translations, and formal replacements for informal phrasing.

**Stack:** TypeScript · Chrome Extension (Manifest V3) · OpenAI & Gemini APIs · Vite · React

**What I built & why it's interesting:**
- **Multi-provider LLM support** (GPT + Gemini) behind a small adapter layer — adding a new provider is a single file
- **BYOK (bring-your-own-key) architecture** — API keys stored locally in the browser, never touching my servers. No backend, no billing, no data retention
- **Floating-button UX** that appears on text selection, built to stay out of the way on dense academic pages
- **Designed for real research workflows**: acronym expansion (e.g. *RAG → Retrieval-Augmented Generation*), cross-language term standardization, informal-to-formal rewriting

---

## 📊 GitHub Stats

<p align="center">
  <a href="https://github.com/yuzen9622">
    <img src="./github-metrics.svg" alt="Yuzen's GitHub stats" width="100%" />
  </a>
</p>

<table width="100%" align="center">
  <tr>
    <td width="50%" align="center">
      <img src="./assets/github-stats.svg" alt="Yuzen's GitHub Stats" width="100%" />
    </td>
    <td width="50%" align="center">
      <img src="./assets/top-langs.svg" alt="Top Languages" width="100%" />
    </td>
  </tr>
</table>

---

## 📬 Get in Touch

- 🌐 Website — [yuzen.dev](https://www.yuzen.dev)
- 💬 Discord — [@yuzen](https://discord.com/users/994875175885611018)
- 📸 Instagram — [@zn._.622](https://www.instagram.com/zn._.622/)

Always open to collaborating on interesting projects, discussing system design, or exploring internship opportunities.

Thanks for stopping by ☕
