FROM bitnami/jupyter-base-notebook:latest
USER root

# install mongosh
RUN apt-get update -y && apt-get install gnupg wget -y
RUN wget -qO - https://www.mongodb.org/static/pgp/server-6.0.asc | apt-key add -
RUN echo "deb http://repo.mongodb.org/apt/debian buster/mongodb-org/6.0 main" | tee 
RUN apt-get update -y && apt-get install -y mongodb-org

RUN conda install --quiet --yes pymongo && \
    conda clean --all -f -y

USER 1001
WORKDIR /var/notebooks/
ENTRYPOINT jupyter lab --ip 0.0.0.0 --port 8888 --no-browser \
               --ServerApp.token=""

