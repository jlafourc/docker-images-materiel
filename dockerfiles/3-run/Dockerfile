FROM debian:9.4

RUN apt-get update && apt-get install -y less htop
RUN ["echo", "$HOME"]
RUN echo $HOME

COPY run.sh /
RUN chmod +x /run.sh
RUN /run.sh