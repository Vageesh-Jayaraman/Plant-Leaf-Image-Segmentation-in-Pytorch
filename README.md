# Plant-Leaf-Image-Segmentation-in-Pytorch
This project focuses on plant leaf image segmentation utilizing the FPN (Feature Pyramid Network) architecture implemented in PyTorch framework. FPN is a deep learning architecture specifically designed for semantic segmentation tasks, allowing for end-to-end pixel-wise predictions.

## Kaggle Notebook
[Link to Kaggle Notebook](https://www.kaggle.com/code/jvageesh11/plant-image-segmentation-fpn)

## Kaggle Dataset
[Link to Kaggle Dataset](https://www.kaggle.com/datasets/humansintheloop/plant-semantic-segmentation)

## FPN Model Structure
![image](https://github.com/Vageesh-Jayaraman/Plant-Leaf-Image-Segmentation-in-Pytorch/assets/143870355/c9704e87-c715-40af-9037-b449fc92cf24)

[Image credits](https://production-media.paperswithcode.com/methods/new_teaser_TMZlD2J.jpg)


## Installation

To install the necessary dependencies, run:

```bash
pip install -U git+https://github.com/qubvel/segmentation_models.pytorch
```
Usage
Once installed, you can import the FPN architecture from the `segmentation_models_pytorch` module and integrate it into your image segmentation pipeline.

```
from segmentation_models_pytorch import FPN

self.architecture = smp.FPN(
            encoder_name = 'tu-efficientnet_b0',
            encoder_weights = 'imagenet',
            in_channels = 3,
            classes = 1,
            activation = None)
```
