# SA-C-GENDER-CLASSIFIER
# Algorithm
1.Install deepface

2.Import necessary packages

3.Read the image

4.Analyze the gender using deepface

## Program:
```python
/*
Program to implement Gender Classification
Developed by   : pradeep ps
RegisterNumber :  212220230034
*/
#install deepface
pip install deepface

#import packages
from deepface import DeepFace
import cv2
import matplotlib.pyplot as plt

#read the image
img=cv2.imread('GowriM.jpeg')
plt.imshow(img[:,:,::-1])
plt.show()

#Analyze gender
result=DeepFace.analyze(img,actions=['gender'])
result2=DeepFace.analyze(img,actions=['emotion'])

#print the gender
print("Gender : ",result['gender'])
```

## OUTPUT:

![Screenshot (161)](https://user-images.githubusercontent.com/102652887/172640449-eb01179d-8a60-4967-8fb0-fb338ba7d28d.png)


