## 🌾🌾AgriAid AI — Crop Recommendation & Plant Disease Assistant using Gemma 3n

This project fine-tunes Google DeepMind’s Gemma 3n large language model to act as an intelligent agriculture assistant. The model provides crop recommendations, farming advice, and plant disease diagnosis support based on soil, climate, and user queries.

## Project Overview

Large foundational models like Gemma 3n are capable of processing multimodal input (text + images) and generating useful outputs across domains. In this project, I fine-tuned the Gemma 3n model on agriculture-specific data to create an AI assistant that:

- Provides personalized crop recommendations based on soil and climate inputs.
- Performs disease diagnosis from plant images.
- Serves as a practical AI tool for real-world agricultural decision support.

## Model Architecture

- Base model: Google Gemma 3n (open weights) — a lightweight, multimodal transformer capable of processing images and text.
- Fine-tuning strategy:
   - Used LoRA (Low-Rank Adaptation) to adapt the model to agriculture data efficiently.
   - Trained on both textual agricultural data and images of plant leaves.
- Model Inputs:
   - Plant images for disease diagnosis.
   - Soil and environmental text features for crop recommendations
- Model Outputs:
   - Textual, speech recommendations and disease labels
 
## Dataset

The model was fine-tuned on a combination of:
   - Domain-specific datasets consisting of soil and climate attributes
   - Labeled crop yield or recommendation targets
   - Plant leaf disease images with expert labels

## Tech Stack

- Python
- PyTorch
- Hugging Face Transformers
- PEFT (LoRA)
- Kaggle Notebooks

## Example Queries & Model Responses

Here are sample prompts used to validate model behavior:
   - “Which crop is suitable for sandy soil with low rainfall?”
   - “What disease do these tomato leaves have?”

## Acknowledgements

- Google DeepMind — Gemma model
- Kaggle — Gemma Impact Challenge
- Hugging Face — Transformers & PEFT libraries

