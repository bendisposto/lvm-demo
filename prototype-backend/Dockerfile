FROM node:6.9.1-alpine
RUN apk update && apk upgrade
RUN apk add git curl openssh
RUN rm -rf /var/cache/apk/*
RUN git clone https://github.com/LVM-IT/prototype-backend.git
RUN cd prototype-backend && npm install
CMD cd prototype-backend && npm run start
EXPOSE 8080