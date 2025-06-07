FROM nginx:latest

COPY nginx.conf /etc/nginx/nginx.conf

COPY conf.d /etc/nginx/conf.d
COPY web /etc/nginx/web
COPY includes /etc/nginx/includes

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]