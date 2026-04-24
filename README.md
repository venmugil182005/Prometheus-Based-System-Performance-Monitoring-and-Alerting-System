Overview

This project implements a real-time system performance monitoring and alerting solution using Prometheus, Node Exporter, and Alertmanager. It monitors CPU usage and sends email alerts when system performance degrades, helping in proactive system management and improving reliability.

Features
Real-time monitoring of system performance (CPU usage)
Automatic alert generation using Prometheus
Email notifications using Alertmanager (SMTP)
Cloud deployment using AWS EC2
Simple and scalable DevOps monitoring setup
Technologies Used
Prometheus
Node Exporter
Alertmanager
AWS EC2 (Ubuntu)
Gmail SMTP
Linux (Ubuntu)
Project Structure
prometheus.yml – Prometheus configuration
alert.rules.yml – Alert rules for CPU monitoring
alertmanager.yml – Alertmanager email configuration
README.md – Project documentation
screenshots/ – Output screenshots
Setup Instructions
1. Start Node Exporter
cd /home/ubuntu/node_exporter-1.8.2.linux-amd64
nohup ./node_exporter > node_exporter.log 2>&1 &
2. Start Prometheus
cd /home/ubuntu/prometheus-2.53.0.linux-amd64
nohup ./prometheus --config.file=prometheus.yml > prometheus.log 2>&1 &

3. Start Alertmanager
cd /home/ubuntu/alertmanager-0.27.0.linux-amd64
nohup ./alertmanager --config.file=alertmanager.yml > alertmanager.log 2>&1 &
