
## Overview

This part of the hackathon focuses on deploying and configuring the **Widgetario** microservices application using Kubernetes resources. The key objectives implemented include setting up secure and scalable deployments, services, and secrets to enable seamless communication between components.

---

## What Has Been Implemented

### 1. Deployments
- **Products API Deployment** 
  Deploys the `products-api` microservice, configured to mount database credentials securely using a Kubernetes Secret (`products-api-db`). The container exposes HTTP on port 80.

- **Products Database Deployment** 
  Deploys the PostgreSQL database container (`products-db`) with environment variables sourced securely from a Secret (`products-db-password`).

- **Web Frontend Deployment** 
  Deploys the `web` frontend container, configured to load feature flags from a ConfigMap (`web-features`) and API backend URLs from a Secret (`web-api`) mounted as a file.

### 2. Services
- **Products API Service** 
  Internal `ClusterIP` service exposing the `products-api` on port 80, enabling communication with other services inside the cluster.

- **Products Database Service** 
  Exposes the PostgreSQL database internally on port 5432.

- **Web Frontend Services** 
  Two types of services are provided:
  - **LoadBalancer Service**: Exposes the frontend externally (in cloud environments) on port 8080.
  - **NodePort Service**: Alternative exposure on port 30008 for local or non-cloud Kubernetes clusters.

- **Stock API Service** 
  Internal `ClusterIP` service exposing the `stock-api` microservice on port 80.

### 3. Secrets
- **Database Credentials Secret** (`products-api-db`) 
  Stores sensitive database connection details for `products-api` securely.

- **Products DB Password Secret** (`products-db-password`) 
  Contains the PostgreSQL password for the `products-db` deployment.

- **Web API Config Secret** (`web-api`) 
  Stores a JSON configuration file with URLs for backend APIs (`products-api` and `stock-api`), which the frontend consumes.

### 4. Configuration Management
- Usage of ConfigMaps (`web-features`) for managing environment variables related to frontend features.

---

## Key Practices Followed

- **Security:** Sensitive data such as passwords and API URLs are stored in Kubernetes Secrets and mounted as read-only volumes or injected as environment variables.
- **Service Discovery:** Services use Kubernetes DNS for internal communication (e.g., `products-api.default.svc.cluster.local`).
- **Modularity:** Deployments separate concerns by using ConfigMaps and Secrets, enabling easy updates without changing container images.
- **Flexible Exposure:** Both `LoadBalancer` and `NodePort` services are created for frontend access to support multiple deployment environments.

