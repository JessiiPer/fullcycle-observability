# Observability

Course of Observability - Fullcycle 2.0

# Summary

* [Elastic Stack](#elastic-stack)
* [Logstash](#logstash)
* [Beats](#beats)
    * [Metricbeat](#metricbeatats)
    * [Heartbeat](#heartbeat)
    * [Filebeat](#filetbeat)
* [APM](#apm)
* [References](#references)

## Elastic Stack

- The Elastic Stack is a group of open source products from Elastic designed to help users take data from any type of source and in any format, and search, analyze and visualize that data in real time.
- 2010 - Elasticsearch N.V (Elastic)
- Fast and scalable
- REST API
- Application, web site and enterprise search
- Logging and analitics
- Works in a distributed way through shards that have data redundancy
- Can scale thousands of servers and handle petabyte of data 

![home](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/home_elasticstack.png)

## Logstash

- Real data collector engine
- Started as log handler
- Works with pipelines
- Receives data from multiple sources
- Normalizes and transforms data
- Send data to multiple sources
- Plugins

## Kibana

- Data visualization and exploration tool
- Used with: Logs, Series Analysis, Application Monitoring and Operational Intelligence
- Integration with elasticsearch
- Aggregators and data filtering
- Dashboards
- Interactive graphics

## Beats

Beats é uma plataforma gratuita e aberta para agentes de dados de finalidade única. Eles enviam dados de centenas ou milhares de computadores e sistemas para o Logstash ou o Elasticsearch.

### **Metricbeat**

Agente lightweight para dados de métricas

**Analitics Discovery**
![metricbeat_discovery](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/uptime.png)

**Inventory Metrics**
![metricbeat_inventory](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/metricbeat_inventory.png)

**Available dashboards**
![metricbeat_available_dashboards](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/metricbeat_available_dashboards.png)

**Example - Docker dashboard**
![metricbeat_docker_dashboard](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/metricbeat_docker_dashboard.png)

### **Heartbeat**

Agente lightweight para monitoramento de tempo de atividade.

![uptime](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/uptime.png)


### **Filebeat**

Filebeat is a lightweight shipper for forwarding and centralizing log data. Installed as an agent on your servers, Filebeat monitors the log files or locations that you specify, collects log events, and forwards them either to Elasticsearch or Logstash for indexing.

## APM 

Elastic APM (Application Performance Monitoring)

Elastic APM's main function is to monitor your application end-to-end, bringing you infrastructure monitoring and mainly services. This function is very useful when you need to understand the integration of services and how they interact with each other, as well as having a view of the user experience.

![apm_transactions](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/apm_transactions.png)

**Backend Transations:**

![backend_transactions](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/backend_transactions.png)

**Frontend Transactions:**

![frontend_transactions](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/frontend_transactions.png)

### **APM Logs**

It is possible create logs (debugs) and see in Elastic APM

![apm_logs](https://github.com/JessiiPer/fullcycle-observability/blob/main/docs/apm_logs.png)

## References

- [Elastic Stack](https://www.elastic.co/elastic-stack/)