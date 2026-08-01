<!-- Profile README for https://github.com/vpeetla-ai (Overview tab) -->
<!-- Canonical: vpeetla-ai/README.md — keep ACF docs/github-profile in sync -->

# Hi, I'm Venkata Peetla — Principal AI Architect

I build **governed agent platforms** — orchestration and governance as separate layers, access-before-ranking RAG, side effects behind gates. One brand, not a catalog tour.

> **5-spine review path** (govern · orchestrate · RAG · publish · ADRs) · full catalog behind it · **29 ADRs** — inspect before we talk.

[![Website](https://img.shields.io/badge/Website-venkat--ai.com-blue)](https://venkat-ai.com)
[![Technical review](https://img.shields.io/badge/15--Min_Technical_Review-Start_here-5eead4)](https://venkat-ai.com/technical-review)
[![Architecture portfolio](https://img.shields.io/badge/Architecture_Portfolio-ADRs_%26_Case_Studies-purple)](https://github.com/vpeetla-ai/ai-architecture-portfolio)
[![90-day plan](https://img.shields.io/badge/Top--1%25_90--Day-Execution_plan-111827)](https://github.com/vpeetla-ai/ai-architecture-portfolio/blob/main/docs/TOP1PCT_90DAY_EXECUTION.md)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2)](https://linkedin.com/in/venkata-peetla)
[![Substack](https://img.shields.io/badge/Substack-Subscribe-orange)](https://venkatapeetla.substack.com)

---

## Start here

| For | Link |
|-----|------|
| **Engineering panels (~15 min)** | [venkat-ai.com/technical-review](https://venkat-ai.com/technical-review) |
| **Hire overview** | [venkat-ai.com/hire](https://venkat-ai.com/hire) |
| **Full portfolio catalog** | [venkat-ai.com/work](https://venkat-ai.com/work) |
| **Flagship essay** | [From Multi-Agent OS to Agent Governance](https://github.com/vpeetla-ai/ai-architecture-portfolio/blob/main/case-studies/from-multi-agent-os-to-agent-governance.md) |

---

## Public spine (D1 — review these five)

Start here. Narrative hub + four live platforms. Everything else is labs, proof services, or teaching stubs — not the first screen.

| # | Layer | Repo | Live |
|---|-------|------|------|
| 1 | **Decisions** | [ai-architecture-portfolio](https://github.com/vpeetla-ai/ai-architecture-portfolio) | ADRs · case studies · [execution plan](https://github.com/vpeetla-ai/ai-architecture-portfolio/blob/main/docs/TOP1PCT_90DAY_EXECUTION.md) |
| 2 | **Governance** | [aegisai-enterprise-agent-platform](https://github.com/vpeetla-ai/aegisai-enterprise-agent-platform) | [Control plane](https://aegisai-enterprise-agent-platform.vercel.app) |
| 3 | **Orchestration** | [venkat-ai-platform](https://github.com/vpeetla-ai/venkat-ai-platform) | [VAP console](https://venkat-ai-platform.vercel.app) |
| 4 | **Knowledge** | [enterprise_rag_platform](https://github.com/vpeetla-ai/enterprise_rag_platform) | [RAG lab](https://enterprise-rag-platform-eta.vercel.app) |
| 5 | **Application** | [ai-content-factory](https://github.com/vpeetla-ai/ai-content-factory) | [Content pipeline](https://ai-content-factory-iota.vercel.app) |

**Proof (linked, not hero):** [golden-eval-registry](https://github.com/vpeetla-ai/golden-eval-registry) · [agent-finops](https://github.com/vpeetla-ai/agent-finops)  
**Career layer:** [ai-architect-interview-playbook](https://github.com/vpeetla-ai/ai-architect-interview-playbook) · [ai-architect-practice-arena](https://github.com/vpeetla-ai/ai-architect-practice-arena)

---

## Agent skills (Cursor + Codex)

**[vpeetla-ai-skills](https://github.com/vpeetla-ai/vpeetla-ai-skills)** — org-wide agent skills for every repo: LangGraph, gateway/HITL, loop engineering, TDD, deploy.

```bash
git clone https://github.com/vpeetla-ai/vpeetla-ai-skills.git
./vpeetla-ai-skills/scripts/install.sh --cursor --codex --project .
```

Inspired by [mattpocock/skills](https://github.com/mattpocock/skills) + [Karpathy agentic engineering](https://www.youtube.com/watch?v=96jN2OCOfLs) + [autoresearch](https://github.com/karpathy/autoresearch).

---

## Top projects (spine detail)

### [AegisAI — Enterprise Agent Governance](https://github.com/vpeetla-ai/aegisai-enterprise-agent-platform)

I'd put an independent gateway in front of irreversible tools — policy, HITL on the scary ones, signed audit. The agent graph doesn't get a back door.

[▶ Live control plane](https://aegisai-enterprise-agent-platform.vercel.app) · Gateway SDK · OPA · FastAPI · Next.js

### [Venkat AI Platform (VAP)](https://github.com/vpeetla-ai/venkat-ai-platform)

What agents should do — LangGraph orchestrators, RAG strategies, gateway-wrapped notify. Orchestration stays separate from governance on purpose.

Chief → parallel specialists → Critic → Slack / Telegram / WhatsApp · pairs with AegisAI

[▶ Live demo](https://venkat-ai-platform.vercel.app)

### [Enterprise RAG Platform](https://github.com/vpeetla-ai/enterprise_rag_platform)

Filter by who the caller is *before* you rank. Hybrid retrieval, decline-to-answer, AegisAI HITL bridge. Prefer Strict/JWT for panels.

[▶ Live demo](https://enterprise-rag-platform-eta.vercel.app)

### [AI Content Factory](https://github.com/vpeetla-ai/ai-content-factory)

Research → drafts → HITL → publish. The end-user workflow that proves side effects stay behind gates — publish fails closed when Strict.

[▶ Live demo](https://ai-content-factory-iota.vercel.app) · LangGraph · Clerk · Render + Vercel

### [Architecture portfolio — ADRs](https://github.com/vpeetla-ai/ai-architecture-portfolio)

**29 ADRs** — what I decided, what I refused, and live proof (`PRODUCTION_STRICT`, NIST AI RMF, multi-tenant isolation).

→ [Featured case studies](https://github.com/vpeetla-ai/ai-architecture-portfolio#featured-case-studies) · [Top-1% execution plan](https://github.com/vpeetla-ai/ai-architecture-portfolio/blob/main/docs/TOP1PCT_90DAY_EXECUTION.md)

---

## How the spine fits together

```text
What should agents do?       →  Venkat AI Platform (orchestration)
What are agents allowed?     →  AegisAI (gateway, policy, HITL, audit)
What knowledge can they use? →  Enterprise RAG (access-before-ranking)
What do they produce?        →  AI Content Factory (governed publish)
Why these choices?           →  ai-architecture-portfolio (ADRs)
How do we prove quality?     →  Golden Eval Registry (proof, not hero)
What did agents cost?        →  Agent FinOps (proof, not hero)
```

---

## Labs & secondary platforms (full catalog)

Not on the Principal 15-minute path. Open these after the spine holds.

| Repo | Hook |
|------|------|
| [OmniForge](https://github.com/vpeetla-ai/omniforge) | Multimodal multi-LLM ask · [demo](https://omniforge-flame.vercel.app) |
| [LoopForge](https://github.com/vpeetla-ai/loop-engine-agent-platform) | Harness · repo fix → PR · [demo](https://demo-omega-taupe.vercel.app) |
| [DomainForge](https://github.com/vpeetla-ai/domainforge-rag-peft) | RAG facts + PEFT behavior · [demo](https://domainforge-rag-peft.vercel.app) |
| [VoiceForge](https://github.com/vpeetla-ai/voiceforge-assistant) | ASR → LLM → TTS · [demo](https://voiceforge-assistant.vercel.app) |
| [vLLM Lab](https://github.com/vpeetla-ai/vllm-architecture-lab) | Educational inference explorer · [demo](https://vllm-architecture-lab.vercel.app) |
| [AegisLoop](https://github.com/vpeetla-ai/aegisloop-agentops-workbench) | Mission fleets + eval gates · [demo](https://aegisloop-agentops-workbench.vercel.app) |
| [Sentinel Brief](https://github.com/vpeetla-ai/sentinel-brief) | Overnight AI radar · [demo](https://sentinel-brief-ruddy.vercel.app) |
| [agent-finops](https://github.com/vpeetla-ai/agent-finops) | Metering + budgets · [demo](https://agent-finops.vercel.app) |
| [golden-eval-registry](https://github.com/vpeetla-ai/golden-eval-registry) | Cross-repo regression contracts |

---

## Teaching stubs (curriculum patterns)

Deterministic stub loops + live trace viewers for interviews and skill-building. **Not** production fleets — compose into VAP / Content Factory for governed graphs. Status tables mark LangGraph production graph 🟡, gateway ❌.

| # | Pattern | Repository | Live demo |
|---|---------|------------|-----------|
| 1 | ReAct | [react-agent-pattern](https://github.com/vpeetla-ai/react-agent-pattern) | [Trace viewer](https://react-agent-pattern.vercel.app) |
| 2 | Reflection | [reflection-agent-pattern](https://github.com/vpeetla-ai/reflection-agent-pattern) | [Trace viewer](https://reflection-agent-pattern.vercel.app) |
| 3 | Plan-Execute | [plan-execute-agent-pattern](https://github.com/vpeetla-ai/plan-execute-agent-pattern) | [Trace viewer](https://plan-execute-agent-pattern.vercel.app) |
| 4 | Multi-Agent | [multi-agent-system-pattern](https://github.com/vpeetla-ai/multi-agent-system-pattern) | [Trace viewer](https://multi-agent-system-pattern.vercel.app) |
| 5 | Swarm | [swarm-agent-pattern](https://github.com/vpeetla-ai/swarm-agent-pattern) | [Trace viewer](https://swarm-agent-pattern.vercel.app) |

---

## Writing

- **Substack** — [venkatapeetla.substack.com](https://venkatapeetla.substack.com) — architecture decisions for production AI
- **Medium** — [@vpeetla.ai](https://medium.com/@vpeetla.ai) — agent patterns & RAG governance
- **Essay** — [From Multi-Agent OS to Agent Governance](https://github.com/vpeetla-ai/ai-architecture-portfolio/blob/main/case-studies/from-multi-agent-os-to-agent-governance.md) (VAP + AegisAI story)

---

## Connect

- 🌐 [venkat-ai.com](https://venkat-ai.com)
- 💼 [LinkedIn](https://linkedin.com/in/venkata-peetla)
- 📰 [Substack](https://venkatapeetla.substack.com)

If any repo helps you, a ⭐ helps other builders discover it.

*Spine narrative locked Jul 2026 — see [TOP1PCT_90DAY_EXECUTION.md](https://github.com/vpeetla-ai/ai-architecture-portfolio/blob/main/docs/TOP1PCT_90DAY_EXECUTION.md). Metrics source: `venkat-ai-portfolio/data/metrics.ts`.*
