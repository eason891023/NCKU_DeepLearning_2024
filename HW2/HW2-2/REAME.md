file discription：

HW2-2.ipynb: the implementation of using 5 Layer Network to achieve 90% performance of ResNet34.
HW2-2_resnet34.ipynb: the implementation of ResNet34.

Introduction：

The Dynamic Convolution Module first generates K attention weights 𝜋ₖ ranging from 0 to 1 when inputs arrive. These weights are then multiplied with K kernels, and their results are aggregated to form the aggregate_weight of the Dynamic Convolution Module. Therefore, the kernel of the Dynamic Convolution Module is not a fixed value but dynamically changes with inputs.
In HW2-2.ipynb, only using 4 layers of Dynamic Convolution and 1 FC layer can get a better results than  ResNet34 in ImageNet mini dataset.
