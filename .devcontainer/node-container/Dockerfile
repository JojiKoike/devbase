FROM node:20.15.0-bookworm-slim as builder

WORKDIR /opt

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    ca-certificates \
    curl git pre-commit openssl

ENV HOST 0.0.0.0
EXPOSE 3000

RUN git config --global --add safe.directory /workspace
