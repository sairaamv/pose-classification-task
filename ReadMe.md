## Problem Statement :

[MPII Human Pose dataset](http://human-pose.mpi-inf.mpg.de/#) is a state of the art benchmark for evaluation of articulated human pose estimation. The dataset includes around 25K images containing over 40K people with annotated body joints.

Although many experiments use neural networks to achieve the classification, some stakeholders demand better explainability.

Here we have a small subset of mpii's annotated data, filtered to include only the positions related to sports and exercise. The challenge here is to use just the annotations (and not the images) for pose classification.

- Machine Learning Task: **Classification**
- Target Variable: **Activity name**
- Evaluation Metric - choose the best !

## Data Description :

poseTrain_Dataset - training dataset that includes the label column (act_name)
poseEval_Dataset - Evaluation dataset that excludes the label column.

|     | Columns  | Description   |
|----:|:--------|:--------|
|  1 | img_id   | image id  |
|  2 | rx1, ry1, rx2, ry2 | coordinates of the head rectangle  |
|  3 | scale    | person scale w.r.t. 200 px height  |
|  4 | x_i, y_i | keypoint coordinates of the ith joint |
|  5 | vis_i    | visibility of the ith joint   | 
|  6 | cat_name | category name |
|  7 | act_name | activity name |


