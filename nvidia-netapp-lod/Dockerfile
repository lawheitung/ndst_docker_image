FROM nvcr.io/nvidia/nemo:v0.10

RUN pip install ansible netapp-lib netapp-ontap

RUN conda install -y -c conda-forge jupyterlab-nvdashboard && \
    conda clean -yac * && \
    jupyter labextension install jupyterlab-nvdashboard

COPY . /workspace/text_classification

# Start Jupyter up by default rather than a shell
ENTRYPOINT ["/bin/sh"]
CMD ["-c", "jupyter lab  --notebook-dir=/workspace --ip=0.0.0.0 --no-browser --allow-root --port=8888 --NotebookApp.token='' --NotebookApp.password='' --NotebookApp.allow_origin='*' --NotebookApp.base_url=${NB_PREFIX}"]

