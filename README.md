# PadChest-lung-metastasis
In this proyect we will try to create a model that can recognize which images have lung metastasis. 
The model will be train with the public repository of PadChest, it contains 160.000 images.  Of the total images, 50.000 of them are classified as 'normal' and 358 as 'lung metastasis' those are the ones that we will use

The images can be downloaded from https://bimcv.cipf.es/bimcv-projects/padchest/ anyone can use it but their conditions must be accepted. 

To facilitate the downloading and organization of the images use the 'Download and augmentation' notebook. In this notebook we implement techniques to augment the amount of images of 'lung metastasis' so that the model can adjust the weights better. From 358 images to

Once the conditions have been accepted and all the compressed files have been downloaded, we will save all the images in the 'extracted_files' folder and organize the images by classes with the names 'normal' and 'lung_metastasis' with the corresponding images.
