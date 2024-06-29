FROM mcr.microsoft.com/devcontainers/go:1-1.22-bookworm

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        ca-certificates \
        curl

RUN go install github.com/cweill/gotests/gotests@latest
RUN go install github.com/josharian/impl@latest
RUN go install github.com/go-delve/delve/cmd/dlv@latest
RUN go install honnef.co/go/tools/cmd/staticcheck@latest
RUN go install golang.org/x/tools/gopls@latest

RUN git config --global --add safe.directory /workspace
