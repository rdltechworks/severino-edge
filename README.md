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
    A["User"] --> B["Severino CLI"]
    B --> C["Cognitive Layer LLM"]
    C --> C1["Refactor"]
    C1 --> D{"Tool Manager"}
    D --> D1["Tool: Network Scan"]
    D1 --> D2["Tool: Connect to Camera R"]
    D2 --> E["Perception Layer"]
    E --> E1["Data Stream: Video Frames"]
    E1 --> E2["ML Model: Object Detection"]
    E2 --> E3["ML Model: Pose Estimatioivity Recognition"]
    E3 --> F["Refactor: Structured Data y Boundary, Activit"]
    F --> G["Cognitive LayerLLM"]
    G --> G1["Break Down:  Child, ty, Asse"]
    G1 --> H["Working Memory"] & J["LLM Inference"]
    H --> I["Semantic Memory"]
    J --> K["Compile: Synthesize Insights  neh"]
    K --> L["Action Layer"]
    L --> L1["Tool: Se"] & L2["Tool: Log Event"] & M["User Feedback/Report"]

```
