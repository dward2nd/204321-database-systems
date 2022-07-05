FROM bitnami/jupyter-base-notebook:latest
USER root
RUN conda install --quiet --yes pymysql && \
    conda install --quiet --yes -c conda-forge ipython-sql && \
    conda clean --all -f -y

USER 1001
WORKDIR /var/notebooks/
CMD jupyter lab --ip 0.0.0.0 --port 8888 --no-browser --ServerApp.token=""

