# Install from a package
1. Go to https://download.docker.com/linux/ubuntu/dists/, choose your Ubuntu version, 
then browse to pool/stable/, choose amd64, armhf, or arm64, and download the .deb file for the Docker Engine version you want to install.
### NOTE: Dowload three .deb files such as ce, cli, ci...
2. Install Docker Engine, changing the path below to the path where you downloaded the Docker package.
```
sudo dpkg -i /path/to/package.deb
```
The Docker daemon starts automatically
3. Verify that Docker Engine is installed correctly by running the **hello-world** image.
```
sudo docker run hello-world
```
This command downloads a test image and runs it in a container. When the container runs, it prints an informational message and exits.

# REF 
* [Install docker on linux](https://docs.docker.com/engine/install/ubuntu/)
