### Setup

#### Setup with docker

1, clone this git repository
2, Install docker and pull the data science docker image running the below commands:
```
docker pull jupyter/datascience-notebook
docker run -it --rm -p 8888:8888 jupyter/datascience-notebook
```
3, Let's move this repo's content to the docker machine:
```
docker ps -a
docker cp . $CONTAINER_ID:/home/jovyan/work
```
4, Open the jupyter notebook in your browser and navigate to the work directory to open the jupyter notebook.

#### Setup with Python

Install requirements.txt on a Python 3.6 environment.

### Troubleshooting

If your Jupyter Notebook requires a token. Stop the image and rerun the docker setup.

### Clean up docker env


1, Delete all containers:
```
docker rm $(docker ps -a -q)
```

2, If you would like to delete all images:
```
docker rmi $(docker images -q)
```
