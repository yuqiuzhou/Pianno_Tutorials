.. Pianno documentation master file, created by
   sphinx-quickstart.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Installation
============

Python Dependencies
---------------------
The following dependencies will be installed along with pianno.
.. code-block:: python

   anndata==0.8.0
   scanpy==1.9.1
   squidpy==1.2.2
   opencv-python==4.5.5.64
   rpy2==3.4.5
   scikit-image==0.19.2
   scikit-learn==1.0.2
   scipy==1.8.0
   protobuf==3.20.3
   numpy==1.19.5
   keras==2.6.0
   nni==2.5
   

R Dependencies
---------------------
.. code-block:: r

   r-scran==1.28.2
   r-saver==1.1.2

Pianno uses the R packages `SAVER` and `scran` in preprocessing for noise reduction and size factor calculation, respectively. These two R packages will be automatically installed during the corresponding analysis in Pianno.


Installation
------------
Downloading Pianno code from https://github.com/yuqiuzhou/Pianno

.. code-block:: python

   # create an environment called Pianno
   conda create -n Pianno python=3.9.10

   # activate your environment
   conda activate Pianno

   # install R in the Pianno environment
   conda install -c conda-forge r-base=4.1.1

   # install tensorflow and tensorflow-probability
   # ensure the version 2 of tensorflow
   pip install tensorflow-gpu==2.6.0
   pip install tensorflow-probability==0.14.0

   # install pianno from PyPi
   pip install pianno

.. code-block:: python

   import pianno as po
   
   
