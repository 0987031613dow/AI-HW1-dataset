# TFT Champion Image Dataset

**Course:** Undergraduate AI Capstone, NYCU Spr2026
**Project:** #1 — Dataset Construction and Analysis
**Student ID:** 313605010

## Overview

A self-collected image classification dataset of TFT (Teamfight Tactics) champion units, captured from in-game screenshots.

| Class | Count |
|-------|-------|
| Azir | 49 |
| Mel | 57 |
| T-Hex | 53 |
| TahmKench | 40 |
| Zilean | 32 |
| **Total** | **231** |

## Data Type

- **Format:** RGB images (JPEG/PNG)
- **Input size used for training:** 224 × 224 pixels
- **Labels:** Folder name = class name (one folder per champion)

## Collection Process

Images were captured via manual screenshotting during live TFT gameplay and from publicly available game footage. Each champion was captured across multiple game states (different board positions, augment effects, and lighting) to introduce natural intra-class variation.

Images were manually reviewed to remove corrupted or mislabeled samples.

**Hardware/Software:** Standard gaming PC, Riot Games TFT client (PC).

## Dataset Structure

```
new_dataset/
├── Azir/
├── Mel/
├── T-Hex/
├── TahmKench/
└── Zilean/
```

## Notes

- One class (Thresh, 12 images) was excluded due to insufficient samples.
- The dataset is moderately imbalanced (Zilean: 32, Mel: 57).
- All images are original screenshots; no images were sourced from existing public datasets.
