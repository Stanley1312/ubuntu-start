# 1.CUDA installtion 
* Go to https: [link](https://developer.nvidia.com/cuda-downloads"https://developer.nvidia.com/cuda-downloads")
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
