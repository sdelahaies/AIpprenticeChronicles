Episode II: the Attack of the YOLOv5

here we choose to work with YOLOv5 with a docker container, to pull the image and start a container use the following command from the `AIpprenticeChronicles` folder
```
t=ultralytics/yolov5:latest && docker pull $t && docker run -it --ipc=host --gpus all -p 8888:8888 -v $PWD:/usr/src/app/AIpprenticeChronicles $t
```
then start jupyter from the container using the command
```
jupyter notebook --ip 0.0.0.0 --port=8888 --allow-root
```
and open the notebook `AIpprentice_chronicles_episode2.ipynb`.