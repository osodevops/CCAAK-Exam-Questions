### Consumers

18. Which Kafka component is responsible for maintaining the state of consumer offsets?
- [ ] Zookeeper
- [ ] Producers
- [ ] Consumer Groups
- [ ] Brokers

**Answer:** Brokers

**Explanation:** Brokers in Kafka are responsible for maintaining the state of consumer offsets. Consumer offsets are stored in an internal topic called `__consumer_offsets`, which is managed by the brokers.

19. Which of the following tasks are performed by a Kafka consumer? (Select two)
- [ ] Committing message offsets
- [ ] Reading messages from Kafka topics
- [ ] Handling message retries on failure
- [ ] Sending messages to Kafka topics

**Answer:** Committing message offsets, Reading messages from Kafka topics

**Explanation:** Kafka consumers are responsible for committing message offsets to track their progress in reading messages from Kafka topics. They also read messages from Kafka topics and process them according to the application logic.

20. When optimizing consumer performance in Kafka, which configurations should you focus on? (Select two)
- [ ] max.message.bytes
- [ ] log.segment.bytes
- [ ] max.poll.records
- [ ] fetch.min.bytes

**Answer:** max.poll.records, fetch.min.bytes

**Explanation:** When optimizing consumer performance in Kafka, you should focus on configurations like `max.poll.records` and `fetch.min.bytes`. `max.poll.records` controls the maximum number of records returned in a single poll request, while `fetch.min.bytes` specifies the minimum amount of data that must be available for a fetch request to be processed.

21. Several applications are producing messages with different compression formats to a single Kafka topic that has multiple partitions. How will consuming applications become aware of the different compression formats used by each producer?
- [ ] Brokers will record the compression type of each message in an internal Kafka topic
- [ ] Producers will indicate the compression type in the header of each message
- [ ] This is not possible, because each Kafka topic requires all of its partitions to have the same compression type
- [ ] Brokers will write each message into the partition that matches the producer's compression type setting

**Answer:** Producers will indicate the compression type in the header of each message

**Explanation:** To make consuming applications aware of the different compression formats used by each producer, producers can indicate the compression type in the header of each message. This allows consumers to identify the compression format and decompress the message accordingly.

22. When attempting to read from a subscribed topic, a consumer application is not seeing produced messages. Which of the following could be the cause? (Choose Two)
- [ ] The consumer is unable to communicate with the __consumer_offsets topic
- [ ] A broker on the In-Sync Replica (ISR) list has failed, delaying broker commit from a producer configured with acks=1
- [ ] The consumer's single call to poll() is trying to access multiple partitions
- [ ] The consumer failure has caused a consumer group rebalance, which has not yet completed

**Answer:** A broker on the In-Sync Replica (ISR) list has failed, delaying broker commit from a producer configured with acks=1, The consumer failure has caused a consumer group rebalance, which has not yet completed

**Explanation:** If a broker on the In-Sync Replica (ISR) list has failed, it can delay the broker commit from a producer configured with acks=1, causing messages not to be consumed. Additionally, if a consumer failure has caused a consumer group rebalance that has not yet completed, the consumer may not see produced messages until the rebalance is finished.

23. On rebalance, calculation of the partition assignment to the Consumer Group members is delegated to which Consumer Group entity?
- [ ] Group Partitioner
- [ ] Group Coordinator
- [ ] Group Leader
- [ ] Group Controller

**Answer:** Group Leader

**Explanation:** On rebalance, the calculation of the partition assignment to the Consumer Group members is delegated to the Group Leader. The Group Leader is responsible for coordinating the rebalance process and assigning partitions to consumers within the group.

24. What role does a Kafka consumer play in the Kafka ecosystem?
- [ ] It manages Kafka broker configurations
- [ ] It produces messages to a Kafka topic
- [ ] It reads messages from a Kafka topic
- [ ] It stores messages on Kafka brokers

**Answer:** It reads messages from a Kafka topic

**Explanation:** A Kafka consumer plays the role of reading messages from a Kafka topic. Consumers subscribe to topics and process messages published by producers.