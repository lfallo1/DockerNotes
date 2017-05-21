# this same shows how we can extend/change an existing official image from Docker Hub

FROM nginx:latest
# highly recommend you always pin versions for anything beyond dev/learn

WORKDIR /usr/share/nginx/html
# change working directory to root of nginx webhost
# using WORKDIR is prefered to using 'RUN cd /some/path'

# could be commented out and still work in dev if a volume / bind mount is specified.  but you will need to copy this file before building/deploying a container since it only exists as a shared file/dir at this point
COPY index.html index.html

# I don't have to specify EXPOSE or CMD because they're in my FROM
