# Image Classification
![](https://firebasestorage.googleapis.com/v0/b/dashboard-web-2e57e.appspot.com/o/images%2Fimg1.png?alt=media&token=efd48297-592a-4c7b-9d22-79ab7c083863)
A ConvNet in TensorFlow for a classification problem.
In detail, the following parameters for all the steps:

 - Conv2D: stride 1, padding is "SAME"
 - ReLU
 - Max pool: Used an 8 by 8 filter size and an 8 by 8 stride, padding is "SAME"
 - Conv2D: stride 1, padding is "SAME"
 - ReLU
 - Max pool: Used a 4 by 4 filter size and a 4 by 4 stride, padding is "SAME"
 - Flatten the previous output.
 - FULLYCONNECTED (FC) layer: Applied a fully connected layer without an non-linear activation function. Didn't call the softmax here. This will result in 6 neurons in the output layer, which is passed later to a softmax. In TensorFlow, the softmax and cost function are lumped together into a single function, which are called in a different function when computing the cost. 
 
The model below should:

 - create placeholders
 - initialize parameters
 - forward propagate
 - compute the cost
 - create an optimizer
 
Finally create a session and run a for loop for num_epochs, get the mini-batches, and then for each mini-batch optimize the function.
This model recognizes SIGN language with almost 95 % and 80% accuracy on the train and test set respectively.
![](https://firebasestorage.googleapis.com/v0/b/dashboard-web-2e57e.appspot.com/o/images%2Fimg2.png?alt=media&token=a2e9eeb8-b20f-426e-9ee6-f7515cd9934e)
![](https://firebasestorage.googleapis.com/v0/b/dashboard-web-2e57e.appspot.com/o/images%2Fimg3.png?alt=media&token=481bda7d-8d58-4bcc-85d5-37d90eb12c06)
