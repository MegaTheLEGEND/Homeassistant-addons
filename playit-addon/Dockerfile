FROM ubuntu:focal

RUN mkdir /app
WORKDIR /app

SHELL ["/bin/bash", "-o", "pipefail", "-c"]

RUN apt-get update && apt-get install -y ca-certificates

COPY . /app
RUN chmod 0755 /app/playit-x64

CMD ["/app/playit-x64"]
