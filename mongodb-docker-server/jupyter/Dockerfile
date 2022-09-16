FROM bitnami/jupyter-base-notebook:latest

USER 1001
WORKDIR /var/notebooks/
ENTRYPOINT jupyter lab --ip 0.0.0.0 --port 8888 --no-browser \
               --ServerApp.token=""

