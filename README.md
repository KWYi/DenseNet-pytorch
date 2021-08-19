# DenseNet
This is a PyTorch implementation of DenseNet (Densely Connected Convolutional Networks, Huang et al., https://arxiv.org/abs/1608.06993).

This code has been used for the paper "Visual Explanation of a Deep Learning Solar Flare Forecast Model and Its Relationship to Physical Parameters" (https://doi.org/10.3847/1538-4357/abdebe).

<img src="https://user-images.githubusercontent.com/48608835/130018652-10254881-c8f9-4b28-a52b-22c67b059585.png" width=980px>

## Usage
```
from DenseNet_model import DenseNet

model = DenseNet(layers_num=5, growth_rate=13, drop_rate=0.5).to(device=DEVICE)
```

## Data Preprocessing
```
transforms.Compose([
                    transforms.ToTensor(),
                    transforms.Normalize(
                     mean=[0.5, 0.5, 0.5],
                     std=[0.5, 0.5, 0.5])
                                          ])
```
