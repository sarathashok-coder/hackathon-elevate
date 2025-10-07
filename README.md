This is a breif note on the docker file:

**FROM nginx:alpine** selects the docker container need to run

**COPY index.html /usr/share/nginx/html/index.html** copies the index.html to the html path in docker env to host the website

**EXPOSE 80** will open port no 80 in the container.

