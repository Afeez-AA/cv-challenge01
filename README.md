
# **Full-Stack FastAPI and React Application**

In this project, we will containerize and deploy a multi-tier web application using Docker, Docker Compose, and reverse proxy configurations. The application consists of a React frontend that interacts with a FastAPI backend, backed by a PostgreSQL database. To ensure smooth monitoring and management of the application's performance, we will integrate a Monitoring Stack that includes Prometheus for metrics collection, Grafana for data visualization, Loki for log aggregation, and cAdvisor for container performance monitoring.

---

## **Features**
- **Reverse Proxy with SSL**: Secured application access using Nginx Proxy Manager.
- **Container Metrics**: Real-time monitoring of container metrics like CPU, memory, disk I/O, and network usage with cAdvisor.
- **Centralized Logging**: Application and container log aggregation and visualization using Loki and Grafana.
- **Database Management**: Simplified database access and management via Adminer.

---

## **Quick Start Guide**

### **1. Clone the Repository**
```bash
git clone https://github.com/Afeez-AA/cv-challenge01
cd cv-challenge01
```

### **2. Start the App Stack**
- Ensure you have Docker and Docker Compose installed.
- Run the following command to start the app:
  ```bash
  docker-compose up -d
  docker compose -f monitoring-stack up -d 
  ```

### **3. Access the Services**
- **Frontend**: `https://your-domain`
- **Backend API**: `https://your-domain/api`
- **API Docs**: `https://your-domain/docs`
- **Adminer (Database)**: `https://db.your-domain`
- **Grafana (Monitoring)**: `http://your-domain:3000`


---

## **Configuration Steps**
1. **Update `.env` File**: Configure the environment variables in the `.env` file for your domain and credentials.
2. **Proxy Hosts**: Use Nginx Proxy Manager to set up proxy hosts for your frontend, backend, and database services.
3. **SSL Certificates**: Request SSL certificates for your domains in Nginx Proxy Manager.

---

## **Additional Documentation**
- For detailed project feature, requirements and instructions, refer to the extended README [here](README.instructions.md).
- For a step-by-step walkthrough, check out the article on [my Dev.to post](https://dev.to/afeezaa/complete-guide-to-containerizing-and-deploying-a-full-stack-application-with-docker-nginx-and-4koj).

---

## **Contributing**
Contributions are welcome! Please create an issue or submit a pull request for any improvements or bug fixes.

