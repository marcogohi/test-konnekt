FROM alpine:3.12

LABEL MAINTAINER "Marco GH <marco.gonzalez@ikerlan.es>"
LABEL APP "MQTT Client"

RUN apk add --no-cache mosquitto-clients ca-certificates && \
    /etc/ca-certificates/update.d/certhash && \
    ln -s /usr/bin/mosquitto_pub /usr/local/bin/pub && \
    ln -s /usr/bin/mosquitto_sub /usr/local/bin/sub

USER nobody
