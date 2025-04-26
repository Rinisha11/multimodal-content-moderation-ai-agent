# Multimodal Content Moderation AI Agent
This project uses LangChain and Hugging Face models to detect inappropriate content from images, audio and text.

AI Moderation Agent—a system that can analyze text, image, and audio content, check platform policies, and decide what action to take. It doesn’t just scan for keywords. It thinks in context. This code successfully simulates or partially simulates most of the claimed functionalities:

It analyzes text, image, and audio.
It can take action, like flagging or removing harmful content. 
It uses RAG to pull up policies and influence decisions.
It can escalate borderline cases for human review.

## Features
Detects hate speech, toxicity, and graphic content. 
Understands content, transcribes audio, flags fake media. 
Aligns with real policies using RAG + FAISS. 
Makes policy-aware decisions and simulates moderation actions. 
Works with text, image, audio content. 

## Built using:
BERT for toxic text detection
CLIP for image classification
Whisper for audio transcription
Sentence Transformers + FAISS for policy retrieval
Few-shot prompting for quick learning

## Why it matters:
Helps platforms stay compliant
Reduces burnout for human moderators
Scales moderation ethically and efficiently

## Getting Started
Run the notebook in a Jupyter environment with necessary libraries.

## Requirements
- Python 3.8+
- transformers
- langchain

## Input Requirements

This notebook uses:

- **API Key** for HuggingFace or OpenAI (not included for security reasons)
- **Datasets** (local images or text files not included in the repo)

### How to Use

1. Set your API key:
   - Create a file named `.env` (or set as environment variable):
     ```
     HUGGINGFACE_API_KEY=your_api_key_here
     ```
   - Or directly set it in the notebook (not recommended for sharing).

2. Place your input files:
   - Store images in a folder like `input_images/`
   - Store text files in a folder like `input_text/`

> **Note:** These files/folders are not included in the repo. Add them locally to run the notebook.
