FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
RUN echo "Before onbuild"
ONBUILD copy index.html /usr/share/nginx/html/index.html
RUN echo "AFter onbuild"
CMD ["nginx", "-g", "daemon off;"]