FROM ghcr.io/home-assistant/base:latest

RUN apk add --no-cache openssl && \
    rm -rf /var/cache/apk/*

RUN curl https://get.acme.sh | sh

ENV LANG C.UTF-8

COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
