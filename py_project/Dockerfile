FROM ubuntu:16.04
MAINTAINER Naveen "email@domain.com"
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev
COPY ./requirements.txt /app/requirements.txt
WORKDIR /app
RUN pip install -r requirements.txt
COPY . /app
ENTRYPOINT ["python"]
CMD ["main.py"]
