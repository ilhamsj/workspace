FROM alpine:latest

RUN apk add --no-cache wget curl && \
    mkdir /app

COPY crontab.txt /app/crontab.txt

RUN crontab /app/crontab.txt

CMD ["crond", "-f", "-L", "/dev/stdout"]
