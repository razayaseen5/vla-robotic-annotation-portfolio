# Vision-Language-Action (VLA) Robotic Annotation Portfolio

This repository contains a highly structured, human-annotated dataset of 10 robotic manipulation tasks. It is designed to demonstrate strict adherence to data labeling constraints required for training Embodied AI, Large Language Models (LLMs), and Reinforcement Learning from Human Feedback (RLHF) systems.

## 🎯 Project Overview
This dataset maps physical robotic actions (bimanual and single-arm pick-and-place tasks) to both human-readable documentation and machine-readable JSON schemas. The source footage features multi-perspective and egocentric robotic operations from open-X embodiment environments.

To prove rigorous QA evaluation and precision, every annotation strictly adheres to the following industry alignment constraints:
*   **Intent Captions:** Second-person imperative commands, present tense, strictly unpunctuated at the terminal end.
*   **Subtask Summaries:** Broken down into atomic actions, written in the first-person perspective ("I will..."), utilizing spatial awareness.
*   **Final Summaries & Outcomes:** Past-tense evaluations that accurately log successful completions, suboptimal jerky movements, system hangs, and complete physical failures.

## 📁 Repository Architecture
*   `/videos`: Contains 10 cropped and optimized MP4 clips of atomic robotic actions.
*   `/annotations/markdown_format`: Human-readable QA evaluation sheets detailing task intents, subtasks, summaries, and outcomes.
*   `/annotations/json_format`: Machine-readable dictionary schemas ready for dataset ingestion and model training workflows.

## 🛠️ Core Competencies Demonstrated
*   AI Data Annotation & QA Curation
*   Embodied AI / Robotics Dataset Structuring
*   Model Alignment Workflows
*   Strict Formatting Constraint Adherence
*   JSON Data Schema Generation
