Trying to solve digit recognizer competition for https://www.kaggle.com/c/digit-recognizer

Following are the methods I have appplied so far:

1. KNN + PCA:
   Convert the 28*28 = 784 dimensional input data to 100 dimensional data using Principal Component Analysis(PCA)
   This solution gave an accuracy of 96.914

2. Using CNN on Augmented data:
   a. First I increased the data set by augmentation methods like ( rotating image 30 degress left and right), adding noise to images.
      (This step is necessary and is usefull because we dont know about the test data it can be rotated than usual and might be noisy)
   b. CNN is mostly used method for image processing or classification probelms.
      Here is the architecture of:

      i. #Convolution layer 1 with 32 filters and kernel size is 5
 	 #Max pooling with strides of 2 and kernel size of 2
   
      ii. #Convolution layer 2 with 64 filters and a kernel size of 3
	  #Max Pooling with strides of 2 and kernel sizes 2

      iii. #flatten the data to a 1-D vector for fully connected layer
   
      iv. #Fully Connected layer 1024 dimension

      v. #Output layer class predicition
   
	


   This solution gave an accuarcy of 97.985
