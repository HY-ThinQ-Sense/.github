# ThinQ Sense

### A Spatially Aware Multi-Agent System for Predictive and Proactive Smart Home Orchestration

**26-2 Hanyang University**  
**CSE406-SW-Projects-2026 · ITE351-AI-Projects-2026**

An integrated academic project developed by a four-member team at Hanyang University.

## Overview

**ThinQ Sense** is a proposed spatial intelligence and multi-agent orchestration system designed to advance smart homes from reactive automation to predictive, context-aware assistance.

The system combines multimodal sensing, human activity recognition, household state modeling, and predictive planning to understand occupants' locations, activities, and potential next actions.

A central multi-agent orchestrator coordinates specialized appliance agents to dynamically plan, prioritize, and adapt home appliance operations according to user activities, preferences, environmental conditions, and operational constraints.

Rather than relying solely on fixed schedules or explicit user commands, ThinQ Sense aims to enable home appliances to act proactively while minimizing interruptions and unnecessary resource consumption.

## System Architecture

```text
Multimodal Spatial Sensing
(Camera / Microphone / mmWave / IoT)
                  |
                  v
      Local Perception & Fusion
                  |
          Semantic Events
                  |
                  v
         Home World Model
                  |
                  v
         Prediction Engine
                  |
                  v
     Multi-Agent Home Orchestrator
                  |
       +----------+----------+
       |          |          |
    Cleaning    Climate    Quiet/Energy
     Agent       Agent        Agent
       |          |          |
       +----------+----------+
                  |
           Policy & Planning
                  |
                  v
        Appliance Action Plans
                  |
                  v
       3D Smart Home Digital Twin
```

## Key Research Areas

- **Spatial Awareness:** Real-time human presence, location, posture, and activity recognition.
- **Multimodal Perception:** Local visual inference and optional radar-based sensing with sensor fusion.
- **Predictive Modeling:** Learning occupants' activity patterns and estimating future household states.
- **Multi-Agent Collaboration:** Coordinating specialized agents with potentially competing objectives.
- **Constraint-Based Planning:** Optimizing appliance operations under occupancy, comfort, noise, and energy constraints.
- **Adaptive Decision-Making:** Exploring reinforcement learning and preference-based policy adaptation.
- **3D Digital Twin:** Interactive visualization and evaluation of household events, decisions, and appliance actions.
- **Privacy by Design:** Processing sensitive sensor data locally and limiting central access to semantic context.

## Representative Use Cases

### Adaptive Robot Cleaning

Dynamically replan robot vacuum cleaning routes based on room occupancy, sleep states, predicted availability, and user interruptions.

### Predictive Sleep Preparation

Anticipate bedtime-related activities and coordinate climate, lighting, and household noise policies before explicit user commands.

### Context-Aware Quiet Home

Coordinate cleaning, laundry, air care, and notifications to reduce disturbances during sleep, remote meetings, and other sensitive activities.

### Personalized Comfort

Adapt room environments based on occupants' locations, activities, and learned preferences while resolving multi-user conflicts.

## Demonstration

The project will demonstrate its decision-making capabilities through an interactive **3D Smart Home Digital Twin**.

The prototype is designed to support two input modes:

1. **Live Sensing:** Real camera and optional radar observations processed into semantic events.
2. **Scenario Simulation:** Virtual occupants and activities generating the same event format.

Both modes use a shared household world model and multi-agent decision engine.

Physical LG appliance integration is outside the initial prototype scope. Appliance behavior will be evaluated through simulated action execution.

## Repositories

| Repository | Description |
|---|---|
| [ThinQ-Sense](https://github.com/HY-ThinQ-Sense/ThinQ-Sense) | World model, multi-agent orchestration, optimization, reinforcement learning, and 3D digital twin |
| [ThinQ-Sense-ai](https://github.com/HY-ThinQ-Sense/ThinQ-Sense-ai) | Spatial perception, multimodal sensor fusion, prediction models, and AI experiments |
| [ThinQ-Sense-docs](https://github.com/HY-ThinQ-Sense/ThinQ-Sense-docs) | Software engineering requirements, specifications, design, verification, and reports |
| [ThinQ-Sense-blog](https://github.com/HY-ThinQ-Sense/ThinQ-Sense-blog) | AI research proposal, technical progress, experimental results, and research documentation |

## Academic Context

**CSE406 — Software Engineering**

Focuses on software requirements, system architecture, multi-agent integration, verification, testing, and demonstration.

**ITE351 — AI & Applications**

Focuses on AI/ML techniques, spatial perception, prediction, sensor fusion, and learning-based decision-making.

## Team Members

| Member | Organization | Primary Responsibility |
|---|---|---|
| Member 1 | Hanyang University | Perception & Sensor Fusion |
| Member 2 | Hanyang University | World Model & Prediction |
| Member 3 | Hanyang University | Multi-Agent Planning & Optimization |
| Member 4 | Hanyang University | 3D Digital Twin & Integration |

## Project Resources

- Technical Documentation: [ThinQ-Sense-docs](https://github.com/HY-ThinQ-Sense/ThinQ-Sense-docs)
- AI Research Blog: [ThinQ-Sense-blog](https://github.com/HY-ThinQ-Sense/ThinQ-Sense-blog)
- Demonstration Video: Coming soon
- Final Presentation: Coming soon

---

**Disclaimer:** ThinQ Sense is an independent academic project and proposed smart home system concept. It is not an official LG Electronics product. Actual ThinQ ON firmware integration and physical appliance control have not been implemented or verified.
