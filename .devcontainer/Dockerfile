FROM mcr.microsoft.com/devcontainers/cpp:1-ubuntu-24.04

# [Optional] Uncomment this section to install additional packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>

RUN export DEBIAN_FRONTEND=noninteractive && \
    apt-get update && \
    apt-get -y upgrade && \
    apt-get -y install g++-14

RUN update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-14 255 && \
    update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-14 255 && \
    update-alternatives --install /usr/bin/cc cc /usr/bin/gcc 255 && \
    update-alternatives --install /usr/bin/c++ c++ /usr/bin/g++ 255