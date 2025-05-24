# DeepFakeDetection
In the era of rapidly advancing computational power, deep learning has enabled the creation of realistic human-synthesized videos—commonly known as deep fakes—that can be nearly indistinguishable from genuine media. While this technology has numerous creative applications, it also poses significant risks, including political manipulation, fake terrorism events, revenge porn, and blackmail. This project tackles the challenge head on: using Artificial Intelligence (AI) to fight Artificial Intelligence (AI).

**Overview**
This repository contains a state-of-the-art deep learning system designed to automatically distinguish AI-generated fake videos from authentic ones. The system specifically addresses:

Replacement deep fakes: where one face is swapped with another.

Reenactment deep fakes: where the facial movements are mimicked on a different face.

By leveraging a combination of Convolutional Neural Networks (CNN) and Recurrent Neural Networks (RNN), the system extracts and analyzes frame-level features to detect manipulations in the video stream.

**Methodology**
Feature Extraction
ResNeXt CNN:
The backbone of the detection system is a ResNeXt convolutional neural network. It is employed to extract robust frame-level features from input videos. The network architecture is chosen for its enhanced capacity to capture detailed spatial features while keeping the number of parameters manageable.

**Temporal Analysis**
LSTM-based RNN:
The extracted features are then passed on to an LSTM-based Recurrent Neural Network. By processing the sequential information in the video frames, the LSTM helps in understanding temporal patterns, which is crucial for detecting subtle inconsistencies that reveal deep fake manipulations.

**Training and Evaluation**
Dataset Composition:
To ensure the method performs effectively in real-world scenarios, the system is evaluated on a large, balanced, and mixed dataset. The training data is curated by integrating several publicly available datasets including:

Face-Forensic++

Deepfake Detection Challenge

Celeb-DF

Robust Performance:
The proposed approach achieves competitive results through a simple yet robust methodology that can be extended and fine-tuned for various deep fake detection tasks.

**Key Features**
Automatic Deep Fake Detection:
The system is fully automated and requires minimal human intervention, making it practical for real-time or batch video analysis.

Hybrid Architecture:
Combines spatial feature extraction using a ResNeXt CNN with temporal analysis using an LSTM-based RNN.

Real-time Simulation:
Evaluation on mixed datasets ensures that the approach generalizes well to real-time data scenarios.

Competitive Performance:
Even with a straightforward strategy, the detection system delivers results on par with more complex models.

**Getting Started**
To get started with this project:

1.Clone the repository:

```bash

git clone https://github.com/nishan2582/deep-fake-detection.git
```


2.Install the required dependencies:
Refer to requirements.txt and install dependencies using:

```bash
Copy
Edit
pip install -r requirements.txt
```

3.Set up the datasets:
Download and prepare the datasets as described in the documentation.

4.Train and Evaluate:
Run the training script and evaluate the results using the provided notebooks and scripts.

**Contributions and Future Work**
We welcome contributions, whether it’s improving the detection model, optimizing the pipeline for better performance, or expanding the system to handle new deep fake techniques. Future directions include:

Integrating additional datasets to cover a wider variety of deep fake manipulations.

Enhancing the model’s speed to support real-time video processing applications.

Experimenting with different network architectures and fusion strategies for improved accuracy.

**Acknowledgements**
This project builds on insights and previous works in the domain of deep fake research. Special thanks to the creators of the Face-Forensic++, Deepfake Detection Challenge, and Celeb-DF datasets for making their data publicly available.

