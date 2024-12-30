# lip-reader-cv

This is a deep learning-based model designed to transcribe speech from video sequences by analyzing lip movements. This repository implements a comprehensive pipeline for lip-reading, including data preprocessing, model training, and prediction. The model leverages 3D convolutional layers for spatiotemporal feature extraction, bidirectional LSTMs for sequence learning, and a Connectionist Temporal Classification (CTC) loss function for alignment-free text prediction.

***Features***

- Video Processing: Preprocesses video data by extracting grayscale frames and normalizing them.
- Text Alignments: Maps frames to text alignments for supervised learning.
- Neural Network Architecture: Combines 3D convolutional layers and bidirectional LSTMs to process spatial and temporal information.
- CTC Loss: Enables the model to handle sequence-to-sequence learning without explicit alignment.
- Real-Time Evaluation: Generates predictions after every training epoch to monitor model performance.

**Model Architecture**

3D Convolutional Layers:
- Extract spatiotemporal features from video frames.
- Includes three Conv3D layers followed by ReLU activation and MaxPooling layers.

Bidirectional LSTMs:
- Process sequential data to capture temporal dependencies.
- Two layers of bidirectional LSTMs with dropout regularization.

Dense Output Layer:
- Classifies characters using softmax activation.

**CTC Loss:
**
- Used for sequence alignment and transcription.

**Dependencies
**Install the required libraries using pip:
pip install tensorflow opencv-python matplotlib gdown imageio


