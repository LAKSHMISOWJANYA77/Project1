# Project1
Project Overview
This project is an extension of the research paper "LRFS: Online Shoppers’ Behavior-Based Efficient Customer Segmentation Model". While the original paper implemented multiple clustering techniques, this project focuses on Deep Embedded Clustering (DEC) to segment online shoppers based on their browsing behavior and purchase intent.

The dataset used is the Online Shoppers Intention dataset, which contains session-level features such as page durations, visitor types, month of visit, and revenue outcomes.

The key difference from the LRFS model is the integration of unsupervised deep learning for clustering, aiming to capture more complex, non-linear relationships in customer behavior.

Methodology
*Data Preprocessing & Feature Engineering
*Removed duplicates and irrelevant columns
*Converted categorical variables to numerical codes
*Created custom features (L, R, F, S) inspired by LRFS metrics
*Standardized features using StandardScaler
*Deep Embedded Clustering (DEC)
*Built an autoencoder to learn low-dimensional latent representations
*Initialized clusters using K-Means on latent space
*Fine-tuned cluster assignments using KL divergence loss and target distribution updates

Evaluation & Insights
*Calculated Silhouette Score for cluster quality
*Performed Customer Relationship Management (CRM) and Customer Profile Analysis (CPA) per cluster
*Assigned descriptive labels to clusters (e.g., Passive Customers, Loyal Buyers).

Results
*Number of Clusters: 4
*Silhouette Score (DEC): 0.3679
*Identified distinct customer groups with varying engagement and revenue potential.
