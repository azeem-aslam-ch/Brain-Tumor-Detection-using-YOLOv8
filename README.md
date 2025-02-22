# Brain Tumor Detection using YOLOv8
In this project we have used different sizes of the YOLOv8 model to detect ansd classsify brain tumor in the MRI images<br>
---
Implementing a brain tumor detection system using YOLOv8. Curate a diverse dataset, annotate images, and train models for accurate detection. Emphasizing ethical healthcare data usage, this project seeks robust precision and recall in identifying brain tumors through the YOLOv8 along with different sizes and optimizers. <br>

---
## Dataset 
[Link To Dataset](https://www.kaggle.com/datasets/ammarahmed310/labeled-mri-brain-tumor-dataset)<br>
Dataset was obtained from Kaggle. It contains 2176 samples of various clinical circumstances. There 455 samples of "glioma", 551 samples of "meningiomas", 620 samples of "pituitary" and 550 samples of "No Tumor". 
## Training 

Training was done on nano and medium size of YOLOv8 model. The training process was optimised with various choice of Optimizers like Adam, Adamax and RMSprop. 
Following are the training parameters and results. 
| **Sr No** | **Size** | **Epochs** | **Batch Size** | **Learning Rate** | **Optimizer** | **Momentum** | **Dropout** | **Precision** | **Recall** |
|:---------:|:--------:|:----------:|:--------------:|:-----------------:|:-------------:|:------------:|:-----------:|:-------------:|:----------:|
|     1     |   Nano   |     25     |       109      |        0.01       |      Auto     |       -      |      -      |      90.1     |    79.1    |
|     2     |   Nano   |     30     |       32       |       0.001       |     Adamax    |     0.85     |     0.5     |      84.5     |    80.6    |
|     3     |  Medium  |     30     |       32       |       0.001       |    RMSprop    |     0.90     |     0.2     |      54.7     |    48.5    |
|     4     |  Medium  |     30     |       32       |       0.001       |      Adam     |     0.90     |     0.3     |      84.4     |    84.7    |
|     5     |  Medium  |     30     |       32       |       0.001       |     Adamax    |     0.89     |     0.4     |      89.9     |    86.5    |




If you have any query, feedback or suggestion feel free to drop a mail at azeem.aslam91@yahoo.com :) 
