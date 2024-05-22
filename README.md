# kafkahandson
Practical Demo for setup Kafka in containers and SSl configuration steps
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

In this Demo We have two docker-compose.yml file for Kafka setup with SSL and with out SSL.

Prerequisite
***********
Install Docker and docker-compose

keep the secrets folder and docker-compose.yml file @ same location
Ex: /home/user_name/secrets
   /home/user_name/docker-compose.yml


Issue : While Executing the docker-compose file 

ERROR: client version 1.22 is too old. Minimum supported API version is 1.24, please upgrade your client to a newer version 

Solution: Change the version number from 2 to 2.1 in docker-compose.yml file 

version: '2' 

To 

version: '2.1'

References:
https://github.com/apache/kafka/blob/trunk/docker/examples/jvm/cluster/combined/ssl/docker-compose.yml
https://medium.com/@cesantin/kafka-brokers-and-zookeeper-7447009637f4
https://www.scaler.com/topics/kafka-tutorial/the-role-of-zookeeper-in-the-kafka-cluster/
