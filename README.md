# Cutis-1: AI-Powered Skin Condition Scanner

*Cutis-1* is a proof-of-concept project that uses deep learning to analyze skin images and identify potential irregularities. Built as part of [PITTAN Inc.](https://www.pittan.life/)'s *Virtual Human Model* initiative, this prototype demonstrates the feasibility of non-intrusive skin diagnostics on edge devices.

## Overview

- Accepts user-submitted skin images and body part labels  
- Uses a fine-tuned EfficientNet-based model trained on the DermNet dataset  
- Classifies conditions across multiple dermatological categories  
- Falls back to “Pass / No Pass” result if confidence is low or classification is uncertain  
- Designed for lightweight deployment in virtual health monitoring systems  

## Proof of Concept

This project is an early-stage prototype. While initial results show promise, the following improvements are planned:

- Boosting accuracy through:
  - Larger and more diverse training datasets  
  - Domain-specific image augmentation  
- Reducing class granularity to improve top-1 prediction confidence  
- Optimizing the model for real-time inference on embedded hardware  

## Tech Stack

- **Model**: EfficientNet-B0 with transfer learning  
- **Frameworks**: PyTorch, torchvision, timm  
- **Data**: [DermNet](https://www.kaggle.com/datasets/shubhamgoel27/dermnet) skin condition dataset  
- **Interface**: Command-line and image processing pipeline (UI TBD)  

## Disclaimer

This tool is **not intended for medical diagnosis**. It is strictly a research and development prototype.
