# BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project

## Classification of Invasive Ductal Carcinoma and Non-Invasive Ductal Carcinoma in Histopathology Section of Breast Cancer Using Convolutional Neural Network

Haoyang Yu (hy2581) & Yilin He (yh3089)

*Fu Foundation School of Engineering and Applied Science*

*Columbia University in the City of New York*

***Abstract***—*Breast cancer is the most common cause of death from cancer among female, only second to lung cancer. Invasive ductal carcinoma is the most common form of breast cancer. Pathological diagnosis is one of the most important diagnostic methods for breast nodules, and pathological classification has been widely accepted as the most instructive classification cri- teria. However, human error, intra-pathologist variability, and time-consuming diagnostic process place obstacles in the improve- ment of accuracy and efficiency. A novel deep learning approach is in demand to address the currently existing challenge with great performance. This report proposes a convolution neural network model with pre-trained weights to classify the invasive tumor tissues and non-invasive tissues in images hematoxylin and eosin stained sections. The whole project comprised of database acquisition, image pre-processing, model establishment and training. The evaluation criteria include accuracy, F-score, sensitivity, specificity, precision rate, and recall value. The binary classification results of invasive tumor tissues and non-invasive tumor/healthy tissues verified the effectiveness and efficiency of the proposed architecture. The performance of this end-to-end CNN model demonstrates its great capacity of distinguishing subtypes of breast cancer and its application prospect in clinical practice.*

***Keywords***—*Breast cancer, Deep learning, Convolution neural network, Hematoxylin and eosin*

### Dataset download
The original database was collected by researchers at Case Western Reserve University in Cleveland, Ohio. It contains 162 whole mount slide images of breast cancer specimens scanned at 40× resolution.

[Kaggle Breast Histopathology Images Dataset](https://www.kaggle.com/paultimothymooney/breast-histopathology-images):

● 277,524 patches derived from 162 whole mount slide images

&emsp;○ 198,738 IDC(-) and 78,786 IDC(+) 

● Ground truth: pathologist diagnosis

&emsp;○ IDC tissues

&emsp;○ Healthy/Non-invasive tumor tissues

### Image Pre-processing
The size of original images is 50 × 50. In the pre-processing step, histopathological images were decoded and resized to 75 × 75 × 3 to be compatible with existing pre-trained models. Then images with their corresponding labels were made into a dataset and fed into the convolution neural network.

### CNN Architecture
This model consisted of one pre-trained Xception model, one GlobalAveragePooling layer, one dropout layer, and three fully-connected layers. 

<div align=center><img src="https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Figures/Flow%20Diagram.png" width = "250" div align=center />

Figure 1. The flow diagram of the proposed convolution neural network mdoel.

<div align=left>
  
### Performance
In supervised learning, the confusion matrix is an enriched summary of the classification result. MOst statistic results can be illustrated from it.

<div align=center><img src="https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Figures/Result.png" width = "400" div align=center />


Figure 2. The classification results of IDC and non-IDC on histopathologic images at 40 magnification.

<div align=left>Another model evaluation criterion is the receiver operating characteristic curve (ROC). The ROC curve plots parametri- cally TPR versus FPR with different steps. The area under the curve (AUC) represents the probability that a classifier will generate a positive prediction for a randomly chosen positive input. In this case, the area under the curve (AUC) is 0.90.

<div align=center>
  
  ![alt text](https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Figures/ROC.png)

Figure 3. ROC curve.

<div align=left>
  
  ### File Description
 - [Pre-processing](https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Pre-pocessing.ipynb)
 
 - [Model Setup & Training & Prediction & Evaluation](https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Training.ipynb)
 
 - [Appendix](https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/tree/master/Appendix) (See detailed information in README file in the Appendix folder.)

