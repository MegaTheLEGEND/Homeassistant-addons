ARG BUILD_FROM=ghcr.io/home-assistant/aarch64-base:3.13
FROM $BUILD_FROM

RUN mkdir /app
WORKDIR /app

RUN apt-get update && apt-get install -y \
    ca-certificates

COPY . /app
RUN chmod 0755 /app/playit-x64

CMD ["/app/playit-x64"]
