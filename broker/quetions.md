
### Brokers

1. Which of the following best describes Kafka as a Distributed Streaming Platform?
- [ ] Kafka is primarily a messaging system with real-time streaming capabilities
- [ ] Kafka is a batch processing system for large data analytics
- [ ] Kafka provides storage, but not message streaming
- [ ] Kafka is a database for structured data storage

**Answer:** Kafka is primarily a messaging system with real-time streaming capabilities

**Explanation:** Kafka is best described as a Distributed Streaming Platform because it combines messaging, storage, and real-time streaming capabilities. It allows for the processing of large volumes of data in real-time, making it ideal for use cases such as data pipelines, event processing, and stream processing.

2. When commissioning a new Kafka broker, which of the following is most critical to maintain cluster availability?
- [ ] Replicate the broker logs to new brokers
- [ ] Stop and restart the cluster
- [ ] Assign the broker a higher partition count
- [ ] Ensure the broker joins the Zookeeper quorum

**Answer:** Ensure the broker joins the Zookeeper quorum

**Explanation:** When commissioning a new Kafka broker, it is critical to ensure that the broker joins the Zookeeper quorum. Zookeeper is used for coordination and metadata management in Kafka, and a broker must be part of the Zookeeper quorum to participate in the cluster and maintain cluster availability.

3. What Kafka configurations ensure durability of messages in a broker failure scenario? (Select two)
- [ ] Set topic partitions to one
- [ ] Enable unclean leader election
- [ ] Enable acknowledgments for producer writes
- [ ] Increase the number of replicas

**Answer:** Enable acknowledgments for producer writes, Increase the number of replicas

**Explanation:** To ensure durability of messages in a broker failure scenario, you should enable acknowledgments for producer writes. This ensures that messages are acknowledged by the broker before being considered written. Additionally, increasing the number of replicas provides redundancy and fault tolerance, allowing for message recovery in case of a broker failure.

4. Which methods can be used to recover data after a broker failure in Kafka? (Select two)
- [ ] Zookeeper coordination
- [ ] Partition replication
- [ ] Log compaction
- [ ] Consumer groups

**Answer:** Zooker coordination, Partition replication

**Explanation:** After a broker failure in Kafka, data can be recovered through Zookeeper coordination, which helps manage the state of the cluster and metadata. Additionally, partition replication ensures that data is replicated across multiple brokers, allowing for recovery and fault tolerance in case of a broker failure.

5. In Kafka, how is fault tolerance ensured within the distributed log?
- [ ] By replicating partitions across multiple brokers
- [ ] By using RAID storage for logs
- [ ] By using external databases to store log files
- [ ] By storing all logs on a single server

**Answer:** By replicating partitions across multiple brokers

**Explanation:** Fault tolerance in Kafka is ensured by replicating partitions across multiple brokers. Each partition has multiple replicas, and in case of a broker failure, the replicas can be used to maintain data availability and durability.

6. What are the benefits of partitioning in Kafka topics? (Select two)
- [ ] Horizontal scalability
- [ ] Easier data compression
- [ ] Improved data security
- [ ] Enhanced fault tolerance through replication

**Answer:** Horizontal scalability, Enhanced fault tolerance through replication

**Explanation:** Partitioning in Kafka topics provides horizontal scalability by distributing data across multiple brokers. It also enhances fault tolerance through replication, as each partition has multiple replicas to ensure data availability and durability.

7. What is the function of Kafka's Exactly Once Semantics (EOS)?
- [ ] Ensuring each message is delivered and processed only once
- [ ] Ensuring messages are stored only once per partition
- [ ] Ensuring messages are stored in memory for faster reads
- [ ] Ensuring consumer offsets are reset after every read

**Answer:** Ensuring each message is delivered and processed only once

**Explanation:** Kafka's Exactly Once Semantics (EOS) ensures that each message is delivered and processed only once, providing strong guarantees for message processing and avoiding duplicate processing or data loss.

8. Which of the following actions ensure high availability in a Kafka cluster? (Select two)
- [ ] Replicating partitions across multiple brokers
- [ ] Using only one broker per topic
- [ ] Compressing all message data before sending
- [ ] Implementing leader election for partitions

**Answer:** Replicating partitions across multiple brokers, Implementing leader election for partitions

**Explanation:** High availability in a Kafka cluster is ensured by replicating partitions across multiple brokers, which provides redundancy and fault tolerance. Additionally, implementing leader election for partitions ensures that there is always a leader replica available to handle reads and writes, even in case of broker failures.

