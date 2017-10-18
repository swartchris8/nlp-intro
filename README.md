Install docker and clone the repo then run the below commands:
```
docker pull jupyter/datascience-notebook
docker run -it --rm -p 8888:8888 jupyter/datascience-notebook
docker ps -a
docker cp nlp-intro.ipynb $CONTAINER_ID:/home/jovyan/work
```
