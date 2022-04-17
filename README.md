# Kafka Streams Hello World Application
by Yetkin Timocin

# Running Locally

1. `docker-compose up` to get Kafka and Zookeeper up and running.
2. Run `KafkaStreamsHelloWorld` class to see the output of the Stream Processor when producer sends some data to the topic.
3. In another terminal, SSH into the container `docker-compose exec kafka bash`
4. Stand up a producer and enter some data:
```
kafka-console-producer \
     --bootstrap-server localhost:9092 \
     --topic hello-world
```
5. See the output of `KafkaStreamsHelloWorld`

# References
Mastering Kafka Streams and ksqlDB Book