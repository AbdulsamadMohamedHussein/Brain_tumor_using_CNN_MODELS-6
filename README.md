#  Brain Tumor Classification Using Deep Learning on MRI Images

##  Project Overview
Brain tumor detection and classification is a critical task in medical diagnosis, as early and accurate identification can significantly improve patient outcomes. Manual analysis of MRI scans is time-consuming and highly dependent on expert knowledge, which motivates the use of automated deep learning systems.

This project presents a **deep learning–based framework for multi-class brain tumor classification** using MRI images. Multiple convolutional neural network (CNN) architectures and transfer learning models were implemented, trained, and compared to determine the most effective approach.

The MRI images are classified into **four categories**:
- Glioma  
- Meningioma  
- Pituitary tumor  
- No tumor  

---

## Objectives
- Build an automated brain tumor classification system using MRI images  
- Compare multiple deep learning models under the same experimental setup  
- Evaluate performance using standard classification metrics  
- Identify the best-performing architecture for reliable diagnosis  

---

## 
Dataset Description
- **Total images:** 7,012  
- **Training images:** 5,701  
- **Testing images:** 1,311  
- **Number of classes:** 4  

The dataset consists of T1-weighted contrast-enhanced brain MRI images. The data was split carefully to ensure the test set remained unseen during training.

---

##  Data Preprocessing and Augmentation
To improve model performance and generalization:
- Images were resized to a uniform input size  
- Pixel values were normalized  
- Data augmentation techniques such as rotation, flipping, and zooming were applied  

---

## Deep Learning Models Used
The following models were implemented and evaluated:

- **DenseNet121** – Dense connectivity for feature reuse  
- **ResNet50** – Residual connections for deep learning stability  
- **ResNet101** – Deeper residual network  
- **Xception** – Depthwise separable convolutions  
- **InceptionV3** – Multi-scale feature extraction  
- **Custom CNN (ConvNet)** – Baseline model built from scratch  

All pre-trained models were initialized with ImageNet weights.

---

##  Training Strategy
- **Training approach:** Supervised learning  
- **Optimizer:** Adam  
- **Loss function:** Categorical Cross-Entropy  
- **Epochs:** 15  
- **Batch size:** Fixed for all models  

The same training configuration was applied across all models to ensure a fair comparison.

---

## 📊 Evaluation Metrics
Model performance was evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion matrices  

Confusion matrices were used to analyze class-wise prediction behavior.

---

## Results Summary
- **DenseNet121 achieved the highest accuracy (>99%)**  
- **ResNet50 showed comparable performance**  
- **Xception and Custom CNN achieved good results**  
- **ResNet101 and InceptionV3 showed comparatively lower accuracy**  

Overall, transfer learning models significantly outperformed the custom CNN.

---

## Confusion Matrix Analysis
- The **no-tumor class** was classified with very high accuracy  
- **Glioma and meningioma** were the most challenging classes  
- Top-performing models showed strong diagonal dominance in confusion matrices  

---

## Future Work
Possible extensions include:
- Using larger and multi-institutional datasets  
- Tumor segmentation in addition to classification  
- 3D MRI volume analysis  
- CNN–Transformer hybrid architectures  
- Explainable AI (XAI) for clinical trust  
- Real-world clinical deployment  

---

## 📚 References
- Cheng et al., *PLoS ONE*, 2015  
- Litjens et al., *Medical Image Analysis*, 2017  
- He et al., *CVPR*, 2016  
- Huang et al., *CVPR*, 2017  
- Dosovitskiy et al., *arXiv*, 2021  

---

## ✅ Conclusion
This project demonstrates the effectiveness of deep learning and transfer learning models for automated brain tumor classification using MRI images. The results highlight the potential of such systems as reliable computer-aided diagnostic tools in healthcare.
