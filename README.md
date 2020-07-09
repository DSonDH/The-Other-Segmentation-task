# Segmentation-task
Segmentation task with Gangnam Severance Hospital

Objective: Normal Subcortical Template 생성
task: 1. using multimodal data (T1, FLAIR, SWAN) finely segment subcortical region (caudate, putamen, globus pallidus, thalamus, subthalamic nucleus, substantia nigra, red nucleus, cerebellar dentate nucleus)

2. transform segmented data to the template space then genereate subcortical probablistic template model

issue: there's no training set for training segmentation deep learning network
temp sol: transfer learning with manual ground truth generation but the ROI seem not suitable for transfer learning
temp sol2: manually segment ROIs and train the network and feedfoward the other data.

Application:
