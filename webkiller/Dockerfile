FROM python:3.9.18-slim-bullseye

WORKDIR /app

ADD requirments.txt .

RUN pip3 install -r requirments.txt

ADD . .

ENTRYPOINT [ "python3", "webkiller.py" ]
