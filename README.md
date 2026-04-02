# Conversation Coaching Experiment

This repository contains my experiment on generating structured coaching feedback for charitable persuasion conversations using open-source large language models.

## Project Objective

The goal of this project was to test whether a smaller open-source base model, after task-specific fine-tuning, could outperform a larger instruction-tuned model used directly in zero-shot mode for coaching feedback generation.

The experiment compares:

- Qwen3.5-9B Instruct (baseline, zero-shot)
- Qwen3.5-4B Base + QLoRA fine-tuning
- Qwen3.5-9B Base + QLoRA fine-tuning

## Dataset

The project uses the **Persuasion for Good** dataset, which contains annotated charitable persuasion dialogues.

## Repository Structure

- `notebooks/` — experiment notebooks
- `src/` — Python code
- `data/input/` — raw input files
- `data/processed/` — processed files for training and evaluation
- `outputs/images/` — plots and visuals
- `outputs/metrics/` — CSV and JSON outputs
- `outputs/artifacts/` — additional result artifacts
- `docs/` — supporting documentation

## Main Outcome

The 4B fine-tuned model emerged as the strongest practical choice under limited compute conditions, showing that task-specific fine-tuning and domain alignment can matter more than raw model size for specialized tasks.

## Notes

- Large checkpoints, caches, and adapter files are intentionally excluded from GitHub.
- This repository focuses on the experiment workflow, data preparation, outputs, and evaluation artifacts.

## Author

Siddharth Tiwari
