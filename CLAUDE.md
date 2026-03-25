# Paper Study Website

## Project Purpose

This project is a personal website for studying and understanding research papers from a target professor's laboratory, in preparation for applying to a master's program. The goal is to deeply comprehend the professor's research direction, methodology, and key contributions before the application.

## Target Professors

- **Kee-Eung Kim** (KAIST AI) — Reinforcement learning, imitation learning, generative models, LLM interpretability
- **Beomjoon Kim** (KAIST AI) — Robot planning, task and motion planning, learning-based planning
- **Seungryong Kim** (KAIST AI) — Computer vision, video generation, dense correspondence, event cameras

## Papers Covered

| Professor | Paper | Venue |
|---|---|---|
| Kee-Eung Kim | DPAIL (Diffusion Policy + Adversarial IL) | NeurIPS 2025 |
| Kee-Eung Kim | VL-DNP (Dynamic VLM Negative Prompting) | NeurIPS 2025 WS |
| Kee-Eung Kim | MONET (Monosemantic Experts for LLMs) | ICLR 2025 |
| Beomjoon Kim | PRESTO (Motion Planning + Diffusion) | arXiv 2025 |
| Beomjoon Kim | Prime the Search / STaLM (LLM + TAMP) | IJRR |
| Seungryong Kim | WorldCam (3D Gaming World Model) | arXiv 2026 |
| Seungryong Kim | TETO (Event Camera Motion Estimation) | arXiv 2026 |
| Seungryong Kim | AgentRVOS (Referring Video Object Seg.) | arXiv 2026 |
| Seungryong Kim | DA-Flow (Degradation-Aware Optical Flow) | arXiv 2026 |

## What This Project Does

- Displays all 9 papers grouped by professor
- Each paper has a pre-written ~3000-word summary explaining the problem, method, and significance in plain language
- Tracks reading progress (Unread / Reading / Done) per paper, persisted in localStorage
- Search by title, author, or topic keyword

## Tech Stack

- Plain HTML, CSS, and JavaScript (no build tools required)
- Reading status stored in `localStorage`
- Single-page application (`index.html`) — open directly in a browser

## File Structure

```
paper/
├── CLAUDE.md                   # This file
├── README.md                   # Project overview
├── index.html                  # Main application (SPA)
└── asset/
    ├── KeeEungKim/             # PDFs for Kee-Eung Kim
    ├── Beomjoon_Kim/           # PDFs for Beomjoon Kim
    └── SeungryongKim/          # PDFs for Seungryong Kim
```

## Development Notes

- No backend or server needed — open `index.html` directly in a browser
- Paper content and summaries are hardcoded in `index.html` (PAPERS array)
- Only reading status is stored in localStorage (key: `paper_status`)
- To add a new paper, add an entry to the PAPERS array in the script section
