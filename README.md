#### Related Work: [FER2013](https://github.com/SJSUMS/Facial-Expression-Recognition)

# Facial Expression Recognition Classification <br>
by [mavisw](https://github.com/mavisw)
<p><img src='https://production-media.paperswithcode.com/datasets/FER2013-0000001434-01251bb8_415HDzL.jpg'></p>

## Dataset [CSV](https://www.kaggle.com/deadskull7/fer2013) | [PNG](https://www.kaggle.com/astraszab/facial-expression-dataset-image-folders-fer2013)
#### Data Info:
30,000 48x48 pixel grayscale RGB images. 
#### Labels:
0 - Angry
1 - Disgust
2 - Fear
3 - Happy
4 - Sad
5 - Surprise
6 - Neutral

## Methodology
- Trained with Keras and Tensorflow on Colab with GPU.
- Split 80/20 
- Trained for 50 epochs, batched.
- Ensembling (Soft Vote)

## Tasks
- [x] Data Collection (cleaned)
- [x] Wrangling/Transform (normalization, channel convert, image augmentation)
- [x] Data Preparation (80/20 split for training/testing)
- [x] Data Loader (Tensorflow ds)
- [x] Build model (keras)
- [x] Training and testing (on Colab w/GPU)
- [x] Evaluation (accuracy, F1, Recall, Precision)

## Models 
- [x] Simple CNN (3 Conv + 1 FC layers)
- [x] Transfer Learning
- [x] Ensembling Metthod

## Results [Slide](https://docs.google.com/presentation/d/1h9cVVBe_7FTmr2uxcdZslfeMWPc9Zyv93_j4pLkAhnM/present?slide=id.p)
|    Model   |   Accuracy on Test Set | 
|:-----------| :--------- |
| Simple CNN (5 layers) |   54%  |
| MobileNetV2  | 64% | 
| Inception | 61% |
| Xception | 55% |
| Top-3 |67%|

## Code
- [x] [EDA (Data Preparation)](https://github.com/mavis-wang/DSNotes/blob/main/sample/FER_dataPrep.ipynb)
- [x] [Model (Transfer Learning)](https://github.com/mavis-wang/DSNotes/blob/main/sample/FER_Ensemble_DL.ipynb)
