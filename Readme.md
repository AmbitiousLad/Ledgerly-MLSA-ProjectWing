# Ledgerly

An open-source, self-hostable expense-tracking platform built with **Next.js**, **Python**, and **AWS** for Lambda functions and S3 object storage. **Ledgerly** helps you manage your expenses and gain insights through advanced monitoring and observability.

## Architecture
![image](https://github.com/user-attachments/assets/8b85c530-695c-45f4-95f8-6983aca603c3)

---

## **Features**
### **Website**
- **Next.js App Router** for building the frontend.
- **Amazon Web Services** for backend functionality with EC2.
- Support for **S3 File Storage** and **Lambda Container image-based Functions**.
- **Edge runtime-ready** for enhanced performance.

### **AWS Infrastructure**
- **Amazon S3**: Utilized for image storage.
- **AWS Lambda**: Processes JSON and filters required data.
- **Amazon EC2**: Manages virtual machine instances.
- **Amazon ECR**: Privately hosts container images.

### **External**
- **Prometheus, Grafana, and GoAccess**: Ensure extensive observability and resource monitoring.
- **Gemini API**: Performs image-to-text extraction using a Vision Model within free tier limits.
- **GitHub Actions**: CI/CD pipelines for building, testing, and pushing application images.
- **Traefik**: Acts as a dynamic reverse proxy and automatically manages SSL/TLS certificates.

---

## **Tech Stack**
- **Frontend:** Next.js
- **Backend:** Python, FastAPI, Uvicorn
- **Infrastructure:** AWS (EC2, S3, Lambda, ECR)
- **Observability:** Prometheus, Grafana, GoAccess
- **CI/CD:** GitHub Actions
- **Proxy:** Traefik
- **Image to Text:** Gemini Vision Model
- **Containers:** Docker

---

## **Overview**

### **AWS Architecture**
The backend consists of three main services:
1. **Python-based REST API**: Developed using FastAPI for serving requests and performing CRUD operations.
2. **RDS Postgres Database**: Stores and retrieves expense data.
3. **S3 Bucket**: Hosts and stores images.

Additional services:
- **Traefik**: Acts as a reverse proxy for automatic SSL provisioning and log generation.
- **Prometheus and Grafana**: Collect and visualize resource usage with custom log exporters.

All services are containerized using **Docker** to ensure availability, scalability, and optimal performance.

---

## **Sections**
- **Features**: A quick summary of the platform’s capabilities.
- **Overview**: High-level architecture and infrastructure details.
- **AWS Setup**: Detailed steps for setting up AWS resources.
- **Backend Setup**: Instructions for setting up the backend services.
- **Usage**: How to use Ledgerly to track expenses.
- **Monitoring**: Insights into observability with Prometheus, Grafana, and GoAccess.
---



---

Feel free to fork and contribute to the Ledgerly project!

