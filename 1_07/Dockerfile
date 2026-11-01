FROM ubuntu:24.04
RUN apt-get update
RUN apt-get install -y curl
COPY script.sh .
ENTRYPOINT ["./script.sh"] 