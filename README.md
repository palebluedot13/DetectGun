# Gun threat detection
Detection of gun threats in image with classification of similar events which are non threatening.

## Overview
Gun violence has been a major cause for concern for a long time now. Hence creating a solution that could even help the officers by a little would amount to a lot when considering issue at hand. The purpose of this project is not only to detect guns in the image but to detect guns that are armed and are being used as a threat. The first phase of this project would only involve detecting the threats by creating an active shooter scenario i.e holding guns in threatning ways instead of it being safely stored in a gun holster or an officers vest or in classifying images we would also consider something that looks very similar to holding a gun i.e a smart phone.

## Dataset
I have collected the dataset from kaggle and by scraping it from google images using SerpApi. This dataset includes a combination of images of guns held in different angles and recorded from different video equipmenets which show the gun being held in a strongly threatning position i.e in the armed position. This data also includes some other types of images that must not be raised as threats in the image like holding a smart phone in a similar fashion or a gun in an officers holster as we do not want to raise any false alarms.

## Results

The possible threatning guns are marked by a bounding box and the non threatning ones are marked with a bounding box as well.

### Active Threat
![](images/demo_1.jpg)

### Gun in Holster
![](images/demo_2.jpg)

### Smart phone in hand
![](images/demo_3.jpg)

### Confusion Matrix

![](image/demo_4.jpg)



## Future  Goals

As detecting the threat purely based on the image is not a very good approach but what would be an even better approach would be tracking the active threat live on the webcam that would require some object tracking and video processing and classification of the active threat. As finding out the active shooter is of utmost importance in such scenarios. As the dataset doesn't have enough data to classify accurately the way the person is holding the gun there are a few false -ve's that come up. But this can easily be solved by traing the model to learn ceratain physical hand gestures and live tracking the positions which come up specifically in an active shooter scenario. 
