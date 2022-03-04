# Unsupervised Domain Adaptation through CycleGAN
Final project for the course "Machine Learning for Vision and Multimedia" @Politecnico di Torino.

* *Main algorithms and techniques:* CNN, CycleGAN, U-Net, PatchGAN, t-SNE.
* *Evaluation metrics:* Feature Embeddings (t-SNE), Generated vs Real images (Nearest Neighbor search), Accuracy, Confusion Matrix.
* *Programming language and main libraries:* Python, Keras/Tensorflow.

### Abstract
The objective of this work is to propose an approach to address the problem of domain adaptation through the use of generative adversarial networks. Specifically, it will be evaluated the effectiveness of CycleGAN in performing the image translation from the source to the target domain, and how much this operation can impact on the final image classification task in terms of accuracy. 
<br>CycleGAN is a GAN-based model which allows to perform unpaired image-to-image translation. It combines two GANs in a cyclical manner: the first generator allows to pass from the domain A to the domain B, then the second generator allows to come back from B to A.
<br>The idea is to train a CycleGAN to translate images among source and target domains, extract the generator which allows to pass from source to target and use it either chained with the final CNN to produce “target-like” images on-the-fly as the training proceeds, or autonomously to generate offline a new version of the dataset which will be used to train the final CNN.

<br>For more details see [*ML4VM-paper.pdf*](ML4VM-paper.pdf).
