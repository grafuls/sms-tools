sms-tools
========= 

Sound analysis/synthesis tools for music applications written in python (with a bit of C) plus complementary lecture materials.

How to use
----------

In order to use these tools you have to install version 2.7.* of python and the following modules: ipython, numpy, matplotlib, scipy, pygame, and cython. 

In Ubuntu (which we strongly recommend) in order to install all these modules it is as simple as typing in the Terminal:

<code>$ sudo apt-get install python-dev ipython python-numpy python-matplotlib python-scipy python-pygame cython</code>

In Mac OS:

<code>$ sudo pip install ipython numpy matplotlib scipy cython</code>

<code>$ sudo port install libsdl-framework</code>

<code>$ sudo port install libsdl_ttf-framework</code>

<code>$ sudo port install libsdl_image-framework</code>

<code>$ sudo port install libsdl_mixer-framework</code>

<code>$ sudo port install mercurial</code>

<code>$ sudo pip install hg+http://bitbucket.org/pygame/pygame</code>

Note: for Mac OS the python-dev package would be satisfied with the installation of python 2.7.*

then for using the tools, after downloading the whole package, you need to compile some C functions. For that you should go to the directory <code>software/models/utilFunctions_C</code> and type:</p>

<code>$ python compileModule.py build_ext --inplace </code>

The basic sound analysis/synthesis functions, or models, are in the directory <code>software/models</code> and there is a graphical interface and individual example functions in <code>software/models_interface</code>. To execute the models GUI you have to go to the directory <code>software/models_interface</code> and type: 

<code>$ python models_GUI.py </code>

To execute the transformations GUI that calls various sound transformation functions go to the directory <code>software/transformations_interface</code> and type: 

<code>$ python transformations_GUI.py </code>

To modify the existing code, or to create your own using some of the functions, we recommend to use the <code>workspace</code> directory. Typically you would copy a file from <code>software/models_interface</code> or from <code>software/transformations_interface</code> to that directory, modify the code, and execute it from there (you will have to change some of the paths inside the files). 


Content
-------

All the code is in the <code> software </code> directory, with subdirectories for the models, the transformations, and the interfaces. The lecture material is in the <code>lecture</code> directory and the sounds used for the examples and coming from <code>http://freesound.org</code> are in the <code>sounds</code> directory.

License
-------
All the software is distributed with the Affero GPL licence, and the lecture slides and sounds are distributed with the Creative Commons Attribution-Noncommercial-Share Alike license.

