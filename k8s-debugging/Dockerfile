FROM ubuntu:16.04

RUN apt-get update -y && apt-get upgrade -y && apt-get install -y \
    build-essential \
    curl \
    dnsutils \
    git \
    golang \
    iputils-ping \
    vim \
    wget

# Kubectl
RUN curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl

# kuberang
RUN cd ~ && \  
    curl --silent https://kismatic-installer.s3-accelerate.amazonaws.com/kuberang/latest/kuberang-linux-amd64 --output kuberang && \
    chmod +x kuberang && \
    cp kuberang /usr/bin/




