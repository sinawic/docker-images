FROM python:3.9.18-slim-bullseye

ENV VERSION=2.0.0

RUN apt update && apt install wget -y

WORKDIR /app

RUN wget https://github.com/iojw/socialscan/archive/refs/tags/v${VERSION}.tar.gz

RUN tar -zxvf v$VERSION.tar.gz

WORKDIR /app/socialscan-$VERSION

RUN pip install .

ENTRYPOINT [ "socialscan" ]
