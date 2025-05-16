Kubernetes CourseLabs Hackathon

Welcome to our submission for the [Kubernetes CourseLabs Hackathon](https://kubernetes.courselabs.co/hackathon/)!  
This repository contains completed labs, custom configurations, and monitoring dashboards — all done locally using **Minikube**, **Helm**, **Prometheus**, and **Grafana**.


Tools & Technologies
- **Minikube** – Local Kubernetes Cluster
- **kubectl** – Cluster Management
- **Helm** – Kubernetes Package Manager
- **Prometheus** – Metrics Collection
- **Grafana** – Visualization and Monitoring


Lab Breakdown

Lab 1: Cluster Setup
- Installed Minikube
- Verified basic cluster functionality

Lab 2: Deployments
- Deployed containerized apps using `kubectl`
- Scaled and updated deployments

Lab 3: Helm Charts
- Installed and customized Helm charts
- Packaged own Helm chart for a sample app

Lab 4: ConfigMaps
- Externalized configurations for pods
- Used `kubectl` to create and mount ConfigMaps

Lab 5: Secrets
- Managed sensitive data using Kubernetes Secrets
- Mounted secrets into containers securely

Lab 6: Persistence
- Implemented persistent volumes
- Used PVCs to ensure data survived pod restarts

Lab 7: Monitoring (Prometheus + Grafana)
- Installed Prometheus and Grafana using Helm
- Collected metrics from containers and nodes
- Created Grafana dashboards to visualize:
  - Container memory usage
  - Namespace-based metrics
  - Cluster-wide health stats






Project Structure:
├── Lab1-Cluster-Setup/
├── Lab2-Deployments/
├── Lab3-Helm-Charts/
├── Lab4-ConfigMaps/
├── Lab5-Secrets/
├── Lab6-Persistence/
├── Lab7-Monitoring/
├── a9ace091-c659-4d80-85a6-5eae96454977.png
├── dd4c70d6-94f7-4feb-ace4-f758c7b9767a.png
└── README.md



Authors:
Ryan Mbindyo, Victor Kahindo, Antony Kimanthi, Maximillian Mwenda 
GitHub: [Mbindyo-Ryan](https://github.com/Mbindyo-Ryan)



License

This project is open-source under the MIT License.



![image](https://github.com/user-attachments/assets/9df6a10b-547e-44ef-9851-e989f7d2c451) - An illustration of the different containers and their memory usage in bytes 

