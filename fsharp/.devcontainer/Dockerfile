FROM mcr.microsoft.com/dotnet/sdk:5.0

ENV SHELL /bin/bash

RUN apt-get update && \
    apt-get --no-install-recommends install -y git sudo make ssh-client

RUN useradd -m --uid 1000 --groups sudo fsharp && \
    echo "fsharp:fsharp" | chpasswd

WORKDIR /home/fsharp