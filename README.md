# SE-NET-from-scratch : 


![1668201137108](https://user-images.githubusercontent.com/99510125/204152064-9b2cb3f4-61ab-45cb-bac1-3fd646ba262d.jpeg)



What is (SENet)?


A SENet is a convolutional neural network architecture that employs squeeze-and-excitation blocks to enable the network to perform dynamic channel-wise feature recalibration.



![1668199684520](https://user-images.githubusercontent.com/99510125/204152067-d0ab9200-ce79-40eb-94b5-9e777fd14af2.png)


with the squeeze-and-excitation block, the neural nets are better able to map the channel dependency along with access to global information. Therefore, they are better able to recalibrate the filter outputs, and thus, this leads to performance gains.

This main idea can be further explained using the Squeeze-and-Excitation block image above from the paper. First, a feature transformation (such as a convolution operation) is performed on the input image X to get features U. Next, we perform a squeeze operation to get a single value for each channel of output U. After, we perform an excitation operation on the output of the squeeze operation to get per-channel weights.

Finally, once we have the per-channel weights, the final output of the block is obtained by rescaling the feature map U with these activations.
