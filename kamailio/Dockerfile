FROM alpine:3.10
LABEL maintainer="Michael Walton"
WORKDIR /root/

RUN apk update \
  && apk add kamailio kamailio-redis kamailio-tls kamailio-db kamailio-json

COPY etc /etc/

EXPOSE 5061
CMD ["kamailio","-DD","-E"]
