1. addNoise script-
	The MATLAB code which is run in octave that adds noise and converts 
images to greyscale as well. 

2. imageCropper -
	Python script that splits an image to multiple parts. In our case, one 
image(5000x5000 pixels) was split into 100 each 500*500. The image source and 
destination are google drive links present in it.

3. SegNet - 
	Colab code which needs to be run to create a new model without prior weights
associated. Change the number of epochs, runs per epoch, GOOGLE drive links of 
dataset and destination to save weights here in the code block titled training.py
Also to predict images, change drive address of saved weights and saved model in 
loading model block, and prediction image drive address in predicting output block.

4. testingSegNet -
	Same as SegNet but here in training block we load prior saved weights and
continue training from there.	

5. UNet -
Consists all the main code implementing the UNet architecture. This notebook enables 
us to  create a new training model by specifying the epochs, run per epoch etc. 

6. SAR -
This notebook doesn't contain any extra code, it needs to be run when a previously saved 
weight is to be used for further training or for predictions.

In both the UNet and SAR notebooks, the older version of keras and tensorflow are to be
installed first because of some dependencies.


