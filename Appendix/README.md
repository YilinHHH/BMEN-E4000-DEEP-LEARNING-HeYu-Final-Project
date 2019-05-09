# Appendix
Deep learning with other databases

## Classification of Benign and Malignant Breast Cancer Mass using Convolutional Neural Network

DDSM (Digital Database for Screening Mammography) is an open-source dataset of digital mammograms of breast. The Cancer Imaging Archive (TCIA) has published an updated version of DDSM, Curated Breast Imaging Subset of DDSM (CBIS-DDSM). This version includes the ROIs of the origin images, which were segmented by the lesion segmentation algorithm.

![alt text](https://github.com/YilinHHH/BMEN-E4000-DEEP-LEARNING-HeYu-Final-Project/blob/master/Figures/ROI.png)
Figure 1. One sample in DDSM.

We also tried to utilize CNN to directly classify benign and malignant breast masses derived from the mammograms. 

This folder contains code which can:

 - Decode and convert the DICOM images to PNG images
 - Decode and convert the DICOM images to pseudocolor images
 - Filter ROI and mask images of which the file paths are mixed up in the csv file
 - Convert gray scale images to three-input-channel images which are compatible with pre-trained models
 - Completely pre-process samples in the dataset
 - Train models
 
No adjustment of architecture and parameters has been conducted yet.
