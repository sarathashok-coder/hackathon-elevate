# 🐳 Dockerfile Overview

This is a brief README about the Dockerfile used to serve a static website using **NGINX**.

---

## 📄 Dockerfile Breakdown

### ✅ `FROM nginx:alpine`
Specifies the base image for the container.  
`nginx:alpine` is a lightweight version of the NGINX web server built on Alpine Linux.

---

### 📁 `COPY index.html /usr/share/nginx/html/index.html`
Copies your local `index.html` into the container’s default web root directory.  
This replaces the default NGINX welcome page with your custom website.

---

### 🚪 `EXPOSE 80`
Informs Docker that the container will listen on **port 80**, the standard HTTP port.

---

## 🚀 Result

Once built and run, your container:

- Starts an **NGINX** server
- Serves your custom `index.html`
- Listens for incoming web traffic on port `80`

---

## 🛠️ Quick Usage

# Build the Docker image
docker build -t my-nginx-app .

# Run the container
docker run -p 8080:80 my-nginx-app
