### Setup
1, clone this git repository
2, Install docker and pull the data science docker image running the below commands:
```
docker pull jupyter/datascience-notebook
docker run -it --rm -p 8888:8888 jupyter/datascience-notebook
```
3, Let's move the notebook to the docker machine:
```
docker ps -a
docker cp nlp-intro.ipynb $CONTAINER_ID:/home/jovyan/work
```
4, Open the jupyter notebook in your browser and navigate to the work directory to open the jupyter notebook.
