FROM php:7.4

ENV PORT=8080

WORKDIR /app

COPY ./html .
COPY ./scripts ./scripts

EXPOSE ${PORT}

ENTRYPOINT ["sh", "./scripts/docker-entrypoint.sh"]