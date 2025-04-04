# 🎓 AI Lecture Notes Generator

An AI-powered agent that converts lecture audio into clean, structured notes using automatic speech recognition (Whisper) and a Large Language Model (Meta-LLaMA-3.1-8B-Instruct).

## 🚀 Features
- Upload lecture audio and get detailed notes
- Uses OpenAI Whisper for transcription
- Uses Meta-LLaMA-3.1 to generate structured markdown notes
- Gradio interface for easy interaction
- GPU-optimized with quantized model loading for performance

## 📋 Output Format
Generated notes include:
- # Topic
- ## Instructor
- ## Summary
- ## Key Concepts (bullet points)
- ## Key Points (bullet points)
- ## Takeaways (bullet points)

## 🧠 Tech Stack
- `torch`, `transformers`, `bitsandbytes`, `gradio`
- Whisper (ASR)
- LLaMA 3.1 (LLM for note generation)
- HuggingFace Hub for model access

## 🔧 Installation
Install dependencies:
```bash
pip install requests torch bitsandbytes transformers sentencepiece accelerate gradio httpx==0.27.2
