# INSTALL OPENCV_CUDA ON LINUX 
This repository will guide you how to install opencv with cuda support 
### Required sofwares to install opencv_cuda
* <strong>CUDA Toolkit</strong> 

* <strong>cuDNN</strong>

* <strong>GCC, G++</strong>

To check the sofware's installation above:
```
nvcc --version #for CUDA
gcc --version #for GCC
g++ --version #for G++

```

### Tutorials are referenced in this blog : https://www.pyimagesearch.com/2020/02/03/how-to-use-opencvs-dnn-module-with-nvidia-gpus-cuda-and-cudnn/

### So in this repository i will focus on a few bugs during the installation process:
## STEP #4  
Maybe in step4 when you installed the virtialenv, the path of <strong> source /usr/local/bin/virtualenvwrapper.sh </strong> is wrong
![alt text](https://github.com/Stanley1312/install_opencv_cuda/blob/master/step4.png?raw=true)

So to point out the correct path of <strong>virtualenvwrapper.sh</strong> file on your computer, use this linux command line below:
```
find / -name virtualenvwrapper.sh
```
The result in my computer:

![alt text](https://github.com/Stanley1312/install_opencv_cuda/blob/master/find_step4.png?raw=true)

Finally, replace the correct path in your computer in <strong>~/.bashrc</strong> file 

## STEP #6 

Before implementing this step you must check the gcc version on your computer by a fews command lines:
``` 
gcc --version
g++ --version
``` 
This will be okay if your gcc version <= 8.0, if your version is higher than 8.0 follow these steps to lower your version of gcc complier
Install your lower gcc version, i will install the gcc and g++ 7.0:
``` 
sudo apt install build-essential
sudo apt -y install gcc-7 g++-7
``` 
Use the <strong>update-alternatives</strong> tool to create list of multiple GCC and G++ compiler alternatives:
``` 
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-7 7
sudo update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-7 7
``` 
After that you can check again with the first two lines of code  
