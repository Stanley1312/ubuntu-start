# 1.CUDA Installtion 
* Go to https: [https://developer.nvidia.com/cuda-downloads](https://developer.nvidia.com/cuda-downloads)
* Select the target platform based on your OS setting.
* I chose to use runfile (local) for installation. There will be installation instructions to follow. My instruction at this moment is:
```
wget http://developer.download.nvidia.com/compute/cuda/10.2/Prod/local_installers/cuda_10.2.89_440.33.01_linux.run
```
* After downloading, run the second script. (If you have installed an updated GPU driver, you can uncheck to not install the driver during the installation.)
```
sudo sh cuda_10.2.89_440.33.01_linux.run
```
* Then, edit the ~/.bashrc.
```
sudo gedit ~/.bashrc

```
* Add the following to the end of file:
```
export PATH=/usr/local/cuda/bin:$PATH 

export LD_LIBRARY_PATH=/usr/local/cuda/lib64:$LD_LIBRARY_PATH
```
* Run the ~/.bashrc again.
```
source /.bashrc
```

# 2.CUDNN Installation.
* Go to login and download cuDNN v7.6.5 for CUDA v10.2. There are 3 deb files. That’s it.
```
sudo dpkg -i libcudnn7_7.6.5.32-1+cuda10.2_amd64.deb
sudo dpkg -i libcudnn7-dev_7.6.5.32-1+cuda10.2_amd64.deb
sudo dpkg -i libcudnn7-doc_7.6.5.32-1+cuda10.2_amd64.deb
```
* To verify, copy the sample files to :
```
cp -r /usr/src/cudnn_samples_v7/ ~
```
* Then change the directory:
```
cd ~/cudnn_samples_v7/mnistCUDNN
```
* Make file:
```
make clean && make 
```
* If failed to install, it should not able to make. One of the solutions is to edit cudnn.h:
```
sudo gedit  /usr/include/cudnn.h./mnistCUDNN

```
* Change #include “driver_types.h” to #include <driver_types.h>.
* Then try to make again:
```
make clean && make 
```
* If successful to install:
* If this step has any error, **Restart !!**
```
./mnistCUDNN
```
* There will be classification results, and say:
```
Test passed!
```
### If you have another version of cuda in your computer, try install cuda in the same way above but install cudnn follow this way

* Dowload CuDNN tar file in NVIDIA website https://developer.nvidia.com/cudnn and unzip this file 
```
tar -xzvf {CUDNN_TAR_FILE_NAME}
```
### Copy the following files into the cuda toolkit directory.
```
sudo cp -P cuda/include/cudnn.h /usr/local/cuda-9.0/include
sudo cp -P cuda/lib64/libcudnn* /usr/local/cuda-9.0/lib64/
sudo chmod a+r /usr/local/cuda-9.0/lib64/libcudnn*
```

# REF 
* [Tutorial: CUDA v10.2 + CUDNN v7.6.5 Installation @ Ubuntu 18.04](https://sh-tsang.medium.com/tutorial-cuda-v10-2-cudnn-v7-6-5-installation-ubuntu-18-04-3d24c157473f)
* [Cuda 9.0 complete installation procedure for ubuntu 18.04 LTS ](https://gist.github.com/andyweizhao/639e94b60c166f57964aafedeb465e90)
