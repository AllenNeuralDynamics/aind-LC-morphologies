# hash:sha256:d8086a476a34180e3e6f96fd77c8e10a7d720b7e118c95c76c4c5dffd7d57efe
ARG REGISTRY_HOST
FROM $REGISTRY_HOST/codeocean/mambaforge3:23.1.0-4-python3.10.12-ubuntu22.04

ARG DEBIAN_FRONTEND=noninteractive
ARG GIT_ASKPASS
COPY git-ask-pass /

RUN conda install -y \
        hdbscan==0.8.33 \
        jupyterlab==4.0.9 \
        k3d==2.16.0 \
    && conda clean -ya

RUN pip3 install -U --no-cache-dir \
    ccf-streamlines==1.1.4 \
    lc-reconstruction-analysis==0.0.34 \
    matplotlib==3.8.2 \
    networkx==3.2.1 \
    numpy==1.26.2 \
    pandas==2.1.3 \
    scikit-learn==1.3.2 \
    scipy==1.11.4 \
    seaborn==0.13.0 \
    tqdm==4.66.1 \
    umap-learn==0.5.5

COPY postInstall /
RUN --mount=type=secret,id=secrets . /run/secrets/secrets \
    && /postInstall
