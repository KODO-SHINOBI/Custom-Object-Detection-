<h1>Some Common Errors</h1>
<p>-->Here we will to try to point out some common errors occur during the program development. And we will also provide you with the possible solution. 
  So we reccomend you to follow the below mentioned points.</p>
<br /><br />

<b>Error-1:</b> No module named ‘xxxxxx’<br/>
<b>Solution-1:</b> Install that module
<pre>!pip install xxxxxx</pre>
 <br/> <br/>
 

<b>Error-2:</b> No module named typeguard<br/>
<b>Solution-2:</b> pip install typeguard <b /> # note the name of the module will not always equal the package name
 <br/> <br/>
 
<b>Error-3:</b> AttributeError: module 'sip' has no attribute 'setapi'<br/>
<b>Solution-3:</b> Downgrade matplotlib to version 3.2 by running the following command
<pre>!pip install matplotlib==3.2</pre>
 <br/> <br/>
 
<b>Error-4:</b> ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject<br/>
<b>Solution-4:</b>  Reinstall pycocotools
<pre>Pip uninstall pycocotools -y
Pip install pycocotools</pre>
 <br/> <br/>
 
<b>Erro-5:</b> ValueError: 'images' must have either 3 or 4 dimensions.<br/>
<b>Solution-5:</b> Restart your jupyter notebook as the Webcam is unavailable. If using images, this normally means your image name and path is incorrect.
 <br/> <br/>
 
<b>Error-6:</b>error: <P>(-2:Unspecified error) The function is not implemented.</p> <p>Rebuild the library with Windows, GTK+ 2.x or Cocoa support.</p><p> If you are on Ubuntu or Debian, install libgtk2.0-dev and pkg-config, then re-run cmake or configure script in function 'cvDestroyAllWindows'<br/></p>
<b>Solution-6:</b> Reinstall opencv and uninstall opencv-headless
<pre>
pip uninstall opencv-python-headless -y
pip install opencv-python --upgrade
</pre>
 <br/> <br/>
 

 
<b>Error-7:</b>When running training script from the command line, you get a No module error. e.g. ModuleNotFoundError: No module named 'cv2'
 <br/>
<b>Solution-7:</b> Remember you need to activate your environment at the command line in order to leverage all the packages you have installed in it. 
 <br/> <br/>
 
<b>Error-8:</b> When training, only the CPU is used and the GPU is ignored. 
<br/>
<b>Solution-8:</b> Ensure you have a matching CUDA and cuDNN version for your Tensorflow version installed. Windows:https://www.tensorflow.org/install/source_windows, Linux/macOS: https://www.tensorflow.org/install/source
 <br/> <br/>
 
<b>Error-9:</b>CUBLAS_STATUS_ALLOC_FAILED or CUDNN_STATUS_ALLOC_FAILED <br/>
<b>Solution-9:</b> This is because the available VRAM on your machine is completely consumed and there is no more memory available to train. Quit all of your Python programs and stop your Jupyter Notebook server to free up the VRAM and run the command again. 
 <br/> <br/>


Template
<b>Error:</b> <br/>
<b>Solution:</b> 
<pre></pre>
