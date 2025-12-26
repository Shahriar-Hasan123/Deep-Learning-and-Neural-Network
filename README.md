# Deep Learning and Neural Network Repository  
  
A comprehensive collection of 14 deep learning assignments organized by progressive learning objectives, covering computer vision, data analysis, and advanced neural network techniques.  
  
## 📁 Assignment-by-Assignment Guide  
  
### Assignment 1: CNN Model Comparison  
**Focus**: Transfer learning performance comparison across 10 CNN architectures  
  
**Key Components**:  
- Dataset: CIFAR-100 (first 20 classes, limited to 4,000 training samples)  
- Models: VGG16, VGG19, ResNet50, ResNet101, MobileNetV2, EfficientNetB0, InceptionV3, Xception, InceptionResNetV2, DenseNet121  
- Memory management with `clear_memory()` function  
- Dynamic resizing (64×64 for most models, 75×75 for Inception family)  

---  
  
### Assignment 2: Activation Function Analysis  
**Focus**: Impact of different activation functions on CNN performance  
  
**Key Components**:  
- Dataset: CIFAR-100 (20 classes)  
- Activations tested: ReLU, Sigmoid, Softmax  
- 10 CNN architectures with systematic comparison  
- Memory cleanup after each model training  
  
---  
  
### Assignment 3: System Architecture  
**Focus**: Transfer learning and feature extraction analysis  
  
**Key Components**:  
- Dataset: MNIST resized to 48×48×3 for VGG16 compatibility  
- Feature extraction before and after transfer learning  
- VGG16 backbone with custom classification head  
- Dimensionality reduction analysis (PCA, t-SNE, LDA)  
  
---  
  
### Assignment 4: Custom Training Loops  
**Focus**: Manual training implementation vs. model.fit()  
  
**Key Components**:  
- Dataset: MNIST with preprocessing  
- Custom training loop using `tf.GradientTape()`  
- Performance comparison between manual and automatic training  
- Simple CNN architecture for demonstration  
  
---  
  
### Assignment 7: YOLO & RNN  
**Focus**: Object detection and sequence modeling  
  
**Key Components**:  
- **YOLO Face Detection**: WIDER FACE dataset integration  
- Kaggle API setup for dataset downloads  
- Ultralytics YOLO implementation  
- **RNN Components**: IMDB sentiment analysis (mentioned in system architecture)  
  
---  
  
### Assignment 8: Data Analysis Pipeline  
**Focus**: Comprehensive data processing workflow  
  
**Key Components**:  
- Dataset: Oxford IIIT Pet via TensorFlow Datasets  
- Pipeline functions: `load_data()`, `clean_data()`, `transform_data()`, `run_analysis()`, `plot_data()`  
- Highest priority assignment (5.46 importance score)  
- End-to-end data analysis demonstration  
  
---  
  
### Assignment 10: Advanced Autoencoders  
**Focus**: Generative models and representation learning  
  
**Key Components**:  
- **Normal Autoencoder**: MNIST reconstruction with 64-dim latent space  
- **Denoising Autoencoder**: Gaussian noise addition and removal  
- **Variational Autoencoder**: Reparameterization trick implementation  
- Image generation from noise vectors (mean=5, variance specified)  
  
---  
  
### Assignment 11: Face Verification  
**Focus**: Metric learning and similarity analysis  
  
**Key Components**:  
- Dataset: LFW People dataset via Kaggle API  
- Three loss functions comparison:  
  - Binary Cross-Entropy loss  
  - Contrastive loss  
  - Triplet loss  
- Siamese network architectures  
  
---  
  
### Assignment 12: Knowledge Distillation  
**Focus**: Model compression and transfer learning  
  
**Key Components**:  
- Dataset: CIFAR-10  
- Teacher models: VGG16, ResNet50  
- Student model: Small CNN with 64 units  
- Distillation with temperature=3, alpha=0.5  
- Both single teacher and ensemble distillation  
  
---  
  
### Assignment 14: Classification Systems  
**Focus**: Comprehensive architecture comparison  
  
**Key Components**:  
- Dataset: Tiny ImageNet (20 classes, 8,000 train/2,000 test)  
- Three architectures:  
  - **FCFNN**: Fully-connected baseline  
  - **CNN**: Small convolutional network  
  - **ViT**: Vision Transformer with patch embedding  
- PyTorch implementation with comprehensive training utilities  
  
---  
  
## 🚀 Common Setup Instructions  
  
### Environment Setup  
```bash  
# Create virtual environment  [header-1](#header-1)
python3 -m venv dl_env  
source dl_env/bin/activate  # On Windows: dl_env\Scripts\activate  
  
# Install core dependencies  [header-2](#header-2)
pip install tensorflow>=2.10.0  
pip install numpy pandas matplotlib seaborn  
pip install opencv-python  
pip install jupyter notebook  
  
# Install specialized libraries  [header-3](#header-3)
pip install ultralytics  # For YOLO implementations  
pip install kaggle       # For dataset downloads
