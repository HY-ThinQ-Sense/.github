# EYEAR

**Eyes and Ears for Proactive Smart Home Orchestration through Spatial Awareness and Multi-Agent Collaboration**

**Hanyang University · Fall 2026**  
`CSE406-SW-Projects-2026` · `ITE351-AI-Projects-2026`

EYEAR (EYE + EAR) is a university project proposing a distributed perception layer and proactive home orchestration system for the LG ThinQ AI Home concept. Multiple **EYEAR Nodes** observe occupants' presence, location, posture, and activity using a **camera, microphone, and mmWave radar**. Small, specialized local perception components generate timestamped **semantic events**, without passing raw audiovisual streams to the central context API.

A **Home World Model** combines observations across rooms. Domain-focused agents propose appliance operations and restrictions, and a **Home Orchestrator** evaluates conflicts, explicit user policies, and device capabilities. A pretrained **LLM supervisor** is an optional/context-interpretation component, not an unrestricted appliance controller; validated decisions are expressed as actionable plans.

> **Project status:** Proposed architecture and academic prototype. EYEAR is not an official LG Electronics product. The project does not claim access to ThinQ ON firmware or control of physical LG appliances.

## Conceptual Architecture

```text
EYEAR Nodes (Camera + Microphone + mmWave)
    -> Local vision / audio / radar perception
    -> Temporal fusion and Semantic Events
    -> Multi-room Context Engine / Home World Model
    -> Domain Agents (Cleaning, Quiet/Activity, ...)
    -> Home Orchestrator (optional pretrained LLM interface)
    -> Policy and Device-Capability Validator
    -> Action Plans
    -> 3D Smart Home / Virtual Appliances
    -> Execution Feedback to World Model
```

## Representative Scenarios

- **Adaptive Cleaning:** Replan robot-vacuum work as rooms become occupied or available; preserve task goals while honoring user restrictions.
- **Activity-Aware Quiet Coordination:** Use occupancy and acoustic activity to detect a *possible* call/meeting context, then defer or modify disruptive virtual appliance tasks. Speech activity alone is not proof of a meeting.
- **Synchronized Sensor Replay:** Replay recorded multimodal observations on a common clock and run perception and planning *during playback*; contrast sensor-driven decisions with authored simulation scenarios.

## Repositories

| Repository | Purpose |
| --- | --- |
| [LG-EYEAR](https://github.com/HY-LG-EYEAR/LG-EYEAR) | Context engine, domain agents, orchestrator, constraints, API, and 3D smart-home demo |
| [LG-EYEAR-ai](https://github.com/HY-LG-EYEAR/LG-EYEAR-ai) | Local perception, multimodal sensing/fusion, model experiments and evaluations |
| [LG-EYEAR-docs](https://github.com/HY-LG-EYEAR/LG-EYEAR-docs) | CSE406 IEEE LaTeX submissions, requirements, specifications, design, and testing |
| [LG-EYEAR-blog](https://github.com/HY-LG-EYEAR/LG-EYEAR-blog) | ITE351 project proposal, technical blog, AI experiments, and research findings |

## Team

| Member | Affiliation | Project role |
| --- | --- | --- |
| Jungbin Song | Dept. Information Systems, Hanyang University | AI Engineer |
| Banseok Shin | Dept. Information Systems, Hanyang University | AI Engineer |
| Hyochang Lee | Dept. Information Systems, Hanyang University | AI Engineer |
| Yewon Joung | Dept. Information Systems, Hanyang University | Full-stack Engineer |

## Coursework

**CSE406 — Software Engineering**: IEEE-format proposal/requirements (Oct. 23/30), specification and development environment (Nov. 6/13), followed by design, implementation, integration, and final demonstration as announced.

**ITE351 — AI & Applications**: Initial group/blog/proposal submission (Nov. 4); subsequent milestones follow course announcements.

## Demo and Reports

- [CSE406 documents](https://github.com/HY-LG-EYEAR/LG-EYEAR-docs)
- [ITE351 research blog](https://github.com/HY-LG-EYEAR/LG-EYEAR-blog)
- 3D demo, evaluation results, and presentation: *to be added*

*LG, ThinQ, and ThinQ ON are trademarks of their respective owners. This is an independent academic project conducted in an LG-related course context.*
