# 🌐 Nginx Load Balancer Demo with Two Frontend Apps

This project demonstrates how to use **Docker**, **Nginx**, and **Docker Compose** to load balance between two frontend applications — `App1` and `App2`.

It shows how:
- Nginx distributes requests **2:1** (two requests go to App1, the next one goes to App2).
- The load balancer runs directly on **http://localhost** (no port numbers).
- Both frontends are styled beautifully using **pure HTML + CSS** with animations.

---

## 🧩 Project Structure

nginx-round-robin-demo/
├── app1/
│ ├── Dockerfile
│ └── index.html
├── app2/
│ ├── Dockerfile
│ └── index.html
├── lb/
│ ├── Dockerfile
│ └── nginx.conf
├── docker-compose.yml
└── README.md


🚀 5. Run the Project
1️⃣ Build and start containers:
docker-compose up --build -d

2️⃣ Check container status:
docker ps


You should see three containers: app1, app2, lb.

3️⃣ Open your browser:

👉 Visit http://localhost


✅ Summary

🖥️ Two animated frontend apps with modern design

⚖️ Nginx weighted round-robin (2 requests → App1, 1 request → App2)

🌍 Runs on http://localhost
 (port 80)

🐳 Fully Dockerized (3 containers)
