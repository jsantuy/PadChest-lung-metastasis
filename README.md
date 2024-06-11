# PadChest-lung-metastasis
In this proyect we will try different models to try to recognize which images have lung metastasis. 
The model will be train with the public repository of PadChest, it contains 160.000 images.  Of the total images, 50.000 of them are classified as 'normal' and 358 as 'lung metastasis' those are the ones that we will use for the model.

The images can be downloaded from https://bimcv.cipf.es/bimcv-projects/padchest/ anyone can use it but their conditions must be accepted. 

To facilitate the downloading and organization of the images use the 'Download' notebook. In this notebook the code helps us to extract the images and separate them into 'normal' and  'lung metastasis.

In the notebook 'Exploratory analysis' you can get an idea of the dataset we are working with. If you want to explore it, you have to download the csv called "PADCHEST_chest_x_ray_images_labels_160K_01.02.19.csv" from the previous link.

In the next notebook 'Organization and Data Augmentation' the images are seprated into train/test and we also implement techniques to increase the amount of images of 'lung metastasis' of the train set so that the model can adjust the weights better with more inputs.  The augmentation flips and rotates the images in different angles, the final amount of images with lung metastasis to train the model is 1716.

Once that we have the images separated we can train the models. There first model is the basic one and has been taken from the article of Thamilarasi (1). Because the model was overfitting, we have created another 4 models that derivate from the basic which they include layers that try to solve the problem. This models include layers of Dropout, BatchNormalization and L2.
We have also tried to train the model with the arquitecture Densenet121 loading the weights of the model and also without loading the weights.

All the models have been tried with 512x512 images and 295x295 and the result has been the same, none of the models have showed any improvement and could not solve the overfitting problem






1- Thamilarasi V, Roselin R. Automatic Classification and Accuracy by Deep Learning Using CNN Methods in Lung Chest X-Ray Images. IOP Conf Ser: Mater Sci Eng. febrero de 2021;1055(1):012099.
