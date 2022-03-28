# syntax=docker/dockerfile:1

FROM nginx
COPY templates/index.html /usr/share/nginx/html

ADD templates/index.html .

WORKDIR /templates/index.html
COPY . /index
COPY requirements.txt .

EXPOSE 8081