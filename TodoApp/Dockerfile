FROM node:lts-alpine
RUN adduser --disabled-password -u 5000 todoapp \
    && mkdir /todoapp
WORKDIR /todoapp
COPY package.*json ./
RUN npm install
COPY . .
RUN chown -R todoapp:todoapp /todoapp
USER todoapp
COPY ./ ./














