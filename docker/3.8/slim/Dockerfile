FROM python:3.8-slim

RUN apt-get update \
    && apt-get install -y gcc make libssl-dev

RUN pip --no-cache-dir install cadctap

RUN apt-get remove -y gcc make \
    && apt-get clean \
    && apt-get autoclean \
    && rm -rf /var/lib/apt/lists/*
