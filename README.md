# 柒君 / Spirtxiaoqi7

> Building continuity for AI beyond the context window.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-Memory%20Systems-blueviolet)
![LLM](https://img.shields.io/badge/LLM-Dialogue%20Agents-black)
![Open Source](https://img.shields.io/badge/Open%20Source-AI%20Memory-green)

我在构建 AI 的外部流动记忆系统，让长期对话智能体在上下文清空、模型切换和长期交互之后，仍然能保持时间意识、人格连续性与可审计的记忆依据。

My main work is **ARPM**, an External Fluid Memory framework for long-term AI dialogue continuity, cross-model persona consistency, and time-aware retrieval.

---

## Main Work

### ARPM — External Fluid Memory for AI Continuity

ARPM is not a normal RAG wrapper.

It is a memory governance framework for long-term AI companions and dialogue agents, focused on:

- Cross-model persona continuity
- Time-aware dialogue memory
- Dual-source retrieval: knowledge memory + dialogue history
- Dual-timescale evidence: physical time + turn-index time
- BM25 + vector retrieval + RRF fusion
- Memory promotion, clustering, merge, rollback and audit logs
- Analysis-style generation instead of pure roleplay prompting

The goal is to make AI continuity external, recoverable, and auditable.

---

## Experiments

ARPM has been tested through real long-form dialogue pressure, including:

- 300–1000+ round dialogue sessions
- Context reset experiments
- Cross-model relay experiments
- Retrieval ablation studies
- Human-in-the-loop dialogue evaluation
- Logs for retrieval, generation, promotion, correction and rollback behavior

I care less about perfect demos and more about whether the system survives real interaction.

---

## Projects

### ARPM

External Fluid Memory framework for long-term AI dialogue continuity.

### Pretext / SillyTavern Tools

Frontend and interaction tooling for long-context AI dialogue workflows.

### AI Companion Tools

Experiments around personal AI assistants, memory governance, and dialogue consistency.

---

## Tech Stack

**AI / Memory Systems**  
RAG · BM25 · Vector Search · RRF · Long-term Memory · Dialogue Agents · Cross-model Relay

**Backend / Engineering**  
Python · FastAPI · API Integration · Logging · Evaluation Pipelines

**Frontend / Interaction**  
JavaScript · SillyTavern Tools · Long-context Dialogue UI

---

## GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Spirtxiaoqi7&show_icons=true&theme=transparent)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Spirtxiaoqi7&layout=compact&theme=transparent)

---

## Principle

A model can be replaced.  
A broken memory chain cannot.

I build the layer in between.
