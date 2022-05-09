# DeepFashion2-using-Detectron2
DeepFashion2 is a comprehensive fashion dataset. It contains 491K diverse images of 13 popular clothing categories from both commercial shopping stores and consumers. It totally has 801K clothing clothing items, where each item in an image is labeled with scale, occlusion, zoom-in, viewpoint, category, style, bounding box, dense landmarks and per-pixel mask.There are also 873K Commercial-Consumer clothes pairs. The dataset is split into a training set (391K images), a validation set (34k images), and a test set (67k images).

![Capture](https://user-images.githubusercontent.com/61115039/167393810-03e0a52c-0c22-4599-9648-f0cf043bea15.PNG)

### Examples of DeepFashion2.


![Capture](https://user-images.githubusercontent.com/61115039/167394152-a405d12a-4482-4b87-bc53-d66d0cbaf7ea.PNG)


# Download the Data
DeepFashion2 dataset is available in [DeepFashion2 dataset](https://drive.google.com/drive/folders/125F48fsMBz2EF0Cpqk6aaHet5VH399Ok?usp=sharing). You need fill in the [form](https://docs.google.com/forms/d/e/1FAIpQLSeIoGaFfCQILrtIZPykkr8q_h9qQ5BoTYbjvf95aXbid0v2Bw/viewform?usp=sf_link) to get password for unzipping files. Please refer to Data Description below for detailed information about dataset.


# Dataset Statistics
Tabel 1 shows the statistics of images and annotations in DeepFashion2. (For statistics of released images and annotations, please refer to [DeepFashion2 Challenge](https://sites.google.com/view/cvcreative/deepfashion2?authuser=0)).

<p align='center'>Table 1: Statistics of DeepFashion2.</p>

| | Train | Validation | Test | Overall |  
|---:|---:|---:|---:|---:|
|images|390,884|33,669|67,342|491,895|
|bboxes|636,624|54,910|109,198|800,732|
|landmarks|636,624|54,910|109,198|800,732|
|masks|636,624|54,910|109,198|800,732|
|pairs|685,584|query: 12,550<br/>gallery: 37183|query: 24,402<br/>gallery: 75,347|873,234|


## Pre-Requisites
For running the notebook on your local machine, following pre-requisites must be satisfied:
- NumPy
- Pandas
- Scikit-image
- IPython
- Matplotlib
- Tensorflow 2.X
- Keras
- Detectron2
- AZURE Cloud

## Solution :

### Object Detection using Detectron2 ==> COCO-Detection/faster_rcnn_R_101_FPN_3x.yaml
![image4_output](https://user-images.githubusercontent.com/61115039/167395949-348225cb-9167-450a-82b8-e5b86435b019.png)  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;   ![image5_output](https://user-images.githubusercontent.com/61115039/167395971-73f2002f-c81b-49f6-8049-40b68b1cac81.png)

![image1](https://user-images.githubusercontent.com/61115039/167395434-ac626b8c-f744-454e-a5c7-224c59e99d5b.PNG)

### Object Segmentation ==> COCO-InstanceSegmentation/mask_rcnn_X_101_32x8d_FPN_3x.yaml
![rahul_gandi](https://user-images.githubusercontent.com/61115039/167396492-1ba91156-5437-4c9d-8335-de9ebf095c0a.png)

![rahul_gandi_1](https://user-images.githubusercontent.com/61115039/167396513-91351882-f4bc-49b6-a00a-5458a13ef16a.png)
![image5_segment](https://user-images.githubusercontent.com/61115039/167396531-16136ea0-1524-4ac4-8938-eae2a226c350.PNG)
