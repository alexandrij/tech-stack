# Система логирования

Современный стек журналирования делится на три компонента:

- Сборщики данных
- Хранилище/Агрегация данных (СУБД и полуСУБД)
- Ситемы визуализации и дашборды;

Опционально алертинг.

### Системы логирования:

1. [PLG](https://grafana.com/products/cloud/logs/) - Grafana stack
    - [Loki](https://grafana.com/docs/loki/latest/) - Хранилище/Агрегация логов
    - [Promtail](https://grafana.com/docs/loki/latest/send-data/promtail/) - Сборщик логов
    - [Grafana](https://grafana.com/docs/grafana/latest/) - Визуализация
2. [ELK](https://www.elastic.co/elastic-stack) - Elastic Stack
    - [ElasticSearch](https://www.elastic.co/elasticsearch) - Хранилище логов
    - [Logstash](https://www.elastic.co/logstash) - Сборщик логов
    - [Kibana](https://www.elastic.co/kibana) - Визуализиция
3. [EFK](https://github.com/giefferre/EFK-stack)
    - [ElasticSearch](https://www.elastic.co/elasticsearch) - Хранилище логов
    - [FluentD](https://www.fluentd.org/) - Сборщик логов
    - [Kibana](https://www.elastic.co/kibana) - Визуализиция

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

### Визуализация:

- Kibana;
- Grafana;
- Metabase;
- Redash;
- Apache Superset;
- DataLens.
