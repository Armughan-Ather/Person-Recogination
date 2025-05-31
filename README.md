# Person-Recogination Using Gait Matching
This project implements a deep learning-based system for person recognition using gait patterns, a biometric modality that enables non-intrusive, contactless identification from a distance. We propose a hybrid CNN-LSTM architecture that captures both spatial and temporal features from silhouette sequences to recognize individuals based on their walking style.

Key features:

Trained on the CASIA-B dataset (25 subjects), which includes walking under normal, bag-carrying, and clothing-varied conditions.

Combines TimeDistributed CNN layers with stacked LSTMs to extract motion-based embeddings.

Supports both closed-set and open-set recognition, identifying unseen individuals as "unknown" using cosine similarity and dynamic thresholds.

Evaluated using 5-fold cross-validation, achieving an average accuracy of 80.67%, with consistent validation performance across folds.

Detects unknown individuals with F1-scores ranging from 0.81 to 0.87, demonstrating robustness for real-world scenarios.

Despite computational constraints (limited to 10 training epochs per fold), the model shows promising results and lays the foundation for scalable gait-based identification systems.

Dataset source: https://www.kaggle.com/datasets/trnquanghuyn/casia-b/data

