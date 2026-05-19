# Visual_Q-A_multimodal_System
Multimodal Visual Question Answering using LongCLIP vision encoding and Qwen3 language modelling.

A custom LLaVA style multimodal Visual Question Answering (VQA) system integrating a LongCLIP vision encoder with the Qwen3 language model for image-based multiple-choice reasoning tasks.

**Overview**

This project implements a multimodal Visual Question Answering architecture designed to jointly process visual and textual information for multiple choice question answering. The system combines pretrained vision language representations with parameter efficient fine-tuning techniques to improve multimodal reasoning performance.

The project focuses on:

Vision-language alignment,
Multimodal feature fusion,
Parameter efficient fine-tuning using LoRA,
Prompt engineering for reasoning improvement,
Training stability and optimisation techniques

The final model achieved a validation accuracy improvement from approximately 24.97% to 69.21% through systematic experimentation and architectural optimisation.

**Architecture**

The multimodal pipeline consists of:

LongCLIP Vision Encoder

Extracts visual embeddings from input images

Qwen3 Language Model

Processes textual questions and answer options

Multimodal Projection Layer

Aligns visual embeddings with the Qwen3 hidden representation space

Fusion Mechanism

Combines projected visual tokens with tokenised textual inputs

Classification Head

Predicts one of four answer choices (A, B, C, or D)

<img width="1536" height="1024" alt="vqa" src="https://github.com/user-attachments/assets/cbdf3f1c-e7a2-4e13-bf93-0a0eda16d018" />


**Key Features**

Custom LLaVA-style multimodal architecture,
LongCLIP vision encoding,
Qwen3 language reasoning,
LoRA fine-tuning for memory-efficient training,
Structured instruction-style prompt engineering,
Residual multimodal projection layers,
Cosine annealing learning rate scheduling,
ColorJitter data augmentation,
Extensive experimentation and ablation analysis and
Performance Optimisation Experiments

The project was trained and evaluated on a multimodal Visual Question Answering dataset consisting of:

Images,
Multiple choice questions and 
Four answer options per sample

The task required predicting the correct answer choice based on both visual and textual understanding.
**Dataset not included due to size/privacy restrictions**.
