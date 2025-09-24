# Img_Cap_Generator
Approach to the problem statement : The encoder-decoder image captioning system would encode the image, using a pre-trained Convolutional Neural Network that would produce a hidden state. Then, it would decode this hidden state by using LSTM mechanism and generate a caption.

But RNNs tend to be computationally expensive to train and evaluate, so in practice, memory is limited to just a few elements. Attention models can help address this problem by selecting the most relevant elements from an input image.

Rather than compressing an entire image into a static representation, the Attention mechanism allows for salient features to dynamically come to the forefront as and when needed. This is especially important when there is a lot of clutter in an image.

The image is first divided into n parts,when the RNN is generating a new word, the attention mechanism is focusing on the relevant part of the image, so the decoder only uses specific parts of the image.

<br>
Dataset
The dataset for this project is taken from the Kaggle dataset website. Here is the link for the dataset: https://www.kaggle.com/datasets/adityajn105/flickr8k
<br>
Models Used
1.ResNet-50 is a deep neural network architecture that incorporates residual blocks, introducing shortcut connections to facilitate the training of very deep networks.
With 50 layers, ResNet-50 employs a bottleneck design, utilizing 1x1, 3x3, and 1x1 convolutions in sequence. Frequently pretrained on large-scale image classification tasks like ImageNet.
ResNet-50 serves as a powerful feature extractor and is widely used for transfer learning in diverse computer vision applications. Its availability in popular deep learning frameworks,
along with model zoos housing pretrained versions, enables researchers and practitioners to easily leverage its capabilities for tasks such as image classification, object detection, and segmentation. ResNet-50's impact extends beyond its architecture, influencing the design of subsequent deep neural networks and contributing to the success of deep learning in computer vision.
