FROM ubuntu:latest

RUN apt update
RUN apt install -y git make cmake gcc-arm-none-eabi libnewlib-arm-none-eabi build-essential

COPY build.sh build_pioasm/
RUN "$WORKDIR/build_pioasm/build.sh"
ENV PIOASM="/pioasm"
