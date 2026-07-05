# ChronosImage AI Studio V6.2

**Image-to-Image • Storyboard • AI Prompt Studio**

Version: **V6.2**

------------------------------------------------------------------------

## Introduction

ChronosImage AI Studio is a local AI image generation studio supporting
multiple AI providers.

### Supported Providers

-   Mock Generator (Offline Demo)
-   OpenAI GPT Image
-   Google Gemini Image (Nano Banana)

------------------------------------------------------------------------

# Features

## AI Image Generation

-   Text-to-Image
-   Image-to-Image
-   Prompt Enhancement
-   Commercial Quality Prompt Builder
-   Batch Generation
-   Aspect Ratio
-   Lighting
-   Camera
-   Mood
-   Detail Level
-   Negative Prompt

## Image-to-Image

Upload a reference image and generate a new image while preserving
important visual characteristics.

Reference Strength:

-   Low
-   Medium
-   High

Supported formats:

-   PNG
-   JPG
-   JPEG
-   WEBP

## Storyboard

Generate storyboard scenes automatically.

Features:

-   Storyboard Planning
-   Frame List
-   Camera Suggestions
-   Mood Suggestions
-   Sketch Storyboard
-   Final Art Storyboard

Supports **2--12 frames**.

## Prompt Enhancement

Transforms a simple prompt into a professional-quality prompt.

Example:

``` text
Input:
A dragon
```

Enhanced:

``` text
A majestic mechanical dragon,
cinematic lighting,
ultra detailed,
professional composition,
masterpiece,
8K,
volumetric lighting,
sharp focus.
```

## History

Stores:

-   Generated Images
-   Prompt
-   Enhanced Prompt
-   Provider
-   Time
-   Quality Score

### New in V6.2

-   Delete Single History
-   Force Clear All History
-   Deletes related generated images and metadata JSON

## Prompt Library

Save and reload prompts instantly.

## Favorites

Save important generated images.

## Export

Each generated image exports a metadata JSON containing:

-   Prompt
-   Enhanced Prompt
-   Provider
-   Size
-   Aspect Ratio
-   Settings

------------------------------------------------------------------------

# Folder Structure

``` text
ChronosImage_AI_Studio_V6_2
│
├── app.py
├── index.html
├── style.css
├── script.js
├── requirements.txt
├── .env.example
├── outputs/
├── uploads/
├── history/
├── prompts/
├── favorites/
├── exports/
├── storyboards/
├── logs/
└── projects/
```

# Installation

``` bash
install.bat
```

or

``` bash
pip install -r requirements.txt
```

# Start

``` bash
start_all.bat
```

or

``` bash
python app.py
```

Backend:

    http://127.0.0.1:7860

# API Configuration

Edit `.env`

``` env
OPENAI_API_KEY=YOUR_API_KEY
GEMINI_API_KEY=YOUR_API_KEY
```

Restart the backend after editing.

# Mock Mode

Mock mode works without any API key and is useful for:

-   UI testing
-   Prompt testing
-   Storyboard testing
-   History testing

# Troubleshooting

## Backend not connected

``` bash
python app.py
```

## Failed to fetch

The backend is not running.

## Missing API Key

Edit `.env`, add your API key, then restart the backend.

## History cannot be deleted

Use **Force Clear All History** and restart the backend if files are
locked.

# Roadmap (V7)

Planned features:

-   FLUX
-   Stable Diffusion
-   ComfyUI
-   Automatic1111
-   ControlNet
-   LoRA
-   Inpainting / Outpainting
-   AI Upscaling
-   Character Consistency
-   AI Video Generation
-   AI Animation
-   Plugin System

# License

This project is intended for learning, experimentation, and personal
development.

Users are responsible for complying with the terms of any third-party AI
service they connect.
