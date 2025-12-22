# Code Generation Model with Salesforce CodeGen

## Overview

This project demonstrates **fine-tuning a pre-trained causal language model (Salesforce CodeGen 350M)** on a custom Python code dataset. The pipeline extracts Python source files from a repository, identifies function definitions, and creates a structured dataset to train the model to generate code from prompts.

The model is optimized for **GPU-efficient training** on limited hardware such as Google Colab T4, using techniques like **gradient checkpointing**, **FP16 precision**, **gradient accumulation**, and memory-efficient data collators.

---

## Features

- Automatic extraction of Python files and function names from repositories
- Dataset creation mapping **source code to function names**
- Tokenization and preprocessing for causal language modeling
- Fine-tuning **Salesforce CodeGen-350M** model
- Memory-efficient training with:
  - FP16 mixed precision
  - Gradient checkpointing
  - Gradient accumulation
- Prompt-based code generation for inference

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/code-generation-model.git
cd code-generation-model
