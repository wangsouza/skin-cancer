# skin cancer

**Install**
1. Install Keras Mask-RCNN (https://drive.google.com/file/d/1Ug6697XbnRpEPjZyN5uLEEHyR27JyeVo/view?usp=sharing)
2. Create sym-link: (e.g. ln -s ~/Mask_RCNN/mrcnn mrcnn)
3. Download the pre-trained network and place it in the main directory: https://github.com/matterport/Mask_RCNN/releases/download/v2.0/mask_rcnn_coco.h5
4. Create isic2018 folder and place the following files:
   - Train data (https://isic-challenge-data.s3.amazonaws.com/2018/ISIC2018_Task1-2_Training_Input.zip)
   - Traing Ground Truth (https://isic-challenge-data.s3.amazonaws.com/2018/ISIC2018_Task1_Training_GroundTruth.zip)

## Project structure
```
   |--- mask_rcnn
   | |--- isic2018/
   | | |--- ISIC2018_Task1-2_Training_Input
   | | |--- ISIC2018_Task1_Training_GroundTruth
   | |--- lesions.py
   | |--- mask_rcnn_coco.h5
   | |--- mrcnn/
```


## Investigate
```python lesions.py --mode investigate```

## Train
```python lesions.py --mode train```

## Predict
```python lesions.py --mode predict --image\
 isic2018/ISIC2018_Task1-2_Training_Input/ISIC_0000000.jpg```

OUTPUT 1:\
![Alt text](readme/ISIC_0000000.png?raw=true "Title")
OUTPUT 2:\
![Alt text](readme/ISIC_0000000.png?raw=true "Title")
OUTPUT 3:\
![Alt text](readme/ISIC_0000000.png?raw=true "Title")
