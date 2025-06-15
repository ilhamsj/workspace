FROM nginx:latest

WORKDIR /etc/nginx

COPY nginx.conf /etc/nginx/nginx.conf

COPY conf.d /etc/nginx/conf.d

EXPOSE 443

CMD ["nginx", "-g", "daemon off;"]