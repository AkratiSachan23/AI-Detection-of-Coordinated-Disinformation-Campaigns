# AI Detection of Coordinated Disinformation Campaigns

This project builds an AI-based system to detect coordinated disinformation campaigns using graph neural networks and social network analysis. It identifies patterns of coordinated user behavior across social media platforms to flag disinformation networks.
This project is an end-to-end pipeline for detecting coordinated influence operations (bots, propaganda clusters, manipulated networks) on social media platforms like Twitter/X.

## Features
- Graph-based modeling of user interactions
- Detection of coordinated patterns and bot-like activity
- Support for large-scale datasets
- PyTorch + PyTorch Geometric based model

## Tech Stack
- Python
- PyTorch
- PyTorch Geometric
- NetworkX
- Scikit-Learn
- Jupyter Notebook

##📊 Architecture Pipeline
 Tweets Dataset  
     ↓  
Extract Mentions (@user)  
     ↓  
Build Social Graph (Nodes = Users, Edges = Mentions)  
     ↓  
Node2Vec Embeddings (12447 × 128)  
     ↓  
GraphSAGE (Unsupervised Embedding Refinement)  
     ↓  
KMeans Clustering → Discover Latent Communities  
     ↓  
Manual Labeling of Suspicious Clusters  
     ↓  
Supervised GNN Classifier  
     ↓  
Evaluation + Explainability  


## Installation
```bash
pip uninstall torch -y
pip install torch==2.2.0+cpu -f https://download.pytorch.org/whl/cpu
pip install torch-geometric
pip install pyg-lib -f https://data.pyg.org/whl/torch-2.2.0+cpu.html
