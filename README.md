# Vision-Language-Action (VLA) Robotic Annotation Portfolio

This repository contains a highly structured, human-annotated dataset of 10 robotic manipulation tasks. It is designed to demonstrate strict adherence to data labeling constraints required for training Embodied AI, Large Language Models (LLMs), Vision-Language-Action (VLA) models, and Reinforcement Learning from Human Feedback (RLHF) systems.

---


<img width="800" height="413" alt="task_02_preview" src="https://github.com/user-attachments/assets/9b5b23a4-88d3-41f6-aab0-c3c9808feae7" />

<img width="800" height="413" alt="task_01_preview" src="https://github.com/user-attachments/assets/48911691-c66e-45c5-a2a8-5276185e32e8" />


## 🎯 Project Overview
This dataset maps physical robotic actions (bimanual and single-arm pick-and-place tasks) to both human-readable documentation and machine-readable JSON schemas. The source footage features multi-perspective and egocentric robotic operations curated from open-X embodiment environments on Hugging Face.

To prove rigorous QA evaluation and precision, every annotation strictly adheres to the following industry alignment constraints:
* **Intent Captions:** Second-person imperative commands, present tense, strictly unpunctuated at the terminal end.
* **Subtask Summaries:** Broken down into atomic actions, written in the first-person perspective ("I will..."), utilizing camera spatial perspective.
* **Final Summaries & Outcomes:** Past-tense evaluations that accurately log successful completions, suboptimal jerky movements, system hangs, and complete physical failures.

## 🎬 Task Previews

| Task 01: Bimanual Tissue Tear | Task 02: Coffee Machine Operations |
| :---: | :---: |
| <img src="assets/task_01_preview.gif" width="400"/> | <img src="assets/task_02_preview.gif" width="400"/> |
| *Bimanual tissue tearing and placement action* | *Multi-step coffee pouch loading and machine interaction* |

---

## 📁 Repository Architecture

```text
vla-robotic-annotation-portfolio/
│
├── videos/
│   ├── task_01_tear_tissue_success.mp4
│   ├── task_02_load_coffee_machine_success.mp4
│   ├── task_03_wipe_wine_spill_success.mp4
│   ├── task_04_open_plastic_container_success.mp4
│   ├── task_05_transfer_pingpong_ball_success.mp4
│   ├── task_06_pour_balls_mug_success.mp4
│   ├── task_07a_stack_tower_success.mp4
│   ├── task_07b_stack_tower_fail.mp4
│   ├── task_08_place_object_bowl_success.mp4
│   └── task_09_grasp_apple_fail.mp4
│
├── annotations/
│   ├── markdown_format/
│   │   ├── task_01_tear_tissue_success.md
│   │   └── ... (all 10 .md task files)
│   │
│   └── json_format/
│       ├── task_01_tear_tissue_success.json
│       └── ... (all 10 .json task files)
│
└── README.md

```

## 🛠️ Core Competencies Demonstrated
*   AI Data Annotation & QA Curation
*   Embodied AI / Robotics Dataset Structuring
*   Model Alignment Workflows
*   Strict Formatting Constraint Adherence
*   JSON Data Schema Generation

*   ## 🔗 Data Sources & Attribution

The video clips in this portfolio were curated and cropped from open-source robotics datasets hosted on Hugging Face:

| Task ID | Task Description | Source Dataset (Hugging Face) |
| :--- | :--- | :--- |
| `task_01` | Tear Tissue & Place near Can | `lerobot/aloha_static_tissue` |
| `task_02` | Load Coffee Machine | [`lerobot/aloha_static_coffee_new`](https://huggingface.co/datasets/lerobot/aloha_static_coffee_new) |
| `task_03` | Wipe Spilled Wine | [`lerobot/aloha_mobile_wipe_wine`](https://huggingface.co/datasets/lerobot/aloha_mobile_wipe_wine) |
| `task_04` | Open Plastic Container Lid | [`lerobot/aloha_static_vinh_cup_left`](https://huggingface.co/datasets/lerobot/aloha_static_vinh_cup_left) |
| `task_05` | Ping Pong Ball Transfer | [`lerobot/aloha_static_pingpong_test`](https://huggingface.co/datasets/lerobot/aloha_static_pingpong_test) |
| `task_06` | Pour Balls into Mug | [`lerobot/dlr_sara_pour`](https://huggingface.co/datasets/lerobot/dlr_sara_pour) |
| `task_07a` | Stack Tower (Success) | [`lerobot/roboturk`](https://huggingface.co/datasets/lerobot/roboturk) |
| `task_07b` | Stack Tower (Collapse) | [`lerobot/roboturk`](https://huggingface.co/datasets/lerobot/roboturk) |
| `task_08` | Place Object in Red Bowl | [`kevin510/lerobot-cat-toy-placement`](https://huggingface.co/datasets/kevin510/lerobot-cat-toy-placement) |
| `task_09` | Grasp Maroon Apple (Fail) | [`Clementppr/lerobot_pick_and_place_dataset_world_model`](https://huggingface.co/datasets/Clementppr/lerobot_pick_and_place_dataset_world_model) |
