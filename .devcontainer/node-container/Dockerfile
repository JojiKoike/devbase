FROM mcr.microsoft.com/devcontainers/javascript-node:0-20

WORKDIR /opt

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    ca-certificates \
    curl pre-commit

ENV HOST 0.0.0.0
EXPOSE 3000

RUN git config --global --add safe.directory /workspace
