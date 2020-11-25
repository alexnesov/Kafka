# Kafka


```update-java-alternatives --list```</br>
```sudo update-java-alternatives --set /path/to/java/version```

Starting zookeeper and kafka:</br>
```zookeeper-server-start.sh ~/kafka_2.12-2.4.1/config/zookeeper.properties```</br>
```kafka-server-start.sh ~/kafka_2.12-2.4.1/config/server.properties```
</br>

```kafka-console-consumer.sh --bootstrap-server 127.0.0.1:9092 --topic first_topic```</br>
```kafka-console-producer --broker-list 127.0.0.1:9092 --topic first_topic```</br>
```kafka-console-producer.sh --broker-list 127.0.0.1:9092 --topic first_topic```</br>

