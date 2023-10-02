# ISL Recognition CNN OpenCV

   In this project, I wanted to raise awareness for the hearing impaired. Do not forget every learning starts with the alphabet. You can make predictions about the ***Indian Sign Language Alphabet*** to the model by camera. So let's dig out the project some more.

<p align="center">
<img src="https://user-images.githubusercontent.com/81585804/168675071-f64e8df6-d62c-42af-a44b-7b554d3212cf.png" width="250" height="250">
</p>


I cover this project on the four step.
* About Dataset
* Deep Learning - CNN
* OpenCV
* How to run

## 1. Dataset
I use standred consiting of 31200 images of all alphabets form A-Z each 1200 images.

## 2. Deep Learning - CNN
First things first we should some pre-process before training. [One hot encoding](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html) and [RGB normalization](https://akash0x53.github.io/blog/2013/04/29/RGB-Normalization/). These links are usefull if you don't know about them. Tradionally CNN is for mostly used for Image Processing and i kept this tradition. The following two figure are Confusion Matrix of respectively test and evaluation.  Before, i mention about the difference about two dataset.  That is the consequence of difference. Test images are so similar with the training set so accuracy and values of Confusion matrix is so high.  On the other hand evaluation set is so much diffrent than training that is the reasen why evaluation scores too low.


|  |  |   
| --- | --- |
| <img src="https://user-images.githubusercontent.com/81585804/168676983-3094ac59-9b7b-4f6e-97f2-3908624eae0c.png" width="500" height="300">| <img src="https://user-images.githubusercontent.com/81585804/168677085-43356f35-aed3-4e2d-b010-cec958e7a4d3.png" width="500" height="300">| %99.609 | %40.46 |


**Finally here some different training result:**

| | OPTIMIZER | EPOCH | TEST ACCURACY |
| --- | --- | --- | --- | --- |
| MODEL-1 | rmsprop | 5 | %98.57 |



## 3. How to run 


1. Fork this repository.
 ```console
$ git clone https://github.com/MelihGulum/ASL-Recognition-CNN-OpenCV.git
```

2. Load the dependencies of the project

**NOTE:** This dependencies not including the Deep Learning part. Colab meet all dependencies (such as tensorflow).

 ```console
pip install -r requirements.txt
```

3. Now you can run ASL_Recognition.py. But if you want you can run .ipynb and you can build your own model. It is up to you. 
