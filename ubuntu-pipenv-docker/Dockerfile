
FROM ubuntu:18.04
MAINTAINER yatszhash

RUN apt-get update && \
      apt-get install -y software-properties-common curl && \
      add-apt-repository -y ppa:ubuntu-toolchain-r/ppa && \
      apt-get install -y python3.7 python3.7-dev python3-distutils && \
      python3.7 --version

RUN  curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py && \
      python3 get-pip.py && \
      pip install pipenv && \
      rm get-pip.py