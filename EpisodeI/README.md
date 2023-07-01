# Episode I: the Tensor Force Awakens

This notebook runs smoothly on a docker image (latest 06/2023) of tensorflow with jupyter and gpu support, the container is launched using the command
```
docker run --gpus all -it -v $PWD:/tf -w /tf -p 8888:8888 tensorflow/tensorflow:latest-gpu-jupyter
``` 
To run without docker please refer to the `requirements.txt` file for exact packages versions. 