9. What is the primary purpose of tuning num.network.threads in Kafka brokers?
- [ ] To optimize data transfer performance
- [ ] To manage the number of partitions per topic
- [ ] To increase the number of producers
- [ ] To control the maximum message size

**Answer:** To optimize data transfer performance

**Explanation:** Tuning `num.network.threads` in Kafka brokers is primarily done to optimize data transfer performance. This configuration controls the number of network threads used for handling network requests, which can impact the throughput and latency of data transfer in the cluster.

10. Which of the following Kafka configurations determines how long log data is kept before being deleted?
- [ ] delete.log.ms
- [ ] data.cleanup.ms
- [ ] retention.ms
- [ ] log.durability.ms

**Answer:** retention.ms

**Explanation:** The `retention.ms` configuration in Kafka determines how long log data is kept before being deleted. This setting specifies the retention time for log segments, after which they can be deleted to manage storage usage and data retention policies.

11. When decommissioning a Kafka broker, which of the following steps should be performed first to prevent data loss?
- [ ] Transfer all partition leadership from the broker
- [ ] Stop the broker immediately
- [ ] Delete all logs from the broker
- [ ] Shut down all producers connected to the broker

**Answer:** Transfer all partition leadership from the broker

**Explanation:** When decommissioning a Kafka broker, the first step to prevent data loss is to transfer all partition leadership from the broker to other brokers in the cluster. This ensures that data is replicated and available on other brokers before shutting down the decommissioned broker.

12. Which of the following actions are part of Kafka broker performance tuning? (Select two)
- [ ] Increasing the number of topics
- [ ] Modifying the number of network threads
- [ ] Adjusting replication factor
- [ ] Increasing the number of consumer groups

**Answer:** Modifying the number of network threads, Adjusting replication factor

**Explanation:** Kafka broker performance tuning involves modifying the number of network threads to optimize data transfer performance and adjusting the replication factor to provide fault tolerance and data redundancy. These actions can improve the overall performance and reliability of a Kafka cluster.

13. What options are available to manage log retention in Kafka? (Select two)
- [ ] Set a maximum log size
- [ ] Set a retention time in hours or days
- [ ] Define the maximum number of partitions per broker
- [ ] Limit the number of producer threads

**Answer:** Set a maximum log size, Set a retention time in hours or days

**Explanation:** Log retention in Kafka can be managed by setting a maximum log size to control storage usage and by setting a retention time in hours or days to determine how long log data is kept before being deleted. These options help manage storage usage and data retention policies in a Kafka cluster.

14. What is the purpose of Kafka's commit log?
- [ ] To provide a durable and sequential record of all messages sent to Kafka topics
- [ ] To track the replication status of messages between brokers
- [ ] To store metadata about topics and brokers
- [ ] To delete old messages once consumed

**Answer:** To provide a durable and sequential record of all messages sent to Kafka topics

**Explanation:** Kafka's commit log is used to provide a durable and sequential record of all messages sent to Kafka topics. It ensures that messages are stored in the order they are received and provides fault tolerance and data durability in case of failures.

15. Which of the following Kafka processes is responsible for log compaction?
- [ ] Zookeeper
- [ ] Log cleaner
- [ ] Broker
- [ ] Consumer group coordinator

**Answer:** Log cleaner

**Explanation:** Log compaction in Kafka is performed by the log cleaner process, which is responsible for removing old and redundant messages from log segments to optimize storage usage and ensure efficient data retention policies.

16. What is the main purpose of capacity planning in Kafka?
- [ ] To automate leader election
- [ ] To optimize topic partitions
- [ ] To predict and manage data storage and throughput needs
- [ ] To ensure proper Zookeeper connectivity

**Answer:** To predict and manage data storage and throughput needs

**Explanation:** Capacity planning in Kafka is done to predict and manage data storage and throughput needs. It involves estimating the storage requirements, network bandwidth, and processing capacity required to support the expected data volume and workload in a Kafka cluster.

17. Which processes are involved when decommissioning a Kafka broker? (Select two)
- [ ] Moving partition replicas from the broker to other brokers
- [ ] Gracefully shutting down the broker
- [ ] Assigning new consumer groups to the broker
- [ ] Deleting all logs and restarting Zookeeper

**Answer:** Moving partition replicas from the broker to other brokers, Gracefully shutting down the broker

**Explanation:** When decommissioning a Kafka broker, the processes involved include moving partition replicas from the broker to other brokers to ensure data availability, and gracefully shutting down the broker to prevent data loss and maintain cluster stability.