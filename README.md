## Computer Vision Workshop - nor(DEV):con
### 28/02/2020 13:30 - 15:00  [Board Room]

Hi there,

I hope you are all excited and looking forward to the Computer Vision workshop. **Please make sure to follow the *Set up your environment* instructions before the start of the workshop**. Thank you, see you there!

### Set-up your environment
##### Please make sure to follow these instructions and get all set up **before the start fo the session**

#### Step 1 - Install Docker
Install docker. For reference see here: https://docs.docker.com/install/

#### Step 2 - Pull the Docker image
Pull [this](https://www.tensorflow.org/install/docker) docker image usings the 'latest-py3-jupyter' tag: 
docker pull tensorflow/tensorflow:latest-py3-jupyter

#### Step 3 - Git Clone this repo
git clone https://github.com/freddifederica/computer_vision_workshop.git

#### Step 4 - Run your container 
Enter the computer_vision_workshop folder and run the docker container:
docker run -it --rm --name cv_workshop_jupyter -v $PWD:/tf/local -p 8888:8888 tensorflow/tensorflow:latest-py3-jupyter bash

#### Step 5 - Install some extra requirements
sh requirements.sh

#### Step 6 - Launch the Jupyter Notebook
jupyter notebook --port=8888 --ip=0.0.0.0 --allow-root --no-browser .

check the notebook at http://localhost:8888


### Extras

Other helpful commands you might need:
docker container ls 
docker image ls
docker stop <container_name>
docker rm <container_name>

(use 'exit' or ctrl+c to exit a container bash)