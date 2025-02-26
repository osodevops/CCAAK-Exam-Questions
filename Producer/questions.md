
### Producers

25. Which Kafka client property determines how many messages are batched together before being sent to the broker?
- [ ] buffer.memory
- [ ] batch.size
- [ ] max.poll.records
- [ ] linger.ms

**Answer:** batch.size

**Explanation:** The `batch.size` property in the Kafka producer determines how many messages are batched together before being sent to the broker. Batching messages can improve throughput and reduce network overhead.

26. Which of the following Kafka configurations affect producer throughput?
- [ ] num.network.threads
- [ ] linger.ms
- [ ] batch.size
- [ ] Log.retention.bytes

**Answer:** linger.ms, batch.size

**Explanation:** The `linger.ms` and `batch.size` configurations in Kafka can affect producer throughput. `linger.ms` controls how long the producer waits before sending a batch of messages, while `batch.size` determines how many messages are batched together before being sent to the broker.

27. Which of the following is not a key feature of Kafka's producer?
- [ ] Configuring batching of messages for efficiency
- [ ] Handling message retries in case of delivery failures
- [ ] Monitoring consumer group health
- [ ] Ensuring message ordering within partitions

**Answer:** Monitoring consumer group health

**Explanation:** Monitoring consumer group health is not a key feature of Kafka's producer. The producer is responsible for publishing messages to topics, configuring batching of messages, handling retries, and ensuring message ordering within partitions.

28. Which of the following are important for achieving Exactly Once Semantics (EOS) in Kafka? (Select two)
- [ ] Message compression
- [ ] Idempotent producers
- [ ] Transactional producers
- [ ] Producer retries set to zero

**Answer:** Idempotent producers, Transactional producers

**Explanation:** Idempotent producers and transactional producers are important for achieving Exactly Once Semantics (EOS) in Kafka. Idempotent producers ensure that duplicate messages are not produced, while transactional producers provide atomicity and consistency guarantees.

29. When a message is committed on a partition, the leader will advance which of the following?
- [ ] Consumer Group offset
- [ ] Partition log offset
- [ ] Log end offset
- [ ] High Water Mark

**Answer:** High Water Mark

**Explanation:** When a message is committed on a partition, the leader will advance the High Water Mark. The High Water Mark represents the offset of the last committed message in the partition.