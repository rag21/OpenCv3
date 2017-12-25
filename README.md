## GENERAL INFO
Script for openCV 3 installation forked from https://github.com/milq/milq/blob/master/scripts/bash/install-opencv.sh
 and modified by Hector R Arce Gonzalez in order to install contrib headers (xfeatures2d for example).

## INSTRUCTIONS
After download add execution permission:
sudo chmod +x

Then execute WITHOUT sudo permissions as:
./install_opencv.sh
The script will ask for user password manually, this is due matlab opencv_contrib files not able to compile in sudo mode.

Finally verify the installation with the following comands:
pkg-config --libs opencv
pkg-config --cflags opencv
pkg-config --modversion opencv
The output of the last one must show "3.2.0"

## CHANGELOG
Dependencies added:
* python-vtk

OpenCv Contrib headers added:
* file source: https://github.com/opencv/opencv_contrib/archive/3.2.0.zip
* cmake option added: -DOPENCV_EXTRA_MODULES_PATH=../opencv_contrib/modules ..
