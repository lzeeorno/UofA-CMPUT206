This is Zheng Fuchen(Leon) 1465251.
There are total 6 documents. 3 models which are corresponding to 3 ipynb documents. 
Part1:
The training.ipynb is the part1 original code after completion.  
	- i complete the two parts, first is Convert data to grey images instead of RGB; 
		second is Normalize image values from -0.5:0.5 instead of 0:225.
The keras_cifar10_trained_model_color.h5 is the model with RGB images that after run the training.ipynb
	-comment the part of code which is the part use to convert RGB to gray images, 
		because this is a model of colorful images. 
The keras_cifar10_trained_model_gray.h5 is the model with gray images that after run the training.ipynb
	-do not comment the part of code which is the part use to convert RGB to gray images,
		becasue this is a model of gray images
Part2&3:
The inference.ipynb document use to test the accuracy of training. 
	- converting gray images part as comment becasue 
		user do not need to convert to gray images when they use color_modul to test 
	-normalize the x_test by /255-0.5
	-show 7 misclassified samples in the test use model.predict, and compare by np.argmax(...)

Part4: Improve Model Accuracy to achieve more than 71%
Base on the training.ipynb algorithm, i use two method to improved the accuracy. 
	-My first method is add one more Con2D(128) layer.
	-My second method is import and apply the BatchNormalization.  


