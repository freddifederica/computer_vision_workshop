## Computer Vision Workshop - nor(DEV):con
#### 13:30 - 15:00 28/02/2020 [Board Room]

Hi there,

I hope you are all excited and looking forward to the Computer Vision workshop. I will give here a brief summary of the topics I am going to speak about, hoping that this will help you decide if you are interested in attending the session. If you do decide that you would like to attend, **please make sure to follow the *Set up your environment* introductions before the start of the workshop**. Thank you!

### What is Computer Vision?

With this session I am hoping to introduce you to some of the wonders and magic of Depp-learning based computer vision approaches.


### Workshop Summary



### Set-up your environment
##### Please make sure to follow these instructions and get all set up **before the start fo the session**

Install docker
https://docs.docker.com/install/
https://www.linux.com/tutorials/how-install-and-use-docker-linux/

Pull this [https://www.tensorflow.org/install/docker] docker image usings the 'latest-jupyter' tag.
You can use the following command:
docker pull tensorflow/tensorflow:latest-jupyter

When the download is completed, you can use the following command to access the bash:
docker run -it --name cv_workshop_jupyter -p 8888:8888 tensorflow/tensorflow:latest-jupyter bash

Other helpful commands you might need:
docker container ls 
docker image ls
docker stop <container_name>
docker rm <container_name>

(use 'exit' or ctrl+c to exit a container bash)

Start your docker and launch your jupyter notebook
docker run -it --rm --name cv_workshop_jupyter -v $PWD:/tf/local -p 8888:8888 tensorflow/tensorflow:latest-jupyter