FROM python:3
USER root
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install --no-install-recommends -y \
    curl \
    && apt-get clean \
    &&  rm -rf /var/lib/apt/lists/*

RUN python3 -m pip install --upgrade pip \
    && pip install --no-cache-dir\ 
    numpy \
    scipy \
    selenium \
    matplotlib \
    japanize-matplotlib \
    ipython \
    scikit-learn \
    pandas \
    pillow \
    mglearn \
    requests \
    pyperclip \
    beautifulsoup4

RUN pip install --upgrade --no-cache-dir \
    jupyterlab \
    jupyterlab_code_formatter