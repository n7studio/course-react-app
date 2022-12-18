FROM node:lts
ARG TIMEZONE
ARG NODE_ENV 

ENV NODE_ENV ${NODE_ENV}

RUN mkdir -p /var/www/react
WORKDIR /var/www/react
COPY ./entrypoint.sh /usr/local/bin
RUN chmod +x /usr/local/bin/entrypoint.sh

ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]

