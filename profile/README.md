# ThinQ Sense

> **Privacy-Preserving Spatial Intelligence for Proactive AI Home**
>
> **26-2 Hanyang University**  
> **CSE406-SW-Projects-2026 · ITE351-AI-Projects-2026**

## Overview

**ThinQ Sense** is a proposed privacy-first sensing and context intelligence layer for LG ThinQ AI Home. It combines local visual, acoustic, and optional radar-based sensing to infer human presence, location, posture, and activities. Rather than exposing raw audiovisual streams to the central agent, the proposed system communicates structured context events.

A household context engine aggregates these events into a real-time home state. A proactive agent can then plan context-aware appliance actions—such as adapting robot vacuum cleaning to occupied rooms, preparing a room before a predicted bedtime, or avoiding noisy appliance operation during sleep or meetings.

This is an **academic prototype and product concept**, not an official LG Electronics product or integration.

## Proposed Architecture

```text
Camera / Microphone / Optional mmWave
                  |
                  v
       ThinQ Sense Perception
      (local specialized inference)
                  |
       semantic events only
                  v
       Home Context / World Model
                  |
                  v
      Proactive Agent & Planner
                  |
                  v
       Appliance Action Intents
                  |
                  v
        Digital Twin Simulator
```

The production concept targets on-device inference; the academic prototype may run inference on an isolated local computer. Real LG ThinQ ON integration and appliance control are **not claimed unless verified and implemented**.

## Key Scenarios

- **Adaptive Cleaning:** replan cleaning order around sleeping or occupied rooms.
- **Predictive Sleep Preparation:** propose room temperature, lighting, and quiet-mode adjustments before bedtime.
- **Context-Aware Quiet Mode:** defer disruptive appliance operations during rest or meetings.
- **Privacy-Preserving Presence:** explore camera-independent sensing with optional mmWave radar.

## Repositories

| Repository | Purpose |
| --- | --- |
| [thinq-sense](https://github.com/HY-ThinQ-Sense/ThinQ-Sense) | Context engine, agent, API, digital twin and demo integration |
| [thinq-sense-ai](https://github.com/HY-ThinQ-Sense/ThinQ-Sense-ai) | Perception, sensor fusion, model experiments and evaluations |
| [thinq-sense-docs](https://github.com/HY-ThinQ-Sense/ThinQ-Sense-docs) | CSE406 requirements, specifications, design, testing and submissions |
| [thinq-sense-blog](https://github.com/HY-ThinQ-Sense/ThinQ-Sense-blog) | ITE351 proposal and technical progress blog |

> Repository links become active after each repository is created.

## Courses

- **CSE406 — Software Engineering:** requirements, architecture, integration, testing and demonstration.
- **ITE351 — AI & Applications:** AI methodology, data analysis, model evaluation and technical blog.

## Team

| Name | Organization | Email | Responsibilities |
| --- | --- | --- | --- |
| TBD (Member 1) | Hanyang University | TBD | Project coordination / requirements |
| TBD (Member 2) | Hanyang University | TBD | Perception / AI |
| TBD (Member 3) | Hanyang University | TBD | Context engine / agent |
| TBD (Member 4) | Hanyang University | TBD | Digital twin / integration / testing |

## Documentation & Demo

- Demo video: *To be added*
- Final paper and presentation: *To be added*

---

*LG, ThinQ, and ThinQ ON are trademarks of their respective owners. This repository presents an independent university research project.*
