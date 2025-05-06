# Multimodal-Recommendation-System
## Cross-Domain Recommendation System

This project aims to build a **Cross-Domain Recommendation System** capable of suggesting movies or music based on a user's preferences in books, and vice versa. It is inspired by the paper [“Personalized Transfer of User Preferences for Cross-domain Recommendation”](https://arxiv.org/pdf/2110.11154v3.pdf) and utilizes the **Amazon Reviews dataset** to train and evaluate models.

## Overview

**Cross-domain recommendation** allows learning user preferences in one domain (e.g., books) and transferring them to another (e.g., movies or music). This is particularly useful when user activity is sparse in one domain but abundant in another.

We began by implementing a basic **single-domain recommender**, then extended the logic to a **cross-domain scenario** using techniques such as embedding alignment, shared latent space learning, and transfer learning.

## Dataset

We use subsets of the **Amazon Product Reviews dataset**:
- Books
- Movies & TV
- Music

The data includes user reviews, ratings, and product metadata.    
It can be found on this [link](https://www.kaggle.com/datasets/maitreyi1506/cross-domain-recommendation)

> Source: https://nijianmo.github.io/amazon/index.html

## Architecture

Our current approach is based on the **EMCDR (Embedding and Mapping for Cross-Domain Recommendation)** model:
- Separate embedding layers for source and target domains
- Mapping function (MLP) for transferring source-domain embeddings
- Shared interaction layers for generating recommendations

> Base paper: [arXiv:2110.11154v3](https://arxiv.org/pdf/2110.11154v3.pdf)

## Testing

The product can be tested on the following link: (https://cross-domain-recommender.streamlit.app/)


