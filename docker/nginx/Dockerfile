FROM nginx:stable

ARG DEV_DOMAIN
ADD san.txt /opt/san.txt
ADD ssl-setup.sh /opt/ssl-setup.sh
RUN chmod a+x /opt/ssl-setup.sh
RUN /bin/bash -c "source /opt/ssl-setup.sh /etc/nginx/ssl ${DEV_DOMAIN}"
