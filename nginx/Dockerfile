FROM    ubuntu:14.04
RUN     apt-get update && apt-get install -y nginx
RUN     ln -sf /dev/stdout /var/log/nginx/access.log \
        && ln -sf /dev/stderr /var/log/nginx/error.log
EXPOSE  80
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
