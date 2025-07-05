# Severino IoT Agent Architecture Diagrams

## 1. Child Safety Monitoring (Camera Example)

This diagram illustrates how Severino processes a user's natural language prompt to monitor a child's safety using a camera, applying the Refactor, Break Down, and Compile steps.

```mermaid
---
config:
  layout: fixed
---
flowchart TD
    A["User Prompt"] --> B["Severino CLI"]
    B --> C["Cognitive Layer"]
    C --> C1["Refactor: Interpret Prompt, Identify Goal"]
    C1 --> D["Tool Manager"]
    D --> D1["Tool: Network Scan"]
    D1 --> D2["Tool: Connect to Camer"]
    D2 --> E["Perception Layer"]
    E --> E1["Data Stream: Video Frames"]
    E1 --> E2["Object Detection"]
    E2 --> E3["Activity Recognition"]
    E3 --> F["Refactor"]
    F --> G["Cognitive Layer"]
    G --> G1["Break DownDecompose Goal"]
    G1 --> H["Working Memory"] & J["LLM Inference"]
    H --> I["Semantic Memory"]
    J --> K["Compile Synthesize Insights"]
    K --> L["Action Layer"]
    L --> L1["Tool Send Alert"] & L2["Tool Log Event"] & M["User FeedbackReport"]

```

## 2. Automated Quality Control (Factory/SMB Example)

This diagram shows Severino's application in an SMB manufacturing setting for automated quality control, demonstrating its ability to monitor, analyze, and act on production data.

```mermaid
---
config:
  layout: fixed
---
flowchart TD
    A["User Prompt Monitor product defects on Line 1"] --> B["Severino CLI"]
    B --> C["Cognitive Layer LLM"]
    C --> C1["Refactor Interpret Prompt Identify Goal Defect Detection"]
    C1 --> D["Tool Manager"]
    D --> D1["Tool Connect to Production Line Camera"]
    D1 --> E["Perception Layer Jetson Edge Device"]
    E --> E1["Data Stream Product Images"]
    E1 --> E2["ML Model Anomaly Detection Defect Classification"]
    E2 --> F["Refactor Structured Data Defect Type Location Severity"]
    F --> G["Cognitive Layer LLM"]
    G --> G1["Break Down Decompose Goal Identify Defect Categorize Prioritize"]
    G1 --> H["Working Memory"] & J["LLM Inference Iterative Reasoning"]
    H --> I["Semantic Memory Defect Catalog QC Standards"]
    J --> K["Compile Synthesize Insights eg Scratch detected on Unit 123 Minor defect"]
    K --> L["Action Layer"]
    L --> L1["Tool Trigger Reject Mechanism eg robotic arm"] & L2["Tool Alert Supervisor SMS Dashboard"]
    L2 --> L3["Tool Log Defect Data"]
    L3 --> M["Production Report Analytics"]


```
