file discription:

HW2-1_myModel.ipynb：the implementation of AdaptiveChannelConv

HW2-1_naive_model.ipynb: the implementation of naiveModel

Introduction of AdaptiveChannelConv：

This module performs channel-wise AvgPooling and MaxPooling on the inputs (size = [batch, in_channel, H, W]) upon arrival, stacking these two tensors into a single tensor with in_channel set to 2 (size = [batch, 2, H, W]). This tensor is then fed into the Dynamic_convolution referenced in this assignment (with in_channel = 2, out_channels//2). Next, the Featuremap output from Dynamic convolution is stacked with the original input x, resulting in a tensor of size [batch, in_channel + out_channels//2, H, W]. If the number of channels is insufficient, additional channels are filled using channel-wise AvgPooling and MaxPooling.
