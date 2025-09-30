
# Monitoring & Logging (Demo)

This project demonstrates centralized logging with the **ELK Stack** and integration of **AWS CloudWatch** & **Prometheus** for proactive alerting and performance monitoring.

---

### Note
> ⚠️ **This is a demo version** of my original project. Resource names and configurations are generic placeholders (“demo”) to ensure safe public sharing.

---

## Features
- Centralized log aggregation with ELK Stack
- CloudWatch metrics and log monitoring
- Prometheus-based performance monitoring
- Kibana dashboards for log analysis
- Alerting rules for proactive monitoring

---


## 📂 Project Structure

```text
monitoring-logging/
│── elk/
│   ├── docker-compose.yml
│   ├── elasticsearch.yml
│   ├── logstash.conf
│   ├── kibana.yml
│── cloudwatch/
│   ├── cloudwatch-agent.json
│── prometheus/
│   ├── prometheus.yml
│   ├── alert.rules.yml
│── README.md
│── .gitignore



Getting Started

1. Prerequisites
Docker & Docker Compose
AWS CLI configured
Prometheus installed or containerized

2. Start ELK Stack
cd elk
docker-compose up -d

3. Configure CloudWatch Agent
sudo /opt/aws/amazon-cloudwatch-agent/bin/amazon-cloudwatch-agent-ctl \ -a fetch-config -m ec2 -c file:/path/to/cloudwatch-agent.json -s

4. Start Prometheus
cd prometheus
prometheus --config.file=prometheus.yml



Learning Objectives

Build centralized logging with ELK Stack
Integrate AWS CloudWatch for log collection and metrics
Set up Prometheus monitoring and alerts
Create Kibana dashboards
Implement proactive alerting rules