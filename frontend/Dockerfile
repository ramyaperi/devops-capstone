FROM nginx:alpine

## Copy our default nginx config
COPY nginx.conf /etc/nginx/nginx.conf

WORKDIR /usr/share/nginx/html
COPY ./dist/frontend ./
