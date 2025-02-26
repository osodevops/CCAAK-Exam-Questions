### Security

41. A large enterprise requires that all data is to be protected on any system where it exists. What steps would you take, as a Kafka Administrator, to protect the data at rest in a Kafka Cluster you manage? (choose two)
- [ ] You can programmatically encrypt data at the producer and decrypt it at the consumer
- [ ] Kafka brokers can natively encrypt data if you set a configuration option in their server.properties file
- [ ] You can use SSL to encrypt data from the producer
- [ ] You can run brokers on a machine with an encrypted file system

**Answer:** You can programmatically encrypt data at the producer and decrypt it at the consumer, You can run brokers on a machine with an encrypted file system

**Explanation:** To protect data at rest in a Kafka Cluster, you can programmatically encrypt data at the producer and decrypt it at the consumer. You can also run brokers on a machine with an encrypted file system to ensure data is protected.

42. Which configurations are part of enabling security in Kafka? (choose two)
- [ ] retention.bytes=log
- [ ] ssl.truststore.location
- [ ] log.retention.ms
- [ ] security.protocol=SSL

**Answer:** ssl.truststore.location, security.protocol=SSL

**Explanation:** To enable security in Kafka, you need to configure the ssl.truststore.location and security.protocol=SSL settings. These settings are necessary for enabling SSL encryption and authentication in Kafka.

43. Which configuration is critical for enabling SASL authentication in Kafka?
- [ ] kafka.security.protocol
- [ ] security.enable=true
- [ ] sasl.auth=true
- [ ] sasl.mechanism=PLAIN

**Answer:** sasl.mechanism=PLAIN

**Explanation:** To enable SASL authentication in Kafka, you need to configure the sasl.mechanism=PLAIN setting. This setting specifies the SASL mechanism to use for authentication.

44. What is the primary purpose of using Kerberos with Kafka?
- [ ] To manage producer retries
- [ ] To partition messages evenly across brokers
- [ ] To authenticate and authorize clients
- [ ] To ensure data durability

**Answer:** To authenticate and authorize clients

**Explanation:** The primary purpose of using Kerberos with Kafka is to authenticate and authorize clients connecting to the Kafka cluster. Kerberos provides secure authentication and authorization mechanisms for distributed systems like Kafka.

45. What is the primary purpose of SASL in securing Kafka?
- [ ] To authenticate clients connecting to the Kafka cluster
- [ ] To manage consumer offsets securely
- [ ] To provide message compression
- [ ] To encrypt data during transmission

**Answer:** To authenticate clients connecting to the Kafka cluster

**Explanation:** The primary purpose of SASL in securing Kafka is to authenticate clients connecting to the Kafka cluster. SASL provides a framework for pluggable authentication mechanisms in Kafka.

46. Which configuration enables TLS encryption for Kafka brokers?
- [ ] sasl.protocol=SSL
- [ ] tls.encryption.enable=true
- [ ] ssl.enable=true
- [ ] security.protocol=SSL

**Answer:** security.protocol=SSL

**Explanation:** To enable TLS encryption for Kafka brokers, you need to configure the security.protocol=SSL setting. This setting specifies the security protocol to use for communication between clients and brokers.

47. Which of the following is a key feature of Kafka's security architecture?
- [ ] Message replication
- [ ] Data compression
- [ ] Load balancing for consumer groups
- [ ] Encryption using SSL/TLS

**Answer:** Encryption using SSL/TLS

**Explanation:** A key feature of Kafka's security architecture is encryption using SSL/TLS. This feature provides secure communication between clients and brokers in a Kafka cluster.

48. Which actions are necessary for securing a Kafka cluster with Kerberos? (Select two)
- [ ] Configure Kafka clients with Kerberos tickets
- [ ] Create ACLs for all users
- [ ] Set up Key Distribution Center (KDC)
- [ ] Configure security.protocol=PLAINTEXT

**Answer:** Set up Key Distribution Center (KDC), Configure Kafka clients with Kerberos tickets

**Explanation:** To secure a Kafka cluster with Kerberos, you need to set up a Key Distribution Center (KDC) to manage authentication and authorization. You also need to configure Kafka clients with Kerberos tickets for secure communication with the cluster.