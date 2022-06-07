# Object-Detection-Image-Segmentation-
* Object Detection Models: YOLO and SSD 
* Image Segmentation Models: FCN, SegNet, UNet, and DeepLabv3

Object Detection aims at providing a bounding box around the desired object class, while image segmentation aims at providing a pixel mask over the entire object class. See below:

![image](https://user-images.githubusercontent.com/63126473/172285545-5240659d-c6ef-4801-97e1-ed3478b81345.png)


A subset of the COCO dataset (https://cocodataset.org/) is used which contains 20 out of the original 91 classes, with around 500 images for each class. This still provides a diverse dataset of 10,732 images in total which significantly reduces resources needed/training time (7771 of these images are used for training and 2961 for validation). 

For experimentation on object detection models, model ensembling, transfer learning, and test-time augmentations (data augmentation and batch normalization) are performed. Experimentation for the image segmentation models was very similar; model ensembling, transfer learning, and varied hyperparamters (learning rate, number of epochs, different loss functions). 

For analysis, we compared various metrics of the original pre-trained models to the experimented/exteneded models. For the object detection models, average inference time and mean average precision (intersection over union) was compared. For the image segmentation models, overall pixel accuracy and per-class pixel accuracy was compared. 
