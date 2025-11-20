FROM almalinux:9
RUN dnf install nginx -y
CMD ["nginx", "-g", "daemon off;"]

# Explanation:
# CMD: This Dockerfile instruction defines the default command or parameters for an executable container.
# ["nginx", "-g", "daemon off;"]: This is the command in exec form.
# nginx: This is the executable for the NGINX server.
# -g "daemon off;": This argument tells NGINX to run in the foreground, disabling the daemon mode. This is essential for Docker containers, as a container will stop if its main process exits. By running NGINX in the foreground, the container remains active as long as NGINX is running.