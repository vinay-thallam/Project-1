# Project-1

# Assignment 1A

Below is the link to the notebook for the assignment. Have added comments in the code blocks describing the value choosen for respective kernels.

https://colab.research.google.com/drive/1tXjiQtNRpRGu3TC-F8iTuQrwhOrgmTby


# Assignment 1A

## What are Channels and Kernels (according to EVA)?

Channels are the similar feature bags. For example, edges in the image are one kind of feature. All edges extracted into a separate image (output) is the channel of edges. Each channel contain only one kind of feature. 


Kernels or filters are the feature extractors. These are carefully choosen values in a matric of 3X3 which when convolved over an images extracts the specific feature into a separate channel.

## Why should we only (well mostly) use 3x3 Kernels?

There are 2 questions to answer in this, i.e why only odd numbered kernel ? Because with even numbered kernel we cannot get the middle value. middle value is spread between two coloumns. But with odd numbered, we can get middle values, helping us to distinguish between left and right values easily.

Another question is why not other odd numbered kernels like 5X5 or 7X7

Because a 3X3 kernel can be repeated many times to get any size we want. For example convolving using 3X3 twice gets the same receptive field as 5X5 kernel. 

## How many times do we need to perform 3x3 convolution operation to reach 1x1 from 199x199 (show calculations)

We need to add 99 layers of convolution using 3X3 kernel to get to 1X1 image starting fom 199X199, since each layer reduces the resolution by 2 pixel.
