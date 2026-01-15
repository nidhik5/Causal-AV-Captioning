# Causal-AV-Captioning

### Project Details
* **Project Name:** Causal Audio-Visual Integration
* **Title:** Measuring Causal Influence of Audio in Multimodal Video Captioning
* **Start & End Date:** Oct 2023 – Present

### Description
This project develops a framework to evaluate the **causal relationship** between audio-visual inputs and model outputs. By using Causal Inference, I measured whether Video-Language Models (VLMs) truly "listen" to audio or rely on visual bias to generate descriptions.

**Core Contributions:**
* **Model Fusion:** Integrated **VideoMAE** (Vision) and **AST** (Audio) encoders with a **GIT** text decoder for multimodal captioning.
* **Causal Evaluation:** Implemented quantitative metrics—**Total Effect (TE)**, **Natural Direct Effect (NDE)**, and **Natural Indirect Effect (NIE)**—to isolate the specific influence of the audio stream.
* **Counterfactual Testing:** Conducted "Audio Swap" experiments to verify model robustness. In tests, the model successfully detected audio-visual conflicts, shifting the caption from "breaking glass" to "bird squawk" based on audio cues, resulting in a **Modality Sensitivity** score of **0.8266**.

---

### Key Results (Matched Test)
| Metric | Value | Interpretation |
| :--- | :--- | :--- |
| **Total Effect (TE)** | **0.1052** | Overall positive influence of audio on prediction accuracy. |
| **Natural Direct Effect (NDE)** | **0.1052** | High direct impact of sound on generated text. |
| **Natural Indirect Effect (NIE)** | **0.0000** | Audio did not alter visual perception; influence was purely additive. |
| **Modality Sensitivity** | **0.8266** | Strong evidence of the model actively prioritizing audio cues. |
