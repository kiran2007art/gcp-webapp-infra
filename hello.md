# GCP Web App Infrastructure

This project builds the infrastructure for a web application hosted on Google Cloud using **Compute Engine** and **NGINX**.

## 🚀 Project Overview

The goal is to:
- Create a Cloud Storage bucket to store product and order files
- Create a Persistent Disk and attach it to a Compute Engine VM
- Host an NGINX web server on the VM
- Allow HTTP traffic for web access

All resources are created in the **us-east4** region and **us-east4-c** zone.

---

## 🧱 Components

| Resource Type | Name | Region/Zone | Purpose |
|----------------|------|-------------|----------|
| Cloud Storage Bucket | `products-bucket` | us-east4 | Stores static files |
| Persistent Disk | `webapp-disk` | us-east4-c | Attached to VM |
| Compute Engine VM | `webapp-vm` | us-east4-c | Runs NGINX web server |
| Firewall Rule | `allow-http` | global | Allows port 80 traffic |

---

## 🧰 Tools Used

- Google Cloud Platform (GCP)
- Compute Engine
- Cloud Storage
- NGINX web server
- Terraform (optional for automation)

---

## 📥 Deployment Instructions

See the [`commands.md`](./commands.md) file for the exact `gcloud` commands used to create the infrastructure.

---

## 👤 Author
Your Name  
Cloud Architect | Google Cloud Practitioner
