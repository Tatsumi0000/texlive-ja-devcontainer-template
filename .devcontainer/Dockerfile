FROM ghcr.io/tatsumi0000/texlive-ja-devcontainer-template/texlive-ja:latest

RUN apt update && apt upgrade -y && apt install -y \
    git \
    cpanminus \
    texlive-extra-utils \
    python3-pip \
    python3-pygments \
    make \
    && apt clean \
    && rm -rf /var/lib/apt/lists/*

RUN cpanm Log::Log4perl Log::Dispatch::File YAML::Tiny File::HomeDir Unicode::GCString