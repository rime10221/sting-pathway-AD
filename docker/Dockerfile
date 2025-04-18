FROM condaforge/mambaforge:23.11.0-0 
RUN mamba install -y python=3.11 jupyterlab numpy pandas scipy scikit-learn \
    statsmodels seaborn plotly r-base=4.3 r-irkernel r-lavaan git-lfs dvc && \
    mamba clean -afy
EXPOSE 8888
CMD ["jupyter","lab","--ip=0.0.0.0","--no-browser","--allow-root"]
