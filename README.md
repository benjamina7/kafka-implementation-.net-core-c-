# kafka-implementation-.net-core-c-
https://www.youtube.com/watch?v=ARqyWaZqn68

Practical Example for Use Apache Kafka In .NET Application, the demo for  Kafka installation in .Net core and you can build Real-time Streaming Applications Using .NET Core c# and Kafka.   Steps 1. Download Prerequisite for Kafka and zookeeper 2. Install Kafka and zookeeper  3. Create a topic in Kafka console 4. Start the Kafka producer server 5. Start the Kafka consumer server 6. Create .Net core microservice as a producer  7. Create  .Net core application as a consumer 8. Test Kafka implementation using postman to see the communication between communication. 

Steps
1. Download Prerequisite for Kafka and zookeeper
2. Install Kafka and zookeeper 
3. Create a topic in Kafka console
4. Start the Kafka producer server
5. Start the Kafka consumer server
6. Create .Net core microservice as a producer 
7. Create  .Net core application as a consumer
8. Test Kafka implementation using postman to see the communication between communication.

-------------------------------------------------------
Prerequisite
7Zip  
https://www.7-zip.org/download.html

JRE8  http://www.oracle.com/technetwork/jav...

zookeeper 
https://zookeeper.apache.org/releases...

Kafka  
http://kafka.apache.org/downloads.html
-------------------------------------------------------
Commands
Zookeeper Start
C:\kafka-2.12- zkServer
Kafka Start
C:\kafka-2.12- .\bin\windows\kafka-server-start.bat .\config\server.properties

Create a Topic
C:\kafka-2.12\bin\windows- kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic temp-topic

Start Producer 
C:\kafka-2.12\bin\windows- kafka-console-producer.bat --broker-list localhost:9092 --topic temp-topic

Start Consumer
C:\kafka-2.12\bin\windows- kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic temp-topic --from-beginning

Topics in the list
C:\kafka-2.12\bin\windows - kafka-topics --zookeeper localhost:2181 --list

-------------------------------------------------------

the package needed in .net core application 
Confluent.Kafka, version 1.4.0

-------------------------------------------------------
