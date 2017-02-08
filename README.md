# TensorFlow Tutorials

[Original repository on GitHub](https://github.com/Hvass-Labs/TensorFlow-Tutorials)

Original author is [Magnus Erik Hvass Pedersen](http://www.hvass-labs.org)

## Introduction

* These tutorials are intended for beginners in Deep Learning and TensorFlow.
* Each tutorial covers a single topic.
* The source-code is well-documented.
* There is a [YouTube video](https://www.youtube.com/playlist?list=PL9Hr9sNUjfsmEu1ZniY0XpHSzl5uihcXZ) for each tutorial.

## Tutorials

1. CIFAR-10 ([Notebook](https://github.com/Hvass-Labs/TensorFlow-Tutorials/blob/master/06_CIFAR-10.ipynb))

2. DeepDream ([Notebook](https://github.com/Hvass-Labs/TensorFlow-Tutorials/blob/master/14_DeepDream.ipynb))

3. Style Transfer ([Notebook](https://github.com/Hvass-Labs/TensorFlow-Tutorials/blob/master/15_Style_Transfer.ipynb))

16. MyDeepDreamCode ([Notebook] - contains the modified code with an interactive UI to tweak different parameters and run the DeepDream)

Modified Codes Files For Style Tansfer by us:

1. Style_Transfer_Averaging_Total_Loss_By_No_Of_Loss
2. Style_Transfer_Calculating_Style_Loss_Before_Content_Loss
3. Style_Transfer_Changing_Style_Content_Layer_Value
4. Style_Transfer_HTML_Inputs_From_User
5. Style_Transfer_Modifying_Function_ For_Denoising_Image_By_Shifting_By_50_Pixels
6. Style_Transfer_Saving_Input_Output_Images
7. Style_Transfer_Saving_Mixed_Image_Every_10_Iterations
8. Style_Transfer_Without_Calculating_Denoising_Loss
9. Style_Transfer_Without_Style_Loss

## Outputs
1. DeepDream:Outputs For Style Transfer Are in: Images/DeepDream Different Outputs
2. Style Transfer: Outputs for Style Transfer are in: Images/outputs_StyleTransfer
    For style transfer each output is in a separate folder in Images/outputs_StyleTransfer. 

    Each folder has the following: 

    a. Original Content Image as Content.jpg
    
    b. Original Style image as Style.jpg
    
    c. Mixed Image Generated: Mixed.jpg
    
    d. Mixed Image after every 10 iteration as mixedi.jpg where i is the iteration number for which the mixed image was generated.
    
    e. A ParametersPassed.txt which has the style transfer program name used for generating the output images. Also the parameters for          which the program was run.  


## Videos

These tutorials are also available as [YouTube videos](https://www.youtube.com/playlist?list=PL9Hr9sNUjfsmEu1ZniY0XpHSzl5uihcXZ).

## Older Versions

Sometimes the source-code has changed from that shown in the YouTube videos. This may be due to
bug-fixes, improvements, or because code-sections are moved to separate files for easy re-use.

If you want to see the exact versions of the source-code that were used in the YouTube videos,
then you can [browse the history](https://github.com/Hvass-Labs/TensorFlow-Tutorials/commits/master)
of commits to the GitHub repository.

## Requirements

These tutorials were developed on Linux using **Python 3.5** (the [Anaconda](https://www.continuum.io/downloads) distribution) and [PyCharm](https://www.jetbrains.com/pycharm/).

There are reports that Python 2.7 gives error messages with these tutorials. Please make sure you are using **Python 3.5** or later!

There are different ways of installing and running TensorFlow. This section describes how I did it
for these tutorials. You may want to do it differently and you can search the internet for instructions.

### Example Setup

After installing [Anaconda](https://www.continuum.io/downloads), you should create a [conda environment](http://conda.pydata.org/docs/using/envs.html)
so you do not destroy your main installation in case you make a mistake somewhere:

    conda create --name tf python=3

Now you can switch to the new environment by running the following (on Linux):

    source activate tf

Some of these tutorials use [scikit-learn](http://scikit-learn.org/stable/install.html)
which can be installed in your new conda environment as follows. This also installs
NumPy and other dependencies:

    conda install scikit-learn

You may also need to install other dependencies, such as:

    conda install jupyter matplotlib scipy pillow

Now you have to install TensorFlow. It is now possible to install the CPU-version of TensorFlow
directly using pip. We also need the [PrettyTensor](https://github.com/google/prettytensor)
add-on package so we install that as well:

    pip install tensorflow prettytensor

It is much more complicated to install the GPU-version because you also need various NVIDIA drivers.
That is not described here.

You should now be able to run the tutorials in the Python Notebooks:

    cd ~/development/TensorFlow-Tutorials/  # Your installation directory.
    jupyter notebook

This should start a web-browser that shows the list of tutorials. Click on a tutorial to load it.

If you are new to using Python and Linux, etc. then this may be challenging
to get working and you may need to do internet searches for error-messages, etc.
It will get easier with practice.

## License (MIT)

These tutorials and source-code are published under the [MIT License](https://github.com/Hvass-Labs/TensorFlow-Tutorials/blob/master/LICENSE)
which allows very broad use for both academic and commercial purposes.

A few of the images used for demonstration purposes may be under copyright. These images are included under the "fair usage" laws.

You are very welcome to modify these tutorials and use them in your own projects.
Please keep a link to the [original repository](https://github.com/Hvass-Labs/TensorFlow-Tutorials).

