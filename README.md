# UpCommerce

UpCommerce is a simple e-commerce web application built with **Python**, **HTML/CSS**, and **JavaScript**, containerized using **Docker**, and deployable on **Kubernetes**. It demonstrates a modern approach to app deployment, monitoring, and alerting.

---

## 🛠 Tech Stack

* **Backend:** Python (Flask)
* **Frontend:** HTML, CSS, JavaScript
* **Containerization:** Docker
* **Orchestration:** Kubernetes (Deployment & Service YAML files)
* **Monitoring:** Prometheus (`prometheus.yml`)
* **Alerting:** Slack & Gmail (`slack-alert.yml`, `gmail-alert.yml`)

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/DebbieArita/UpCommerce.git
cd UpCommerce
```

### 2. Run locally

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app.py
```

Visit [http://localhost:5000](http://localhost:5000)

### 3. Run with Docker

```bash
docker build -t upcommerce .
docker run -p 5000:5000 upcommerce
```

### 4. Deploy to Kubernetes

```bash
kubectl apply -f deployment.yml
kubectl apply -f service.yml
```

---

## ⚙️ Configuration

* `deployment.yml` — Kubernetes deployment file
* `service.yml` — Kubernetes service definition
* `prometheus.yml` — monitoring setup
* `gmail-alert.yml` / `slack-alert.yml` — alerting configs
* `values.yml` — Helm values file (optional)

---

## 📈 Features

* Basic web storefront with HTML templates
* Dockerized for portability
* Kubernetes manifests for deployment
* Prometheus monitoring and alerting examples
* Easily extendable (auth, payments, inventory, etc.)
