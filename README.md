# Log with ELK

## Overview
This repository provides a setup for logging using the ELK stack (Elasticsearch, Logstash, Kibana) via Docker.
The configuration allows you to easily deploy and start logging with ELK.

## Prerequisites
- **Docker**
- **Docker Compose**
  
## Setup

1. Clone this repository
```bash
git clone https://github.com/Ewins518/log-with-elk.git
cd log-with-elk
```

2. Start the ELK stack using Docker Compose:
```bash
docker-compose up -d
```

3. Access Kibana:
Open your web browser and go to http://localhost:5601.

## Configuration

- **docker-compose.yml** Configures the Docker containers for Elasticsearch, Logstash, and Kibana.
- **logstash.conf** Defines Logstash pipeline for ingesting, filtering, and sending logs to Elasticsearch.

## Usage
Place your log files in the logs directory. Logstash will automatically process these logs and send them to Elasticsearch. Use Kibana to visualize and analyze the logs.
