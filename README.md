# Node.js-React.js-PostgreSQL project

A comprehensive React-Node-Postgres boilerplate which includes all the server-client communication and basic CRUD and supported with awesome ant design features. Sequelize ORM is used to set up  the database, models and whole db communiation. 
## Prerequisites

* Node.js
* PostgreSQL

## Getting Started

### Root
# Node React Postgres Application

A full-stack web application built with **Node.js**, **React**, and **PostgreSQL**, containerized using **Docker**, orchestrated with **Docker Compose**, and prepared for deployment with **Kubernetes**. CI/CD workflows are managed via **GitHub Actions**.

---

## 📁 Project Structure

.
├── .github/workflows/ # GitHub Actions CI/CD workflows
├── apiserver/ # Backend (Node.js / API server)
├── client/ # Frontend (React application)
├── k8s/ # Kubernetes manifests
├── node-react-postgres-main/ # Project root or legacy directory
├── Dockerfile.backend # Dockerfile for backend service
├── Dockerfile.frontend # Dockerfile for frontend service
├── docker-compose.yml # Docker Compose configuration
├── package.json # Root dependencies & scripts
├── package-lock.json # Dependency lock file
├── .gitignore # Git ignored files
└── README.md # Project documentation
* Run npm i to install concurrently.
* Run project with npm start for development after installing server and client pakages.


---

## 🚀 Tech Stack

**Frontend**
- React
- JavaScript / JSX

**Backend**
- Node.js
- Express (if applicable)

**Database**
- PostgreSQL

**DevOps / Infrastructure**
- Docker
- Docker Compose
- Kubernetes
- GitHub Actions

---

## ⚙️ Prerequisites

Make sure you have the following installed:

- Node.js (v16+ recommended)
- Docker & Docker Compose
- Kubernetes cluster (optional, for k8s deployment)
- kubectl (optional)

---

## 🛠️ Local Development (Docker Compose)

### 1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
#########################################################

docker-compose up --build

Access the application
Frontend: http://localhost:3000
Backend API: http://localhost:5000 (or configured port)
PostgreSQL: Exposed via Docker network

Docker Setup
Backend Image
###############################################
docker build -f Dockerfile.backend -t backend-app .
Frontend Image
#############################################
docker build -f Dockerfile.frontend -t frontend-app .

☸️ Kubernetes Deployment

Kubernetes manifests are located in the k8s/ directory.
Apply all resources

kubectl apply -f k8s/
kubectl get pods
kubectl get services
########################################
Environment Variables

Create a .env file if required (example)

POSTGRES_HOST=postgres
POSTGRES_PORT=5432
POSTGRES_DB=app_db
POSTGRES_USER=postgres
POSTGRES_PASSWORD=password



### Apiserver

* Head over apiserver and run npm install.
* Create a .config.env file and add your env variables
* Create a folder named "images" for image upload


### Client

* Cd over client and run npm install.




