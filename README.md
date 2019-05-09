# BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project

## Classification of Invasive Ductal Carcinoma and Non-Invasive Ductal Carcinoma in Histopathology Section of Breast Cancer Using Convolutional Neural Network

Haoyang Yu (hy2581) & Yilin He (yh3089)
*Fu Foundation School of Engineering and Applied Science*
*Columbia University in the City of New York*

***Abstract***—Breast cancer is the most common cause of death from cancer among female, only second to lung cancer. Invasive ductal carcinoma is the most common form of breast cancer. Pathological diagnosis is one of the most important diagnostic methods for breast nodules, and pathological classification has been widely accepted as the most instructive classification cri- teria. However, human error, intra-pathologist variability, and time-consuming diagnostic process place obstacles in the improve- ment of accuracy and efficiency. A novel deep learning approach is in demand to address the currently existing challenge with great performance. This report proposes a convolution neural network model with pre-trained weights to classify the invasive tumor tissues and non-invasive tissues in images hematoxylin and eosin stained sections. The whole project comprised of database acquisition, image pre-processing, model establishment and training. The evaluation criteria include accuracy, F-score, sensitivity, specificity, precision rate, and recall value. The binary classification results of invasive tumor tissues and non-invasive tumor/healthy tissues verified the effectiveness and efficiency of the proposed architecture. The performance of this end-to-end CNN model demonstrates its great capacity of distinguishing subtypes of breast cancer and its application prospect in clinical practice.

**Keywords**—Breast cancer, Deep learning, Convolution neural network, Hematoxylin and eosin

### Dataset download
The original database was collected by researchers at Case Western Reserve University in Cleveland, Ohio. It contains 162 whole mount slide images of breast cancer specimens scanned at 40× resolution.

[Kaggle Breast Histopathology Images Dataset](https://www.kaggle.com/paultimothymooney/breast-histopathology-images):

● 277,524 patches derived from 162 whole mount slide images

&emsp;○ 198,738 IDC(-) and 78,786 IDC(+) 

● Ground truth: pathologist diagnosis

&emsp;○ IDC tissues

&emsp;○ Healthy/Non-invasive tumor tissues




<div align=center><img src="https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Figures/Flow%20Diagram.png" width = "250" div align=center />

Figure 1. The flow diagram of the proposed convolution neural network mdoel.

![alt text](https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Figures/Xception.png)

Figure 2. The architecture of Xception model.

![alt text](https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Figures/Result.png)

Figure 3. The classification results of IDC and non-IDC on histopathologic images at 40 magnification.

![alt text](https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Figures/ROC.png)

Figure 4. ROC curve.


