FROM node:lts-alpine

RUN apk update && \
    apk upgrade && \
    apk add --nocache --update coreutils tzdata curl unzip git openssl nss ca-certificates && \
    rm -rf /var/cache/apk/* && \
    update-ca-certificates && \
    git config --global --add safe.directory /workspaces/browser-extension-examples && \
    npm install --global web-ext
