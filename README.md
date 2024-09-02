# MULTIMODALSEARCH
## Overview
The MULTIMODALSEARCH project aims to build a multimodal search system by combining text and image embeddings. The project involves loading and processing product data, generating embeddings for both text and images, and using these embeddings to find similar products. This system can be applied to tasks such as product recommendation and content-based image retrieval.

## Project Goals
Data Processing: Load and preprocess product data and images from CSV files.
Feature Extraction: Generate text embeddings using a SentenceTransformer model and image embeddings using a MobileNet model.
Embedding Storage: Store and manage embeddings for efficient retrieval and comparison.
Search and Visualization: Implement a nearest neighbors search to find similar products and visualize results.

## Getting Started
### Prerequisites
Ensure you have the following Python packages installed:

numpy
pandas
tensorflow
matplotlib
Pillow
scikit-learn
sentence-transformers
pickle5

## Data Acquisition
CSV Data: The project reads product data from train.csv.
Images: Images are loaded from the train_images/ directory.

## Code Walkthrough
1. Loading Data:

Load product data from train.csv and preview the dataset.
Display some sample images and their corresponding product titles.

2. Text and Image Embeddings:

Generate text embeddings using the stsb-distilbert-base SentenceTransformer model.
Generate image embeddings using MobileNet, resized to 224x224 pixels.

3. Embedding Storage:

Store text and image embeddings using pickle for future use.

4. Search Implementation:

Use Nearest Neighbors to find similar products based on combined text and image embeddings.
Visualize search results with matched images and titles.

5. Evaluation:

Evaluate search performance on test data and visualize results.

## Model Training and Evaluation
1. Text Embeddings:

Extract embeddings from product titles using a pre-trained SentenceTransformer model.

2. Image Embeddings:

Extract embeddings from product images using a pre-trained MobileNet model.

3. Nearest Neighbors Search:

Use the Nearest Neighbors algorithm to find similar products based on combined embeddings.

4. Visualization:

Visualize sample images and their similar counterparts to validate search results.

## Results
The project demonstrates a functional multimodal search system that integrates text and image data for finding similar products. The search results are visualized with matched images and product titles, providing an intuitive way to explore similar items.