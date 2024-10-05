# Image_Superesolution_Using_DRRN

This code is implemented from the CVPR 2017 paper Image Super-Resolution via Deep Recursive Residual Network https://ieeexplore.ieee.org/document/8099781, this network applies residual connection to a 54 layer recursive neural network. There are total 9 recursive blocks used and in each recursive block there are three residual blocks you can refer to this image for more clearity.

![image](https://github.com/user-attachments/assets/f3e660d2-b3dd-4cfe-98e0-31f4f271b1ba) 

This architecture helps learning complex features and also keeps initial input alive which removes problem of vanishing gradient. Also gradient clipping is added to control exploding gradient. this model is trained on a 640 images kaggle dataset by extrating patches of size 31*31. making total of 103455 trainable patches with stride = 21. now the model was kept training for 50 epochs with a early stopping criteria and model early stopped on 27 epochs.

### Dataset link

https://www.kaggle.com/datasets/adityachandrasekhar/image-super-resolution

### Results

Model achieved validation loss of just: 0.0014 and val_accuracy of 0.8542.

![image](https://github.com/user-attachments/assets/dfc663ed-6edb-4950-89e8-7727f8f071de)

Here are some superesolved images

![image](https://github.com/user-attachments/assets/b514eaab-3617-42fc-9e78-11cd21a778e2)

![image](https://github.com/user-attachments/assets/3f0a48b8-2937-48a3-8a3c-350fd96a0557)

![image](https://github.com/user-attachments/assets/82ca0e1b-6d0f-400e-b626-7a0fcddfa36f)


### How to implement in you local pc







