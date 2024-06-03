FROM ubuntu:22.04

ARG USERNAME=vscode
ARG USER_UID=1000
ARG USER_GID=$USER_UID

# non interactive frontend for locales
ENV DEBIAN_FRONTEND=noninteractive

# installing miktex and utils
RUN apt-get update && \
    apt-get -y install --no-install-recommends ca-certificates make git curl gzip wget perl zsh sudo

RUN apt-get -y install --no-install-recommends texlive texlive-lang-german texlive-latex-extra texlive-full 

RUN apt-get -y install python3-pygments

RUN groupadd --gid $USER_GID $USERNAME \
    && useradd --uid $USER_UID --gid $USER_GID -m $USERNAME -s /bin/bash \
    && echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME \
    && chmod 0440 /etc/sudoers.d/$USERNAME
    
USER $USERNAME