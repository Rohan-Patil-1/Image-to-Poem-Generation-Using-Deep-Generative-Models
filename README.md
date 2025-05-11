# Image-to-Poem-Generation-Using-Deep-Generative-Models

Welcome to the Image-to-Poem Generation project! This repository contains the implementation of a deep generative model designed to create creative, emotionally resonant poetry from visual inputs. The system leverages pre-trained convolutional neural networks (CNNs) and the CLIP model for feature extraction, combined with a fine-tuned GPT-2 decoder to generate poems that capture the mood, theme, or aesthetic of an input image, rather than literal descriptions.

## Project Overview
This project is an interdisciplinary exploration of computer vision, natural language processing, and computational creativity. Inspired by the methodologies outlined in the research paper Beyond Narrative Description: Generating Poetry from Images by Multi-Adversarial Training (Liu et al., 2018), we aim to advance AI-generated artistic expression. The model is trained and evaluated using the MultiM-Poem dataset (or an alternative curated dataset) and follows a two-stage encoder-decoder architecture.

**Authors:** Neha Anusooya Thimmarayi (nanusooy@depaul.edu), Rohan Shankar Patil (rpatil5@depaul.edu)

**Date:** May 11, 2025

**Status:** Under active development (submission deadline: June 3, 2025)

## Features
• Extracts visual features from images using the CLIP model.

• Transforms features into a conditioning prefix for a GPT-2 decoder.

• Generates stylized poetry reflecting the emotional and aesthetic content of images.

• Includes preprocessing pipelines for image-poem datasets.

• Supports evaluation with automated metrics (BLEU, ROUGE-L, Perplexity) and human judgment.

## Installation

### Prerequisites
• Python 3.9 or later

• Git (for cloning the repository)

• Access to a GPU is recommended but not required (CPU fallback supported)

### Dependencies
Install the required Python packages using pip. Run the following command in your terminal:

```
pip install torch torchvision transformers pandas numpy pillow requests tqdm
```

### Setup Instructions

1. Clone the Repository:

```
git clone https://github.com/your-username/Image-to-Poem-Generation-Using-Deep-Generative-Models.git
cd Image-to-Poem-Generation-Using-Deep-Generative-Models
```

2. Create a Virtual Environment (Optional but Recommended):

```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install Dependencies:

```
pip install -r requirements.txt
```

(Note: Create a requirements.txt file with the listed dependencies if not already present.)

4. Dataset Preparation:
   
• Download the MultiM-Poem dataset or an alternative (e.g., PoetryFoundation dataset from Kaggle) and place it in the data/ directory as multim_poem.json.

• Alternatively, the code will attempt to download and process a subset of images automatically (requires internet access).


## Project Structure

```
Image-to-Poem-Generation-Using-Deep-Generative-Models/
├── data/
│   ├── images/              # Directory for downloaded images
│   ├── processed/           # Processed datasets (e.g., cleaned_poems.csv)
│   └── multim_poem.json     # Raw dataset file
├── Image_to_Poem_Generation_CodeBase.ipynb  # Main notebook
├── README.md                # This file
├── requirements.txt         # Dependency list (to be created)
└── LICENSE                  # License file (optional)
```

## License
This project is released under the  MIT License. Feel free to use, modify, and distribute the code, provided you include the original copyright notice.

## Acknowledgments
• Inspired by the MultiM-Poem dataset and research by Liu et al. (2018).

• Built using open-source libraries from PyTorch, Hugging Face, and others.

• Thanks to DePaul University for academic support.

## Contact
For questions or collaboration, reach out to:

• Neha Anusooya Thimmarayi: nanusooy@depaul.edu

• Rohan Shankar Patil: rpatil5@depaul.edu