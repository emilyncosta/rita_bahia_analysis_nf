FROM continuumio/miniconda:4.7.10

MAINTAINER Abhinav Sharma <abhi18av@outlook.com>

RUN apt-get update -y && apt-get install -y \
    procps

COPY conda.yml .

RUN conda env update -n root -f conda.yml && conda clean -a

RUN git clone https://github.com/xiaeryu/SpoTyping-v2.0 

WORKDIR /SpoTyping-v2.0/SpoTyping-v2.0-commandLine/
