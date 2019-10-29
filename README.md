# Semantizer
This module takes an input raster map and generates a semantically segmented image of the raster map with a 
number of channels per pixel. Each channel represents the probability of a pixel belonging to a specific 
class of geographic features. The number of channels represents the number of geographic feature types (plus 
one type of “others”). For each pixel, the sum of the probability from every channel is 100%. This is a 
typical semantic segmentation problem that might be solved using deep learning semantic segmentation models. 
The challenges include how to generate a large amount of training data for maps and historical documents 
that could suffer from the poor quality in the original map or scanning process. Another challenge is cross-
modality of historical maps, i.e., a specific feature (e.g., a road) can be represented in a very different 
shapes and styles across different map publishers.

**Input**: a raster historical map.

**Output**: a raster image in which each channel represents the probability of a pixel belonging to a 
specific class of geographic feature (e.g., roads)
