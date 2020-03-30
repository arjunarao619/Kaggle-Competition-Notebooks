# Kaggle Competition Notebooks
### A collection of iPython Notebooks written to attempt various Kaggle deep learning competitions
Note: This is the joint README for all competition files. 
My Kaggle profile can be found [here](https://www.kaggle.com/arjunrao2000)
All notebooks have been written as an iPython Notebook. Models run on Nvida Tesla P100 GPUs provided by Kaggle. 
All information on competitions below obtained from respective Kaggle competition pages.
## 1. [APTOS 2019 Blindness Detection Challenge](https://www.kaggle.com/c/aptos2019-blindness-detection)
### Dataset:
Provided with a large set of retina images taken using fundus photography under a variety of imaging conditions.
A clinician has rated each image for the severity of diabetic retinopathy on a scale of 0 to 4:
```
0 - No DR

1 - Mild

2 - Moderate

3 - Severe

4 - Proliferative DR
```
Images may contain artifacts, be out of focus, underexposed, or overexposed. The images were gathered from multiple clinics using a variety of cameras over an extended period of time, which will introduce further variation.

#### Sample test data images:
</br>
<a href='https://postimg.cc/xX1f1ZkS' target='_blank'><img src='https://i.postimg.cc/6pdyYJtT/Screen-Shot-2020-03-30-at-6-34-00-PM.png' border='0' alt='Screen-Shot-2020-03-30-at-6-34-00-PM'/></a> 

### Model Used:
- Keras ImageDataGenerator used with Primitive CNN
- Trained on 80 epochs, categorical crossentropy loss with an ADAM optimizer
- Final validation accuracy 0.63
</br>
<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/d1gx15nC/download-2.png' border='0' alt='download-2'/></a>

## 2. [Aerial Cactus Identification Challenge](https://www.kaggle.com/c/aerial-cactus-identification)
### Dataset:
Dataset contained a large number of 32 x 32 thumbnail images containing aerial photos of a columnar cactus (Neobuxbaumia tetetzo). Kaggle has resized the images from the original dataset to make them uniform in size. The file name of an image corresponds to its id.

classifier must be capable of predicting whether an images contains a cactus.

#### Sample dataset images

<a align = "center" target='_blank'><img src='https://i.postimg.cc/L5cwC2Wh/cactii.png' border='0' alt='cactii'/></a><br /><a href='https://postimages.org/' ></a><br />

### Model Used

Keras EfficientNet - Link to paper: https://arxiv.org/abs/1905.11946
</br></br></br>
<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/FH3LWLGN/Screen-Shot-2020-03-30-at-7-04-04-PM.png' border='0' alt='Screen-Shot-2020-03-30-at-7-04-04-PM'/></a>
- Keras ImageDataGenerator used to augment images
- Trained on 50 epochs, Binary crossentropy loss with an Adam optimizer
<a  target='_blank'><img src='https://i.postimg.cc/bvgqrCCd/download-3.png' border='0' alt='download-3'/></a><br /><a href='https://keyboardtester.co/keyboard-tester'></a><br />
- Final competition score: 0.9996 (553rd place)

## 3. [Humpback whale identification challenge](https://www.kaggle.com/c/humpback-whale-identification)
### Dataset:
This training data contains thousands of images of humpback whale flukes. Individual whales have been identified by researchers and given an Id. The challenge is to predict the whale Id of images in the test set. What makes this such a challenge is that there are only a few examples for each of 3,000+ whale Ids.

#### Sample dataset images:
<a target='_blank'><img src='https://i.postimg.cc/Gp94ygt7/download-4.png' border='0' alt='download-4'/></a><br /><a></a><br />

### Model Used:
- Primitive CNN written in Keras with ImageDataGenerator for augmentation.
- Categorical crossentropy with Adam optimizer
<a target='_blank'><img src='https://i.postimg.cc/NMYYqbSG/download-5.png' border='0' width = "300"/></a>

## 3. [Kinship Detection Challenge](https://www.kaggle.com/c/recognizing-faces-in-the-wild)
### Dataset:
In this competition, you will predict if two people share a kinship relationship or not based on their facial images. The data is provided by Families In the Wild (FIW), the largest and most comprehensive image database for automatic kinship recognition.

FIW's dataset is obtained from publicly available images from celebrities. For more information about their labeling process, please visit their database page.
 #### Sample dataset images
 <a  target='_blank'><img src='https://i.postimg.cc/90GkBjJc/Screen-Shot-2020-03-30-at-7-23-32-PM.png' border='0' height = "400"/></a>
 ### Model Used:
 vggface_resnet50 - relevant model link: https://www.robots.ox.ac.uk/~vgg/software/vgg_face/
 - Trained on 130 epochs with training accuracy of 0.73
 
 ## 4. [Seedling classification challenge](https://www.kaggle.com/c/plant-seedlings-classification)
 
Provided with a training set and a test set of images of plant seedlings at various stages of grown. Each image has a filename that is its unique id. The dataset comprises 12 plant species. The goal of the competition is to create a classifier capable of determining a plant's species from a photo. The list of species is as follows:
```
Black-grass
Charlock
Cleavers
Common Chickweed
Common wheat
Fat Hen
Loose Silky-bent
Maize
Scentless Mayweed
Shepherds Purse
Small-flowered Cranesbill
Sugar beet
```
#### Sample train csv file
<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/zfnS0mMf/Screen-Shot-2020-03-30-at-7-38-12-PM.png' border='0' width = "400" /></a>
</br>
#### Dataset images:
</br>
<a  target='_blank'><img src='https://i.postimg.cc/9FS6jVnF/download-6.png' border='0' width = "400" align = "left"/></a>
</br></br></br></br></br></br></br></br></br></br></br></br></br></br></br></br>

### Model used:
- Primitive CNN - Conv, MaxPooling, and batch normalisation along with dropout and L2 norm regularization
- Trained on resized 256x256 images for 25 epochs


     


