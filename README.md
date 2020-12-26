# Introduction
In this integrative work, we are going to propose a new implementation of an autoencoder to learn the MNIST database. We are going to mention the main reasons why we chose this model. We will detail what the topology of this new neural network is like and we will specify the chosen parameters that define how the learning stage will be carried out. We will continue to train the autoencoder and show relevant graphics such as Train Error vs. Test Error and Image Original vs. Reconstruction. Finally, we will make a comparison between this autoencoder and the one that was implemented using only one fully-connected hidden layer with 512 neurons and we will make a conclusion about it.

# Previous Work
Before this project, we implemented an autoencoder with a fully-connected hidden layer with 512 neurons. The disadvantage of this architecture is that the input image must be converted to a one-dimensional vector. This alteration generates the loss of spatiality since each neuron of the hidden layer will be "looking" at all the pixels of the input image.
This may be warning us that the topology of this neural network is not the most suitable for the processing and extraction of information from an image.

# New Proposal
Instead of using fully connected layers, we are going to use ***convolutional*** and ***pooling*** layers to reduce our input to an encoded representation. In this way, the image should no longer be converted to a one-dimensional vector and therefore the spatial information we continue to have.  
We believe that this factor can help improve the task of learning the identity function.
