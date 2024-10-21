# KAFKA

Mise en place du KAFKA

## [INSIDE THE CONTAINER JUST RUN]

```bash
- cd /opt/kafka/bin/
```

  Create a Topic
  
```bash  
- ./kafka-topics.sh --create --topic my-topic --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1
```

Produce Messages:

```bash
- ./kafka-console-producer.sh --topic my-topic --bootstrap-server localhost:9092
```

Consume Messages:

```bash
- ./kafka-console-consumer.sh --topic my-topic --bootstrap-server localhost:9092 --from-beginning
```
