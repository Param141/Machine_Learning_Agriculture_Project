Fasal Saathi: Core AI Models for Agricultural Crop Disease Detection 🌱
This repository contains the core deep learning and machine learning architectures developed and benchmarked for automated crop disease classification. The finalized, high-performing model pipelines in this repository serve as the core intelligence engine deployed in the production Android application Fasal Saathi on Google Play[cite: 19].

The models here address disease detection across two custom-curated agricultural datasets:

Indian Ridge Gourd Leaves: Healthy, Leaf Minor Infested, and Mosaic Virus[cite: 17, 20].

Brinjal (Eggplant) Leaves: Healthy vs. Unhealthy (Phomopsis Blight and Little Leaf / Leaf Curl)[cite: 20].

📌 Project Highlights & Research Impact
📱 Production Deployment: The best-performing quantized architectures power the live mobile application Fasal Saathi[cite: 19].

📄 Research Publication: Benchmarked Ridge Gourd models formed the research presented at the MIND 2025 conference[cite: 17].

📜 Patent Recognition: The underlying AI-assisted methodology for leaf disease classification is recognized under a Granted Indian Design Patent[cite: 17].

📊 Open Datasets:

Ridge Gourd Dataset (9,000 images): Published on IEEE DataPort[cite: 17].

Brinjal Leaf Dataset: Published on Mendeley Data[cite: 20].

🤖 Architectures & Model Exploration
Multiple convolutional neural network baselines, transfer learning backbones, and hybrid configurations were implemented to identify the optimal trade-off between edge device inference latency and classification accuracy:

DenseNet-121 Pipelines: Best-performing transfer learning architecture for fine-grained feature extraction across diseased leaf regions.

Hybrid CNN Architectures: Feature extractor fusion (e.g., DenseNet121 feature backbones paired with custom dense decision heads).

MobileNet & MobileNetV2: Parameter-efficient, lightweight networks benchmarked specifically for real-time mobile inference constraints.

Custom CNNs: Baseline convolutional architectures built from scratch for feature ablation.

CNN + Support Vector Machine (SVM): Hybrid classification setups using deep convolutional representations evaluated with maximum-margin decision boundaries.

📁 Repository Structure
Plaintext
├── DenseNet121_Correct_Brinjal.ipynb   # Best-performing DenseNet121 pipeline for Brinjal leaf classification
├── densenet_test_results.pkl           # Serialized evaluation metrics & test predictions for DenseNet121
├── hybridcnn(dn121).py                 # Hybrid DenseNet-121 architecture implementation
├── Normal_CNN.py                       # Standard custom CNN baseline pipeline
├── customcnn.py                        # Custom deep CNN variant
├── copy_of_mobilenet.py                # MobileNet baseline implementation
├── copy_of_mobilenetv2_softmax.py      # MobileNetV2 with specialized Softmax classification head
├── svm+cnn.py                          # Deep feature extraction paired with Support Vector Machine
└── README.md                           # Documentation
⚙️ Installation & Usage
1. Prerequisites
Ensure Python 3.8+ is installed along with the primary deep learning and data processing libraries:

Bash
pip install torch torchvision torchaudio opencv-python scikit-learn numpy matplotlib pandas
2. Running an Architecture
To train or evaluate one of the stand-alone PyTorch scripts:

Bash
python "hybridcnn(dn121).py"
To run the full training and evaluation notebook for the Brinjal leaf disease classifier:

Bash
jupyter notebook DenseNet121_Correct_Brinjal.ipynb
📊 Datasets & Citation
If you make use of the models or datasets associated with this repository, please reference the corresponding public releases:

Indian Ridge Gourd Dataset: IEEE DataPort Entry[cite: 17]

Brinjal Leaf Image Dataset: Mendeley Data Entry (DOI: 10.17632/c39p3k87g2.1)[cite: 20]
