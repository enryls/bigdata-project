FROM jupyter/pyspark-notebook

RUN mamba install --quiet --yes \
    "ipython" \
    "jupyter" \
    "jupyterlab>=3" \
    "pandas-profiling" \
    "scikit-learn" \
    "plotly::plotly" \
    "seaborn" && \
    mamba clean --all -f -y && \
    fix-permissions "${CONDA_DIR}" && \
    fix-permissions "/home/${NB_USER}"
