# FaceMaskDetection

This a Real-Time Face Mask detection appilication using Deep Learning. 
This system can predict whereas a person wearing a face mask or not. 
Dataset used:mFace Mask Detection ~12K Images Dataset by Ashish Jangra

### `How to Run`

1. Download and open FaceMaskDetection project directory.
2. Open Anaconda Powershell Promt (or any other terminal).
3. Write Jupyter Notebook and press Enter.

Then you will find a Home page like the below figure. Open "MaskPredct.ipynb" and run the project. :) 

### `Appilication Home Page`

<img src="gitimg\homepage.png" />

<br>

### `Image Processing`

At first dataset images need to be processed. All the images have been converted in grayscale from RGB.
And re-sized into (48, 48) because CNN (Convolution Neural Network) takes same size input.

<img src="gitimg\imgpro.jpg" />

<br>

### `CNN Model Training`

Sequential model has been used in this project. Sequential is the easiest way to build a model in Keras. It allows you to build a model layer by layer. I've used the 'add()' function to add layers to the model. The first 2 layers are Conv2D layers. And at the last I've added the Prediction layer.

<img src="gitimg\model.jpg" />
<br>
For fitting the model 15 epochs have been runed and gained a satisfactory accuracy :D
<img src="gitimg\modelfit.jpg" />
<br>

### `Results`

The accuracy of 97% has been gained for both Training and Validation which pretty impressive.

<img src="gitimg\acc.png" />

<br>

The loss is very low. For Training dataset the loss is 6.87% and for Validation dataset the loss is 10.56%.
N.B. For calculating the loss categorical_crossentropy has been used.
<img src="gitimg\loss.png" />
<br>

### `Face Mask Prediction Page`

Here Haarcascade classifier has been used for face recognition. And for face mask prediction "fmaskmodel.h5" model has been used which has been trained on the mentioned dataset.

<img src="gitimg\maskpredict.png" />

<br>


### `Project Overview`

No musk

<img src="gitimg\nomask.png" />

With musk

<img src="gitimg\withmask.png" />