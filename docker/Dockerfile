# syntax=docker/dockerfile:1

FROM quay.io/fenicsproject/stable:latest

USER root

RUN pip3 install --upgrade pip

RUN pip3 install --no-cache-dir joblib POT seaborn nbdev tqdm

RUN pip3 install --upgrade --no-cache-dir jupyter jupyterlab

EXPOSE 8888/tcp
ENV SHELL /bin/bash
ENTRYPOINT ["jupyter", "lab", "--ip", "0.0.0.0", "--no-browser", "--allow-root"]