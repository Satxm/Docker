FROM ubuntu
RUN rm /etc/apt/sources.list
RUN ln -s /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
ADD sources.list /etc/apt/sources.list
RUN apt-get update && apt-get install -y openjdk-8-jre
EXPOSE 25565/tcp
VOLUME /mcserver
WORKDIR /mcserver
CMD /mcserver/start.sh
