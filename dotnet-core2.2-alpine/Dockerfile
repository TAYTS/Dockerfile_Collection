FROM microsoft/dotnet:2.2-sdk-alpine

RUN apk update && apk add ca-certificates && \
    rm -rf /var/cache/apk/*

# COPY CA cert
COPY ./sample.crt /usr/local/share/ca-certificates/custom.cert

RUN update-ca-certificates
