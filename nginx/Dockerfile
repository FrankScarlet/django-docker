# 如果不做https
# 用Dockerfile.dev
# 否则Dockerfile.prod
FROM nginx:1.19-alpine

RUN rm /etc/nginx/conf.d/default.conf
# 80 default rewrite
COPY default.conf /etc/nginx/conf.d 
# 443
COPY nginx.conf /etc/nginx/conf.d
COPY scarlet.pro.key /etc/nginx/cert/
COPY scarlet.pro.pem /etc/nginx/cert/
