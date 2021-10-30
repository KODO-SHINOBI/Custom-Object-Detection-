# Custom Object Detection Using TensorFlow
 
<p>This is the complete guide to show how to train and leverage your own custom object detection model using the Tensorflow Object Detection API. Here we have also added the required code and details like how the specific code works.</p>
<br />
<strong>NOTE :- This is just a guide where we have shown how to program a custom object detection model and resources required to do it. This model will be helpful in detecting any object not only what we have used for. We highly recommend to use your own datasets(images/videos) during this process.</strong>
<br /><br />
## Steps
<br />
<b>Step 1.</b>At first, we need to </b>clone this repository: https://github.com/KODO-SHINOBI/Custom-Object-Detection
<br/><br/>

<b>Step 2.</b> Then we need to create a new virtual environment 
<pre>
python -m venv cod
</pre> 
<br/>

<b>Step 3.</b> To proceed further we will have to activate our virtual environment
<pre>
source cod/bin/activate # Linux
.\cod\Scripts\activate # Windows 
</pre>
<br/>

<b>Step 4.</b> Then, install dependencies and add virtual environment to the Python Kernel
<pre>
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=cod
</pre>
<br/>

<b>Step 5.</b> One can collect images of their choice which must include:-(i)  objects that you want to detect<sup>**</sup>.
                                                                          (ii) images with different perspective<sup>**</sup>.
<img src="https://github.com/KODO-SHINOBI/Custom-Object-Detection-/blob/main/image/dep.png"> 
<br/>

<b>Step 6.</b> Here we will need to do manual classification and therefore manually divide collected images into two folders train and test. So now all folders and annotations should be split between the following two folders. <br/>
\COD\Tensorflow\workspace\images\train<br />
\COD\Tensorflow\workspace\images\test
<br/><br/>

> <b>Step 7.</bAfter the classification process is done start training process by opening <a href="https://github.com/nicknochnack/Custom-Object-detection/blob/main/2.%20Training%20and%20Detection.ipynb">2. Training and Detection.ipynb</a>, this is guide about installing Tensorflow Custom Object Detection, making detections, saving and exporting the respective model. 
<br /><br/>

<b>Step 8.</b> During this process the Notebook will install Tensorflow Custom Object Detection. One should ideally receive a notification indicating that the API has installed successfully at Step 8 with the last line stating OK.  
<img src="https://github.com/KODO-SHINOBI/Custom-Object-Detection-/blob/main/image/com.png">
If not, the we can resolve installation errors by referring to the <a href="https://github.com/nicknochnack/Custom-Object-Detection/blob/main/README.md">Error Guide.md</a> in this folder.
<br /> <br/>

<b>Step 9.</b> Once we get to step 6. Train the model, inside of this guide, we may choose to train the model from within the notebook. As because training inside of a separate terminal on a Windows machine we're able to display live loss metrics. 
<img src="https://github.com/KODO-SHINOBI/Custom-Object-Detection-/blob/main/image/ver.png"> 
<br />

<b>Step 10.</b> One/we can optionally evaluate their model inside of Tensorboard. Once the model has been trained and we have run the evaluation command under Step 7. We should navigate to the evaluation folder for the trained model e.g. 
<pre> cd Tensorlfow/workspace/models/my_ssd_mobnet/eval</pre> 
and need to open Tensorboard with the following command
<pre>tensorboard --logdir=. </pre>
Tensorboard will be accessible through our browser and we will be able to see metrics including mAP - mean Average Precision, and Recall.
<br />
