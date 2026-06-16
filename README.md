# Google Cloud GenAI Skills Validation Workshop

My submissions for the Google Cloud **Generative AI Skills Validation Workshop** — a series of
challenges building secure, accurate, production-quality generative-AI solutions on Google Cloud
(Gemini, BigQuery, Model Armor, Vertex AI).

## Challenges

| # | Challenge | Pts | Artifact |
|---|-----------|----:|----------|
| 1 | **Gemini Prompt Security** — a guarded chatbot with Model Armor input/output filtering and Gemini safety settings | 20 | [`challenge1-evandena.ipynb`](challenge1-evandena.ipynb) |
| 2 | **Programming a RAG System in BigQuery** — embeddings + `VECTOR_SEARCH` over proprietary data | 20 | [`challenge2-evandena.ipynb`](challenge2-evandena.ipynb) |
| 3 | **Testing & Evaluation** — `pytest` unit tests + the Gen AI Evaluation Service | 20 | [`challenge3-evandena.ipynb`](challenge3-evandena.ipynb) |
| 4 | *(Bonus)* **Building Agents with AI Applications** — Conversational Agent with a playbook + data store | 10 | screenshots: [1](challenge4-evandena.jpg) · [2](challenge4-evandena-2.png) · [3](challenge4-evandena-3.png) |
| 5 | **Alaska Department of Snow Online Agent** — the capstone: a deployable, guardrailed RAG agent | 40 | [`challenge5/`](challenge5/) |

**Total: 110 points (80 required to pass).**

## Challenge 5 — the capstone

[`challenge5/`](challenge5/) integrates the earlier challenges into one production-quality,
deployable RAG chatbot for the (fictional) Alaska Department of Snow: BigQuery RAG, Model Armor +
DLP guardrails, Cloud Logging, Gen AI Evaluation (groundedness), real-time National Weather Service
data via Gemini function calling, and a FastAPI service deployed to Cloud Run. See
**[`challenge5/README.md`](challenge5/README.md)** for the full writeup, architecture diagram, and
screenshots of the running agent.

## Tech used

Python · Gemini 2.5 Flash (`google-genai` / Vertex AI) · BigQuery ML (`text-embedding-005`,
`VECTOR_SEARCH`) · Model Armor · Sensitive Data Protection (DLP) · Cloud Logging · Vertex AI Gen AI
Evaluation Service · National Weather Service API · FastAPI on Cloud Run.
