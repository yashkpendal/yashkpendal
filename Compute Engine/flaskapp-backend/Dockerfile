# syntax=docker/dockerfile:1

FROM python:3.8

ADD app.py .

WORKDIR /app
COPY . /app
COPY requirements.txt .

RUN pip install -r requirements.txt
RUN pip3 install --upgrade pip
RUN pip3 install Flask 
RUN pip3 install --upgrade google-cloud-datastore
RUN pip3 install --upgrade google-cloud

EXPOSE 3306

CMD [ "python3", "./app.py" ]
