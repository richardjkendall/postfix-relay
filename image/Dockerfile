FROM alpine:latest

RUN apk add --no-cache postfix cyrus-sasl-login rsyslog supervisor \
    && /usr/bin/newaliases

COPY . /

EXPOSE 25

ENTRYPOINT [ "/tx-smtp-relay.sh" ]

