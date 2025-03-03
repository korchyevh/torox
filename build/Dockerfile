FROM alpine:3.21.3
RUN apk --update --no-cache add tor torsocks

RUN echo 'SocksPort 0.0.0.0:9050' > /etc/tor/torrc

EXPOSE 9050
EXPOSE 9049

CMD [ "/usr/bin/tor", "-f", "/etc/tor/torrc" ]