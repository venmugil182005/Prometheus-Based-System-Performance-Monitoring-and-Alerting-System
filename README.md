# Overview

This project implements a real-time system performance monitoring and alerting solution using Prometheus, Node Exporter, and Alertmanager. It monitors CPU usage and sends email alerts when system performance degrades, helping in proactive system management and improving reliability.

---

## Features

- Real-time monitoring of system performance (CPU usage)
- Automatic alert generation using Prometheus
- Email notifications using Alertmanager (SMTP)
- Cloud deployment using AWS EC2
- Simple and scalable DevOps monitoring setup

---

## Technologies Used

- Prometheus
- Node Exporter
- Alertmanager
- AWS EC2 (Ubuntu)
- Gmail SMTP
- Linux (Ubuntu)

---



```bash
cd /home/ubuntu/node_exporter-1.8.2.linux-amd64
nohup ./node_exporter > node_exporter.log 2>&1 &
