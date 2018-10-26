# Solar Panel Detection using Mask RCNN

To detect solar panels from satellite images for Indian rooftops, using Mask RCNN.

## Getting Started

mrcnn contains the model configuration in custom.py and evaluation using mAP metric in eval.py.

solar_panel_dataset contains:
* train - Training Images with annotation file
* val - Validation Images with annotation file

Two models have been trained on:
* Original Images 
* Sharpened Images using filter2D 

## Training

python3 custom.py train --dataset=solar_panel_dataset --weights=coco

## Evaluation:

python3 eval.py 

## Results:
After being trained on 102 images, 
* mAP for original dataset: 0.484
* mAP for sharpened images dataset: 0.344

## References

* Paper Link: [Mask R-CNN](https://arxiv.org/abs/1703.06870).
Link to the repository: https://github.com/matterport/Mask_RCNN

