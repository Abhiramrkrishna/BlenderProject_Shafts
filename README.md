# Bin Picking of Shafts 

I have been working on a project focused on image processing and machine learning, involving the development of a training model to refine the detection of objects from a bin. My works includes modelled different shafts in Blender, built textures and various illuminations setups, used Python and Blender libraries for scripting, worked with compositing nodes for image analysis and semantic segmentations, and contributed to the implementation and training of YOLO networks using a blend of synthetic and real data, focusing on refining object localization precision through iterative model enhancements. 

## This is the Blender Scripting for the Gneration of Synthetic Image

1. We are generating RGB image from the viewer viewport with diamension 256 x 256. We are also generating iteratively the synthetic data (image) with same resolution and size along with the corresponding anotation file.
2.  The anotation file includes the following information:
   1. Classes (0 since we have only one class object)
   2. The x and y coordinate
   3. Gamma and Phi angles (rotation around 2 axes is being considered)
   4. Two Confidence scores, first one based on the larger vertices and the second one on the small vertices.


I am including a sample synthetic image, a training image and a sample annotation file.

I also did seantic segmentation of images based on confidence scores. I will briefly explain the work I did here.
Based on the confidence threshold we set, we can modify the Object ID Index of the shafts with higgest confidence scores. We can use composite nodes in compositing in Blender for the purpose. ID Masking node can be used to set the mask and few image post-processing nodes are also utilized.  

_____________________________________________________________________________________________________

Content of folders:
Synthetic Images 
Training Images
Real Images
Anotation file
Segmented images

_____________________________________________________________________________________________________


This is an ongoing project and I cannot share laetest codes and updates. I am sharing the part of project that I did.
