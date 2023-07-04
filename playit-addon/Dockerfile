FROM ubuntu:focal

RUN mkdir /app
WORKDIR /app

SHELL ["/bin/bash", "-o", "pipefail", "-c"]

RUN apt-get update && apt-get install -y ca-certificates

# Define a volume for persistent storage
VOLUME ["/data"]

COPY . /app
RUN chmod 0755 /app/playit-0.9.3

CMD ["/app/playit-0.9.3"]
