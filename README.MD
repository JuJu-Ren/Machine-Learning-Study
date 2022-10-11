# Deep Learning Fundamentals: Linear Neural Networks, Multilayer Perceptrons

## [History](https://github.com/JuJu-Ren/Machine-Learning-Study/blob/main/files/history.MD)
* Convolutional Neural Networks: **LeNet, AlexNet, VGG, Inception, ResNet**

*  Recurrent Neural Networks: **RNN, GRU, LSTM, seq2seq**

* Attention mechanism: **Attention, Transformer**

* Optimization Algorithms: **SGD, Momentum, Adam**

* High Performance Computing: **Parallel, Multi-GPU, Distributed**

* Computer Vision: **Object Detection, Semantic Segmentation**

* Natural Language Processing: **Word Embeddings, BERT**


卷积神经网络（CNN）
卷积神经网络
深度卷积网络：实例探究
目标检测
特殊应用：人脸识别和神经风格转换
序列模型（RNN、LSTM）
循环序列模型（RNN）
自然语言处理与词嵌入
序列模型和注意力机制

## Surpervised Learning
* Feed Forward Neural Networks

Feed Forward Neural Networks (FFNNs), dating back to the 1940s, are networks without any loops. Data is passed from input to output in a single pass without any previous "state memory". Technically, most networks in deep learning can be thought of as FFNNs, but often "FFNN" refers to its simplest variant: a densely connected multilayer perceptron (MLP).
Dense encoders are used to map an already compact set of numbers on the input to predictions: classification (discrete) or regression (continuous).

* Convolutional Neural Networks

CNNs (aka ConvNets) are feedforward neural networks that use a spatial invariance technique to efficiently learn local patterns in images, most commonly seen in images. Spatial-invariance means that, for example, on an image of a cat face, the cat ears in the upper left corner have the same characteristics as the cat ears in the lower right corner of the image. CNNs share weights across space, making detection of cat ears and other patterns more efficient.

Instead of just using densely connected layers, CNNs use convolutional layers (convolutional encoders). These networks are used for image classification, object detection, video action recognition, and any data that has some spatial invariance in its structure (such as speech audio).

* Recurrent Neural Networks

RNNs are networks that have loops and therefore have "state memory". They can be unfolded in time to become weight-sharing feed-forward networks. Just as CNNs share weights in "space", RNNs share weights in "time". This enables them to process and efficiently represent patterns in sequence data.

There are many variants of RNN modules, including LSTMs and GRUs, to help learn patterns in longer sequences. Its applications include natural language modeling, speech recognition, speech generation, and more.

* Encoder-Decoder Architectures

The "Encoder-Decoder" architecture is a more advanced concept that generates high-dimensional output through a decoding step that upsamples the compressed representation, rather than making predictions.

Note that the encoder and decoder can be very different from each other. For example, an image captioning network might have a convolutional encoder (for image input) and a recurrent decoder (for natural language output). Applications of the Encoder-Decoder architecture include semantic segmentation, machine translation, etc.

## Unsupervised Learning
* Autoencoder

An autoencoder is a simpler form of "unsupervised learning" that takes the encoder-decoder architecture and learns to generate an exact replica of the input data. Since the encoded representation is much smaller than the input data, the network is forced to learn how to form the most meaningful representation.

Since the ground truth data comes from the input data, no human intervention is required. In other words, it is self-supervised. Applications of autoencoders include unsupervised embedding, image denoising, etc. Most importantly, its basic idea of ​​"representation learning" is the core of generative models and all deep learning in the next section.

* Generative Adversarial Networks

GAN is a framework for training networks that are optimized to generate new realistic samples from specific representations. In its simplest form, the training process involves two networks. One of the networks, called the generator, generates new instances of data in an attempt to fool the other network, the discriminator, which classifies images as real and fake.

Over the past few years, GANs have seen many variants and improvements, including the ability to generate images from specific classes, the ability to map from one domain to another, and a surprising increase in the realism of the generated images. 

## Reinforcement Learning
* Networks for Actions, Values, Policies, and Models.

Reinforcement learning (RL) is a framework for teaching an agent how to act in a way that maximizes reward. When learning is done by a neural network, we call it Deep Reinforcement learning (Deep RL).

There are three types of RL frameworks: policy-based, value-based, and model-based. The difference is that the task of a neural network is to learn. For a detailed explanation, please refer to Lecture 6 of this series of courses.

Deep RL allows us to apply neural networks in simulated or real-world environments when we need to make a series of decisions. Including games, robotics, neural architecture search, and more.
