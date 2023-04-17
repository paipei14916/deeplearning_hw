# Deep Learning Assignment II

## LeNet5 
>- Original LeNet5: lenet5_sigmoid.ipynb
>- Adaptive Activation Function: lenet5_sigmoidx.ipynb
>- Kernel Size=3: lenet5_sigmoidx_conv3.ipynb
>- Increase One Convolution Layer: lenet5_sigmoidx_modify.ipynb

### Data Preprocessing
<img width="1028" alt="截圖 2023-04-17 下午12 06 02" src="https://user-images.githubusercontent.com/101318155/232375543-7d611f72-1cfe-4d10-b16e-66344e789dfe.png">

### Model Architecture

#### Input Layer
The LeNet5 model is typically applied to grayscale images, but it can also be adapted for use with RGB color images. Since RGB images have three color channels (red, green, and blue), the input layer of the model would be modified to have three layers instead of one. Each layer would correspond to one of the color channels, and the filters in the convolutional layers would be updated accordingly to handle the additional input dimensions. By incorporating color information into the model, the accuracy of image classification tasks can be improved.

#### Convolutional Layer
The convolutional layer applies a set of learnable filters (also known as convolutional kernels) to the input image. The filters are designed to extract features from the input image by convolving over the image and capturing spatial information.

#### Pooling Layer
It is typically used to downsample the feature maps and reduce the spatial dimensions of the input image. In LeNet5, max pooling is used to capture the most salient features of the input image, and this process helps to improve the model's invariance to small image translations.

#### Fully Connected Layers
The fully connected layers of the LeNet5 model take the high-level features extracted from the convolutional and pooling layers and use them to classify the input image into one of several predefined categories.


![image](https://user-images.githubusercontent.com/101318155/232376313-d2d8b991-f794-4cb8-9022-07622dd843fb.png)
The LeNet-5 Architecture (LeCun et al., 1998)

## Computational Graph
> imgclass_bp.ipynb

## Installation
```python
!pip install opencv-python
!pip install tqdm
!pip install multiprocess
```

## Reference
- LeCun, Y., Bottou, L., Bengio, Y., & Haffner, P. (1998). Gradient-based learning applied to document recognition. Proceedings of the IEEE, 86(11), 2278-2324.

- OpenAI. (2020). GPT: Language Models are Unsupervised Multitask Learners. https://github.com/openai/gpt-2/blob/master/model_card.md

- https://github.com/toxtli/lenet-5-mnist-from-scratch-numpy 

- https://github.com/gy910210/neural-network-from-scratch 

- https://github.com/harrypnh/lenet5-from-scratch


