# pull official base image
FROM python:3.8.15-alpine

RUN apk update && apk add python3-dev gcc libc-dev libpq-dev libevent-dev libffi-dev

WORKDIR /app

RUN pip install --upgrade pip
ADD ./requirements.txt /app/

RUN pip install -U channels["daphne"]
RUN pip install -r requirements.txt



