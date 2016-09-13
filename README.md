Kafka Startup :- 


For Basic local setup :- 

1) Download Apache kafka from http://kafka.apache.org/
2) Unzip it at a location

3) Start Zookeeper
bin/zookeeper-server-start.sh config/zookeeper.properties

4) Start Broker
bin/kafka-server-start.sh config/server.properties

5) Topic Creation
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic test

6) List Topic
bin/kafka-topics.sh --list --zookeeper localhost:2181

7) Start Producer
bin/kafka-console-producer.sh --broker-list localhost:9092 --topic test 

8) Start Consumer
bin/kafka-console-consumer.sh --zookeeper localhost:2181 --topic test --from-beginning



========================================================================


