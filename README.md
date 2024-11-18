Dialect-Aware Text-to-Image Generation Using Diffusion Models

Project Overview:

This repository contains the implementation of a research project focused on enhancing text-to-image generation models for Arabic dialects using diffusion-based models. The project investigates the performance of models like Alt Diffusion on various Arabic dialects, including Egyptian, Saudi, Moroccan, and Khaleeji, by transforming dialect prompts into Modern Standard Arabic (MSA) or English.


Objectives:

Evaluate the ability of text-to-image generation models to interpret and generate accurate images from Arabic dialects.

Transform dialectal prompts into MSA and English to enhance image quality.

Compare the performance of different text-to-image generation models, including Alt Diffusion.

Key Contributions:

Development of workflows for translating Arabic dialects into MSA and English.

Evaluation of the impact of dialect transformation on image generation quality.

Creation of a dialect-specific dataset based on the Flickr8K dataset.


Features:

Dialect Transformation: Converts dialectal Arabic captions to MSA and English using state-of-the-art models.

Text-to-Image Generation: Generates images from transformed captions using Alt Diffusion and other models.

Evaluation Metrics: Uses FID, Inception Score, and CLIP Score to assess the quality and relevance of generated images.

Repository Structure:

Dialect-Aware-Text-to-Image-Generation

README.md

LICENSE

requirements.txt

dataset.py

train.py

eval.py

utils.py

Installation:

1- Clone the repository:

git clone https://github.com/your-username/Dialect-Aware-Text-to-Image-Generation.git
cd Dialect-Aware-Text-to-Image-Generation

2- Install dependencies:

pip install -r requirements.txt

Usage:

1. Data Preparation

Use Generating_and_Preprocessing_Dialects_Data_last_version.ipynb to preprocess the Flickr8K dataset and generate dialectal captions.


2. Dialect Transformation

Run From_Arabic_Dialects_to_MSA_and_English_Transforamation_last_version.ipynb to transform dialect captions into MSA and English.

3. Image Generation:

Test the Alt Diffusion model with MSA-transformed captions using Testing_Alt_Diffusion_with_MSA_transformation_last_version.ipynb.

4. Evaluation:

Evaluate generated images using scripts in the src/ directory.

Evaluation Metrics:

Fréchet Inception Distance (FID): Measures similarity between generated and real images.

Inception Score (IS): Evaluates quality and diversity of generated images.

CLIP Score: Assesses alignment between text prompts and generated images.

Results:

Preliminary experiments with Alt Diffusion show that transforming dialectal prompts into MSA or English significantly improves image quality. Future experiments will incorporate Stable Diffusion and Flux Model for comparative analysis.

License:

This project is licensed under the MIT License.

