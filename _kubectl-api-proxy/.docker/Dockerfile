FROM nginx:1.23-alpine

COPY --chown=nginx:nginx ./nginx.conf /etc/nginx/nginx.conf
COPY --chown=nginx:nginx ./nginx-dev.crt /var/www/certs/nginx-dev.crt
COPY --chown=nginx:nginx ./nginx-dev.key /var/www/certs/nginx-dev.key
COPY --chown=nginx:nginx ./default.conf /etc/nginx/conf.d/default.conf
COPY --chown=nginx:nginx ./accounts.conf /etc/nginx/conf.d/accounts.conf
