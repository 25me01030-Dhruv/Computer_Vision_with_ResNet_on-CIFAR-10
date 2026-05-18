# Computer_Vision_with_ResNet_on-CIFAR-10
I have trained a CNN model for training the CIFAR 10 dataset. I used ResNet 18 by building it from scratch.  

# The code is based on Pytorch on google colab runned under T4-GPU. One can access it and run the commands to verify the results. 
The learning rate is chosen to be 0.1 for the training pipeline. 
The batch size is 200 applied with the Stochastic Gradient Descent (SGD) and 'cross entropy loss'.

# The epoch value was set to 10. 
AND applying these constraints I achieved the overall train accuracy of     and overall test accuracy of '77.83%'. 
A visualization on epochs vs accuracy and epochs vs loss is also shown.

# Preview : The resnet model (Residual network) model is a pretrained deep learning CNN architecture that is utilized for the task of image recogniton. Originally    the ReSNet architecture was introduced in 2015 through the paper 'Deep Residual Learning for Image Recognition'. It was developed to counter a very common problem named 'Vanishing Gradient'. 

Vanishing gradient problem : Since deep learning models are built on deep neural networks. So when optimizers were applied to fetch the new value of the weights, 
                            the gradients were so low that the visible change in the weights was almost none. Thus due to this problem the deep NNs surprisingly 
                            would give poor results than shallower models. The first clue for the vanishing gradient problem was that 'The model was not overfitting
                            in training'. 

The fix by ResNET : ResNet introduced the concept of skip connections. A residue term variable X was added to F(X) by passing the value directly by skipping the CNN                      layers and the final result was H(X) = F(X) + X. Thus due to this residue term X the gradient could never to significantly small to be neglible.

The ResNet model thus became more successful in image recognition problems than VGGNET, Alexnet and plain networks. IN ImageNet dataset the resnet model could achieve much more deep neural networks than other models with no degradation problem and even with lesser FLOPS than other architectures.


