FROM alpine:latest

RUN apk update && apk add mysql-client
RUN mkdir -p /opt

WORKDIR /opt

COPY import.sh /opt
COPY mydatabase.sql /opt

RUN chmod +x /opt/import.sh

EXPOSE 3306

CMD /opt/import.sh
