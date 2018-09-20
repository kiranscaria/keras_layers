# Various Keras Layers that can be used with TensorFlow Eager Execution

## SparseConv2D
Sparse Convolution layers allow CNNs to process sparse sensory data. To make the convolution operation invariant against sparsity, the sparsity related information is propagate through the network and the output of the layer is normalized depending on the number of information-carrying elements in the convolution window.

Sparsity Invariant CNNs [arXiv:1708.06500](https://arxiv.org/abs/1708.06500)

### MaxPoolingWithArgmax2D and MaxUnpooling2D
In convolutional encoder-decoder architectures, one may want to invert the max pooling operation without loosing spatial information. This is exactly what these layers do. MaxPoolingWithArgmax2D is a max pooling layer that addidionally outputs the pooling indices and MaxUnpooling2D uses them for unpooling.

SegNet: A Deep Convolutional Encoder-Decoder Architecture for Image Segmentation [arXiv:1511.00561](http://arxiv.org/abs/1511.00561)
