# Система логирования

Современный стек журналирования делится на три компонента:

- Сборщики данных
- Хранилище/Агрегация данных (СУБД и полуСУБД)
- Ситемы визуализации и дашборды;

Опционально алертинг.

### Системы логирования:

1. [PLG](https://grafana.com/products/cloud/logs/) - Grafana stack
    - [Promtail](https://grafana.com/docs/loki/latest/send-data/promtail/) - Сборщик логов
    - [Loki](https://grafana.com/docs/loki/latest/) - Хранилище/Агрегация логов
    - [Grafana](https://grafana.com/docs/grafana/latest/) - Визуализация
2. [NPG](https://grafana.com/products/cloud/logs/) - Prometheus/Grafana stack
    - [Node exporter](https://prometheus.io/docs/guides/node-exporter/) - Сборщик логов
    - [Prometheus](https://prometheus.io/docs/introduction/overview/) - Хранилище/Агрегация логов
    - [Grafana](https://grafana.com/docs/grafana/latest/) - Визуализация
3. [ELK](https://www.elastic.co/elastic-stack) - Elastic Stack
    - [ElasticSearch](https://www.elastic.co/elasticsearch) - Хранилище логов
    - [Logstash](https://www.elastic.co/logstash) - Сборщик логов
    - [Kibana](https://www.elastic.co/kibana) - Визуализиция
4. [EFK](https://github.com/giefferre/EFK-stack)
    - [ElasticSearch](https://www.elastic.co/elasticsearch) - Хранилище логов
    - [FluentD](https://www.fluentd.org/) - Сборщик логов
    - [Kibana](https://www.elastic.co/kibana) - Визуализиция
5. [Zabbix](https://www.zabbix.com/ru) - Zabbix (for [Astra Linux](https://wiki.astralinux.ru/pages/viewpage.action?pageId=38699775))
    - Сборщик логов:
      - [Zabbix agent](https://www.zabbix.com/documentation/6.4/ru/manual/concepts/agent)
      - [Zabbix agent 2](https://www.zabbix.com/documentation/6.4/ru/manual/concepts/agent2)
    - Zabbix сервер (сервер, веб-интерфейс и хранилище в базе данных.):
      - [Zabbix Server](https://www.zabbix.com/documentation/6.4/ru/manual/concepts/server)

### Инструменты системы логирования

#### Сборщики логов:

- Logstash;
- Promtail;
- Fluentd;
- Fluent bit;
- Vector;
- Filebeat;
- Elastic Agent;

#### Хранилища:

- Elasticsearch
- Object storage (S3, minio, etc);
- Kafka;
- ClickHouse;
- Grafana Loki;
- Manticore Search;
- PostgreSQL;
- HDFS.

#### Визуализация:

- Kibana;
- Grafana;
- Metabase;
- Redash;
- Apache Superset;
- DataLens.

### Настройки логирования

- [Apache logs](https://sematext.com/blog/apache-logs/)
- [RabbitMQ logs](https://sematext.com/blog/rabbitmq-logs/)
- [Node.js logs](https://sematext.com/blog/node-js-logging/)
- [Java logs](https://sematext.com/blog/java-logging/)
- [Linux Logs](https://sematext.com/blog/linux-logs/)
- [PostgeSQL logs](https://sematext.com/blog/postgresql-logs/)
