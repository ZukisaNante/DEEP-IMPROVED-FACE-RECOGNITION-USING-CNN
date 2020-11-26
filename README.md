# DEEP-IMPROVED-FACE-RECOGNITION-USING-CNN
Trying to Improving the accuracy of CNN
---
### INTRODUCTION
> The aim here is to try and improve the accuracy of CNN in face recognition (FR).
> Some of the code used here is a credit to all CNN programmers who post their findings and tutorials and researchers who share the new findings.
---
### CNN Architecture
---
![CNN ARCHITECTURE](https://github.com/ZukisaNante/DEEP-IMPROVED-FACE-RECOGNITION-USING-CNN/blob/main/images/15_09.png)
---
### Modifications in the code
> - CNN architecture was changed as you can see the model.summary() from the code.
> - The 7x7, 5x5 and 3x3 convolution filters pixels were changed to 7x7 for all layers.
> - The following image shows this model. the model can go dipper but will demand a lot of training time in CPU. Still on modification to get more accuracy.
---
![CNN ARCHITECTURE](https://github.com/ZukisaNante/DEEP-IMPROVED-FACE-RECOGNITION-USING-CNN/blob/main/images/15_09.png)

Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d (Conv2D)              (None, 112, 92, 64)       3200      
_________________________________________________________________
conv2d_1 (Conv2D)            (None, 112, 92, 64)       200768    
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 56, 46, 64)        0         
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 56, 46, 128)       401536    
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 56, 46, 128)       802944    
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 28, 23, 128)       0         
_________________________________________________________________
conv2d_4 (Conv2D)            (None, 28, 23, 256)       1605888   
_________________________________________________________________
conv2d_5 (Conv2D)            (None, 28, 23, 256)       3211520   
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 14, 11, 256)       0         
_________________________________________________________________
flatten (Flatten)            (None, 39424)             0         
_________________________________________________________________
dense (Dense)                (None, 2024)              79796200  
_________________________________________________________________
dropout (Dropout)            (None, 2024)              0         
_________________________________________________________________
dense_1 (Dense)              (None, 1024)              2073600   
_________________________________________________________________
dropout_1 (Dropout)          (None, 1024)              0         
_________________________________________________________________
dense_2 (Dense)              (None, 512)               524800    
_________________________________________________________________
dropout_2 (Dropout)          (None, 512)               0         
_________________________________________________________________
dense_3 (Dense)              (None, 20)                10260     
=================================================================
Total params: 88,630,716
Trainable params: 88,630,716
Non-trainable params: 0
_________________________________________________________________
