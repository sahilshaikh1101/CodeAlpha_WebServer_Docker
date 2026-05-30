# 🚀 CodeAlpha Docker Web Server

## 📖 Project Description

This project demonstrates the deployment of a simple web server using Docker and Nginx on RHEL 9 Linux as part of the CodeAlpha DevOps Internship.

The objective of this project is to understand Docker containerization, image creation, container lifecycle management, port mapping, and web server deployment using Nginx.

---

## 🎯 Objectives

- Learn Docker fundamentals
- Understand containerization concepts
- Build and manage Docker images
- Deploy a web server inside a Docker container
- Understand Docker networking and port mapping
- Gain hands-on experience with DevOps tools

---

## 🛠 Technologies Used

| Technology | Purpose |
|------------|----------|
| Docker | Containerization Platform |
| Nginx | Web Server |
| HTML | Web Page |
| RHEL 9 | Operating System |
| Git | Version Control |
| GitHub | Code Repository Hosting |

---

## 📂 Project Structure

```text
CodeAlpha_WebServer_Docker/
│
├── Dockerfile
├── index.html
└── README.md
```

---

## 📄 HTML Page

The web page displays a simple success message indicating that the Docker web server is running successfully.

### Sample Output

```html
Docker Web Server Running Successfully 🚀
Created by Sahil Shaikh
```

---

## 🐳 Dockerfile

```dockerfile
FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html
```

---

## ⚙️ Implementation Steps

### Step 1: Install Docker

Docker was installed on RHEL 9 and the Docker service was started.

### Step 2: Create HTML Page

A custom HTML page was created and saved as:

```text
index.html
```

### Step 3: Create Dockerfile

A Dockerfile was created using the official Nginx image.

### Step 4: Build Docker Image

```bash
docker build -t codealpha-webserver .
```

### Step 5: Run Docker Container

```bash
docker run -d -p 8080:80 codealpha-webserver
```

### Step 6: Verify Running Container

```bash
docker ps
```

### Step 7: Access Web Server

Open browser and visit:

```text
http://localhost:8080
```

---

## 🔧 Docker Commands Used

### Build Image

```bash
docker build -t codealpha-webserver .
```

### Run Container

```bash
docker run -d -p 8080:80 codealpha-webserver
```

### List Running Containers

```bash
docker ps
```

### List All Containers

```bash
docker ps -a
```

### Stop Container

```bash
docker stop <container_id>
```

### Start Container

```bash
docker start <container_id>
```

### Remove Container

```bash
docker rm <container_id>
```

### List Images

```bash
docker images
```

---

## 🌐 Output

The deployed web server is accessible at:

```text
http://localhost:8080
```

Output displayed:

```text
Docker Web Server Running Successfully 🚀
Created by Sahil Shaikh
```

---

## 📚 Learning Outcomes

Through this project, I learned:

- Docker architecture
- Docker image creation
- Container deployment
- Port mapping
- Nginx web server deployment
- Container lifecycle management
- Linux command-line operations
- Basic DevOps workflow

---

## 🚀 Future Enhancements

- Deploy multiple containers using Docker Compose
- Add custom CSS and JavaScript
- Integrate CI/CD pipeline
- Deploy containerized applications on cloud platforms

---

