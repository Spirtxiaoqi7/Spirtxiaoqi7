<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:08111f,48:12314a,100:0f766e&height=190&section=header&text=柒君%20%2F%20Spirtxiaoqi7&fontSize=40&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Long-term%20AI%20Memory%20%C2%B7%20Auditable%20RAG%20%C2%B7%20Persona%20Continuity&descSize=17&descAlignY=58" alt="Spirtxiaoqi7 header" />
</p>

<p align="center">
  <a href="https://arxiv.org/abs/2605.14802"><img src="https://img.shields.io/badge/arXiv-2605.14802-B31B1B?style=for-the-badge&logo=arxiv&logoColor=white" alt="ARPM paper"></a>
  <a href="https://arxiv.org/abs/2607.01248"><img src="https://img.shields.io/badge/arXiv-2607.01248-B31B1B?style=for-the-badge&logo=arxiv&logoColor=white" alt="Practice auditing paper"></a>
  <a href="https://github.com/Spirtxiaoqi7/ARPM"><img src="https://img.shields.io/github/stars/Spirtxiaoqi7/ARPM?style=for-the-badge&logo=github&label=ARPM" alt="ARPM stars"></a>
</p>

<p align="center">
  <a href="https://github.com/Spirtxiaoqi7/ARPM"><strong>ARPM</strong></a>
  ·
  <a href="https://github.com/Spirtxiaoqi7/Mindspace"><strong>Mindspace</strong></a>
  ·
  <a href="https://github.com/Spirtxiaoqi7/mindspace-dsh-local-rag"><strong>Local RAG for DSH</strong></a>
  ·
  <a href="https://github.com/Spirtxiaoqi7/mindspace-dsh-session-memory"><strong>Session Memory for DSH</strong></a>
</p>

---

## Research identity

I build **memory infrastructure for long-lived AI systems**: external memory governance, hybrid retrieval, persona continuity, evidence-bound generation, and user-auditable interaction.

我关注的不是让模型“看起来记得”，而是让长期 AI 在**上下文清空、模型切换、高噪声知识库和长期互动**之后，仍能给出可追溯的连续性，并允许用户查看、纠正、删除与回滚其记忆依据。

> **Continuity is not a prompting trick. It is a memory-governance problem.**

My work currently connects three layers:

1. **Research** — formalize long-term persona consistency and AI-use auditing;
2. **Systems** — implement external memory, temporal retrieval, controlled analysis, and evidence governance;
3. **Products & plugins** — ship the ideas through ARPM, Mindspace, SillyTavern extensions, and DeepSeek Harness plugins.

---

## Publications

### 1. A Heterogeneous Temporal Memory Governance Framework for Long-Term LLM Persona Consistency

