FROM ubuntu:latest

RUN apt-get update
RUN apt-get install -y python python-pip wget
RUN pip install Flask

ADD hello.py /home/hello.py
EXPOSE 5000
WORKDIR /home
ENTRYPOINT ["nohup", "/usr/bin/python","/home/hello.py", "&"]
