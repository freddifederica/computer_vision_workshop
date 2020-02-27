## Computer Vision Workshop - nor(DEV):con
### 28/02/2020 13:30 - 15:00  [Board Room]

Hi there,

I hope you are all excited and looking forward to the Computer Vision workshop. **Please make sure to follow the *Set up your environment* instructions before the start of the workshop**. Thank you, see you there!

### Set-up your environment

#### Step 1 - Install Docker
Install docker. For reference see here: https://docs.docker.com/install/

#### Step 2 - Pull the Docker image
Pull [this](https://www.tensorflow.org/install/docker) docker image usings the 'latest-py3-jupyter' tag: 
```console
$ docker pull tensorflow/tensorflow:latest-py3-jupyter
```

#### Step 3 - Git Clone this repo
```console
$ git clone https://github.com/freddifederica/computer_vision_workshop.git
```

#### Step 4 - Run your container 
Enter the computer_vision_workshop folder and run the docker container:
```console
$ docker run -it --rm --name cv_workshop_jupyter -v $PWD:/tf/local -p 8888:8888 tensorflow/tensorflow:latest-py3-jupyter bash
```

#### Step 5 - Install some extra requirements
```console
$ sh requirements.sh
```

#### Step 6 - Launch the Jupyter Notebook
```console
$ jupyter notebook --port=8888 --ip=0.0.0.0 --allow-root --no-browser .
```

check the notebook at http://localhost:8888


### Extras

Other helpful commands you might need:<br/>
docker container ls <br/>
docker image ls <br/>
docker stop <container_name> <br/>
docker rm <container_name> <br/>

(use 'exit' or ctrl+c to exit a container bash)