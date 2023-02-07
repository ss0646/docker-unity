FROM ubuntu:18.04

RUN set -eux \
    && apt update \
    && apt install -y sudo wget \
    && sudo sh -c 'echo "deb https://hub.unity3d.com/linux/repos/deb stable main" > /etc/apt/sources.list.d/unityhub.list' \
    && wget -qO - https://hub.unity3d.com/linux/keys/public | sudo apt-key add - \
    && apt update \
    && apt install -y unityhub