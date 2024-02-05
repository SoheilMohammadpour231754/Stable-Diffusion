# Fine-Tuning Stable Diffusion on Gaming Assets

<br>

## Introduction

Welcome to our repository dedicated to fine-tuning Stable Diffusion, an open-source neural network for generating high-quality images. This project aims to enhance the capabilities of Stable Diffusion by fine-tuning it with gaming asset datasets.

Stable Diffusion is a deep learning, text-to-image model released in 2022 based on diffusion techniques. It is primarily used to generate detailed images conditioned on text descriptions, though it can also be applied to other tasks such as inpainting, outpainting, and generating image-to-image translations guided by a text prompt (Wikipedia contributors, 2024). 

<br>

## Getting Started

### Prerequisites

- Python 3.9+
- Installing the dependencies listed in `requirements.txt`.
```
pip install -r requirements.txt
```





<br>

## Data Preparation

To prepare your data for fine-tuning the Stable Diffusion model, follow these steps:

### Step 1: Organize Your Image Dataset

Place the images you wish to use for fine-tuning inside the `./data/images/` folder. Ensure that your dataset consists of high-quality images relevant to the gaming domain or any other style you're targeting.

### Step 2: Write Prompt for Images 

#### Single Prompt (for Dreambooth)

In Dreambooth, only a single well-defined prompt is used for fine-tuning all the images. This ensures that the model deeply underestand the specific theme we are aiming for.


#### Multiple Prompt Generation using BLIP (for Keras-CV)

To implement stable diffusion with Keras-CV, we require a separate prompt for each image in our dataset, in contrast to the approach in Dreambooth. We utilize the BLIP model to automatically generate descriptive captions for each image in the dataset. You can find the script in ./preparation/auto prompting using BLIP.ipynb and follow the step-by-step guide for generating the prompts.



<br>

## Fine-Tuning Process

#### Fine-tuning Stable Diffuison using Dreambooth

To do.

#### Fine-tuning Stable Diffuison using Keras-CV

To do.

<br>

## Evaluation

To do.

