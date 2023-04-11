### Transunet
Repo for the sample implementation of the paper "TransUNet: Transformers Make Strong Encoders for Medical Image Segmentation" on Keras

Unet is a popular image segmentation method used for semantic segmentaion. The architecture of Unet is shown below.
![Original Unet Architecture](https://miro.medium.com/v2/resize:fit:4800/format:webp/0*38vydfXeaN0Nc1p7.png)

Original Unet Paper: [U-Net for Biomedical Image Segmentation](https://arxiv.org/pdf/1505.04597.pdf)

Unet relies on convolution operations for segmentation tasks. The U-Net model provides several advantages for segmentation tasks: first, this model allows for the use of global location and context at the same time. Second, it works with very few training samples and provides better performance for segmentation tasks.

But due to instrinsic locality of convolution operations, U-net demonstrates limitations in modelling long range dependency. The author of the paper "TransUNet: Transformers Make Strong Encoders for Medical Image Segmentation" purposed TransUnet. The architecture of TransUnet is shown below.

![Tranunet Architecture](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*1l_NSL1H1Evbn6IImZzx0A.png)

Original TransUnet Paper: [TransUNet](https://arxiv.org/pdf/2102.04306.pdf)


This repo contains two variations of the Unet studied on the Original Paper. Both of these are written using Keras Library

1. Resnet50 based Unet
> This variation of Unet uses a pretrained (trained on Imagenet) Resnet50 network as the encoder.
2. TransUnet

Necessary Libraries are mentioned on the requirements.txt file
> pip install -r requirements.txt

Datset Used:
[Breast Ultrasound Images Dataset](https://www.kaggle.com/datasets/aryashah2k/breast-ultrasound-images-dataset)

The implementation of TranUnet employes the use of a pretrained RensNet50 model (trained on Imagenet) and a ViT for encoding process as shown in the figure above. The weights of ResNet50 are frozen for training while ViT is trained.


****

Test folder contains a test TransUnet architecture tested on a different dataset from Kaggle: 
[Data Science Bowl 2018](https://www.kaggle.com/competitions/data-science-bowl-2018/overview)

