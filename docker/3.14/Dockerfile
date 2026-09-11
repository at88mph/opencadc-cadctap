FROM python:3.14-slim AS build

RUN apt update \
    && apt install -y gcc make libssl-dev

RUN pip --no-cache-dir install cadctap

FROM python:3.14-slim

COPY --from=build /usr/local/ /usr/local/

CMD ["cadc-tap"]
