# Installation-of-Dependencies-on-Windows
Here, installing Python 3.5 along with opencv 3.3, Keras Using Anaconda.

----------------------------------------------------------------------------------
#Requirements:
    -  Make sure u have 64 bit windows OS
    -  with minimum requirements such as 2GB RAM, minimum of i3 processor, 10 to 20 GB free space on the harddrive
 
 Step 1: Downloading the anaconda Package
 -----------------------------------------
  Download the anaconda that suits with your OS from this officail link : https://www.anaconda.com/download/  
  (lets assume you are using 64-bit python 3.5 version)
 
 Step 2: Installing Anaconda
 ----------------------------
    - Run the setup and follow the installation.
    - While installing make sure to use a seperate destination folder, lets say you are creating the 
    destination folder under                 ---->          "c:\deeplearning\anaconda" 
    - press next and then next until package starts installing.
    ( after completing installation, we need to add our path to system environment variable
    otherwise system wont recognise anaconda.)
    -  Go to Control Panel  --> All Control Panel Items --> System --> Advanced system settings --> Environment variables
    - Under system Variables, there will be a variable named 'path', choose that variable and press Edit. 
    - Press 'new'  --> simply paste our anaconda installed path "C:\deeplearning\anaconda" (without quotes)
    - similarly add the below path also,
                  
                  ---       "C:\deeplearning\anaconda\Scripts"
                  ---       "C:\deeplearning\anaconda\Library\bin"
      
      (Note: kindly cross check with the availablility of these paths via our anaconda installed path)
     
    - After adding path, our system will recognise the anaconda. Now, open up a anaconda command prompt 
    (cmd) as administrator and execute the following command. These command will install some supportive libraries. 
        
            conda install libpython
            
   Step 3: Validating Anaconda
 ------------------------------
      -  open up a anaconda command prompt type the following
                  python
      -  After typing python, we will able see the version of python.
      -  Python comes with some in-built packages which are very useful for image processing such as Numpy,
      Scipy, Matplotlib, ipython and so on. Lets check whether these packages are avaliable or not. type
      the following command after executing the above "python" command.
             import numpy
             import scipy
             import matplotlib
      - if u want to install any package use the below syntax,
             pip install  xxx     # xxx is the name of the package
         
         
    Step 4: Installing C++ compilers (like MinGW-w64)
  ---------------------------------------------------
       - Download the MinGW-64 compiler from the official site http://www.mingw.org/
       - Run the setup and follow the installation.
       - While installing make sure to use a seperate destination folder, lets say you are
       creating the destination folder under      ---->          "c:\deeplearning\mingw" 
       
       - press next and then next until package starts installing.
    ( after completing installation, we need to add our path to system environment variable
    otherwise system wont recognise anaconda.)
       -  Go to Control Panel  --> All Control Panel Items --> System --> Advanced system 
       settings --> Environment variables
       - Under system Variables, there will be a variable named 'path', choose that variable and press Edit. 
       - Press 'new'  --> simply paste this path "“C:\deeplearning\mingw\mingw64\bin"  (without quotes) 
      
      
    Step 5: Installing Git
  -------------------------    
      - We will use git for cloning the reprository from github or any other sources.
      - Go to this URL https://git-scm.com/download/win and download Git the suitable Git.
      - Simply, Install the Git package.
      
    
    Step 6: Installing Tensorflow
  --------------------------------
      - TensorFlow is an open-source software library for dataflow programming across a range of tasks. It is 
      a symbolic math library, and is also used for machine learning applications such as neural networks.
     
      - open up a anaconda command prompt type the following
            
               pip3 install --upgrade tensorflow
      
      - After installing, type the "python" command and import the tensorflow to confirm the correct installation.
      
                    import tensorflow 
      
    Step 7: Installing Keras
  ---------------------------
  
       - open up a anaconda command prompt type the following
            
               pip install keras
      
       - After installing, type the "python" command and import the keras to confirm the correct installation
      
               import keras
        

    Step 8: Installing additional packages
  -----------------------------------------
  
      - Install the additional packages such as imutils, mahotas by the using pip
      
                pip install imutils
                pip install mahotas
                
       - After installing, type the "python" command and import the keras to confirm the correct installation
      
               import imutils
               import  mahotas
               
    
  Note: If there is any unknown or uncleared errors, don't hesitate to mail me.
