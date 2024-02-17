# ApacheKafkaDemo
## Few usefull commands which needs to be executed to run apache kafka server before running this spring boot project
### First download Apache Kafka zip from offical website then unzip it and keep it in your c drive. 
#### 1. Run below commands to start the zookeeper
bin\windows\zookeeper-server-start.bat config\zookeeper.properties

#### 2. Run below commands to start the kafka server
bin\windows\kafka-server-start.bat config\server.properties

#### 3. Run below commands to create your own topic, here my topic name is user-topic1
bin\windows\kafka-console-producer.bat --topic user-topic1 --bootstrap-server localhost:9092

#### 4. Run below commands for consumer to check the messages from producer
bin\windows\kafka-console-consumer.bat --topic user-topic1 --from-beginning --bootstrap-server localhost:9092

example:
bin\windows\kafka-console-consumer.bat --topic location-update-topic --from-beginning --bootstrap-server localhost:9092
## Below image describes sucessfully running the project
![ApacheKafka_working_fine](https://github.com/KSHIRODBADIA/ApacheKafkaDemo/assets/55657175/5009b942-4fb5-47ef-a01a-b1c7fb73451b)
