# Enterprise Infrastructure Automation using Ansible on AWS

## Project Overview

This project demonstrates the deployment and automation of a multi-tier enterprise infrastructure on AWS using Ansible and RHEL 9. The infrastructure includes web servers, database services, centralized file sharing, load balancing, security hardening, monitoring, and backup automation.

The objective was to implement Infrastructure as Code (IaC) principles to reduce manual configuration effort and ensure consistent, repeatable deployments across multiple servers.

---

## Architecture Components

* Ansible Control Node
* Apache Web Servers (Web1 & Web2)
* MariaDB Database Server
* NFS File Server
* HAProxy Load Balancer
* Prometheus Monitoring Server
* Grafana Visualization Dashboard

---

## Technologies Used

* AWS EC2
* AWS VPC
* RHEL 9
* Ansible
* Apache HTTP Server
* MariaDB
* NFS
* HAProxy
* Firewalld
* Prometheus
* Grafana
* Git & GitHub

---

## Key Features

### Infrastructure Automation

* Automated server configuration using Ansible playbooks and roles.
* Reusable role-based architecture for scalability and maintainability.

### Web Server Deployment

* Automated Apache installation and configuration.
* Website deployment across multiple web servers.

### Database Automation

* MariaDB installation and service management using Ansible.

### Centralized File Sharing

* NFS server configured to provide shared storage across web servers.

### Load Balancing

* HAProxy configured to distribute traffic between web servers.

### Security Hardening

* Automated firewall configuration using firewalld.
* SSH hardening by disabling root login.

### Monitoring & Observability

* Node Exporter installed on web servers.
* Prometheus configured for metrics collection.
* Grafana dashboards created for infrastructure monitoring.

### Backup Automation

* Automated backup scheduling using cron jobs.

---

## Project Structure

```text
rhce-project/
├── group_vars/
├── inventory/
├── playbooks/
├── roles/
│   ├── apache/
│   ├── mariadb/
│   ├── nfs/
│   ├── haproxy/
│   ├── security/
│   ├── monitoring/
│   └── backup/
├── templates/
└── site.yml
```

---

## Deployment

Run the complete infrastructure deployment using:

```bash
ansible-playbook -i inventory/hosts site.yml
```

---

## Monitoring

Prometheus collects system metrics from web servers through Node Exporter.

Grafana provides dashboards for:

* CPU Usage
* Memory Usage
* Disk Utilization
* Network Statistics

---

## Learning Outcomes

* Infrastructure as Code (IaC)
* Configuration Management with Ansible
* Linux System Administration
* AWS Networking and Security
* Load Balancing Concepts
* Monitoring and Observability
* Enterprise Infrastructure Automation

---

## Author

Nandhitha Binu
