# Self_and_semi_supervised_MNIST
Solution to handwritten digit recognition problem with only 100 labeled data, using self-supervised approach based on image rotations (0°, 90°, 180° and 270°).

# Architecture of the CNN :
We chose to build the architecture of our CNN inspired by the VGG-16 model, while adding Batch Normalization layers to avoid overfitting.

# Self-supervised approach : 
Our approach consists of using the unlabeled data we have to train our model on a pretext task - in this case, image rotation - to help capture knowledge about the images through representation learning. Then with the few labeled data we have (100 labeled images), finetune the pretrained model on our downstream task : image classification/digit recognition, through transfer learning.

# Results : 
We have reached an accuracy of 81% on a 5000 images test set. 
