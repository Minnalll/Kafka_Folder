.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
.\bin\windows\kafka-server-start.bat .\config\server.properties 

.\bin\windows\kafka-topics.bat --create --bootstrap-server localhost:9092 --replication-factor 1 --partition 1 --topic test 

.\bin\windows\kafka-topics.bat --list --bootstrap-server localhost:9092

.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic test

.\bin\windows\kafka-console-consumer.bat --topic test --bootstrap-server localhost:9092 --from-beginning 

.\bin\windows\zookeeper-server-stop.bat .\config\zookeeper.properties 
.\bin\windows\kafka-server-stop.bat .\config\server.properties

From <https://www.youtube.com/watch?v=BwYFuhVhshI> ![image](https://github.com/user-attachments/assets/ce2b9c39-1a29-4367-9cef-ad0a4c204ff3)
