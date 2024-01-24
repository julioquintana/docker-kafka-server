2.2. Iniciar el servidor Kafka
Iniciemos el servidor Kafka haciendo girar los contenedores usando el comando docker-compose :

$ docker-compose up -d
Creating network "kafka_default" with the default driver
Creating kafka_zookeeper_1 ... done
Creating kafka_kafka_1     ... done
Copiar
Ahora usemos el comando nc para verificar que ambos servidores estén escuchando en los puertos respectivos :

$ nc -z localhost 22181
Connection to localhost port 22181 [tcp/*] succeeded!
$ nc -z localhost 29092
Connection to localhost port 29092 [tcp/*] succeeded!


https://www.kafkatool.com/download.html