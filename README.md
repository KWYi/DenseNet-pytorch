# DenseNet
DenseNet Code

This code has been used for the paper "Visual Explanation of a Deep Learning Solar Flare Forecast Model and Its Relationship to Physical Parameters" (https://doi.org/10.3847/1538-4357/abdebe).

## Usage
```
from DenseNet import DenseNet_v1

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
