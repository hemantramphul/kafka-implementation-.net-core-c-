# kafka-implementation-.net-core-c-
Practical Example for Use Apache Kafka In .NET Application, the demo for  Kafka installation in .Net core and you can build Real-time Streaming Applications Using .NET Core c# and Kafka. 

### _Steps_ 
1. Download Prerequisite for **Kafka and zookeeper**
2. Install **Kafka and zookeeper** 
3. Create a topic in **Kafka** console
4. Start the **Kafka producer server**
5. Start the **Kafka consumer server**
6. Create **.Net core** microservice as a producer 
7. Create  **.Net core** application as a consumer
8. Test **Kafka** implementation using postman to see the communication between communication.
          
## Prerequisite
### [7Zip](https://www.7-zip.org/download.html "7Zip")
### [JRE8](https://www.oracle.com/java/technologies/javase-jre8-downloads.html "JRE8")
### [Zookeeper](https://zookeeper.apache.org/releases.html "Zookeeper")
### [Kafka](http://kafka.apache.org/downloads.html "Kafka")

## Commands

#### Zookeeper Start

```sh
C:\kafka-2.12- zkServer
```

#### Kafka Start

```sh
C:\kafka-2.12- .\bin\windows\kafka-server-start.bat .\config\server.properties
```

#### Create a Topic

```sh
C:\kafka-2.12\bin\windows- kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic temp-topic
```

#### Start Producer 

```sh
C:\kafka-2.12\bin\windows- kafka-console-producer.bat --broker-list localhost:9092 --topic temp-topic
```

#### Start Consumer

```sh
C:\kafka-2.12\bin\windows- kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic temp-topic --from-beginning
```

Topics in the list

```sh
C:\kafka-2.12\bin\windows - kafka-topics --zookeeper localhost:2181 --list
```

## Package Installation
The package needed in .net core application **Confluent.Kafka,** `version 1.4.0`

