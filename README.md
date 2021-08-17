# Live-Dashboard-using-Kafka-and-Spring-Websocket
This Demo application reads data from Apache Kafka topic and updating the View using Spring Websocket on real-time.

Check the working Video : https://www.youtube.com/watch?v=GD0t-LwVRIM
Check the Tutorial : https://dzone.com/articles/live-dashboard-using-apache-kafka-and-spring-webso

Goto Kafka Folder in Desktop and perform Following Steps
========================================================
bin/zookeeper-server-start.sh config/zookeeper.properties
bin/kafka-server-start.sh config/server.properties
bin/kafka-topics.sh --create --topic quickstart-events --bootstrap-server localhost:9092
bin/kafka-console-producer.sh --topic quickstart-events --bootstrap-server localhost:9092
bin/kafka-console-consumer.sh --topic quickstart-events --from-beginning --bootstrap-server localhost:9092

bin/kafka-topics.sh --create --topic livedashboard --bootstrap-server localhost:9092

bin/kafka-console-producer.sh --topic livedashboard --bootstrap-server localhost:9092

bin/kafka-topics.sh --list --zookeeper localhost:2181

