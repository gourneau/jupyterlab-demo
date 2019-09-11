FROM jupyter/all-spark-notebook

RUN pip install --no-cache-dir vdom==0.5

RUN conda install --quiet --yes \
    ' jupyterlab=1.1.2' \
    && \
    conda clean --all -f -y && \
    fix-permissions $CONDA_DIR && \
    fix-permissions /home/$NB_USER