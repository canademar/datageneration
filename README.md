# README #


CHANGE PATHS TO INSTALLATION DIRECTORY!

Zookeeper: 

	cd ~/apps/kafka_2.10-0.8.2.1/ && bin/zookeeper-server-start.sh config/zookeeper.properties

Kafka:

	cd ~/apps/kafka_2.10-0.8.2.1/ && bin/kafka-server-start.sh config/server.properties

Json-generator:

	cd ~/apps/json-data-generator-1.2.0/ && java -jar json-data-generator-1.2.0.jar bd4bfSimulator.json

Flume:

	cd ~/apps/apache-flume-1.6.0-bin/ && bin/flume-ng agent -C ~/apps/kafka_2.10-0.8.2.1/libs/zookeeper-3.4.6.jar -n agent1 -c conf -f conf/bd4bf.properties
