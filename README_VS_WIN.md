Steps to setup the matplotlib-cpp for VS2022 (should also work VS2019, VS2017) for WIN

1) clone the this repo
2) install the latest python (https://www.python.org/downloads/), for example, here is the patch for my installation C:\Users\yudan\AppData\Local\Programs\Python\Python310\
3) install numpy => pip install numpy
4) add python and numpy path to your VS project 

C:\Users\yudan\AppData\Local\Programs\Python\Python310\Lib\site-packages\numpy\core\include;C:\Users\yudan\AppData\Local\Programs\Python\Python310\include;

5) add python310.lib in the path and dependencies, note this only works for release build, need to find the python310_d.lib for debug version

6) build the project

You can just modify the matplotlib-cpp.vcxproj in the examples folder

