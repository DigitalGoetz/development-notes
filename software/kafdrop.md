# Kafdrop

Light-weight Kafka cluster monitoring tool

## Running in Docker

```bash
docker run -d --rm -p 9000:9000 \
    -e KAFKA_BROKERCONNECT=172.17.0.1:9092 \
    -e JVM_OPTS="-Xms32M -Xmx64M" \
    -e SERVER_SERVLET_CONTEXTPATH="/" \
    --net docker-stack_tdf-network \
    obsidiandynamics/kafdrop
```