# wxwidgets-template
This is a wxwidgets starter template setup with CMake.

I took the code from [Hello world](https://docs.wxwidgets.org/3.2/overview_helloworld.html) example on the wxWidgets website.

To compile, please run
```
mkdir build
cd build
cmake ..
make
./hello
```
First-time compilation could take a while since I've configured it to build static lib.

You can configure the file name and so on by chaning the configs in `CMakeLists.txt`
