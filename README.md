Script for openCV 3 installation forked from https://github.com/milq/milq/blob/master/scripts/bash/install-opencv.sh
 and modified by Hector R Arce Gonzalez in order to install contrib headers (xfeatures2d for example).


Dependencies added:
* python-vtk


OpenCv Contrib headers added:
* file source: https://github.com/opencv/opencv_contrib/archive/3.2.0.zip
* cmake option added: -DOPENCV_EXTRA_MODULES_PATH=../opencv_contrib/modules ..
