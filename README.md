# Segmentation-task1: subcortical segmentation
Segmentation task with Gangnam Severance Hospital

Objective: Normal Subcortical Template 생성

task: 
1. using multimodal data (T1, FLAIR, SWAN) finely segment subcortical region (caudate, putamen, globus pallidus, thalamus, subthalamic nucleus, substantia nigra, red nucleus, cerebellar dentate nucleus)

2. transform segmented data to the template space then genereate subcortical probablistic template model

issue: there's no training set for training segmentation deep learning network

temp sol: transfer learning with manual ground truth generation but the ROI seem not suitable for transfer learning

temp sol2: manually segment ROIs and train the network and feedfoward the other data.

temp sol3: Use the similar data obtained from the other images of different diseas (NMOSD, MS)
the images obtained from Freeserfer includes parceled images of subcortical regions, which can be the training label for the segmentation network.

Application: Using the obtained normal subcortical template, atlas, 


# Segmentation-task2: WHM segmentation
Segmentation task with changwon gyeongsang national university hospital (CGNUH)

Objective: White Matter Hyperintensity (WMH) map generation

task: 
1. using multimodal data (T1, FLAIR) finely segment WMH lesion

2. Much less false positive
issue: No exact training dataset exept WMH map of NMOSD and MS (which is not exactly fine segmentation map)

temp sol: semi-superviesed learning

Application: Using the obtained segmenation map, we can study the distribution of lesion easily
