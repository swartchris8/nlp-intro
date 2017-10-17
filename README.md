
docker pull jupyter/datascience-notebook
docker run -it --rm -p 8888:8888 jupyter/datascience-notebook
docker cp nlp-intro.ipynb $CONTAINER_ID:/home/jovyan/work
