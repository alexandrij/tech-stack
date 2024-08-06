# Триссировка

Современный стек трассировки похож на логирование и делится на три компонента:

- Экспортер данных. Отправляет данные сборщику. OpenTelemetry Protocol (OTLP). SDK: opentelemetry, opentracing и т.д.;
- Сборщик данных. Очищает/обогащает и сохраняет в серверной части хранилище; 
- Хранилище данных. СУБД, ElasticSearch и т.п.;
- Ситемы визуализации и дашборды. Jaeger UI, Grafana, Kibana и т.п.; 

### Системы трассировки:

1. [Jaeger](https://www.jaegertracing.io//) - Платформа трассировки
   Jaeger. [Архитектура](https://www.jaegertracing.io/docs/1.59/architecture/).
    - [OpenTelemetry SDK](https://opentelemetry.io/) - Экспортер логов 
    - [Jaeger Сollector + DB](https://www.jaegertracing.io/docs/1.59/architecture/#collector) - Хранилище данных.
        - [Jaeger Сollector + Kafka + JaegerIndgexter + DB](https://www.jaegertracing.io/docs/1.59/architecture/#ingester) -
          For Kafka. Считает трассировки из Kafka и записывает их в хранилище.
    - [Jaeger Query + Jaeger UI](https://www.jaegertracing.io/docs/1.59/architecture/#query) - Визуализация данных.
   
    Пакет трассировки для go [opentelemetry-go](https://github.com/open-telemetry/opentelemetry-go)
2. 