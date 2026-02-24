
Medical Visual Question Answering (VQA) – PathVQA
Problem Statement
This project focuses on building a Medical Visual Question Answering (VQA) system for pathology images.
The system takes a pathology image and a related clinical question as input and predicts the correct answer based on visual understanding.

Example:
Image + Question → Answer
"Is the tumor malignant?" → "Yes"

Dataset
Dataset Used: PathVQA (Pathology Visual Question Answering)
The dataset consists of pathology images paired with clinical question–answer sets.
Questions include yes/no, tissue identification, disease classification, and reasoning-based queries.

Model Architecture
Text Encoder: BERT-base (bert-base-uncased)
Used to generate contextual embeddings from clinical questions.

Image Encoder: ResNet-50 (ImageNet pre-trained)
Used to extract visual features from pathology images.

Fusion Method:
Image features and question embeddings are concatenated and passed through fully connected layers for answer prediction.

Training Details
Transfer Learning applied on both BERT and ResNet-50

Multi-class classification task

Optimizer: AdamW

Loss Function: CrossEntropyLoss

Total Answer Classes: 799

Results
Best Test Accuracy Achieved: 30%
