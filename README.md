# kafka

[INSIDE THE CONTAINER JUST RUN]

cd /opt/kafka/bin/
Create a Topic
./kafka-topics.sh --create --topic my-topic --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1
Produce Messages:
./kafka-console-producer.sh --topic my-topic --bootstrap-server localhost:9092
Consume Messages:
./kafka-console-consumer.sh --topic my-topic --bootstrap-server localhost:9092 --from-beginning
