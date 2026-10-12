# Parsa Naderi

[LinkedIn](https://linkedin.com/in/parsanaderi) · [Scholar](https://scholar.google.com/citations?user=lHdgX5wAAAAJ&hl=en)\
parsanaderi@aut.ac.ir\
parsanaderi2004@gmail.com

- Computer Science undergraduate at Amirkabir University of Technology (Tehran Polytechnic)
- Undergraduate research assistant at Sharif University of Technology
- Working on generative models for financial time series and on robustness and interpretability in machine learning

## Research

**StochLOB: Heavy-Tailed Score Matching for Robust Limit Order Book Trend Prediction**\
*Third author · Accepted as an oral at the NeurIPS 2026 Workshop on AI for Stochastic Dynamics (STODY) · [Code](https://github.com/ArshiAbolghasemi/Penny)*

- Gaussian training-time corruption in denoising score matching under-represents large market moves, so StochLOB uses compound Poisson and clipped α-stable noise instead
- The heavy-tailed noise helped in several of the most volatile windows, while the Gaussian baseline stayed competitive on clean data
- The score head is used only in training, so inference remains a single deterministic forward pass
- My part: the stress-regime evaluation, the OF-SATNet baseline, the attention-pooling module and the workflow figure

**Diffusion Models in Finance: A Systematic Review**\
*Lead author · Manuscript in preparation*

- Started after finding no finance-specific review of diffusion models; wrote the protocol and recruited collaborators
- Screening and data extraction are complete, and the manuscript is being written

**A Feature-Engineered Dataset and Benchmarks for the LM Arena 140K Human Preference**\
*With collaborators at Sharif University of Technology and the Alan Turing Institute · Manuscript in preparation · [Dataset](https://huggingface.co/datasets/Gholamali/Arena_Human_Preference_90K_features_verified) · [Code](https://github.com/Nazanin-Mirzaei/arena-preference-features)*

- Released on Hugging Face as *Arena Human Preference 90K: Engineered Features and Correctness Annotations*: about 90K battles with interpretable features, computed without reading the preference label and without any transformer inference
- A human-reviewed subset of 218 battles shows that roughly a third of preference labels don't track correctness
- My parts: the language-identification module for noisy LLM outputs, and the 34 A-vs-B comparators (218 features) in the pipeline code

**Arena Preference Classifier** · [Code](https://github.com/ParsaNaderiX/arena-preference-classifier)

- Predicts all four outcomes (A wins, B wins, tie, both bad) from the released features
- Swapping A and B as augmentation halved position bias, unlike a random-swap control
- Ties and "both bad" are partly predictable (AUC 0.60-0.63), though argmax rarely picks them
