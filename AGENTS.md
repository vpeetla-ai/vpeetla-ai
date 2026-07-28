# Agent Instructions — vpeetla-ai org

Read [CONTEXT.md](CONTEXT.md) for shared vocabulary.

## Agentic engineering (Karpathy)

1. **Think before coding** — state assumptions, plan, success criteria
2. **Simplicity first** — minimum diff; no speculative features
3. **Surgical changes** — match existing style; no drive-by refactors
4. **Goal-driven execution** — tests/evals define done; iterate until pass

## Stack awareness

This org builds **governed agent systems**, not chat demos:

- Orchestration (VAP) and governance (AegisAI) are **separate layers**
- RAG uses **access-before-ranking**
- Side effects require **gateway or HITL**
- Self-improvement uses **harness + eval loops** (LoopForge)

## Repo conventions

- Python 3.11+, FastAPI, Pydantic v2, LangGraph for agent graphs
- `pip install -e ".[dev]"` + `pytest -q` before claiming done
- README: badges → problem → 60s diagram → **honest status table** → quick start
- Deploy: Vercel (UI) + Render (API); see `render.yaml`

## Book writing (Enterprise AI Architecture Handbook)

Repo: [enterprise-ai-architecture-handbook](https://github.com/vpeetla-ai/enterprise-ai-architecture-handbook) — the manuscript, proposal, diagrams, and research for Venkata's book. Not a code repo; treat it as an editorial project.

- Voice: natural and human — like a principal architect telling a colleague what actually happened, not a compliance document. No robotic, form-letter prose.
- Every chapter follows `STYLE_GUIDE.md`'s 15-section structure for *coverage*, but the order and headers are a checklist, not a script — open with a real failure story, a specific system, a judgment call, not a restated section title.
- Draft one chapter at a time. Follow `CANONICAL_TOC.md` (36 chapters, 7 parts) — don't reduce or renumber without a documented editorial decision (`proposal/editorial-decisions.md`).
- Flagship samples first, per `proposal/writing-roadmap.md`: Ch. 4 (Control Plane) → Ch. 7 (Agent Runtime) → Ch. 18 (Evaluation).
- Keep terminology aligned with `GLOSSARY.md`; record sources in `research/source-notes/` and `research/bibliography/references.bib`.

## Skills repo

Install org skills from [vpeetla-ai-skills](https://github.com/vpeetla-ai/vpeetla-ai-skills):

```bash
./scripts/install.sh --cursor --project .
./scripts/install.sh --codex --project .
```

## When stuck

1. Check which **stack layer** the task belongs to
2. Read the target repo's `docs/ECOSYSTEM.md` or `docs/ARCHITECTURE.md`
3. Use **tdd-agent-loops** for graph changes; **aegis-gateway** for side effects
