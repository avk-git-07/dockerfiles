FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/shared/nginx/html/index.html
# This onbuild instruction will run only when any user uses this image
ONBUILD COPY index.html /usr/shared/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]