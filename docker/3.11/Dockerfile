FROM python:3.11-slim AS build

RUN apt-get update \
    && apt-get install -y gcc make libssl-dev

RUN pip --no-cache-dir install cadctap

FROM python:3.11-slim

COPY --from=build /usr/local/ /usr/local/
