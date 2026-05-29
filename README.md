# 🐳 Docker-Frontend-app

A lightweight, containerized static frontend application served with Docker and Docker Compose.

---

## 📁 Project Structure

```
Docker-Frontend-app/
├── Dockerfile          # Docker image definition
├── docker-compose.yml  # Multi-container orchestration config
└── index.html          # Static frontend entry point
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/) (v20.10+)
- [Docker Compose](https://docs.docker.com/compose/install/) (v2.0+)

### Running the App

1. **Clone the repository:**

   ```bash
   git clone https://github.com/<your-username>/Docker-Frontend-app.git
   cd Docker-Frontend-app
   ```

2. **Build and start the container:**

   ```bash
   docker compose up --build
   ```

3. **Open your browser and visit:**

   ```
   http://localhost:<port>
   ```

   > Replace `<port>` with the port defined in your `docker-compose.yml`.

### Stopping the App

```bash
docker compose down
```

---

## 🐋 Docker Details

### Dockerfile

The `Dockerfile` defines the image used to serve the static frontend. It typically:
- Uses a lightweight web server base image (e.g., `nginx` or `httpd`)
- Copies `index.html` into the appropriate serving directory

### docker-compose.yml

The `docker-compose.yml` orchestrates the container, defining:
- Port mappings
- Volume mounts (if any)
- Service configuration

---

## 🛠️ Development

To make changes to the frontend, edit `index.html` and rebuild:

```bash
docker compose up --build
```


## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

*Built with Docker 🐳*
