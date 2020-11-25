# Kafka


```update-java-alternatives --list```</br>
```sudo update-java-alternatives --set /path/to/java/version```

Starting zookeeper and kafka:</br>
```zookeeper-server-start.sh ~/kafka_2.12-2.4.1/config/zookeeper.properties```</br>
```kafka-server-start.sh ~/kafka_2.12-2.4.1/config/server.properties```
</br>

Create topic (impossible to create a topic with rep. fact. > n°brokers):
```kafka-topics.sh --zookeeper 127.0.0.1:2181 --topic first_topic --create --partitions 3 --replication-factor 1```

List the topics:</br>
```kafka-topics.sh --zookeeper 127.0.0.1:2181 --list```</br>
```kafka-topics.sh --zookeeper 127.0.0.1:2181 --topic first_topic --describe```

Delete topic:</br>
```kafka-topics.sh --zookeeper 127.0.0.1:2181 --topic first_topic --delete```

Launch consumer:</br>
```kafka-console-producer.sh --broker-list 127.0.0.1:9092 --topic first_topic```

Launch producer:</br>
```kafka-console-producer.sh --broker-list 127.0.0.1:9092 --topic first_topic```
