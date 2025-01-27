# Multi-Headed vs. Single-Headed Attention in Transformer-based Models

This repository contains the implementation and results of experiments investigating the impact of multi-headed and single-headed attention mechanisms in transformer-based models. The project focuses on understanding the significance of individual attention heads and evaluating the performance differences between multi-headed and single-headed configurations.

## Project Overview
Transformers have revolutionized Natural Language Processing (NLP), with multi-headed attention being a key innovation. This project explores:

The importance of individual attention heads in transformer models.
The performance trade-offs of multi-headed vs. single-headed attention configurations.
Experimental results on two popular pre-trained transformer models: GPT-2 (decoder-only) and DistilBERT (encoder-only).
Key Features
Experiments with head pruning strategies (top-K, bottom-K, and random-K).
Analysis of head importance using gradient-based metrics.
Comparison of multi-headed and single-headed attention mechanisms.
Evaluation on the Stanford Sentiment Treebank (SST-2) dataset.
Repository Structure
code/: Implementation files for training and fine-tuning models.
notebooks/: Jupyter Notebooks for analysis and visualization.
results/: Experiment results and performance metrics.
report/: Detailed project report and findings.
README.md: Project documentation.
Technologies Used
Frameworks: PyTorch, Hugging Face Transformers.
Models: DistilBERT, GPT-2.
Dataset: Stanford Sentiment Treebank (SST-2).
Tools: Jupyter Notebook, Matplotlib, Gradient-based analysis.
Results Summary
Disabling the most important heads significantly degrades performance.
Disabling the least important heads or random heads has minimal impact, with some cases showing slight improvements.
Single-headed models underperform multi-headed models, reinforcing the importance of attention diversity.
How to Use
Clone this repository:
bash
Copy
Edit
git clone https://github.com/username/repo-name.git
Install dependencies:
bash
Copy
Edit
pip install -r requirements.txt
Run the notebooks in notebooks/ to replicate the analysis:
bash
Copy
Edit
jupyter notebook
Future Work
Extending experiments to additional datasets and tasks.
Investigating dynamic head pruning methods.
Exploring linguistic phenomena linked to attention heads.
Acknowledgments
This project was completed as part of DS4440 coursework at Northeastern University. Special thanks to the teaching team for their guidance
