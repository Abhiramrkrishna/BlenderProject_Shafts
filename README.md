# Bin Picking of Shafts 

I have been working on a project focused on image processing and machine learning, involving the development of a training model to refine the detection of objects from a bin. My work includes modeling different shafts in Blender, building textures and various illuminations setups, using Python and Blender libraries for scripting, working with compositing nodes for image analysis and semantic segmentations, and contributing to the implementation and training of YOLO networks using a blend of synthetic and real data, focusing on refining object localization precision through iterative model enhancements. 

## This is the Blender Scripting for the Generation of Synthetic Image

1. We are generating RGB images from the viewer viewport with dimensions 256 x 256. We are also generating iteratively the synthetic data (image) with the same resolution and size along with the corresponding annotation file.
2.  The annotation file includes the following information:
   * 1. Classes (0 since we have only one class object)
   * 2. The x and y coordinate
   * 3. Gamma and Phi angles (rotation around 2 axes is being considered)
   * 4. Two Confidence scores, the first one based on the larger vertices and the second one on the small vertices.


I am including a sample synthetic image, a training image, and a sample annotation file.

I also did semantic segmentation of images based on confidence scores. I will briefly explain the work I did here.
Based on the confidence threshold we set, we can modify the Object ID Index of the shafts with the highest confidence scores. We can use composite nodes in compositing in Blender for this purpose. ID Masking node can be used to set the mask and a few image post-processing nodes are also utilized.  

_____________________________________________________________________________________________________

Content of folders:
- Synthetic Images 
- Training Images
- Real Images
- Annotation file
- Segmented images

_____________________________________________________________________________________________________


This is an ongoing project and I cannot share the latest codes and updates. I am sharing the part of the project that I did.
