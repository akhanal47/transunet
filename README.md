### Transunet
Repo for the sample implementation of the paper "TransUNet: Transformers Make Strong Encoders for Medical Image Segmentation" on Keras

Unet is a popular image segmentation method used for semantic segmentaion. The architecture of Unet is shown below.
![Original Unet Architecture](https://miro.medium.com/v2/resize:fit:4800/format:webp/0*38vydfXeaN0Nc1p7.png)

Unet relies on convolution operations for segmentation tasks. The U-Net model provides several advantages for segmentation tasks: first, this model allows for the use of global location and context at the same time. Second, it works with very few training samples and provides better performance for segmentation tasks.

But due to instrinsic locality of convolution operations, U-net demonstrates limitations in modelling long range dependency. The author of the paper "TransUNet: Transformers Make Strong Encoders for Medical Image Segmentation" purposed TransUnet. The architecture of TransUnet is shown below.

![Tranunet Architecture](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*1l_NSL1H1Evbn6IImZzx0A.png)


This repo contains two variations of the Unet studied on the Original Paper

1. Resnet50 based Unet
2. TransUnet

Necessary Libraries are mentioned on the requirements.txt file
> pip install -r requirements.txt
