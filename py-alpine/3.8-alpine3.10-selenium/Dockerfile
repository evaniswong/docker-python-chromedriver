FROM python:3.8-alpine3.10

# install chromedriver
RUN echo "http://dl-4.alpinelinux.org/alpine/v3.10/main" >> /etc/apk/repositories && \	
    echo "http://dl-4.alpinelinux.org/alpine/v3.10/community" >> /etc/apk/repositories


# upgrade pip
RUN pip install --upgrade pip && pip install selenium bs4 requests

COPY ./docker_web_func.py /

WORKDIR /

ENTRYPOINT ["python","cloud_web_func.py"]


