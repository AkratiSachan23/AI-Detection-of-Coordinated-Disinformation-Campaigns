# AI Detection of Coordinated Disinformation Campaigns

This project builds an AI-based system to detect coordinated disinformation campaigns using graph neural networks and social network analysis. It identifies patterns of coordinated user behavior across social media platforms to flag disinformation networks.

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

## Installation
```bash
pip uninstall torch -y
pip install torch==2.2.0+cpu -f https://download.pytorch.org/whl/cpu
pip install torch-geometric
pip install pyg-lib -f https://data.pyg.org/whl/torch-2.2.0+cpu.html
