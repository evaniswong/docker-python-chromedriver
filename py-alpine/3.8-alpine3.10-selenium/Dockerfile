FROM python:3.8-alpine3.10

# install chromedriver
RUN apk update && apk add chromium chromium-chromedriver

# upgrade pip
RUN pip install --upgrade pip && pip install selenium bs4 requests

COPY ./docker_web_func.py /

WORKDIR /

ENTRYPOINT ["python","cloud_web_func.py"]


