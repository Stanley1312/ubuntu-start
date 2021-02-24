# NVIDIA_SMI BUGS:

### BUG LOG:
![alt text](https://github.com/Stanley1312/install_opencv_cuda/blob/master/nvidia-bug.png)

### SOLUTION 
If you have tried all the links on google but still cannot fix it, try this command line:
```
sudo apt-get install --reinstall linux-headers-$(uname -r)
#check again
nvidia-smi
```