**arXiv:2605.14802 · cs.AI · 2026**<br>
[Abstract](https://arxiv.org/abs/2605.14802) · [PDF](https://arxiv.org/pdf/2605.14802) · [Code: ARPM](https://github.com/Spirtxiaoqi7/ARPM)

Introduces **ARPM**, an external temporal memory-governance framework that separates static knowledge from dialogue experience and combines vector retrieval, BM25, RRF fusion, dual-temporal reranking, chronological evidence reading, and controlled analysis.

The work treats long-term persona consistency as a **traceable, auditable, and transferable** systems problem rather than a property hidden inside model weights.

### 2. A Practice Auditing Framework for Large Language Model Use

**Collective Empiricism, Pseudo-Rational Cognition, and Governance of AI-Generated Content**<br>
**arXiv:2607.01248 · cs.CY / cs.AI · 2026**<br>
[Abstract](https://arxiv.org/abs/2607.01248) · [PDF](https://arxiv.org/pdf/2607.01248)

Proposes a practice-auditing framework for LLM use and AI-generated content. It examines collective empiricism, pseudo-rational cognition, subjectivity illusion, template loops, statistical misjudgment, and **memory pollution when generated content re-enters retrieval or agent systems**.

The proposed response is operational: requirement definition, evidence-source auditing, practical validation, reverse questioning, logging, version management, rollback, and renewed cognition.

---

## Research programme

<p align="center">
  <strong>Interaction & sources</strong> → <strong>Governed memory</strong> → <strong>Hybrid retrieval</strong> → <strong>Evidence-bound analysis</strong> → <strong>Inspection & rollback</strong>
</p>

### Memory governance

- Separate knowledge, dialogue experience, user profile, preferences, instructions, and relationship state;
- preserve physical time, turn order, source location, and revision history;
- merge compatible information and explicitly replace contradictions;
- keep memory editable and recoverable instead of treating a vector index as an opaque truth store.

### Retrieval under conversational pressure

- hybrid lexical and semantic retrieval rather than vector-only similarity;
- parent-child chunking and source-preserving evidence;
- session-isolated dialogue recall plus global knowledge retrieval;
- graceful lexical fallback when the local embedding route is stopped or unavailable.

### Auditable human-AI interaction

- distinguish model fluency from verified understanding;
- keep generated content from silently polluting future memory;
- bind important claims to inspectable evidence and execution traces;
- return AI output to reproducible practice instead of accepting structured prose as proof.

---

## Selected systems

| Project | Role in the research line | What is implemented |
|---|---|---|
| [**ARPM**](https://github.com/Spirtxiaoqi7/ARPM) | Core research framework | Analysis-based role-playing with memory, dual-source retrieval, vector + BM25 + RRF, temporal weighting, controlled state/analysis/response protocol, LOCOMO evaluation |
| [**Mindspace**](https://github.com/Spirtxiaoqi7/Mindspace) | Local-first AI companion system | LangGraph orchestration, layered memory, standard character cards, visible tools, local voice stack, desktop launcher, long-term RAG |
| [**mindspace-dsh-local-rag**](https://github.com/Spirtxiaoqi7/mindspace-dsh-local-rag) | Independent RAG branch for DeepSeek Harness | Model-invoked local retrieval, PDF/DOCX/TSV ingestion, vector + BM25 lanes, session-isolated compaction summaries, source preview, editable/versioned corpora |
| [**mindspace-dsh-session-memory**](https://github.com/Spirtxiaoqi7/mindspace-dsh-session-memory) | Structured memory governance for DeepSeek Harness | Per-session user profile, categorized preferences, assistant requirements, relationship mission, role preset, conflict replacement, visible memory audit |
| [**st-ARPM**](https://github.com/Spirtxiaoqi7/st-ARPM) | SillyTavern protocol adapter | Keeps visible response history, extracts compact relationship state, removes hidden analysis from future requests |
| [**st-pretext-height-profiler**](https://github.com/Spirtxiaoqi7/st-pretext-height-profiler) | Long-dialogue UI experiment | Real-height virtual scrolling, node reuse, overscan, and A/B performance measurement for long chat histories |

---

## Evidence from released work

- ARPM was evaluated under a **5.1-million-character noise substrate**, periodic context clearing, and multi-model handoff.
- In the reported ablation, removing dialogue-history retrieval reduced strict accuracy from **100% to 66.7%**; removing BM25 reduced it to **80.0%**.
- The public ARPM repository includes reproducible evaluation material and a full LOCOMO run.
- The DeepSeek Harness Local RAG plugin ships with source-aware ingestion, session-isolation tests, model lifecycle tests, and governance/rollback coverage.
- Mindspace carries the research into a local desktop system rather than leaving it as a paper-only prototype.

I care less about a perfect one-shot demo than whether a system survives **real long-form interaction, correction, migration, and failure recovery**.

---

## Current focus

- long-term persona consistency across model and context boundaries;
- heterogeneous temporal memory and retrieval governance;
- local, inspectable RAG for user-owned files and conversation history;
- structured personalization memory with conflict-aware updates;
- memory pollution and evidence auditing in agent systems;
- practical AI companions that preserve user control.

<p align="center">
  <img src="https://img.shields.io/badge/Python-Memory%20%26%20Agent%20Systems-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/TypeScript-DSH%20Plugins-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/LangGraph-Agent%20Orchestration-1C3C3C?style=flat-square" alt="LangGraph">
  <img src="https://img.shields.io/badge/Retrieval-BM25%20%C2%B7%20Vector%20%C2%B7%20RRF-0F766E?style=flat-square" alt="Hybrid retrieval">
</p>

---

## Principles

> A model can be replaced. A broken memory chain cannot.

> Retrieval without provenance is suggestion, not evidence.

> AI productivity matters only when its results can return to verification, intervention, and rollback.

---

## Links

- GitHub: [@Spirtxiaoqi7](https://github.com/Spirtxiaoqi7)
- Main research system: [ARPM](https://github.com/Spirtxiaoqi7/ARPM)
- Local companion system: [Mindspace](https://github.com/Spirtxiaoqi7/Mindspace)
- arXiv: [2605.14802](https://arxiv.org/abs/2605.14802) · [2607.01248](https://arxiv.org/abs/2607.01248)

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f766e,52:12314a,100:08111f&height=120&section=footer" alt="footer" />
</p>
