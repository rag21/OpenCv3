
features.cpp example from openCV 3 documentation: https://docs.opencv.org/3.0-beta/doc/tutorials/features2d/feature_detection/feature_detection.html


*Compile:

g++ features.cpp -o features ` pkg-config --cflags --libs opencv `


*Execute:

./features gala.jpg mandelbrot.jpg
