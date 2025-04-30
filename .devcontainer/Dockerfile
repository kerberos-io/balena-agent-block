FROM mcr.microsoft.com/devcontainers/go:1.24-bookworm

# Install node environment
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    nodejs \
    npm \
    && rm -rf /var/lib/apt/lists/*
    
RUN wget https://github.com/balena-io/balena-cli/releases/download/v21.1.9/balena-cli-v21.1.9-linux-arm64-standalone.zip \
    && unzip balena-cli-v21.1.9-linux-arm64-standalone.zip && \
    cp /go/balena-cli/balena /usr/local/bin/balena