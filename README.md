Here’s a fully reformatted and professional version of your README file for the **Kubernetes CourseLabs Hackathon** submission, improving structure, readability, and visual appeal:

---

# 🚀 Kubernetes CourseLabs Hackathon Submission

Welcome to our submission for the [**Kubernetes CourseLabs Hackathon**](https://kubernetes.courselabs.co/hackathon/)!
This repository showcases our completed labs, custom configurations, and monitoring dashboards — all set up **locally** using:

> 🐳 **Minikube** · 📦 **Helm** · 📊 **Prometheus** · 📈 **Grafana**

---

## 🛠️ Tools & Technologies

| Tool           | Purpose                                |
| -------------- | -------------------------------------- |
| **Minikube**   | Local Kubernetes cluster setup         |
| **kubectl**    | Cluster control and management         |
| **Helm**       | Kubernetes package management          |
| **Prometheus** | Metrics collection from pods and nodes |
| **Grafana**    | Monitoring and dashboarding            |

---

## 📚 Lab Breakdown

### 🔧 **Lab 1: Cluster Setup**

* Installed Minikube on local machine
* Verified cluster status and node health

### 🚀 **Lab 2: Deployments**

* Deployed containerized applications with `kubectl`
* Demonstrated scaling, rolling updates, and rollback

### 📦 **Lab 3: Helm Charts**

* Installed third-party charts from Helm Hub
* Packaged and deployed a custom Helm chart for a sample app

### ⚙️ **Lab 4: ConfigMaps**

* Created ConfigMaps for externalizing environment variables
* Mounted ConfigMaps into pods via volumes and environment keys

### 🔐 **Lab 5: Secrets**

* Managed sensitive data using Kubernetes Secrets
* Mounted secrets into running containers securely

### 💾 **Lab 6: Persistence**

* Created Persistent Volumes and Persistent Volume Claims
* Ensured data persistence across pod restarts

### 📊 **Lab 7: Monitoring with Prometheus & Grafana**

* Deployed Prometheus and Grafana using Helm
* Collected metrics from Kubernetes components
* Built custom Grafana dashboards visualizing:

  * 📌 **Container Memory Usage**
  * 📌 **Namespace-Specific Metrics**
  * 📌 **Cluster-Wide Health Statistics**

---

## 📁 Project Structure

```
.
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
```

---

## 🧑‍💻 Authors

* **Ryan Mbindyo**
* **Victor Kahindo**
* **Antony Kimanthi**
* **Maximillian Mwenda**

📎 GitHub Profile: [@Mbindyo-Ryan](https://github.com/Mbindyo-Ryan)

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---

## 📸 Sample Dashboard

![Grafana Dashboard](https://github.com/user-attachments/assets/9df6a10b-547e-44ef-9851-e989f7d2c451)
*Above: Real-time visualization of memory usage by container in bytes.*

---

Let me know if you'd like a badge header, markdown anchor links, or CI/CD integrations added.
