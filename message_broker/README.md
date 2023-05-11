# Message Brokers Belgeler

Microservice'ler arası asenkron veri alışverişi sağlayarak High Availability'yi destekler, message broker servisleri asenkron iletişimi farklı algoritmalar ile yapabilir. Message Broker servislerine bir microservice veri yazar, diğer bir bu veriyi okur. Genelde message broker'a bir veri ekleyen servise Producer, veriyi okuyan ve çıkarak servise consumer denir.

### Mesage Broker'ların kullandığı protokoller:

|     Protokol	 | OSI Katmanı | 	Altında Yatan Protokoller  |
|--------------:|------------:|-------------------------------|
|          AMQP | 	Katman 5-7 | TCP, TLS/SSL                  |
|          MQTT | 	Katman 5-7 | 	TCP, TLS/SSL               |
|         STOMP | 	Katman 5-7 | 	TCP                        |
|          CoAP | 	Katman 5-6 | 	UDP                        |
|          XMPP | 	Katman 5-7 | 	TCP, TLS/SSL               |
|         Kafka |  Katman 4   | 	TCP                        |
| Redis Pub/Sub | 	Katman 5-7 | 	TCP                        |
|  ZeroMQ (ZMQ) | 	Katman 4-7 | 	TCP, UDP, SCTP, TLS/SSL    |
|           DDS | 	Katman 4-7 | 	UDP, TCP, DDS Security     |

