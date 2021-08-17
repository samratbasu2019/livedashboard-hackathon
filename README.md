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

