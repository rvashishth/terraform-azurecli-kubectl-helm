FROM alpinelinux/docker-cli

ENV AZURE_CLI_VERSION 2.7.0
ENV HELM_VERSION v3.0.3

# Install needed packages and Azure CLI
RUN apk add \
    python3 \
    py3-pip \
    curl \ 
    git \
    jq \
    gettext && \
    apk add --virtual .build-deps \
    gcc \
    libffi-dev \
    musl-dev \
    openssl-dev \
    make \
    python3-dev \
    linux-headers && \
    pip3 install --no-cache-dir --upgrade pip && \
    pip3 install --no-cache-dir azure-cli==$AZURE_CLI_VERSION && \
    apk del .build-deps && \
    rm -rf /var/cache/apk/*

# Install Helm
RUN curl https://get.helm.sh/helm-${HELM_VERSION}-linux-amd64.tar.gz | tar -xzO linux-amd64/helm > /usr/local/bin/helm && \
    chmod +x /usr/local/bin/helm
