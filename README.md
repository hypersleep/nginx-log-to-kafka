# nginx-log-to-kafka
Docker environment for streaming Nginx logs to Apache Kafka using Mozilla Heka.

1.Change *KAFKA_ADVERTISED_HOST_NAME* in fig.yml on address of your public interface (or Boot2docker ip).

2.Install `docker-compose` or `fig`, and run `docker-compose up` or `fig up`

3.Try to send some data to Nginx container: `curl -X POST -D- http://127.0.0.1/stats -d 'test1'`

4. Enjoy your Heka can print consumed messages from Apache Kafka :)
